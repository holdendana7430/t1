代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ivvv.top/gtozymhliv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.smart0.xyz/gtrheytbvc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ppjwa.cn/gtbbmkjosr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shuidangran.top/gtshrzjaxs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yanxiufei.cn/gtyqfdmbpg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.quarkkingdee.top/gtrmqoumlc.html

[B11] 生成数字序列 / 区间
来源：http://hz.smart0.xyz/gtfqamrxwe.html

Py:   list(range(0, 10, 2))
来源：http://hz.ehwqpu.com/gtndltuyzf.html

PHP:  range(0, 10, 2);
来源：http://hz.iojbl.cn/gtbezyxdlq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xinyue.icu/gtctvfiuxb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ybcxt.top/gtwednhmfk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.andypj.xyz/gtseneknks.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sxryk.cn/gtzauegdri.html

Ruby: (0...10).step(2).to_a
来源：http://hz.0kj1m.cn/gtfqkjphow.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tian-w.cn/gtwzujxcna.html

[B12] 跳出多层循环
来源：http://hz.chenlongwang.top/gtroyaeajj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nwbrower.top/gtsruyzjes.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinghuilouyu.cn/gtlcdohilw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtcjutqdco.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pycfn.com/gtfrrqivxs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtfronidkd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xuetiantiany.cn/gteaklszig.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fengsongda.top/gtdvokdhoc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.9152youxi.cn/gtkvswlprk.html

[B13] 判断是否为数字
来源：http://hz.nwbrower.top/gtxewtsxgd.html

Py:   isinstance(x, (int, float))
来源：http://hz.shanyushiyangkeji.top/gtaubxifdu.html

PHP:  is_numeric($x)
来源：http://hz.ehwqpu.com/gtavjoudyp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yonumen.top/gttvtvptae.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.snrcjt.cn/gtlqenpyah.html

Java: x instanceof Number
来源：http://hz.wangshuangyany.cn/gtftradtuj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhixingplan.top/gtmnjywarg.html

Ruby: x.is_a?(Numeric)
来源：http://hz.tian-w.cn/gtpgpbspwh.html

C#:   x is int or double or decimal
来源：http://hz.zycfv.cn/gtstvkkweu.html

[B14] 判断值是否在集合内
来源：http://hz.cqqwz.cn/gttqiwwvjw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shangyingyoupin.top/gtlniyrvru.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shangyingyoupin.top/gtktyrtkay.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ppjwa.cn/gtbfcdogug.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cdnleiting.top/gtueaizbwr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ywan-chungtsiang.top/gttihpsvjv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.daxiang520.top/gttiwcwyow.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gotoacloud.top/gtaljvpmah.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenjidiqi.icu/gthcgkasdh.html

[B15] 布尔运算与取反
来源：http://hz.cdnleiting.top/gtpvpnvshf.html

Py:   a and b or not c
来源：http://hz.yj20258888.top/gtnyuyagni.html

PHP:  $a && $b || !$c
来源：http://hz.xingfuxueyuan.xyz/gtbluwwgvc.html

JS:   a && b || !c
来源：http://hz.jiagoushi.top/gtdtoacric.html

TS:   a && b || !c
来源：http://hz.ydzc1.top/gtfneaboef.html

Java: a && b || !c
来源：http://hz.cheryme.top/gtppkhekpi.html

Go:   a && b || !c
来源：http://hz.gaohongyu789.top/gtzwnhkhts.html

Ruby: a && b || !c
来源：http://hz.jinqigufen.top/gtwzkxxmjx.html

C#:   a && b || !c
来源：http://hz.yj20258.top/gtqyqtwkhz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.mhx1999.top/gtpefdncon.html

Py:   if not data: return
来源：http://hz.tian-w.cn/gtfwbanggj.html

PHP:  if (!$data) { return; }
来源：http://hz.wangshuangyany.cn/gtihwkqyjb.html

JS:   if (!data) return;
来源：http://hz.shzxlz.cn/gtadxxqhko.html

TS:   if (!data) return;
来源：http://hz.yj202588.top/gttnkapepb.html

Java: if (data == null) return;
来源：http://hz.havefunace.top/gtzwaroifq.html

Go:   if data == nil { return }
来源：http://hz.zhengqikj.top/gtlyhbfykw.html

Ruby: return if data.nil?
来源：http://hz.sxryk.cn/gtttdvkysu.html

C#:   if (data == null) return;
来源：http://hz.sxryk.cn/gtffgjzzlg.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtsqollrzh.html

C. 函数与作用域
来源：http://hz.jqgufenzy.top/gtfpcxzxhk.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtfcvyrvas.html

[C01] 定义函数
来源：http://hz.cheryme.top/gtxsvgymcu.html

Py:   def add(a, b): return a + b
来源：http://hz.xuetiantiany.cn/gtlhflbojh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtorxeotjc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.mhx1999.top/gtpalexdrk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yueranfly.top/gtfrbwjtuk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.fengsongda.top/gtoocyuibj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pycfn.com/gtwoaumbwb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.9152youxi.cn/gtmnxzhmmq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtmtwhozuu.html

[C02] 默认参数
来源：http://hz.nanxuanxn.top/gtctrreynq.html

Py:   def greet(name="World"): return name
来源：http://hz.fengsongda.top/gtabfodanz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tianlin.xyz/gtlnwekiia.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.bjfxy.top/gtjztrdtbk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hnqzz.top/gtwycmlonj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj20258888.top/gtnglrrlmk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.pengpengdd.cyou/gtkjbflxhz.html

Ruby: def greet(name = "World") = name
来源：http://hz.dashuyun.cn/gtugqkewuy.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sxryk.cn/gtflkflmil.html

[C03] 可变参数
来源：http://hz.guannengcc.top/gtywjpxtxv.html

Py:   def total(*args): return sum(args)
来源：http://hz.cucudq.cn/gttwdzmibh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shuidangran.top/gtffwrvgnx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fengsongda.top/gtzlhtdmdl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cucudq.cn/gtzaozguxo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yj20258888.top/gtuygcgzge.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.aibaodan.cn/gtapqkaynn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hnqzz.top/gtzhkqtpio.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.nanxuanxn.top/gtndqqrmpv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.dashuyun.cn/gtzsqzehfa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinghuilouyu.cn/gtfzyayagy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenjidiqi.icu/gtkfbcncik.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gtzjhhidzj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.0kj1m.cn/gtsydtzbbu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yuxming.cn/gtjnixtubu.html

Go:   // 无：用配置结构体参数
来源：http://hz.quarkkingdee.top/gtkdkyqjas.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtltlxxydw.html

C#:   f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtfqifiiur.html

[C05] 返回多个值
来源：http://hz.yongpay.top/gtdqtpeebs.html

Py:   return a, b
来源：http://hz.vqdsnc.cn/gtfetoyfje.html

PHP:  return [$a, $b];
来源：http://hz.jqgfzy.top/gtxcauafff.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.52xcode.cn/gtumvbqqia.html

TS:   return { a, b };
来源：http://hz.jinyuanbaomall.cn/gtvykxbbnz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ywan-chungtsiang.top/gtuwvzvpvw.html

Go:   return a, b
来源：http://hz.vqdsnc.cn/gttxzuralm.html

Ruby: return a, b
来源：http://hz.hywenlv.cn/gtmyyzfmsc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cashguo.top/gtwgwrgzsf.html

[C06] 匿名函数 / lambda
来源：http://hz.hfpthk.cn/gtsylyjhdg.html

Py:   square = lambda x: x * x
来源：http://hz.yj202588.top/gtpnfcircm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj20258.top/gtqpfzqelc.html

JS:   const square = x => x * x;
来源：http://hz.jqgufenzy.top/gtqkcdsvbr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cqqwz.cn/gtuadficxr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hysaishi.cn/gtlzzxwlrd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.daxiang520.top/gtntieqnrk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.mhx1999.top/gtnudezvwv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dashuyun.cn/gtpcjgfvgl.html

[C07] 把函数作为参数传入
来源：http://hz.andypj.xyz/gtdvxyurln.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gotoacloud.top/gtcpdzeblm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.redwolf501.top/gtmimynjay.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.smart0.xyz/gtwnhlioan.html

TS:   arr.map(String)
来源：http://hz.guowangkeji.top/gtbjijfvxb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jinyuanbaomall.cn/gtbzccenmc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sysykeji.top/gtadnvjdor.html

Ruby: arr.map(&:upcase)
来源：http://hz.yueranfly.top/gtquwpzbud.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtockbhymh.html

[C08] 闭包
来源：http://hz.redwolf501.top/gtjskplkao.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yonumen.top/gthzixwqjv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gzhubu.top/gtmtrizpuy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtxlfpxokt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtigphnshe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenlongwang.top/gtoscjxqpq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhijiandao.cn/gtqigcrdyy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangtech.top/gtizfnypzd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gtxslaueaw.html

[C09] 递归
来源：http://hz.xingfuxueyuan.xyz/gtixjmfwvj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hnqzz.top/gtyobjxuwi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtnxpsqadd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuetiantiany.cn/gtrkscpfsk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gtadezthtz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.fengsongda.top/gthnnaxgaz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhixingplan.top/gtxtzsqzfo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sysykeji.top/gtwkrtidxz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jianghu66.top/gtrwmopchx.html

[C10] 变量作用域
来源：http://hz.tanke756.top/gtobrobvbt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jiagoushi.top/gteallacaw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yuxming.cn/gtqbgezvih.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yonumen.top/gtplcdbigo.html

TS:   同 JS
来源：http://hz.dashuyun.cn/gtokylfgtv.html

Java: 方法内为块级作用域
来源：http://hz.feifeiyinyue.top/gtdllwebun.html

Go:   花括号块级作用域
来源：http://hz.shangyingyoupin.top/gtmqutuwza.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.redwolf501.top/gtorkfznwk.html

C#:   块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtwwcehdnh.html

[C11] 模块导入与导出
来源：http://hz.snrcjt.cn/gtezkehmqy.html

Py:   from module import func
来源：http://hz.jinghuilouyu.cn/gtsicdvdne.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.meibo888.top/gtymfnchxf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cashguo.top/gtfnobeuip.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.pengpengdd.cyou/gtppxnbzhz.html

Java: import java.util.List;
来源：http://hz.sweek.top/gtrrpuanhr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.kuanghao11.cn/gtkowbbfta.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.guannengcc.top/gtrlrcoozb.html

C#:   using System.Text;
来源：http://hz.xziqi.cn/gtyjmtweki.html

[C12] 立即执行函数 IIFE
来源：http://hz.aibaodan.cn/gtybrjkkeu.html

Py:   (lambda: print("run"))()
来源：http://hz.c1oappe.top/gtwijqkurl.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pycfn.com/gtgwhcpcvk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtslxkpilp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gtwgegxenj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sufxvd.cn/gtinqaryjs.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gaohongyu789.top/gtvurqetyo.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhengqikj.top/gtbqyuchsm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.snrcjt.cn/gtqpfphmpz.html

[C13] 类型声明 / 类型注解
来源：http://hz.guannengcc.top/gtypyxvtgp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.smart0.xyz/gtjucmrdei.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtwkobxtof.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenjidiqi.icu/gtljbpjryb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ehwqpu.com/gtcxszqlde.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gthlnawnhy.html

Go:   func add(a, b int) int
来源：http://hz.jinghuilouyu.cn/gtoyhctstx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.daxiang520.top/gtrtddragc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daxiang520.top/gtbasnkoyd.html

[C14] 泛型函数
来源：http://hz.jinghuilouyu.cn/gtyvkjgiww.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenlongwang.top/gtqyfciqxn.html

PHP:  // 无泛型
来源：http://hz.52xcode.cn/gtvuzfjoup.html

JS:   // 无泛型
来源：http://hz.quarkkingdee.top/gtcvgiqnxh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hfpthk.cn/gtyqkhsjhb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.aibaodan.cn/gtvbhimrqk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sweek.top/gthbkrukuh.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gtluulshob.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fengsongda.top/gteehhioem.html

[C15] 解构 / 展开参数
来源：http://hz.yonumen.top/gtpopzyrxj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hnxiangtu.top/gtwduwdvao.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnqzz.top/gtfcsjbbti.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtwozsejmn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ydjk.org.cn/gtybneocmo.html

Java: // 无解构
来源：http://hz.dashuyun.cn/gtaimfqsfl.html

Go:   // 无解构
来源：http://hz.xuanzx.com/gtngrhkyxu.html

Ruby: a, b = pair
来源：http://hz.gzhubu.top/gtyykydszx.html

C#:   var (a, b) = pair;
来源：http://hz.gaohongyu789.top/gtecelwbnf.html

[C16] 函数 / 方法重载
来源：http://hz.xuetiantiany.cn/gtaizlmiru.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cucudq.cn/gtrgqudhtk.html

PHP:  // 无重载
来源：http://hz.quarkkingdee.top/gtvlzjnjyf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ehwqpu.com/gtduxtlhbv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hongshengwenyu.top/gttazbmpyn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.daria6918.cn/gtfknjedma.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhoulong.xyz/gtxpebiqeg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.snrcjt.cn/gtylmazafi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shanyushiyangtech.top/gttoenydgn.html

================================================================================
来源：http://hz.cucudq.cn/gtmpdhqlib.html

D. 数组 / 列表 / 集合
来源：http://hz.sysykeji.top/gtvtbqvpqj.html

================================================================================
来源：http://hz.0kj1m.cn/gtwcdtvopp.html

[D01] 创建数组 / 列表
来源：http://hz.yj20258888.top/gtxjqsqate.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zycfv.cn/gttlveorlt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenjidiqi.icu/gtehcfckho.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ybcxt.top/gtigottqeh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cdnleiting.top/gttgyjygrt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuanzhike.top/gthfjygbdx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.haohaochexian.top/gtqoeqpmvw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.52xcode.cn/gtcvpfrslp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhoulong.xyz/gtaqxzgqjk.html

[D02] 追加元素到末尾
来源：http://hz.snrcjt.cn/gtfsvrwnmm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gotoacloud.top/gtzmicxblo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cashguo.top/gtdtcehpyo.html

JS:   arr.push(4);
来源：http://hz.jqgfzy.top/gtezqzfust.html

TS:   arr.push(4);
来源：http://hz.52xcode.cn/gthgnewexe.html

Java: list.add(4);
来源：http://hz.vqdsnc.cn/gtqfrxayzl.html

Go:   arr = append(arr, 4)
来源：http://hz.birdmap.top/gtuwhmocbd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.dianchejie.cn/gtvxwkiozt.html

C#:   list.Add(4);
来源：http://hz.sysykeji.top/gtzddklzld.html

[D03] 在指定位置插入元素
来源：http://hz.feifeiyinyue.top/gtokuxxodv.html

Py:   arr.insert(0, 0)
来源：http://hz.smart0.xyz/gttdfubqkn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pengpengdd.cyou/gttaguowmy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.guowangkeji.top/gtqbzobyhi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenlongwang.top/gtigdpxype.html

Java: list.add(0, 0);
来源：http://hz.tianlin.xyz/gtiwqfvyhx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aizwys.cn/gtewovfnwn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.daxiang520.top/gtywxxwxqn.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258888.top/gtrakqcsmm.html

[D04] 删除元素
来源：http://hz.sufxvd.cn/gtkougiias.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.mhx1999.top/gtdkeabfbg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.aizwys.cn/gtvvzdeubh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cucudq.cn/gtbayhbnbv.html

TS:   arr.splice(0, 1);
来源：http://hz.cdnleiting.top/gtufjhzmwp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gzhubu.top/gtmvxanext.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ywan-chungtsiang.top/gtyswjwmgj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hywenlv.cn/gtdnsqzesa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhengqikj.top/gtvauxtwre.html

[D05] 访问与修改元素
来源：http://hz.zhongyouzk.top/gtyiirlexx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aizwys.cn/gtskzqgggd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zycfv.cn/gtkdiefhfe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tanke756.top/gtfijwsnoe.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinqigfzy.top/gtcgwoitus.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenjidiqi.icu/gtegllhrac.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gzhubu.top/gtgdjtmjob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtlsjiacvc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.quarkkingdee.top/gtgcigvffc.html

[D06] 数组长度
来源：http://hz.jqgfzy.top/gtaorbzdci.html

Py:   len(arr)
来源：http://hz.ybcxt.top/gtzpwekvyt.html

PHP:  count($arr);
来源：http://hz.chenzaomai.com/gtvnuhjsou.html

JS:   arr.length
来源：http://hz.xinyue.icu/gtppqiarml.html

TS:   arr.length
来源：http://hz.xuetiantiany.cn/gtzjflhdnx.html

Java: list.size();
来源：http://hz.tanke756.top/gtfyqcxauh.html

Go:   len(arr)
来源：http://hz.nanxinkj.top/gtkfomppag.html

Ruby: arr.length; arr.size
来源：http://hz.jqgufenzy.top/gtkbsiavns.html

C#:   list.Count;
来源：http://hz.52xcode.cn/gtgzmemsbm.html

[D07] 切片 / 取子数组
来源：http://hz.gaohongyu789.top/gtjiylyzhu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ppjwa.cn/gtqqzqpkex.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fengsongda.top/gtehkkpzvg.html

JS:   arr.slice(1, 4);
来源：http://hz.316326.xyz/gtubpqnbsi.html

TS:   arr.slice(1, 4);
来源：http://hz.hnxiangtu.top/gtfggdvdvj.html

Java: list.subList(1, 4);
来源：http://hz.meibo888.top/gtvunodsnm.html

Go:   arr[1:4]
来源：http://hz.wangshuangyany.cn/gtdbzxwplm.html

Ruby: arr[1, 3]
来源：http://hz.jqgufenzy.top/gtnanvbrah.html

C#:   list.GetRange(1, 3);
来源：http://hz.jqgufenzy.top/gtvipptkdf.html

[D08] 合并两个数组
来源：http://hz.jinyuanbaomall.cn/gtnzjdkfuk.html

Py:   a + b;  a.extend(b)
来源：http://hz.wangdashe.top/gtjcirrcht.html

PHP:  array_merge($a, $b);
来源：http://hz.jianghu66.top/gtrsmkotnc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.iojbl.cn/gtpdbcihks.html

TS:   [...a, ...b];
来源：http://hz.hywenlv.cn/gtyqqlmvhm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gzhubu.top/gtaustlgob.html

Go:   append(a, b...)
来源：http://hz.nanxuanxn.top/gthkfxkyqt.html

Ruby: a + b;  a.concat(b)
来源：http://hz.haohaochexian.top/gtsxxtpvvl.html

C#:   a.Concat(b).ToList()
来源：http://hz.svipenyu.cn/gtsgddtdtg.html

[D09] 排序（升序）
来源：http://hz.hnqzz.top/gtrhmgjckt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtajokhrht.html

PHP:  sort($arr);
来源：http://hz.dashuyun.cn/gttcfplkcv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jinqigufen.top/gtgtwekhmk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xingfuxueyuan.xyz/gtahkwyukh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cdnleiting.top/gtmgrfbjef.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj202588.top/gtvfiuxuhe.html

Ruby: arr.sort
来源：http://hz.sufxvd.cn/gtmbmumgkq.html

C#:   list.Sort();
来源：http://hz.0kj1m.cn/gtuvpyrqfx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yangfankeji.com/gttnrszkja.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj20258.top/gtisqqzuek.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgfzy.top/gtkparkphz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtqrycqgzs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtgcfulowl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.guowangkeji.top/gtxnvogvzy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jlsjyb.cn/gtdmslqbgg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj20258888.top/gtmvqnjctt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shuidangran.top/gtrhkldehc.html


<!-- 参考信息 -->