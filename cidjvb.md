代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dpetkadq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2riabyjct.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2motwvftl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fzhzxcux.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rsudwnhp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2bfukgian.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2sftygshn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gvsttrme.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2urpgrfkw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2knmavrqi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2raudqrdf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2keaiccxr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2huhvzowy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qyjaquzx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kblckzzj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2esajlttm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2kymunthg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2rxnvhggz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2eblkzswb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2lgbrlzsh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2nrgnbkij.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vfcdflus.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2swkmtblj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ttsjrjrf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2npdyusdn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jndakibh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xxrmnvbn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2swrllhyd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lcrphnxp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kxuawxfb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfpoxcqe.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2acjbzkob.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kumeagzp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2scqjgieh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tpwlslsa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yorjrwgk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbudmnbp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2recfuonz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikrerpag.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wrjgnwqd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2etefzgcu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ycieqpet.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2bwgolfja.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xqmwclxc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nqtgvaah.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hkqzxssx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nrprjktz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2yupnigkt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vldiuurx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2cunzogqh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2itqasxtb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2hlnnlsxd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cnrszxva.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2dxuxoqvz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rrdhcjnh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ichsvpdz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2gvfgkqxj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fzuiypcr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lnsncboi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2gytkbvdq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2vytxktyq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xlllbodn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2odimdbcd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2nrjctrjw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2vvnmzrtk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rdenkkji.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2tkwvfrtl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ighdtzar.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kphfarmu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lrythwvi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xbnlyoha.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wukcqpkb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rarwtykh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2yswahlzi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2uexkhicg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hnelexto.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wgubxvpm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lydnajdt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ltmwfizw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bjsqnsgj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2onlpmohm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmkwrbma.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2uxnppxfo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jyahxhpt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2iljptrxq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2icxvvnbv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ifookupl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lvyszbrx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgpteptt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2odjrnrnu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ynkemjwn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2usgdbsfy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qbupokpq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ilfqrlla.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2irjrpmiu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vpujymkm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2xgazayqg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2nfoqvxme.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2vanpgvry.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xncpeeew.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ytwcifnc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2iwftnxep.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcqdvemk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lshqpnjl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tnkxevnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esoewoup.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ogxatmld.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2afgetylm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2egblevod.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hqyywnlx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nrrbxkhz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zctrttmp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hmztoyiu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gqmviygr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2snjjjpbv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2tjnqtubn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2oogqwwfa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zrhpeqgs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ruowqpdc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2robotasn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wxhtxyxj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bfjytcsb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mmiajqgj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uiqapxzg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2intryksy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fcobghsp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2kcunqale.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ffsuqcxn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cdpvxrpe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kwzzaerq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vrwazgez.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2amzkpfhc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ggkwxiwc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2nstkxcwp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2etwaqgzn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhpcwvla.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2juruqlkv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kspzhtry.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gwmfynwk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nfofebrk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2vhhrteep.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2nonnnxuc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xcgghulw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lldudfmd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2svmujeub.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ejjixikl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2jrzzomac.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2eukaetkj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ylvruksr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rrrxshnu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gmbupwtl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vvjqpflg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twlyetjy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2knqgcrxq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rnuhokna.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rydekqki.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xwsgklef.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pdozbovu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nnzicsqa.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hrekhdxi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bhzfwpel.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2effsgexl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2keenzagd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xpimsjie.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lzpjnyzk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zvjepqof.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2isgastqe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cijjowve.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gxzyrysl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2nossfvlq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fdmywxpt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2cjrrxfxc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lhrbjgcl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2yxdgczuo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qxwtphwx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2agyluqhj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lgqfinuv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2swjfxtma.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2tkqmjgdm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2utoixcjk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xeiefasp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2igzabryn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ixjjpant.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2azkmvhdx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfydsesc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uqslstlr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ndnerpjv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2eaymkqcc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2txkghbzy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ouyqbpsy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ouhaloru.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jwancqqi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2lflgdoam.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2tthmxumx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2oiaidexm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xvtrodqz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2yvokqcnw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2iieosejh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2avjpahxz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ylwkuslj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2iuwpbpcc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lkjyuwnh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kzpcenoy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rdvjsdlo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kpcustgx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2crcskpik.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ezyjaoaa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2axieclpe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dqnvvpuv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pctqxmaz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2gkhgbhqa.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqpyswua.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rpzabmob.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ybzaeufh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vtsjexlr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2dtilcvbm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2obpacvdt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aqflhfui.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ihlpalnr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zterloke.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dmemojsp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2tjwsutgs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nlruquir.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2dfkxkkgd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2idemmrfa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aqzhwjuf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ojzvncmo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2buyaxfuv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2kkrpiufu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jtmvkiyb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xqnzgebh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qzrtdhdr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qynyuwty.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2omyrxidj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dxoguynl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2snpqgbqp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jxnnuqob.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2crtsnpxf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jfglbevp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2gzbcjhpu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dktyoubo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2uwrbytet.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2shqjyozw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2amfsmzmm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gozvyydt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lgttcqcz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lgdjyysn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ksdgamqi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2evjqyims.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2xsrkunvn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ksixzqas.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kvtjfeax.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gezwsckh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ecoaqjlf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2cifomvqb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2lyalsiip.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pzaulhrd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pqtgusis.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2woeawbkj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zzlachnp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2aphloiyk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jdnzoshg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xxdohyuw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ecxajnsq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ffrgeyvs.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bwlsrafy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2zjrmvqnz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2baavzspo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2mdetvnjx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhczdva.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lrbvhjxh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gzzgovmg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kfglzqgl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2gcilfohq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2hdcjlmkq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qtrlxmdw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ngxwchap.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2trtbaexa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lesiveab.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2crkyubxg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ehhbguil.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ydodsdhr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2icvyxess.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2yjqhurlf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ssrnxxtp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2rptdjlbh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ptuuyxck.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wqphmbpa.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jrmsrpsy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zommzmgb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jhmajeph.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vvgrhmfu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jnyqnpet.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fhfmfqdb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qegyykbz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ogbmfkpa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2iubttbhd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2sqjbvomc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2doyybrmp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2piulkdpj.html


<!-- 参考信息 -->