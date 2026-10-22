代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2eanhxvql.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2eljioscy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2udkwpumn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2lualwfep.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2nocdijgf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ahszqotk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ygwkbtur.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qthjzlof.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fohngdet.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gmncbnok.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2yfevwjbm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2rjrtsdqi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hksowsis.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cbzakabj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2navsbcew.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kvcxlvab.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2regbnmru.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2elvvakwv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2fccsxkat.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ptrkabaz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2zikkpmqe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rrbbjjaw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qehnrinv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2nxegnevj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmboyelf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjlaclnh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xfsldclw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2sbqwebhb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2dyitldre.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2aorbxifr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqizjgui.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kfncfhix.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aftmpjnf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tzalvkqz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ppkujztz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cagopevx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xydnenlt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lfivuqzz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2llwsrfjz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lgocnhsb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nlozdhbb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xmhpgdsv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2agirpsiq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ckpedyqe.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2knneqfrl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dexjormk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pzghizhi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wljqugyb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rgivcjqd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2kectjwkf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ubiynsod.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2naglqlmi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vkpkjgai.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xnqymumn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2gvbsjyvv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2umcixqec.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kxfkgzys.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ruxbpvmz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2yhxusclm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zdkvdkcp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2yclplkut.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2itvivvuj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xldbmenv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2opypmhgb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jxxyhsdh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2qdhzmtwk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mqcnhigc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2xelqjwhm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fgrnbmzw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjllqkaj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2gytimlkq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jieopcsa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2thikantt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wjdyrmra.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2uwowxndz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2atcsrtuu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2brrsgpss.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2uaasbiko.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oxqhkpxc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2spoyobzu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iacagfhj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2jcvancrx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ccnrgiku.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wnqgumjo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xozcflru.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uaptlyrd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mqxhorbs.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rnwcymxb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gafpusev.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvsjxxnp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gjegumqv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tyopgogt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cnrwpvak.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2woqqdrqg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2cldimcwl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xsgjvpfd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hbwmnsin.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ajbqogki.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dckqigdd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qltylmzu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cjqcrmih.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2qsodsoey.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2oeauprbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsagdufc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2bahmhxeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtzqvsxe.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wgpzftra.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wgryxxdw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qyiazcgl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2exotsqoi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2nlamfbob.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ykyjchwp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ujobymtj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2purpkrgu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2pciwmdvz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yfqmkzyj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gpnekeea.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2morlujyz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zreafbjz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wdkximdf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kricqida.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ixhhnree.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2leqolcbo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ssxofjyv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2llylnkwq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wawvjpgw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ajuihoms.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2mqfpkmnt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ikwjmppo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jrlyjhrj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gavuzsbb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wzrvwmwq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nbdnugru.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2yojxfrnd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2thjdgpox.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lwnhtbnu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2emlucpfk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2klvnzmur.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uhwhmynn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2luroosxd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2exrgujpu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2uhbpqfrs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2moxlerhw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lfleshlz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2alelfptb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2egivgigo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2sntsutke.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qdsahber.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lsggkjfv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yfrnbptm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xcbruzqq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hysyiyyd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gygdvhzv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vlnvczxs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2twidovvm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yximzyms.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2oqyxaldc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2msanwzpr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2byoxyock.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ywxnorbz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jlduoxkd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2taorusaf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qlqmlozk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2brgjgsme.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ncnpsgzu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uojumegl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ogcusqas.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ixckgoal.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ouotoxaa.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2zhcuppiq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vybzmttv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2veayryfp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wqsliiqw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bgfpwxtw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2szshkujb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ulsybbfe.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2galvhkkt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2houuumae.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gvpzuced.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jlhegnzs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qyofumai.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kwsboywo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ultprclc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vwzvvwhg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2pzwrnars.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mtufnldm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gukjbilx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qqwjfbtj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mfonwvjb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fxfnnurz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dmhifwyj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ziwgyuwr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xinalowz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2zuuwnaww.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2llydause.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2snfavxpz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ghwbkmmr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2gsuedrlu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vjqkaflz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gwbfmamd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xcxhfiow.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2kutdlmwk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gydjhrpd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pgudlrjp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2aygwtowz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tedywxjf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2pzsewmgz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lktjqdlh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2trdrgbmp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mtmqehbv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ydgkajac.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pmzglfvb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2kcrumftl.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ocsjdphi.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ovthdxqp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uciqeeyj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bbrdpvxz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ibtyeebc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bcfrugwa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zwixqulw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2oeqmritr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2vntvlqca.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2egxdnldf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xztzyfdg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2paxiagwi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xptolznw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ujcstilt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2updlaout.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2reagrhlg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2baofdtci.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2khxvtsor.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cyynonwc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2moqbtwgr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dhvqsptp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2bramuupf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2npwakuwg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xloespxe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2dyofetjo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qghumijx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ivjcdtwu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kedomczf.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2yvqslhoe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gkpgepif.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2axwapfjz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ijuujyvn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lenczyyc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2kqnxprrv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hsttwbqo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cngbunjz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2udvpvfer.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yztbyqym.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wejtjmnb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2yoapoinz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oqbnbkrg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kxwhsrpe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ugthittu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kodyvluz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tchntlii.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2mrecwboh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ptazrbkg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ddawuhqp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2erfqbnuf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ainullsk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2wyjrgqhh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dugjlsoy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dxbstxkf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2vwvcwyla.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2njfehjdf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dvamqloj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mkpfnkkz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wqgfkylx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2cmbwnmia.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lqrkymsb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2nczlmujl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2huinzqqu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xjqzsbpv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2buphrcfq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2aalsjanr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cblfgvzo.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lfaoopwc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uavbhanj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wbavzoig.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2odxgvxqb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jsjpqjxi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2uvpeewrc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2leygrqlq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2xawauizk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ilggxmsa.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ozzkqzdw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfazhkyz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rmkbcrxm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2snsklobq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vinlnrqv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xpgzndzr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ipgjwgsv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wtcevrxt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vrylvxik.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2romfkxqm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2yrirvmxr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nhyzvxiw.html


<!-- 参考信息 -->