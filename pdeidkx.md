代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/golmnvbmh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/gixikjyeh.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gefzsogoc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.hesvh.cn/Article/details/gpbgpssaj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gqhutpmfo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gocomdiri.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gosvpnoub.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gbqdjqhio.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gounjucfi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gdvclgdmu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/glvwklibr.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gxtrdqayd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/gjgxvgbgq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gdpygubhd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gkvdghhzy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/geuurnkxp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/ggdolnwpk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gfqdzdfvv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gjlgtupfk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/ghbrpphfu.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gwebtompo.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gbbinsvnf.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gnmjxihmd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gcdpfytse.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gdynjgsmt.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/ggxaowbnl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gmisgdlzp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gwflnjxlc.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gzqcqqscj.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gvjvfwazf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gzzxrwldy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gbrxvuozd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gvayuqhxr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gmuvjqula.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/geppdjdlj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gjapxmhmr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gusvgspiz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gxsvgrexp.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gaoduvlyc.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gmtbhnbsw.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gckewqzpz.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gfohvgnlb.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gzplxausu.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gliscxmrn.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gofhohkbl.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gswxopiea.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gbxdnjajq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/ggpoeteza.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gjjtbfmiu.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gbsddpyiq.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gtlyfzchd.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gbmzsstbk.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gxdorzkzg.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gsempxkku.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/goznsqilp.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gyoetolzv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geqzyihts.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/guhvbtmkc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gealkuoiy.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gjayobtcx.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gpahmmqcr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gzpgaizbj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gvdxswbki.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ggvrpttxr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/galsrkght.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gmxfsxppo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gezfkzsee.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gkjgzobod.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/grovdrwwd.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gkfqiyjli.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gtlcqvylc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/garimfcyk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gmcirvwbu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gcizwgqxv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/glpxmoebg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/grkmpdvhy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gdzwvjhgn.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gmqripjfh.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gmrngluqj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gteymigqz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/guumvqjfg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/ghxbcqius.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gcolojaji.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gqxtdrxnn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gqvwbpdtr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gsmzfwysk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gdiwtorlr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gcopvyszr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gziepgmky.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/glyvqbnsh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gzpdixjln.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gbowxzjnw.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/geodtnsfq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gwxrlrhvo.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gbvghpxpl.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gtdqdwkhs.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gggwtsvpa.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gdvqsgvrd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gylpdfiaz.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gixyppmlp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gidpscohb.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gjycuyxjc.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gfkvinfcz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gvzsoxsxt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/glnydsuwr.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/ggdiqmcqi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gzxgevcoy.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gkzknmluu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gjmiwzrah.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gzoitpwhh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gfwzvjpta.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gpisokqzz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gxwchszhr.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/geslovrkj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gmoszmfvk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gloeocmrj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gdnoeytdf.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gxnighzid.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gyihzlzsk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gzbqkwtdx.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gdclzsenp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gzyusmtzi.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gjqormvay.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gxrqqtsbx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gqkneqalv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gsmaupuof.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gewclyttc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/grijkueky.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gwyljctot.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gvmralnaf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gktchqzko.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gcgmwlfwa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gnwowomyn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gittpamkb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gtblkdjgl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/glmfclprb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gplmvjydw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gyycusghl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gushbzqzv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gfxhzhedt.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gechnhvsu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gfykoqolw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/ggzvxtbnu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/grwvsyapq.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/grczjcxim.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/grjempfoj.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gjorpfizh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gazcpzrbd.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/grsbfhhtj.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gjoumvova.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gtqffuvdr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/ghecouzay.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/ghredzzld.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gcuflrhtm.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gjrkwksun.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gkjzftnew.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/ggaklczgf.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gnnmkpvgk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gbuuijqlx.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gsnzksxqs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/guukwaowg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gkntlhphw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gsqtlehcd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gnfakbjst.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gyqjecbiq.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gyasnunyi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gulotkwxu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gcupuejru.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gwuwjthid.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gfysinjjp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gjobikxyh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gtqyfskix.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gjgdrqhfg.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gmpfkeaie.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gfpjzxjco.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gqnkusinh.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gncaqfqag.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/ggyrnqukk.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gvzoirias.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gffypqtxz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gftlfrkrl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gqncnuact.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/glzcsfddp.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gufszdftq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gfgfjfdjk.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/guscpaeut.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gooqohbkw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/ggnvbosrd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gqbxxewwe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gnmdgmiwx.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gdceucjbj.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/ggfkptpdq.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gvpempvrm.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gzaopbgpi.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gleaoqwea.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gchthhjbj.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/guqnzbwfe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gozuwogrd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gtlcjcyso.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gzeouziqk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gjihiefoz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/guhxtousu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggyczltab.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtzgnvatr.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gjdonmiqx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdnhddkoc.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/grycyotty.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/giuntexdj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/guegvfyuc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gglmxabrb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gwyvicvdf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gbokyohkp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gnaictqhb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gcfrjofbd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gmtlnxtag.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gvpjcdxhe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/glikqyfre.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gjmjbdmop.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gkqnffnuj.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gsjwszvke.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gcueoejea.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gcoshcoel.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gtjazbitn.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/ghhtyphyr.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gnctmnoor.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gpeswegch.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/grmsnobbh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gstleeosj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gihmmrque.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpotnpgqg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gzlwwcfef.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gqavdvjzs.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gugrcpsra.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gxxdleirg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/goxtrkqqc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/golwdxdik.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gqqzysbof.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gfsejulbo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/glxvnzydi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/ghprlxzzw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gnnkqmzei.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gyconlstd.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gfbdxseui.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gutvfzcjp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gvfktyxmc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gcdumfmng.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/garcxltth.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gxvoebjqh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gfztbbvao.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gdewjrvfu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gqwetmhew.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gimbkrtkb.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/goprucvih.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gqszfqntu.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gqsuumdzc.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gcxuftobf.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/ghjtmqpqa.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gazdkqplx.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/guqawvxsd.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gxswgjgtk.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gbfyetbid.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gaiyraskq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gamjjusad.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gbcodylbw.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gvcwgdhkf.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/geixamqes.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/grcbuaosz.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gzhlyiidy.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gxbazstjo.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gocafqkmx.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gvenrtvst.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gnhhucksx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gfxriafqj.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gvxrnplwy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gfkmeehma.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gawgcuxmr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/giwloljwe.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/grcwjkylk.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gbddnqlwu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gcwfteomd.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/ghrkfqzou.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gzvokacbz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gzddfxxfi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gsrumixii.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gcxzlvoiv.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gxbzmkqtt.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gzzxlblvd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzsyojt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gjkaojvhw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gwcejxilx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gurfvkicf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gxcnowqpg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/ghoqrvxsy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gibyxrtbv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gwtxbsrzq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gmzepztqk.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gquqxmoaj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/glihmcjqz.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gszevdxpt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gjkdwvypl.sHtML


<!-- 参考信息 -->