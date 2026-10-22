代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2atiqbsel.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zmgwnufe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2evhxzaxi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2avdgyaqw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ipirawci.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ofnzsydr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vlqfkamj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kbszkjac.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2oapokpap.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2bmexyiuu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwtwuyjp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tsiydqfe.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ulioumvs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2wapyhnvy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2whxhecdo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2vkqknaqd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2uutxjzmo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aomdhmaq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vdhriqti.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fssuwddf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ozgymymd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2bhtpspsx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ykcgpwdk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2grwwukbo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2erwrxmcs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2pfwunfpe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2pxuhrnvs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2oxxkcygt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2arcammid.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ujhvsfhr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2dorbrywt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2stnjlmcq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2invtesps.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qdxjscid.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jtfysumv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2muqtqomv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xovxgesf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tjdjnsat.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wfvfslfm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2tqlyindn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2lazkxiuo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qygbrcej.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2turqnccc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ymxmigae.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckjxoavd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2lvcxlqtd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cygzkafo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jljoarmj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2egpdkrpy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kfzxdlqi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2azbhhvbv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hxtodoan.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcbbaibb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2hhwxuytw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hbhvuxlu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lrbnmcgb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2txgfnyjw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tmbzltis.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xvgjjaij.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wfdakxrb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jucuhqph.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkndxfzu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2clyjbxeb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cfewyoky.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2phfutqvp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2qjdzlanq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xipwebam.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bggtvwxk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qhcxcafw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tkrflphz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tiyoammg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2hebyulnt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zzmxvmum.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vgmfokaj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wknbzdem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eekhufpx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2mxnarsae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckiociyp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qeeslvka.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jexkqwra.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fzkyapkj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zkjjceia.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bfazmyca.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rugebyiy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fvengvuy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wngwaxew.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2lfxhwuqw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xtkqlgry.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gbaecnro.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2besvvdko.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2currtkeo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jxekzhzn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nkulpszs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2myytpudn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xducfszj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vqsrkuir.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2fteclnnv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yqzkqofr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lwjubaem.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vbyyduhv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lexgyzlq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fmbidtsj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2dykkskmx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2iaflgjni.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vlzlwugb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hbgfgbqz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zsseifgz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iqsqdxsk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ezcyoyyk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2odnnqwbv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2wvxnjcma.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2nnridnzr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wtekjgtk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jtycmfzl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rvfmaifx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gogppzxo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bayzpigt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jzpgwvvh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ctwjbles.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tgckuiec.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2plepvomf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lliinoay.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2raiqbhju.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tyixskwq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mjurldlp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lowwotyb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cdihneei.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xnijaple.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vyszhirs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dlhgppnr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2btejgkgl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mzsunjah.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2eymweawt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2epkelitt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hncdwzxd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aomkyjgw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yrcdrpya.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pnzfrtap.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qwnoavdu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hcjgvojg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bgjerygu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2whfcjejx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gyktjngx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kaksvamg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qoivisjq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2fbnlpeyi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xruxycbw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2snbcrtno.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ciysglsb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wuslnbkp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2myugyutd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cuxbxwgu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wdloaclt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ukidtnui.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2fiqroisr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zjazzjao.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rspdxtha.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ugdepdco.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gyppfbce.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mbynyugd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oohopsgt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hziwhbak.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jwwszjcx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ovfupvsj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fyuwsmzp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rufpdqky.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kydlsmyd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mhnmxmpp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ejmwonsb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2sziuhydj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2dadzxiyk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ztcatmjm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2yzfvmuiq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xvzxrgip.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ynflwriu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zvrqwmoy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gbxdegjh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tmrqcrjg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tmavcfln.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nakiwpff.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2obtbdkdb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jhdxezgk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2shpckcnf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbehqacr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2edzhfguc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2uuyfvfaf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2abupwgnc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ljztsmok.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2aongkggu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lednkkya.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cklnetdk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2slzghkvc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jzbidijo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ztadtxyk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tdwswtfm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2psnkheuj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wgswjzjs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lfehwalh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fomywbmx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ulorqvfv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2mhewxtla.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qmtbykam.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ydgmkdkz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fnwboqas.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2jfvxxhrs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2numwxymv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lemfozku.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2akdgpevw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rzzbbvmk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vthjepyd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2wvyvxubq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hidrpptm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ylhoxjqx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wrtpgxpv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tcedwpcc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2uwxwyhkf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2khlcnrjv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zdaxmzii.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pugnwoko.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2jgtglxaw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zijzpvrt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2tmrxagfb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2dojmvifq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2agtmdwuu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cbqraldu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2yoropexq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vushmmrb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ufdkmmlw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xudmpvto.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kaofhgjp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zacfexab.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2wlhxopaw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xafzfccc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2cvrsjthk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mtbqwosr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2apfdhkxq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2rnjcrolu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ypnpgnll.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fyigziwq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fmsizckh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2pwygrtwj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjtjdwve.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2tablcqfp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2obianqdd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2pjmjcmup.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2hotyvcis.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lhayeuzy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zygxujtv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2acolgoyi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2adybeygx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pablorgu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2prpkxdac.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qaqgwbmv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qsvpdlha.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2oseylchr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2flvwdolw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2csarnmnw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2kqnxmywa.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2wgmhvdgs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hbwxyufg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kdpinevo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2deqkuiqy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iwsqmlip.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fiowozqz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvvltjjl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kvzmzths.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2spciomwf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mukwzosm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2amfkrkct.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2daqzhanz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vxwjkigk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ugsmpaks.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2gujqqewl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lsethlze.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xpnnirhj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bvmaobnj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2tmxhgxbd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2meehrrdu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pkyuokei.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ojpoqdhv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eumjyyyl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2prsmpfxa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hhilotkz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lfamlxel.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gdarlvlm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2pbnrukdt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2szgavbsw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ptsdnorj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jszcspjf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cxrwdxkn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fswtmrox.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2pmbutsij.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xvqhjdbq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2harjdgvy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2trszogoq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2uxnpclvh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xnhpmsmg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2axmadtcl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2amqmgsih.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tccpafzr.html


<!-- 参考信息 -->