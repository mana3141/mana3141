#include <iostream>
#include "getVolumeSurface.h"

using namespace std;

int main()
{
    double wide, height, depth;

    cout << "高さを入力してください。\n"; 
    cin >> height;

    cout << "幅を入力してください。\n";
    cin >> wide;

    cout << "奥行を入力してください。\n";
    cin >> depth;

    double volume, surface;
    volume = getVolumeSurface(wide, height, depth, &surface);

    cout << "体積は" << volume << endl << "表面積は" << surface << endl;

    string a;
    cin >> a;
    return 0;
}
