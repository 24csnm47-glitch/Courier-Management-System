# Courier Management System (CMS) - Simple Python Version

import datetime

couriers = []

def add_courier():
    print("\n--- Add New Courier ---")
    track_id = input("Tracking ID: ")
    sender = input("Sender Name: ")
    receiver = input("Receiver Name: ")
    address = input("Delivery Address: ")
    status = "In Transit"
    
    courier = {
        "tracking_id": track_id,
        "sender": sender,
        "receiver": receiver,
        "address": address,
        "status": status,
        "date": str(datetime.date.today())
    }
    couriers.append(courier)
    print(f"✅ Courier {track_id} Added Successfully!")

def track_courier():
    print("\n--- Track Courier ---")
    tid = input("Enter Tracking ID: ")
    for c in couriers:
        if c["tracking_id"] == tid:
            print(f"\nTracking ID: {c['tracking_id']}")
            print(f"Sender: {c['sender']}")
            print(f"Receiver: {c['receiver']}")
            print(f"Address: {c['address']}")
            print(f"Status: {c['status']}")
            print(f"Date: {c['date']}")
            return
    print("❌ Courier Not Found!")

def view_all():
    print("\n--- All Couriers ---")
    if not couriers:
        print("No couriers yet.")
        return
    for c in couriers:
        print(f"{c['tracking_id']} | {c['sender']} -> {c['receiver']} | {c['status']}")

def update_status():
    tid = input("Enter Tracking ID to update: ")
    for c in couriers:
        if c["tracking_id"] == tid
