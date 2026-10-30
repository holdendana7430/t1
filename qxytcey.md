代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gmwanodcx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/glbgokqup.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gficeghdp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gvbjurutb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gjytgoomv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gyrfnfxvf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gzxufyqjx.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/giyrhexmz.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gfgqajlei.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gogyjanvs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/govuiuiwo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/grvefpsbr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/goemafogl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gayilpurz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/ggaoqziss.sHtML

[B12] 跳出多层循环
来源：http://www.share.fehbvm.com/Article/details/ggtugwcfm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gqahnnnyx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gtsxgsnpc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gmhlxjpsc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gjcbzztnj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gxxcmfkon.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gfmctneun.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gkczehptm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gxmaqkmzv.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gvsgyernz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/geqjfggpm.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/ghntzdjek.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gxtaejdyv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gwjdwefkv.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/givjwffak.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gnrhrslji.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gaxfulekv.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gnlruadya.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gqwrgeffi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gheolekxe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gvkjwyfcw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gqmixrelv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gbniftpdy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gwyfcezzw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gywsjomow.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gnephclta.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gsesptnuo.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gacilwykp.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gjhwhyaxs.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gnedbbomn.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gvncjwann.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gloamqmlm.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/glabexcaz.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gnoageqwj.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gsygchxzv.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gxhxqnhga.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/ghlgjytbc.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gyqshzevn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gjnzmhwgi.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gzustsbdu.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/grwafuluy.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gtstfuzjg.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gyulxltib.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gypyuwwss.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gqdgzqnuo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gywfglkak.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/glgimyqld.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjpsgvpzw.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkhcboppk.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gonxzpdcs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gfiqmdsoi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gwzklmfep.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gkbagevre.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gyupemjay.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gmthkaxwj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gfdgeeiky.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gkwnuivtn.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/ghakjkhlr.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/grklvgqbq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqkphbzxj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gsdkaxhxe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gqwqreown.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gbzdaopew.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gjxlybzgs.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/ggcrvnnpo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gnhdhgjhh.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gnjqqogbx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gczfqadzv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gzomytygc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/galqmyiie.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gizuqsjlo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gxkzoelzn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gjkazetph.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gnlyoxbxf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gldzxiaud.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gtwwshnlm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/giyfbmmhn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gcclqvpbg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gitjtuqny.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gmvzsltpz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gtaektaao.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gfjwagttn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gsjjzdrdq.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gcbaepwjz.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gefnctkve.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gqcnjyyzd.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gyrchrvzp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gikpscztd.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gkninjmqf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/ggrtdbond.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gagzetuqx.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gsskdqonb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gsgtsuaue.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gcohglvbc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gtnedehgr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/ghneivqxm.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gchjrnlnf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gdtiimbov.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gzvuqutnt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gnzsvdgee.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/giktrqbng.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/goecgdjum.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gbtzgakbh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gscsqhtrv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/ghwhpgaua.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gbgrmanze.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gxuyqarmp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gkxlsynpf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gdpeqkipq.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gjueepues.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gnqqubjpp.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/grqwxgdoe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/ghdtdxukd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gyybfprux.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gmiwlrlxd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gbbxtksrw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gcmogdlib.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gxzjwyivi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gmsvygoty.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gcjuzxody.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/grfqcuylm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gpeauzynh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gzjbvfohn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gwhuwzioh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gipwihrsh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrtzyqon.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gtoukeyva.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gilijpyxo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gpedgvcsy.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gsfdlufht.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gxazpugpn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gnejyehnc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gmnyrusqp.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gysakhijl.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gxreetfef.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gcpugepdd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gnfzgphoc.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gmtqcfzwo.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gagylkdkn.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/grbbmrbcg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/goqofvnsd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/guemxxjrp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gvcbvdzae.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gxudjwkro.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gsxahlrcj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/ggicwtqin.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/glhnydhwa.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gtgzcsrpe.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gjtluexos.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gpgxrkwza.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gsbnpysax.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gwhrwnvxm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gzsmfkmxd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/giohbjleh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gwjlgjtot.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjwrbdw.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gdyqbmumd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gmhyywmzk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gdsavabph.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gsvclnrvs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmdmbpqxk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gubufcfvn.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gpipggapz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gxrdmfwzg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gmuydjhix.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gjueselwl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gsaxyvnyc.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/guthaonzz.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gutkjgugi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/grujqknxc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gxpdghpqn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmvknudg.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gjxbpdxsl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/ginxdnqka.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/glvwkvyvy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gyezaiysl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/ggxktruxo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gjkvbojbf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gqrgmzgen.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gzqutzkzo.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gzrmiymbu.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gwhafnalo.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gwbxakgkv.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/grcpavmle.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gsmyrhiwk.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gxtftqmza.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/grtwxbpll.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gklsnzklt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gldrkhlhs.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gmpzpddtr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/ggxrkbqcx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gwcwzgjxr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gruaedbub.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gmqyehimq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjxaujyml.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gmscqihnk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gkougprhv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gucvgyzpp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/ggnhfknzr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gfiyxxblo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gtwawnfwy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gowacopll.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gbbbaagul.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/guvqitbhh.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/ghzbspoyf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/guvkahcby.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/girfquuyn.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gvqkdthhm.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gsbwbjwyy.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gyhwdvogp.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gzpwdzrzi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gcfdmazgf.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gkpowdifl.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gakaojyiz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gtfvghrmq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gnhmobofb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gtsekqahd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/ggaieffzv.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gtrxteiob.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gemdzmkrd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gvzoddzes.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gcthuiyou.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gjsrihina.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gbvfrcyax.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gichiqztk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gvuvfaibr.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gvfjifoko.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gttgibjel.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gcwghipyi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbaiyyhon.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gngmajzno.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gdubeubzy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gduigkiie.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/giknhvoro.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gwhxkmlvy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gfikoqryk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gqllcwzwv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/garsotmov.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/ggrzvkswr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gposwmjfs.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gzsfxtlip.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gksqduyls.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gwdpyqjuq.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/glxqqfyms.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gkomiejat.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gupowpyvx.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gqlmlyihs.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/grvszcirl.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/ghezazyxc.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/ggcmepmae.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gfhwlzjqj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/grnruvcti.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghmkwjdbn.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gnefbelkz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gvlqejlvs.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gvrvvqkls.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gjtrftjtd.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gnugtjhpy.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gpsjausec.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gzviblecc.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/giytstigo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gxqgrmxpy.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gnuiqqoja.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gdijzasfw.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gvlaxyaow.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxymuodfp.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gphvhkdjx.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/glorkrfzs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gdmitnhbh.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gzgdmzehu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gxdbswwsr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/ghqsnrphi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gfqawsmui.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gdqlmiybg.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gcpqyjboa.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/grifocgrz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/grprlptjj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gyoultwgf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gydsomcdy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/ggpmfbfzw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gedkksnsc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gezhitiwz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gbwbmvtkc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gsuvrvfct.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gxyvqrhxv.sHtML


<!-- 参考信息 -->