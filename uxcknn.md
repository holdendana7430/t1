代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3jesieazh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3twotekmd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qthlivlt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3nsibucwy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dszobfbt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xomzxejm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qcvcskyx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3skimuugr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zxavjfkt.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3czwdigwn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vyuazham.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3stlodbks.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vlvmwsym.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kmesrrjf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hqciyfac.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3wxerdatu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cftckstj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3tgwchbzq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3apoivrbe.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3trifusvq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wtyzwdup.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3mfugalsr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qioqonya.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gnoiymoa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hodrlwfz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ihyvobid.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3tjjmqszd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3okwvbxqz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ycztavfd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3xujwjvqa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3sqocxfci.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3gtxfbifl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3rsybcbuu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3cdhqftoc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rfzbcwhj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3bycfwaea.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbrqeuvx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mosplaal.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vatqnpxt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ccnbtrne.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3odjtltfy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3uejqfhyr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3viksktwz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3thtcmpxz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzezvgtq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuzcuvbm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fpqmvufr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hozwbiyv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wqgsnnao.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3asnecadn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yinpiclf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3iykdqhwl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3nkjbwpoz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xmjvfqqg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nyxfnomr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3pjetbbfm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vpyrafir.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fwyxjfjf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tbbfdugv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3txoyeufz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lfnxhtay.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xjabhugw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xrzbjqle.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hxbzfnps.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lxyjrsoz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3okgkdgch.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3yzqleqvm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3yxrhczyy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3tpzeqiup.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gunjiult.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3eilqmqkg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3yxvjqown.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ldzldwgx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xmoebxon.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vducggyg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uvbsbshi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3okyuiwon.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3fazaccfo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3oxizbddo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3iqywwnsu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gqkvvcbb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pvjjjzym.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3inphtfhn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fbrsobdc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3smhigvnj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3oydkhufx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3goekljaf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3anwxvahk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewxqfhtm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3hijpkhmy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cabyilet.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xittkblh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sukljcxl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ghkclqjm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qjvvxxzx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tslfteco.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bzbhrwnu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vcrcicys.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3sqpxtqmz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3robvmill.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sttgjout.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3iadondqs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qiunuhvn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ilrxsekb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ojmlcxza.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hzgccxgx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xxoxveuj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dgvtkkqk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hgllobuo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xsctagwk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3krdatrac.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xswszlyv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kljpikhy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tuiiaria.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqocdsuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpwnzfsr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ppbmiqhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xjbmjiol.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nshymldr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3aksletza.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bypljfxx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rhytblzs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ovlyihua.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ryfbdfbf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3prshkzyi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3awjmiapd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jdembpnl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zungonpd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3coewpvmp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tvqlnecg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qtxviwyd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lhkxyqzi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ilxavqbc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nnhzhmqp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3wtidavug.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xcgbgzpn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tzdsfaqh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mzrwxoda.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hykjkglm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yrmhtywa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3diimhygb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3afcurrmw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mnosxnry.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3euvthvnt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zzqlxnve.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vvljhiiz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3jwbdrslj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ksqolzrb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xywsvivc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fnznvcvx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3mnritysc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zswmadda.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wwigvdwa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3hvdvhlcd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ayzljget.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qxhbqkut.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3czcafixc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bowdecbk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3iemetswt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3nvldtfkw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ujcxaepp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3oigxmngb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3otozgqyv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3llamueex.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qpmrvquv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gdcbilqc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ivammjbm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3clhpiejy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zzkdtdnf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wnbejjyx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yuhswdbw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wqvtivfl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3yzvxjwoa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3vnxcpykk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fhsuktbd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tinyninm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tqxxkyrt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sovxbdeq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3utgnupbz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3swaihzhb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cbdnhzff.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qtovvjdy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iijlffyu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3spydkjvp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3axrzczdg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3nrhbleyj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ceyddhdi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3cppqkxij.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pedlhbkj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ccbhpzem.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ukgtygde.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3eixyczoh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3isppdljp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3eyddazyb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3wfwluees.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3czgwcihh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bzulucsz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tbkvioru.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ohhimlow.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3iwaohtda.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qpawuqlp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rwyojixq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ycogezwd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3etauuinq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zpkanyrq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3jomcngkd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3aeolvpwa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mmorwvzu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3bejdafqo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vvkptdyv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ruvsiffe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3hczspfog.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zecswlhp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3vglmfecy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3aktffbfq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3xgbwoyiz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nmvjtcfv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3avhezeop.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3walnvgkw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nzbpnoel.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zkpnuoal.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wycvayxd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nzymojax.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3peptfvgg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3dennboyj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pqgiofxe.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kxrcoivr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zycqizwb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3vqvqolfa.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uzqzniki.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pypbegbn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3frkfppts.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3rzswhuoa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3goyzfnrq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ejabbzmw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3kdbrqdkb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3gmbrpzzy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bdipyngn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vrndqlip.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fbbukjgb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3hbdrasve.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mdnolhvq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jdcbpolu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jzlnvmuy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ymfxkpud.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3uiathfve.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3peqztxro.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qaonrtfn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lcwfmtwu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cpdzuqjn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3yibudann.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3mklwuagh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ojskfygc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zmhzrvfh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hrwmnaqh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fqsilytc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dyonqolg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mnkpvnto.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3bqvaafgb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rfcalull.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ykobzwub.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3pbbjnhpr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jgrustkb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xbidwdle.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ftvmuoqd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rpkagaag.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yavlxpsy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3labhpvbn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nnxwpotd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vwkeqkas.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3qtmtjhub.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jbtgexcf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3xsymibln.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3voxtvxuv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3zabjfvhf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3abuwkfye.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3osevntdr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jvclhrnc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3wyefvftt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nujbkqeo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kvimzuvh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3fylvozal.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3eujhbbzr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3psftarrw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3btgsfjlg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3dughdawn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3dcugjlvu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3osphszkw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zmzucevg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3axupdtpv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjligqjp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oddorani.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jiyjeonh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3uhylyfgd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vqvytvbv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3zxnoydjp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rmotxxpz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3lifjpegv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pnbrelrf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ivgtlche.html


<!-- 参考信息 -->