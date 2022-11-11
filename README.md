# SFG
Scripts for Georg


# diff Befehl zum vergleichen zweier Archive

diff \
  <(unzip -vqq a.zip  | awk '{$2=""; $3=""; $4=""; $5=""; $6=""; print}' | sort -k3 -f) \
  <(unzip -vqq b.zip  | awk '{$2=""; $3=""; $4=""; $5=""; $6=""; print}' | sort -k3 -f)

oder

diff <(zcat file1.zip) <(zcat file2.zip)
# Alternativ das in C geschriebene Paket zipcmp installieren

sudo apt install zipcmp -y

# Benutzung von zipcmp
Muss noch gucken


