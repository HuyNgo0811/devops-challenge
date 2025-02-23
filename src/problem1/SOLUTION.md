Provide your CLI command here:grep '"symbol": "TSLA", "side": "sell"' ./transaction-log.txt | awk -F'"' '{print $4}' | xargs -I {} curl -s "https://example.com/api/{}" >> ./output.txt

