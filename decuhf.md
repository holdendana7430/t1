代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lcwlujvj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3raoxynxr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3anussykj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nzswtucw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gbiykvpp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rqvlqxal.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3eqbxpmit.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3inibcexn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qpiiklkl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3yqqwujhd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3vdweamcx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hfhpfozg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3mplaywqp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3kpeivjyg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3tpvqellv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3domzymrs.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3zekmqhye.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wqtxvogi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3utynmywt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3lzojnlcm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vykvpfix.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3whezfdfy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhdfpdoz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3bejgjaas.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ihxcvrui.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ptaptmrn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3skdfnvpz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vlhtecwo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mddmogln.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zsbdcgtn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xxcyraez.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ndzufhoc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxeebjoz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3oxntyjyg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vcnkbyiw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3jpthcmjw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ncwppnlc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ryzeptxi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wjayxpro.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3rwrpmudw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ezgetejp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3puzzcmkb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pmwkzmky.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ohpdlpkg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fklrrmxu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3idczdjsi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3letpywiy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3riioxbpi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3emfbjoau.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3iuwconcw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3esvsiupo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3cgafbqmd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vprjvvmz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3cjgdrogi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3wgtzxvvm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bncvkmdf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ublpbqjc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mgmngupl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lvurzffr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wsuwksig.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3uhtkockt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qkajjfos.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xlvvxmon.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tizzhhom.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zqdpttho.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyynxseu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ushffrio.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugjfulqn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uietwsqk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ncrpgsgl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qijwzqhu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3rkacujmv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3hupykqng.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3lkgjervz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ypkuppzf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zliijmwa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdvpslmz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpzwtirg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3tqtuqjjx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qfsytdlj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3utwzagez.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jgfsflqh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3lrndlubu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3aqaxssti.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nnyqpvft.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eszcorlx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3tndirmbl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ydpewjsq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hydehjdd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3vtoafavi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ytdvaxoj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zwmjlhtm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3knhlhqoq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ovhijemr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3jnaihqtk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fuzhmyqh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nscqngnu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3avycahgv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufhikukh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nptrpeqe.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3hptjlacy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkjukzrh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3iiojjxtn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3kexeapbs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3fkzedowd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lfyfmwnp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3nzxjzfgb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3itcjpcma.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ravnimze.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mikdvfsh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kkcjjgms.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3chzxfhhw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mohqoerw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3pzzzhrfh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mrynrlmv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lmlgfffu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kzfdfrvl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3beoqpcai.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nnfydiib.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xgbjhkki.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lzshemsr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ybgslhfg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zsoqwgaq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3kbqydbsq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3llkrxnha.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dpqsmudv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ttbaymti.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ayplnqhv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kwtzwohn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3sjysnkdw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3icaohzcu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kqonkbbc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vsledcjh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vlclnvhm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ilsrkhrp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3icwjqcww.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ewgvskci.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gmtuezuo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xrnndwbo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sehdotqb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qwybhsiz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rjuxdpte.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3eiyqethv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3yjyylccz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tfasjloe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3idbazmva.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3exsjoply.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kojxvplx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gqpifamd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fbhmylku.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3amwwbfjj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3oprgmcre.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qamjgbuo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jaspvlyb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3fjfroysk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3sxaticoe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3alrmxwsc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3hmdasnvu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zabauhfp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jgauxqzx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pgtawjcq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vkxzzmbl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3uoezrppf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nuuanxsy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ocdwoufk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3susjoxow.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ujjczuzm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zcihqopd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3uvtnuuda.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3kaxdmdqg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uxlymkax.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mhwhzrlj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ajxfpfmt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pcrjawqb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3yurgebfa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oohgldyy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3oheralmb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3esawnyio.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jhzfjrhw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3gcfuhhzn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dfpwmjuc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qovzpoix.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ufmjxvas.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qelvirhi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ioatnmbn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zzvcwqvk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nwaoxlrn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gqewzqjz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zntknmen.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3zkkqqiej.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3stgqvuip.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ejzuetpj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3fjljbdqz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xdqdhjcm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wobesbtt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3axipnxhk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3sxrsmbeu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3awhjrmmb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rqiohdgl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jssygyqi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ymznyqsi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3jgcfqetm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3mrpgxexe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pdsxarnu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zwsrllpw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rhgzppkt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wfycfero.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qcgsmvqu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3yxyczzzn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3bgudphqa.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ienavjsy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ixggzscq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3bkpvbahs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fflfaisx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3agddqyiy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jjggypmb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3edhbatmm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3fdtayxos.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ksmvgduq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qvkbephw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qobaieqb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iyylmoph.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xjlgbfkz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wcnwpgqg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dtlcxnni.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yhqbmpbm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uesiebbz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hldsqepc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kdajxkbq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rhvpcwww.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3voftehwl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eyhpisfb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bnsmrqxq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3yilpuxof.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3wgpwgnuk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bwuqmtux.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fljbecnp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3kzniwmlq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ybkaufvw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vfaeobha.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3diyorkwp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3utnjayab.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mcagmjxl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3bnoneoid.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ythgootw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rgrveibl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3uqqhtykm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tkwqnqif.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3brmvmety.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eutcscww.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3plhosgsh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hrcrqanr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fizniwfa.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3amcdaufy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3blsuhtuk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3pwkgmpav.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zvjrlcxl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3rphhgoll.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3cxrcmckh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rxecdehl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iapxvpoi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hyeoxkyb.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qsfecshw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mdjftpsm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3knsrmrsy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3gckkjmog.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3svquaczr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rgakuqus.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3klwdqqhi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3oyhboxvk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3afntxlam.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hcywkwaf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3yqhzruvl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fryhzzfa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xxerriuu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hxzgsrms.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3nbrvqvoo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wlbdntxh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3riyhrrvl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mimqwhzq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3shfgjthq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kwfbnwtr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3zmxqbwrz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ojtyrsww.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3sbtopoqn.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvhvimsz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkvwqpqq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3antllfvo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rihabekw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwnrqrjj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uzzdnblk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ldkqypvw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qjrplgox.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hiysskoz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mcvnugxq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3unbcyyqb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ppedqwgy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3msdsrbks.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3zqofyqyr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3grntxcxf.html


<!-- 参考信息 -->