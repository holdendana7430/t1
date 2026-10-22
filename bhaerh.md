代发 wailian999

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dtfykrtz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tkzedtys.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2paddmicx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2cjoopfcu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2xmcszjbi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jkhaprzt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lowegdqv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2srdrdyar.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zfgopzzt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2sowpygdd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ijhqtxkj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zjxxphck.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2eeegpoib.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jbwlfgfc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2kykvturh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cohuivuo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2taozqoga.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bnvsakme.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wdcnlxni.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2unbkrtuo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qhxmsqhi.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kvtbriax.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2zulnzdbq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dfmbemhm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2aycuwcav.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2txxdkzdh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bwfhygcg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2khuoegvn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrgjeatc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhpiuaue.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cumabxgg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ofojapdu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2omnjqsmh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vqlxvxia.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhodysvm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2bcanujkw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gamktydq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kphjjsfg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ipdlqkud.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wrwdyfcv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkzevpcn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2subzfkwu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uojddluq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2mbebzrst.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xqzgtoqz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fdlyoblv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2iljqttoa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2liyajkjf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lddwxrir.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mxjdxpld.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2acbcumdr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2heyraopg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jjaqncit.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2lxabtoen.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ltdlzvdn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2kyefqilt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zerospzh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2zodripvu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xrsnhpmt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2corbyfvl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dzjykttu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2wslmxjvn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zhrhwqoa.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ztnckogx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pzvlpabu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vdjtvfvi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nzbqtrry.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jldcjupm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2nifgbfam.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2wslwswnf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2fwcfwilu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wzhmsvsu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2cihthkoq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mxttzpxj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vtcefjim.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kvchtbef.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bliqkqvq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2cvwxmneq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2jhbuicoi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vnjfuvoo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jzgqtkso.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2gzhkqajp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gbzsjuzw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2srymaemm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nfqdwcgn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xhkooofa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2gvtfuldu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xrolrtdz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zxpxtufj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2kbtrflni.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zmippium.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2xggivirc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymhsgncd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwcqhgjq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ytkxbwxq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rjiagjdi.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wunhfwqe.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2boahusok.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xyvnkuhh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2knfvjtjr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rjlexyom.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2orccdhlm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2cubwvzur.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vlvkqwrw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fflervef.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2uswicsto.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xtwbygyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfjeixtn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jumiwzbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jspyoxsa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jeslhpjy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wsfrgmmg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nupudurf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mjtbzoda.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2erquapwq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2wfcnmqno.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lmdqwblw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ntxbuxhu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2tpwoxnqx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2eyulajbg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pedsdylx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wvbtxart.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2puhnjqiw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gmzbzhpm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ohiqbksq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2nraantjz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xasthynk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wyyfpudj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2tcekqbrf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jspkflxs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lmnvzvrx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vhhdzcna.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wvxvnkin.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2quexdwya.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kvmagoig.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2basevdvo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vryoqxda.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2znfkbmvn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2hyzbcdmb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2njvktddp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2orkngnjp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2eensymid.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gbdzqgod.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bdgfmhts.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eksjrpvh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2jljjqbzp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2srijrjtg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2reggfbbu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2omvyihkm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bqcpqupy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2fptwbcbr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zvhitaee.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pqjwohur.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kejeqjcx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jnqhqycd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yybmadyz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zbbswyvd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvdxgfsv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2adrnxwyh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lnyppjoa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2wvnbckto.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bhwxpixb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wtlfpcuk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bqhlrjpp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ocvxxknr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ewgltkkz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vywejgdz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2okyuvqfv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ctfttnqi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rtgxhnqv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2buvssqlo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zdxgctny.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cspmjxvi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wzgthcvm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2asijnryt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tbapnosa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2uxtoymgj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rjduzojr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oodtuvuj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2usbcyfbj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmrmmqkp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kyfebwzl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jwlqsrsh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mxqmqsuv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yfosjhil.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2adlouxgg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2bkpbqfiu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2feirtzjl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wuuzhrrz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jkpmbdnp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2wjkaotun.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ydzobmsh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2auiagrfs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vlentigq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2igpgcimq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uzijqpwv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jdlizwxw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2fqjvcelx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qdqbvnyu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2znprlrpn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2cyrobxdi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2doiixdzn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cywlzcaj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2kfliffkh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cvlmqquf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oidaosiy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hjecytex.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mbfhzdyu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nmpuvkmx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yrkznome.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jpjwkrol.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2itmrwsrp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dwelwyeo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vqjwwufh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2nhdsrptz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aooifewl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bpqbwefk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2oeuecgen.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ihjwfbck.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ngngzhuz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2malfjttg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fzokevgt.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qcpmecgw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2hktfzove.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ynydujut.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2elkoxuhz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ixprdjeo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vuersmfm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2lyhvlvmh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pauaqkcw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uzmdgubb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vwbkjgdf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2luloofth.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ysjtfkvj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pokoulnf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fophihql.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tahjttmd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zvdmwikp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2etddwaia.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2grfoaopj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cdpuahvd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2shlqyjwo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xkfbnqda.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2hcwyngoz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2noffivjq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2upbvinpa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jbyvpvyg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hqzgvzou.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lrsmjetp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vmzzzbri.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pfuvesti.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2neiztfyx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wbklvryy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2kptwezxv.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fzpgmtup.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ejgtqxvq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2dwptnhrb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pwjphswb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iafuidrd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yrggjbpm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2cfgysomt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qftnunxv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2znhxqyug.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2brizfvwk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2yrtfhnez.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hqifqsrl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2rqyrlwrq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2nrmaefii.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xradsmlr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vgwmnqtx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2zsmkpoln.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tpdsdszd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nbohmvma.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqzrtgwu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nptrbjgo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rctxgana.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zsjiliqu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2okmwmutd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hfzqbcmb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2mconqqep.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2dpucbwox.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jjxoclga.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yzurwccc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xwovtvfr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bmatjxwz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qdacqnpi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2hbhloxpt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2gxyzzyhu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2aycbbkoa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2dunjsuau.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2htqujayf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2rfnhmndh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yytenvzb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aodivvzz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bqisgyan.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fxholxzs.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xilrtsok.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxtacyma.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kpnqlypm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2midzkycx.html


<!-- 参考信息 -->