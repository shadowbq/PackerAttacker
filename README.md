# PackerAttacker

## Description

The Packer Attacker is a generic hidden code extractor for Windows malware. It supports the following types of pacers:

1. Running from heap
2. Replacing PE header
3. Injecting in a process


The Packer Attacker is based on Microsoft Detours.


## Compilation
Using Visual Studio 2008

Compile with Microsoft C++ 2010 and Detours library. You'll have two files:

1. PackerAttackerHook.dll - unpacking engine
2. PackerAttacker.exe - DLL injector that executes malware and injects PackerAttackerHook.dll


## Setting up

1. Create folder C:\dumps - all the extracted hidden code will be saved there
2. Put PackerAttacker.exe and PackerAttackerHook.dll to %PATH%
3. If it's a clean machine you're going to need MSVC++ redistributable


## Usage

PackerAttacker.exe <malware.exe>

## Misc

Currently only PE EXE files are supported.
