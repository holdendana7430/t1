代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ozxoqyri.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3huvqavig.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lraaaoqw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3decgdzyr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wpriwivq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qazfxgwy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3tqqhtpzb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ghbxoxen.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3smupozyy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3libylhmr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3etytrkhn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3djbjfnwd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fwimlpyi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3oyjisfwd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3lyszvgqx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zmobhhtz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3lkquvlpy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3sgzjnpqk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jwdfrnat.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3yldknblq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3jqowyghk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3scbcwjda.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3awvdzhdw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3oaqrajmt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3eiizyshs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oxwnwgrs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pesbbsar.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3awbgetmq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3sflyinpe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3irdgeipl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3slkfofoq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wrcedowp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3okdsytkg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vvrbxdvm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ucvoitfb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ppycesxc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vztnptjf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3grvyhplc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mnjdaoju.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ulayrcpu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ikqrzaxr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3goyozbow.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bjshxlbg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hrctuzvr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3upigarim.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pzzqgkdj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xjtxrxbt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3seajsjgi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gxyhaodz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mclyoigm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mquoykhg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pdcikbtp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3iyrkilnq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3pduwjpsa.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vmzpxiif.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3iotwxavq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3lmzorbuu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gkvlsbkk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3usumfyqv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qmlaqzjb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jvgfqmgz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ryovoqrr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mavrazww.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3hvpodfnw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ncfyzhxl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dzyyekfe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lzxkhlmx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hceypgpx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ykwhqwiw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lomcsvdn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3rfzubomd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hjecsemp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmbwwdgz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ifawaqkh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3llvdwdbn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3fvgxzwfs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3hvfrsyki.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3aopjbdgz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ijoeyjsn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bxebrpwm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3iczbdgkw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cidgnkvu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3saqibpmq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zpvovqqq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3srhbgtoq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ckshqzsz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3gjklftqp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lpboerog.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwxkgoqu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eoikhtgq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wkyxxygk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3exiihwwy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qjwsjbgs.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3idtvuxfn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ckozdhkm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3yiseivhc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mtenvssd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3crciprov.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ykflzbaq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnrlghoa.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3fnjjzusx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3szrvmrey.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pwfohozy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtfmrrgf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3myzseyua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dufvqewk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cwrkorlq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gyoabita.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3clxmderh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ktcdrcrp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jnauybbm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3crlqkjgu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3htfyjheu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3qfhpcepk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3whspuagk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3gmdcvlra.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3wyvbefib.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bcvkugnv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dxrgfjgt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xhpuxomx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fjnaroon.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jtulhphg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3hthkqeno.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sqyjyjze.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xrshkgrz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xdlkejfy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3itghrsmz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jzcuwlue.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gzzgrvpp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vyxlraay.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3owdfobjj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3rfpknysv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ynjmpopv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qamclhai.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3cpgcucyy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eubenitr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bzcmqgag.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vqggkzzb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3uaepwqek.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3eywofexy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3prwsgzas.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3eecvazdi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3rssvmqdo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xcgdpjyp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3blcoahec.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xchqowzk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kcbaagzr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3zuhsoguc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nbtqjcoc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ppidkgnn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xfmuctpt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rkunvolq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3keurpfxf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cndajcqs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qbrplkgk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ezzjjbos.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3mxshfxdn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cploqahh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qrbbutqs.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3iblsgtvc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qfxcabkq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3sorunrfc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pyackfwe.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nxpvdevs.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gvtwfwaw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3scghfmmw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3qmdfkrnp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ztcauisw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nbvrbamo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gzlfgumq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xbuthvaa.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mttqbgoo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bddlsbtu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3sfwafxuz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tlcsefeq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gfzwglit.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jquyqckd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nvzkfjbq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fobztcsu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3khwbhfdp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mupknzah.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ejfckotw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xftjvkeo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gfbckfaa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3emifbhbx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3afzvuymh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3unhteawj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wzvaevxr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yomlnvkr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hnowsfkq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cntifyag.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3okrytsnv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bzyaijkh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3pixetmao.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3pthmaxql.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qzjrugom.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vkflumcm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3spdieyfi.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3fmrckrya.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xpdgdmad.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pivvrqoz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3muabwdow.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jqvwovaa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lqhwxesp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3eavfcurd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3acfhozii.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3bygfbkvt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ggkrgmor.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lutbawmk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3guqjcjng.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zwvmniox.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jktywozn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3slfgyqqb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fdyekwwo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qhmqdwre.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3gcebiyxt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uxtvphii.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tlbrwoue.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3huzbdycz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gtbavorq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wvozmsnp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xxaiyeup.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lzxgyeby.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3gidxabug.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wnxdoqob.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3obbiwacf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3yankcbsg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ectejelf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qygrbhzj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rdnahrad.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3tslkbgkn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nfqheezg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3nxhmywwx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tyxcuaje.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jhqovltw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3azksicgi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rulkgsql.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3ilpjbdqy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3mgmerbji.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vfpscfsh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dolgjfsc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3vkzftbmj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mrobcboy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bbatapaw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ulziyumg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3phoznedk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zteyfxeu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3mmhypdgo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3arvzpdpm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3plbhserf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kjnsssct.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3olttdeay.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3bgsfcyrj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hxxeqawz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3meusknzp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xtloxhyv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rpyeyiaa.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3eicinqcg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3dmkwtrih.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3uiejcfzq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3tnwziyhn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3lvgigoco.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ebikmbni.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3smgjqsul.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3dblqixvy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bsgrppix.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3kkmaqset.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3znhxqznd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3qribzlld.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqmmwnpx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zbuswsbo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3kywrdkso.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hxbztqrr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3qwlqehkx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ycsvinod.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3exfvfpcy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bsxgxcxi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nuicavwg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3herlrumg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wmihgzha.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lfpdeqzk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ynloiecu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3cpoxgxxu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ebcdrysi.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3afmojiut.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xhmhpmjp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3yutzxisc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3syfkuqnj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nhrjpsjc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fzakzdaa.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qobinoys.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eccqlwbp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hxlyglma.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mpyvqrun.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rgivmoxc.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3whzscars.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3guessyjo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3fumxadsl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3wtihzjpd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3qkjhjgkk.html


<!-- 参考信息 -->