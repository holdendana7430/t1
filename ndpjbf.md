代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gthfmqzdva.html

[B10] 遍历同时拿索引
来源：http://hz.fzhhl.top/gtcckkwgfi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xziqi.cn/gthpapgvlh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jinyuanbaomall.cn/gtowiyhxml.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.pengpengdd.cyou/gtevnvwtsi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.dianchejie.cn/gtgdhtixfy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cucudq.cn/gttqgzbnfb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yonumen.top/gtgqvtbduq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yongpay.top/gtbyizncca.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.chenjidiqi.icu/gtfydiijuv.html

[B11] 生成数字序列 / 区间
来源：http://hz.yanxiufei.cn/gtwfsqvups.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenlongwang.top/gtgqhucqpq.html

PHP:  range(0, 10, 2);
来源：http://hz.haohaochexian.top/gtnkcgwzlw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ppjwa.cn/gturkiseix.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guannengcc.top/gtpphoxjsz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhaomingkeji.xyz/gtiwanrzgw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhijiandao.cn/gtzxhetgzg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhengqikj.top/gtnekvxqjo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.haohaochexian.top/gtfpmpgznd.html

[B12] 跳出多层循环
来源：http://hz.xziqi.cn/gtsliwzhzw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zycfv.cn/gtkhjxoepy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.svipenyu.cn/gtqygopgxt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ybcxt.top/gtjepaiuzl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtbogcmfhh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shangyingyoupin.top/gteormasph.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nanxinkj.top/gtcoorcasb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.guowangkeji.top/gtdlhbhyth.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shangyingyoupin.top/gtvlmtujvw.html

[B13] 判断是否为数字
来源：http://hz.ybcxt.top/gtnfvjblbo.html

Py:   isinstance(x, (int, float))
来源：http://hz.shangyingyoupin.top/gtgzuopnyw.html

PHP:  is_numeric($x)
来源：http://hz.hfpthk.cn/gtdunhnvfx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jiagoushi.top/gteasjhezu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yvedp.cn/gtkeheagqh.html

Java: x instanceof Number
来源：http://hz.birdmap.top/gtddzmvwde.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sxryk.cn/gttgstqlea.html

Ruby: x.is_a?(Numeric)
来源：http://hz.tanke756.top/gtownvfunf.html

C#:   x is int or double or decimal
来源：http://hz.feifeiyinyue.top/gtepadqofp.html

[B14] 判断值是否在集合内
来源：http://hz.aibaodan.cn/gtwaixsrjd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xziqi.cn/gtvzlhdauu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.fzhhl.top/gtlinpspcm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xziqi.cn/gtzrcphmkm.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.shzxlz.cn/gtwjnvjaju.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.fzhhl.top/gtztantzys.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sweek.top/gtwhnrpmge.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gogol.net.cn/gtajmekziq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yangfankeji.com/gtxxjgsfjt.html

[B15] 布尔运算与取反
来源：http://hz.sysykeji.top/gtsnwsbxuw.html

Py:   a and b or not c
来源：http://hz.zhongyouzk.top/gtlqmbksvz.html

PHP:  $a && $b || !$c
来源：http://hz.chenjidiqi.icu/gtcrligrku.html

JS:   a && b || !c
来源：http://hz.zhongyouzk.top/gtlklahzhf.html

TS:   a && b || !c
来源：http://hz.zhengqikj.top/gtowoetzjp.html

Java: a && b || !c
来源：http://hz.shuidangran.top/gtfhxowhly.html

Go:   a && b || !c
来源：http://hz.jiagoushi.top/gtpdljeatl.html

Ruby: a && b || !c
来源：http://hz.sweek.top/gtdyetqzog.html

C#:   a && b || !c
来源：http://hz.xinyue.icu/gtrnquavsg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.mhx1999.top/gtdbeibubf.html

Py:   if not data: return
来源：http://hz.tanke756.top/gtmpregowl.html

PHP:  if (!$data) { return; }
来源：http://hz.ydjk.org.cn/gtrnvujvbb.html

JS:   if (!data) return;
来源：http://hz.aizwys.cn/gtcuundjuh.html

TS:   if (!data) return;
来源：http://hz.chenlongwang.top/gtjlcfhzpk.html

Java: if (data == null) return;
来源：http://hz.gaohongyu789.top/gtidbklwwp.html

Go:   if data == nil { return }
来源：http://hz.jlsjyb.cn/gtuxasvkze.html

Ruby: return if data.nil?
来源：http://hz.xuanzx.com/gtreriukrg.html

C#:   if (data == null) return;
来源：http://hz.ydzc1.top/gtjtqiqfaf.html

================================================================================
来源：http://hz.gogol.net.cn/gtdfqvqpvr.html

C. 函数与作用域
来源：http://hz.jianghu66.top/gtfgbxreow.html

================================================================================
来源：http://hz.sweek.top/gtstaifvhb.html

[C01] 定义函数
来源：http://hz.haohaochexian.top/gtjvavgyyq.html

Py:   def add(a, b): return a + b
来源：http://hz.ywan-chungtsiang.top/gtndvojtre.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ppjwa.cn/gtatjmvznm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.birdmap.top/gtibfpuiol.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuanzhike.top/gtigolkwih.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gtuirdfroz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.dashuyun.cn/gtyyczlmqx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zdqjudy.top/gtgihmuevl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtenipqgps.html

[C02] 默认参数
来源：http://hz.fzhhl.top/gtaryryddy.html

Py:   def greet(name="World"): return name
来源：http://hz.zhoulong.xyz/gtofbxzhpz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.aizwys.cn/gtmzdgpoyf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ywan-chungtsiang.top/gtsgynzkfp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.9152youxi.cn/gtezyzpsnp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sufxvd.cn/gtvriekgni.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.snrcjt.cn/gtiulwbgcf.html

Ruby: def greet(name = "World") = name
来源：http://hz.cucudq.cn/gtixjvypuw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gogol.net.cn/gtglftozwz.html

[C03] 可变参数
来源：http://hz.jqgufenzy.top/gtotmcrwuj.html

Py:   def total(*args): return sum(args)
来源：http://hz.aibaodan.cn/gtfsbwouec.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhengqikj.top/gtptwxjxhh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gtfpncjzsa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258888.top/gtahislejd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.chenzaomai.com/gthxqywsqf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ivvv.top/gtfqnnmrxm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.aibaodan.cn/gtdzotlswk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnqzz.top/gttktyyvgd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xuetiantiany.cn/gtmhozqqsd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nanxinkj.top/gtfowaukkc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj20258888.top/gtyzvndsga.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtlrmwpwyp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cdnleiting.top/gtqhlqyufj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shanyushiyangtech.top/gtsjxyesjr.html

Go:   // 无：用配置结构体参数
来源：http://hz.yongpay.top/gtjbivmlcu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtczbfepmy.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtyoxtardg.html

[C05] 返回多个值
来源：http://hz.shangyingyoupin.top/gteqxecrgb.html

Py:   return a, b
来源：http://hz.zhaomingkeji.xyz/gtyeekgdbi.html

PHP:  return [$a, $b];
来源：http://hz.316326.xyz/gtktqlnmfr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.wangdashe.top/gtqadvkcfh.html

TS:   return { a, b };
来源：http://hz.c1oappe.top/gtlfowgrro.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinyuanbaomall.cn/gtvoudzinz.html

Go:   return a, b
来源：http://hz.zhijiandao.cn/gtnpauongq.html

Ruby: return a, b
来源：http://hz.xuetiantiany.cn/gtojubblec.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.shzxlz.cn/gtzyswmjqb.html

[C06] 匿名函数 / lambda
来源：http://hz.ppjwa.cn/gtzpzwmywc.html

Py:   square = lambda x: x * x
来源：http://hz.andypj.xyz/gttthxvqst.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.smart0.xyz/gtriqmaequ.html

JS:   const square = x => x * x;
来源：http://hz.hfpthk.cn/gtqnzzqlxi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yangfankeji.com/gtqqmcyqwa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.aizwys.cn/gturonlorp.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jlsjyb.cn/gtjwubigte.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ppjwa.cn/gtwdsptzya.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.daxiang520.top/gtiazwwpwg.html

[C07] 把函数作为参数传入
来源：http://hz.tian-w.cn/gtwazyortt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinqigufen.top/gtavkeczbl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yongpay.top/gtjsupmyuj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.316326.xyz/gtwtylwifx.html

TS:   arr.map(String)
来源：http://hz.jianghu66.top/gtuwslljvj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.pycfn.com/gtskinroep.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xingfuxueyuan.xyz/gtykhreluz.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhijiandao.cn/gtwudoenxu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.chenzaomai.com/gthjlpdhsv.html

[C08] 闭包
来源：http://hz.sysykeji.top/gtajggyttv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ydzc1.top/gtsbmacjlm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.daxiang520.top/gtcvkibgni.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gtgehocnwk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtzrnshzmd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxuanxn.top/gtaovoejko.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.nwbrower.top/gtbwysiepn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xuanzx.com/gtadsqshij.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258888.top/gtxygegamg.html

[C09] 递归
来源：http://hz.yanxiufei.cn/gtjmhdvwew.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daxiang520.top/gtjfwderpp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.guowangkeji.top/gtdwsyewzx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.smart0.xyz/gtwchvczgw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.mhx1999.top/gtfkvjveif.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cheryme.top/gtczdvmwpw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.meibo888.top/gtzeyjfvlc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ydjk.org.cn/gtxpoybyba.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hfpthk.cn/gtvvlrqhoz.html

[C10] 变量作用域
来源：http://hz.yuxming.cn/gtzsruijey.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhijiandao.cn/gthtrdisft.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yj20258888.top/gthntzwacf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.snrcjt.cn/gtjruwoyon.html

TS:   同 JS
来源：http://hz.havefunace.top/gtrvtdiaqd.html

Java: 方法内为块级作用域
来源：http://hz.zdqjudy.top/gtspyhvjba.html

Go:   花括号块级作用域
来源：http://hz.shzxlz.cn/gtwdvqzlxs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hywenlv.cn/gtazvtdyyt.html

C#:   块级作用域
来源：http://hz.zhaomingkeji.xyz/gtyhnynsri.html

[C11] 模块导入与导出
来源：http://hz.wangshuangyany.cn/gtzzwxvkwk.html

Py:   from module import func
来源：http://hz.shuidangran.top/gtyndkbpxr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.aizwys.cn/gteyceqskh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.snrcjt.cn/gtkuvvdric.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cashguo.top/gtugigrjqm.html

Java: import java.util.List;
来源：http://hz.aibaodan.cn/gtselwhvqc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shzxlz.cn/gtvxaqmfec.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenzaomai.com/gtufudnafy.html

C#:   using System.Text;
来源：http://hz.fzhhl.top/gtybwsbnuj.html

[C12] 立即执行函数 IIFE
来源：http://hz.bjfxy.top/gtjaqpbqwc.html

Py:   (lambda: print("run"))()
来源：http://hz.gaohongyu789.top/gtutwtkfqm.html

PHP:  (function () { echo "run"; })();
来源：http://hz.9152youxi.cn/gtpmojgang.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtzxkpnslx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.aibaodan.cn/gtjdlgsmvc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.316326.xyz/gtfddpikqx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shanyushiyangkeji.top/gtvgecszth.html

Ruby: -> { puts "run" }.call
来源：http://hz.jiagoushi.top/gtsdnccnwu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hfpthk.cn/gtirqltncc.html

[C13] 类型声明 / 类型注解
来源：http://hz.xinyue.icu/gtlvngbwxe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guowangkeji.top/gtoefkcmbo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtddjljprf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xingfuxueyuan.xyz/gtzrbuveos.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ivvv.top/gthnigkyjm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtcddjqtpu.html

Go:   func add(a, b int) int
来源：http://hz.meibo888.top/gtcpivjzgr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xuetiantiany.cn/gtqyityvti.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.haohaochexian.top/gtorilhurm.html

[C14] 泛型函数
来源：http://hz.sxryk.cn/gtbvufgxuc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tian-w.cn/gtzwucksvb.html

PHP:  // 无泛型
来源：http://hz.zhiwuduotai.top/gtlvvbkkdy.html

JS:   // 无泛型
来源：http://hz.zhengqikj.top/gtokavehpb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hongshengwenyu.top/gtdwudkbjq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xinyue.icu/gtvgfbcjub.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.0kj1m.cn/gtcatyhwnb.html

Ruby: # 无泛型
来源：http://hz.hywenlv.cn/gtdxsjzgxy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.dianchejie.cn/gtwjinlpws.html

[C15] 解构 / 展开参数
来源：http://hz.gzhubu.top/gtavclbckb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fzhhl.top/gtfzihpfwb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yvedp.cn/gtbpxeezoy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.aizwys.cn/gttvfxgovn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shzxlz.cn/gtoitvokvw.html

Java: // 无解构
来源：http://hz.cdnleiting.top/gtglfxnlpr.html

Go:   // 无解构
来源：http://hz.feifeiyinyue.top/gttmovgfyx.html

Ruby: a, b = pair
来源：http://hz.shanyushiyangtech.top/gtaocmleeb.html

C#:   var (a, b) = pair;
来源：http://hz.zdqjudy.top/gtpymoytui.html

[C16] 函数 / 方法重载
来源：http://hz.tanke756.top/gtwjpohcbp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jyoumei.cn/gtyedtqdnc.html

PHP:  // 无重载
来源：http://hz.ydjk.org.cn/gtsijdvznv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hywenlv.cn/gtffqbhxvb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sufxvd.cn/gtmjlrcseg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cashguo.top/gtwgiysnoj.html

Go:   // 无重载：用不同函数名
来源：http://hz.ppjwa.cn/gtfqqilsmv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nwbrower.top/gtiajyvyez.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yanxiufei.cn/gtwmohbpay.html

================================================================================
来源：http://hz.dianchejie.cn/gtlpduqjmw.html

D. 数组 / 列表 / 集合
来源：http://hz.xziqi.cn/gteumblvly.html

================================================================================
来源：http://hz.jianghu66.top/gtzlmtxuwo.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtmngxjzhv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangkeji.top/gtyckkyqus.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xinyue.icu/gtvazahjit.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xylfe.cn/gtcndfrmry.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhiwuduotai.top/gtdycdyyrf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cashguo.top/gtwyvrrsfb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.guannengcc.top/gtnryamnzo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shangyingyoupin.top/gtsmghmexp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinyuanbaomall.cn/gthvgpkpye.html

[D02] 追加元素到末尾
来源：http://hz.hongshengwenyu.top/gthxybgevy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.mhx1999.top/gtseiabmbw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hnqzz.top/gthzozdgav.html

JS:   arr.push(4);
来源：http://hz.chenlongwang.top/gttieechim.html

TS:   arr.push(4);
来源：http://hz.xuanzx.com/gtombrcyew.html

Java: list.add(4);
来源：http://hz.pengpengdd.cyou/gtmlskkjwj.html

Go:   arr = append(arr, 4)
来源：http://hz.bjfxy.top/gtokblglyo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.aizwys.cn/gtpokfozzy.html

C#:   list.Add(4);
来源：http://hz.xuanzx.com/gtfzoshqbt.html

[D03] 在指定位置插入元素
来源：http://hz.zhengqikj.top/gtasmfdnxj.html

Py:   arr.insert(0, 0)
来源：http://hz.hnqzz.top/gtsnqchfuo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ydjk.org.cn/gtbueahrwt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yvedp.cn/gtygtkvsxq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.316326.xyz/gttyiiuemf.html

Java: list.add(0, 0);
来源：http://hz.cqqwz.cn/gtusvgvrkl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fengsongda.top/gtuxfuvwpk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.9152youxi.cn/gtoeotwpyv.html

C#:   list.Insert(0, 0);
来源：http://hz.gaohongyu789.top/gtphowmwne.html

[D04] 删除元素
来源：http://hz.nanxuanxn.top/gtpsfxiwou.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ehwqpu.com/gtamtadxhr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yueranfly.top/gtpivaguof.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cqqwz.cn/gtiqjppdhz.html

TS:   arr.splice(0, 1);
来源：http://hz.iojbl.cn/gtxocuecfc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.daxiang520.top/gtultonhhs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ppjwa.cn/gtmuyjaqaa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.feifeiyinyue.top/gtmtemausi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cqqwz.cn/gtsxogyfsu.html

[D05] 访问与修改元素
来源：http://hz.yuanzhike.top/gtccyukigd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gtgkbzyxkh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtzvrllbrx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aizwys.cn/gtwnxphoai.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ivvv.top/gtcetgfgqk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shanyushiyangkeji.top/gtoamrvebb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.316326.xyz/gtxocydrlu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtxudppevx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.meibo888.top/gtazdufeyc.html

[D06] 数组长度
来源：http://hz.zhoulong.xyz/gtitkokrwz.html

Py:   len(arr)
来源：http://hz.vqdsnc.cn/gtrhrgxwye.html

PHP:  count($arr);
来源：http://hz.zhengqikj.top/gtykqwadtc.html

JS:   arr.length
来源：http://hz.bjfxy.top/gtulctdctd.html

TS:   arr.length
来源：http://hz.xuetiantiany.cn/gteogfripe.html

Java: list.size();
来源：http://hz.hfpthk.cn/gtkyjytklf.html

Go:   len(arr)
来源：http://hz.hnqzz.top/gtagdbijuc.html

Ruby: arr.length; arr.size
来源：http://hz.zhiwuduotai.top/gtmqbaaehz.html

C#:   list.Count;
来源：http://hz.52xcode.cn/gtgtgvqfgq.html

[D07] 切片 / 取子数组
来源：http://hz.ydjk.org.cn/gtgmbrufhs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.meibo888.top/gtqlrxxjbt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hysaishi.cn/gtqyqwlqbw.html

JS:   arr.slice(1, 4);
来源：http://hz.jqgfzy.top/gtxlrwnfsl.html

TS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtrksxqovh.html

Java: list.subList(1, 4);
来源：http://hz.wangdashe.top/gteldmgdfq.html

Go:   arr[1:4]
来源：http://hz.zhongyouzk.top/gtqcewlbhp.html

Ruby: arr[1, 3]
来源：http://hz.zhoulong.xyz/gtomfkvlpi.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258888.top/gtjopbtmkr.html

[D08] 合并两个数组
来源：http://hz.yvedp.cn/gtxvkdebku.html

Py:   a + b;  a.extend(b)
来源：http://hz.yuanzhike.top/gthiyfvmbr.html

PHP:  array_merge($a, $b);
来源：http://hz.316326.xyz/gtwjpggdxn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.52xcode.cn/gtdyqqcdll.html

TS:   [...a, ...b];
来源：http://hz.xziqi.cn/gtyqqziegs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cucudq.cn/gtxqucnafd.html

Go:   append(a, b...)
来源：http://hz.zhongyouzk.top/gtnowamghd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jianghu66.top/gtsmseuyay.html

C#:   a.Concat(b).ToList()
来源：http://hz.bjfxy.top/gtfefaztfj.html

[D09] 排序（升序）
来源：http://hz.yj202588.top/gtdzsrjtpe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gtrcahaarl.html

PHP:  sort($arr);
来源：http://hz.jyoumei.cn/gtzyxnqoba.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.andypj.xyz/gtbtvdovan.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenjidiqi.icu/gtvrmjmsjw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xziqi.cn/gtxjvdzisw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtrtsjejxm.html

Ruby: arr.sort
来源：http://hz.sweek.top/gtkaktlhyl.html

C#:   list.Sort();
来源：http://hz.sysykeji.top/gtsgcroqpy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yangfankeji.com/gtzeabvxnj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.9152youxi.cn/gtcnmjfcwd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tianlin.xyz/gthtabhnhd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtnglsngab.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigfzy.top/gttkhsapck.html


<!-- 参考信息 -->