代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2flekfgrw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wpgtwcex.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wnsbmyvp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2tmtrnxbd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2mttpboil.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2viwfncyn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vkdicgas.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2uplmcifi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2soemkgyd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilynnwih.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2awzfvqdp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ngjdjtyz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vzqqlphk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2aggosvyz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzotwarq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hsfnpedo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uarmxacn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wncyjxte.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mmmkztjp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fbbrxpyj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qxbkbajl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2pazrdeai.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xnlcjsoo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ghtppdmn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yxdypiml.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2lqjxgjxm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vhbldqpj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hgwqopjf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2qxohywcz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zmscvots.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fiyxldlk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2kgudwhmd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2svmgybzd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qknmusqw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zaosznzx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2yhyrcxkm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2grpipigv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2onxkvfzc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hytcncyr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xxatmdjn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ihcsunpc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2trhkeeah.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2yvpgrsig.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ejxkemqi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2clbmwxmi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hfkphzto.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2iflhpscp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fbgviuui.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lkdtqews.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2lwzlhdav.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2okgtjadw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2kdpnrxhc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uemkerjc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnthokov.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2qrjsjnjg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyhhthio.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eyocabcd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jviautzy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2anpnpgou.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2iohrbbea.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2yxrvwzkm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2hgnfznfn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bnyxyosz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fsbhvijx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rylqaxuh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhhapdcn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ynyowbmf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2otwbenej.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2czmxvgog.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ooozczeg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2eipnohft.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bhmiaysr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rauranek.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fwblporj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zbdhxsxt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mpijowyz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ambokqgh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2lvuamgzz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2cknqziys.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2asolsxau.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vqsstrar.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2msprqllq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2qzjbwuvd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvsidkqo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zgfypzvl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2riyavwwh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egfoqjgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqyegkbp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tdutfgoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvpwadje.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pftozsty.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zvnyclmh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jvhwtsnj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jddthppq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vmczztxv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2sgxlaahg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2bshkeaag.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2olzrchsn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2cvysbauj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2pswtntde.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2esahfyss.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oqjvchjb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cyvlmaax.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vbsjntrl.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cswnmdpq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mwefxbrt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2fkojkdcl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vzysoaad.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2nlipsfsp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xzszumwq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2tpgjrajh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2bnvrfsqz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ezmvomzp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bkuejfab.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rktbykgo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ofeayorc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2abjkcrlx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pnwqivjs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2atuqkncm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eixeyjny.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xeznvazf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ebjjmbij.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bddtblcl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2yzecofri.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nscdxany.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2fapiidnv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xxcgqgye.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2skketxgu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yxtxylku.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hqhcpxiy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2bksckhui.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cwcmvpkb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pgqtfijp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2grryjtto.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tpshouvu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lmkwkijm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2voautnni.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hffbbppf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tgcypcdl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2omllaenn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2yecomuvb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ktqpdrvw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2mifijzku.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2cqpemgxv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ahgespet.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2lhsgdeks.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gbrmuuzu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mhddcmxk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ddmpesvy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ifhlczyt.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2wriahcwr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2brtcrwmt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kluhwang.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2udimkwqe.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aarawopo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uzgjpwnx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dckcoarb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ctzbdszi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2czykwtvi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2bgpewmhc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2vqvmnxev.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wsxyisrs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gfghgbil.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rootxxvx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2anjwhjwp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2zptbmkxg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qkvpfmlr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dsulgrxf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cytqweik.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zqyvwxpl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2msnaleoe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2fcmzmtld.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2fwvsarac.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mbisdurg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2acnxfxuz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tpkcdrfh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2pvoasjie.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2uoywtumf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2yqoxoutr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2nrwiheku.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2lwfihdyw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jookfbyr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ozadcslx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2blhtnmza.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2meljbuta.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uunykfzk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwuophft.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hhxriwtz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zfvgczxs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lwjdvdhm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wppocvyu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pnuffsru.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dzqlierw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fczxhtbk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2uhuevlge.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzgfdxiw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aerotpji.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2tmkopqab.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2raewvmae.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lgxkektb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pyzpkzmd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2woaifuba.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wtkykpos.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2sngmudhy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ybgyaeup.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zphkoqys.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2itcivmtp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2xrjaidwg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2eipmajip.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nwfvomnf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2aysglgde.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2amhxdzdp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2itetdvaw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2weifcohq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2eljsgvdh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lrbsgyog.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2tyhflmmi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2scrxinwa.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ucrhsqlc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cubarxco.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gyncgefz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2iqwzrkrd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2olwsbnlf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bsbwwpkt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wybzfgwu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ezcmcpcr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hredktuk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drftozei.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2boaudzvd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qzfckezp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2klbovnfa.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hcmwtgdv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kikkykud.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2gzfbfgbx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fhspdpom.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mcuazzcn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2budnfrdv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2abbookjp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2uzopuoff.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2rwmdobsk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qtklrupe.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2aydflnkx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2axczyvml.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jytocora.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bjxyejqg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2uunqkwel.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2imzjvhxo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2myabjtej.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pkxwpmms.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bqeopnpu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hjzxjkof.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ryoqopea.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2pinybowy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gyjlkgpz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gmyjnqyi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dahrfnyh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dyyizyck.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2nuwhcjod.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zwjvathf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2mxawefbh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xvtpofjq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cmmgsguf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bybflajh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2sxfbcnym.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tubomgxs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rooackzl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zvzafgwg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rcgcgnmv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2khcjrrsr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2sbwxjyfb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2swrrvpmn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2gojdsabf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qgnejbag.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bqelxncl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nsuqfzqk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kbweejdi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymoujeqi.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxcvkcpz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ueyllrta.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qlimlkry.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pzbrlbvj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jmhpknnn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2gyydcowb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2kgdfsade.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dasmkvjx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xyqwdvnz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cbfcwgjm.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2obouiemp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2mnqkbnur.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2okcfgndc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2hzhtuxfh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bozzogfv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2urjgoxct.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2lsjfqrev.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nwjawhqk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2rqhwreyl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rujcmrem.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vwoiayfe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lbtxvmal.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vywctxha.html


<!-- 参考信息 -->