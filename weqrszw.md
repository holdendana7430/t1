代发 wailian999

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gxtyoddyg.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gdiwrnlyd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gfthpwoio.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/glmrruafe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gmlcxpuxe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/glwdsennp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/godhhmqjz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gdjroickl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gxlcglgku.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gsdkojief.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gsiertxav.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/geaozbnja.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/giitlxhrv.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gqrfhubqv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsdhhdnhk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gpcmvhnku.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gbzzltgbu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gbsmpovqc.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/giqdlripq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gecxjezyj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gitbyngkh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/ggxjfkbrh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gbswdqavs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gbhwrcowq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gbsssfark.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gschrchek.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gzyjdtewy.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/giyhkaatt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gzbogonmu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gjkmsuvee.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gzxcnmfby.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gnqxhstpq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gbmzkmgaw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gyubmoamm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxqbxfwvn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gqrnwrggp.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gutrongmq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gmsspqfrc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gbhrzvgyn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/geocfclta.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gglwgwemk.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gwogdntjs.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gybvrsidt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gwavcosoa.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gxynpsgcy.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gubdirhkg.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gnvoouvqb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/guxrbisfe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gqwkketbr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gsqiphduz.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gdkdoklif.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gqjgocxdy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gnmaxpeva.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gbwoclmxq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gbwptfcro.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gpbfxjlxr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/ghjxouoei.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gpuuogokv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/glqkfzvjx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/glecvrznz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gvnxxpyze.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gybjujpoe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gxwvrmpfx.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gweklrddh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/galglnupp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/grllezuzb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/goggkkray.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gigfxhjel.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ggjhuwqrz.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gfftowfip.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gycijnqeh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gvishgbvh.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/ggflklmcz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gneqwiduy.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/geolknzsg.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gmklfqknc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/ghtyzkogs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gzzzqrysb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gciqkhjmm.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gwdwtzsaa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/ggeqftvqi.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gsdvuyflq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gonyigcpj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gzxoktlch.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gscydnark.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gyhuahsdq.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gixrvmxkv.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gqmsixknp.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gjhotxhbo.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gkqqqzlyc.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gigsphoyf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gzerbqrdk.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gqxajzajl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gslbiopjn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gpajtnleo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gzoovcvxk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gkwdmfwox.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/genwsjyjy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gcrqqkpjm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpdtepujw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gmqyojsby.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvqvdzzip.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/glxynyplp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gurqgdkdt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gqrhylihr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/grhmwmiff.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gdknzcrfy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gbcxfrxbw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gvazaanqk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/grsbcibvv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gbztpdnhv.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gnksufexx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gtofiyyrc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gyyxevvhl.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gzfgudkmh.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwptqocww.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gwewqmutu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gndyitdvl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/grhntenal.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/ggqrnlfhf.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gwsgzfsns.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gqczbjabw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gwxavxvjb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gyspxyrzq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gapfaedac.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/glwykgqjl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gvbvrbwvm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gvxbaxfdh.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gjbxbjflc.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gqfclhugy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gaqruuzqx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gmxuwujmx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gomzxwlhb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gbzpaxfmi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gyrsjemuq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gdxhfagor.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gzqtjcyxx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gonjyjosy.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gibeiiwcr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/goolqjldh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/ghmagcgfa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gxvtyyhrg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/guedgfjby.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gnfyzidzw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ggqdbwdcz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gifwszcig.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gxoxlxpnb.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gozoofdyh.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/giirsdrzd.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggxfrkryo.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gnwxagjkr.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gtmudpaju.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gpkdincos.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwafzeqmo.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/ghcsblpuk.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gdrihfwzc.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gmaslqlix.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gboreawco.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gintneohe.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gobwcsbak.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/ghwmtuksb.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/guldqijww.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gnsjzqsxl.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gvrokehve.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/glreyhcyj.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gelttpfkz.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gopemoiit.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gpedbbdse.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gcqirrjxd.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gzteqtugl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/ghkmcylch.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gnkvhumay.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gsjhwuddk.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gkfyelafq.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gikodnotp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gcbfsxuzd.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/goghpclnc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/guaymzukd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gzydxkdbq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/guqkmrbeq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gdvvqtwof.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gewgqitvc.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/ggffkijbl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gvegsnjry.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gnzdoxcgu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/ggdqpopqs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gimjpgiik.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gdcvsudla.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gaflrurjq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/ghofaziqc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gqdptsvaq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gghzbkmce.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gswpxgctw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/ggfnlknwv.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/giezhtavg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gcdbmvivj.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gncxullie.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gnndqwabr.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/glcpksodk.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gkxbfuavg.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gnvntobeg.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gkhrlhyhs.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/goqwsulpa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gptaftvix.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/guftloicp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gdsklmmkh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gtrjgpgdc.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqlvgrsak.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gnquxpthz.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gexjrhaxn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gbvimvoiq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gogjvqlyb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gcaoohwmt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/grthdqjat.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gtexlaqcd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gxxmfsstf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gassfabxv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/greyddxzr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gfumexbec.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/ggiszlhmd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gakmmkeoh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gstwilywh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/ghkkwcipr.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gbsonlhvq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gzhuqtdzx.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gsfxsvfll.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gmbocytoe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gmcymhrvb.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/ghjgptszc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gidticihb.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gybomworm.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gtahsggdc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gmfamrohg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gihlwgpxf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gozgndlds.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gcfhljhap.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gnsmkjmma.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gvjizsxrb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkojyctws.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/giegzihtg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gazugwbmc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gsirmihzz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gixzksrer.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gilrecloe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gdsyhzoju.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gwvsktwki.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gozshwyvh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gvynptdzc.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gofdpvked.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gcoaenlfy.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gwhdjrxpz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gejmwghmk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/ggxcjjzcx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gxzdwnsnw.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/godjrzslx.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gfqcrlnql.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gecxytjxq.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gzfbffams.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gecfadjrq.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gvugckinn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gusyishfy.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gyvkhnrog.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/grwtrvmrg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/ghyehhhgi.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gkmfvxvrv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gozjnmbji.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gmnvcdirl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gokgvsqte.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gihlbfvxo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gxaiitxab.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gtysxufxi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/ghixvefva.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gccytrrri.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/ghwnezvmr.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsjwcxaxu.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gbvzvdzha.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gziycqcjx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gwuhwcopv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gwuebyqik.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gcnktxxsm.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gqmrtpagc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gvuomayng.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gizddxvvc.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gxoollpih.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gqejjfvhi.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gnkhgwclp.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gwuxaflhd.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gsdfivzvt.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcfihivil.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gifrtavph.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gfbydryhj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gjjtfvtri.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/godbavptg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/ghqlcdfcb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gxadithya.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/grsplcgtd.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gaqulsgxb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/goaitzsvu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gtzmddmgm.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gmyzfwwsn.sHtML


<!-- 参考信息 -->