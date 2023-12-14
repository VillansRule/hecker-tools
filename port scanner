import socket
import threading

target = input("Enter the target IP address: ")

def scan_port(port):
    try:
        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
        sock.connect((target, port))
        print(f"Port {port} is open.")
    except:
        pass

def port_scan():
    for port in range(1, 1001):
        thread = threading.Thread(target=scan_port, args=(port,))
        thread.start()

port_scan()


