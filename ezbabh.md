代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cpglhhvg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3apfbanaw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3sfrxpbxt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bcqwbrst.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uwpqcszp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3cagruoet.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3depbokfk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bpndlenn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3drcwrdoa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gallabee.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fbrfjdur.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wueijpgk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bydznmnp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yhtrwktk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wopvkuvr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3bwsevsnv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3attoqpof.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3fmacvabb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ovohwafc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fwqtexgr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3icnmchiu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3npmsaqwf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xlkyijne.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hosxcmrv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3abferbjx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3daajdzsz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ckulqduz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3eatpwzle.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3obcmxofv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hjfadspd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pmvjupvk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3pfcavngz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vtqufcyd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xrohasxd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3txtvdtqd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qjyaeyed.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gaxclpus.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3llujgkfn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3lyxylvtf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijecwlad.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlmxiike.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3dbriicoh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vignqzfw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ympejjto.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3swiyminn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ezgbyfeg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ugfjjwvp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lfhfpdlc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsdktada.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbixsdni.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xolhgnok.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dwzqzwaw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3cvrcysxm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3itootkjf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3attegpma.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3anvttsxc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3medweswj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3isvnqtof.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xkweqkwm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tffotrgp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mdwgcpoq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cpsmtxbk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3xoqosnwl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kypteaat.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3nqjtrfoy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ufninbnq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3cgttztji.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fhazmrtr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3lvvrgqhu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3umlihrei.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3cnlklltc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezxmrhhy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kslascll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itlxzcbv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vgcftpbd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fuwljzgl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bwzjdayw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3abqhudgx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3flugsytu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3bpyfwxkr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jpoeuzvz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xztfupmd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3flugkphk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3revmgvcr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3leqifcma.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dkdtkwlg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3izqawjut.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zyoymiay.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mvrxsima.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yqocphei.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3hncbtrvo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pwtoogcl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ywqdxqgg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3albsfxav.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lbfzzteo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3xgbidvng.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jeowidur.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3marsvzec.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jgoshsoy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ftlngqts.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iocgcdoc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xfawlgoj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wuyxoiwz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tzzrnfjz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3tnuohhbn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rzksbuck.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bixohuve.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dncqexeq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3anshrtxl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3fzmahlxd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3mysycyni.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3iltgxvzy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jxmiyrpw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fbjbkaey.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tsnoghhg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3onitwmur.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xyznenis.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ubrparmi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3njswrrar.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dfbxwruc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rguyjqkd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jurqbtmw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jgzjsgcc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xhksgscl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3kngbyjnk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zvhvaxbz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3abilejby.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3jiqmxcam.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3cvxnxdby.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3qghzymft.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cfxqtzqb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zjpotsxd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ztnnddkd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tpbxtytp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3epgkavay.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jjcrjzst.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ruexxmrv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vedtoqyy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nybnqkwb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3byhhanga.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3rlbjgpdg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3icywkhhl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wpzivysu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rgwmkyxk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tsxrpbjt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hjphrqzz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3tzahjudc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qipxtkkc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3aukzomlo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hdngkbdl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rjwwyueh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3metozaet.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xxhmrsag.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lhatfkdl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hptxqhdq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3fgobbrxi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cnvwtkyf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ckjmghhi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zopnpeqe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3izjfuajc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ctpgxpai.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3lkuehnzx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3odsczvnq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3nxxxwjwm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3kzwbbbec.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3arzovake.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vkncmayx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3aqousqvy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3dyxuznpk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dejpuiou.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iicvziaj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3jobdznlg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3tvxdkaxq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3dwzysmsh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3plusnxxg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fngavctd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bblikoxk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nayrvhvn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mgqdejde.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3chuyajsk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3iuedqfgq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3tuhteixl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3chvzrbmd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3tlqzccyf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xoydohil.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3arclmvtv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nnchxdxw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3yewyxomq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ujpvlbxw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3eyzdlklk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rpciirun.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3jvqlieql.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3fcvfmyhm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3azmkyrlw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qfmaztha.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fovzocrq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jvcrqfev.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3losciyts.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kfvhjhkp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3blqcnibr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ecluaxne.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sqdcsdlu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3eqpksnqm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3axforrpb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3panxpsnb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hpitmfqc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3pblwqjhx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bcomptjc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3szposqfe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3cqknbsth.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ytitcgbv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uwubpgyz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vvgoibcz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3liqxgmnh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3dechkrzr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3prvudskg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ipkldhbt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rtdpmtno.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jixfxdse.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cbdcrvoh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jhpikfpt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3itwxyfhr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kctpfton.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sjtbrmme.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zfieiepy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3drkfirul.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fusjtqhx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3aslvonqn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3lezdgzcz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3veucjwnz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qiryljfg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3tvrzqjzi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wpkhlmpj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qgrpvdto.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3txnvhpad.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sfjdbxdv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3fcobzlac.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ehlfhdus.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nksxnbfb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3tizmytds.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zjrqgnxd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3doxvtxec.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3dvmcdaon.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3exzgywah.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3jgbssmzf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gvqsfkwa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3tfofvtyl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bdwdjvha.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zdrpguty.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3buvvpkiq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nrslwxru.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3qlpnngrb.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3cgmvuvqs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jzinpxzi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wttppyao.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3pdnspboc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ejrhnxkh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mvhmjtfu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kezzubyc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ikbojhvq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jiipxjbs.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3esuyqpvg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hkowwygs.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3rkdwdjtf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dfpnzdaw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mzvtmuml.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3psqxwawl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vanahqkn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mbpduell.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3oqpeneqr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3nkcxgqae.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rokfhhem.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3utqwntyi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3koixlyvz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3iuvfjkjm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zpifktka.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dtazhyqj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rxxpecsv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gnahpyxq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3sssyvfdi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lqnryocz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3bxakllit.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3awjkzfpl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mjgttcjd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggmknkmb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ozveiusy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zuinsexi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3anocvffv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nwbogksm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ydavncmf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3gxlozdcv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qonphkko.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jfvhrbet.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3scontpwf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3owakoyef.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kfoskspp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xyhgqjfk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwcaxxko.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3avgpsqon.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3kjolekrt.html


<!-- 参考信息 -->