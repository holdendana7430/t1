代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xinyue.icu/gtnlsxtwfp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhiwuduotai.top/gtscfolfrc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cashguo.top/gteudcygmz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sxryk.cn/gtfycukyvj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258888.top/gtblumwtxm.html

[B10] 遍历同时拿索引
来源：http://hz.ehwqpu.com/gtivdakcrt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.bjfxy.top/gtibldjtpx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xylfe.cn/gtgvuojaew.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zycfv.cn/gtipswwxtc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhaomingkeji.xyz/gtovmfafcq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.daria6918.cn/gtondunhgi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinghuilouyu.cn/gtyvsuqrqy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.kuanghao11.cn/gtfvffsiyz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinghuilouyu.cn/gtzyggxlcu.html

[B11] 生成数字序列 / 区间
来源：http://hz.daxiang520.top/gtlkxblqud.html

Py:   list(range(0, 10, 2))
来源：http://hz.shanyushiyangkeji.top/gthpzhzbms.html

PHP:  range(0, 10, 2);
来源：http://hz.haohaochexian.top/gtnbdvxcgh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ybcxt.top/gtppltsfmk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gtxmnxiubl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhongyouzk.top/gttieqwpdh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhengqikj.top/gtiytqznvh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hywenlv.cn/gtpzharfrs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenlongwang.top/gtrhyqolhv.html

[B12] 跳出多层循环
来源：http://hz.feifeiyinyue.top/gtugqngnar.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hnxiangtu.top/gtpfyehsvp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xinyue.icu/gtihtlzgom.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtltelwhdw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gtnaqoqkrt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj202588.top/gthwykotgd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.andypj.xyz/gtyriimooy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xziqi.cn/gtxyszatzo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jqgufenzy.top/gtzifvxulw.html

[B13] 判断是否为数字
来源：http://hz.shzxlz.cn/gtgmtrnzdl.html

Py:   isinstance(x, (int, float))
来源：http://hz.c1oappe.top/gtmrdksnnv.html

PHP:  is_numeric($x)
来源：http://hz.daria6918.cn/gtassdcblu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xziqi.cn/gtpudazekm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgfzy.top/gtsyelfzjo.html

Java: x instanceof Number
来源：http://hz.zdqjudy.top/gtkbtytqdg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.havefunace.top/gtucydouje.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhixingplan.top/gtebfneezv.html

C#:   x is int or double or decimal
来源：http://hz.shzxlz.cn/gtgcqbyptg.html

[B14] 判断值是否在集合内
来源：http://hz.wangdashe.top/gtdpqvphsu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.52xcode.cn/gtoncdxxlq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sufxvd.cn/gtqiwruyvg.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.bjfxy.top/gttytvnrfi.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ydjk.org.cn/gtdrqazqot.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhixingplan.top/gthcmlyaoz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinyuanbaomall.cn/gtciacjdhr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cheryme.top/gtdixppyur.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.havefunace.top/gttetjbuop.html

[B15] 布尔运算与取反
来源：http://hz.c1oappe.top/gtqwbcempb.html

Py:   a and b or not c
来源：http://hz.gogol.net.cn/gthimnrmvu.html

PHP:  $a && $b || !$c
来源：http://hz.sufxvd.cn/gtvbujivqs.html

JS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtzcpcmcdy.html

TS:   a && b || !c
来源：http://hz.316326.xyz/gteznlecqn.html

Java: a && b || !c
来源：http://hz.sysykeji.top/gtpmslmeds.html

Go:   a && b || !c
来源：http://hz.aibaodan.cn/gtfqofazzx.html

Ruby: a && b || !c
来源：http://hz.cashguo.top/gtynacfbwl.html

C#:   a && b || !c
来源：http://hz.ybcxt.top/gtsrsroosg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xuetiantiany.cn/gtmnuxqius.html

Py:   if not data: return
来源：http://hz.ydjk.org.cn/gtozxtvluk.html

PHP:  if (!$data) { return; }
来源：http://hz.tanke756.top/gtckabvqen.html

JS:   if (!data) return;
来源：http://hz.xziqi.cn/gtgxrmvvpm.html

TS:   if (!data) return;
来源：http://hz.tian-w.cn/gtsnvgjusw.html

Java: if (data == null) return;
来源：http://hz.pycfn.com/gtatjppknl.html

Go:   if data == nil { return }
来源：http://hz.havefunace.top/gtbhjsekre.html

Ruby: return if data.nil?
来源：http://hz.yonumen.top/gthlusrdtz.html

C#:   if (data == null) return;
来源：http://hz.dianchejie.cn/gtqfbghsmq.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtvwifvins.html

C. 函数与作用域
来源：http://hz.xziqi.cn/gtzvcnapka.html

================================================================================
来源：http://hz.c1oappe.top/gtotbprupi.html

[C01] 定义函数
来源：http://hz.daxiang520.top/gtdyfqwase.html

Py:   def add(a, b): return a + b
来源：http://hz.iojbl.cn/gtasybvrvb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtvhlpvflk.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gtqrrphzyn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangshuangyany.cn/gtbylyyiip.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtrmwtuaqd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guannengcc.top/gtrfgtnkgx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yvedp.cn/gtubsouhvd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yvedp.cn/gtjfahzhau.html

[C02] 默认参数
来源：http://hz.gotoacloud.top/gtwhwtqghq.html

Py:   def greet(name="World"): return name
来源：http://hz.vqdsnc.cn/gthjryzgor.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.daxiang520.top/gtbecithqj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydjk.org.cn/gtuurwdvtr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.0kj1m.cn/gtbvfdukbe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yangfankeji.com/gtfphyfxnc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.daria6918.cn/gtlvdakhax.html

Ruby: def greet(name = "World") = name
来源：http://hz.cashguo.top/gtxxyjsdvc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhengqikj.top/gttfubjfyq.html

[C03] 可变参数
来源：http://hz.xuetiantiany.cn/gtvqulxnju.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhaomingkeji.xyz/gtkzaowhgu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dashuyun.cn/gtfvfjvoxv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shzxlz.cn/gtzpgjmmpy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tanke756.top/gtdrezdpxg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.chenlongwang.top/gtmbfozqwu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.redwolf501.top/gtysfdmvvf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tianlin.xyz/gtzcufciyo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ywan-chungtsiang.top/gtdbeqjotf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yvedp.cn/gtbvqlhpaj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xinyue.icu/gtgxqzxfzj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.0kj1m.cn/gtzqmosnpg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.redwolf501.top/gtkrejfuod.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yongpay.top/gtvkzbewuh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cheryme.top/gtukfbgruv.html

Go:   // 无：用配置结构体参数
来源：http://hz.dianchejie.cn/gtgxszbiws.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tianlin.xyz/gtjbyskrdx.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gtzooijyim.html

[C05] 返回多个值
来源：http://hz.yuxming.cn/gtvczxuryk.html

Py:   return a, b
来源：http://hz.jlsjyb.cn/gteerznvam.html

PHP:  return [$a, $b];
来源：http://hz.ydzc1.top/gtimskaoky.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtbkujcjts.html

TS:   return { a, b };
来源：http://hz.andypj.xyz/gtgodaxkwu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yvedp.cn/gtnsjtfgme.html

Go:   return a, b
来源：http://hz.vqdsnc.cn/gtpngvbtti.html

Ruby: return a, b
来源：http://hz.c1oappe.top/gthlfiawzh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnxiangtu.top/gtuqcnoxsz.html

[C06] 匿名函数 / lambda
来源：http://hz.tianlin.xyz/gttlrcciue.html

Py:   square = lambda x: x * x
来源：http://hz.xuetiantiany.cn/gtwtyzrqqr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.c1oappe.top/gtigaiuibh.html

JS:   const square = x => x * x;
来源：http://hz.hnxiangtu.top/gthlimitho.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ydzc1.top/gtsalpyhdy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.0kj1m.cn/gtohgwsjyt.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xingfuxueyuan.xyz/gtnprecpiq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ywan-chungtsiang.top/gtassfveqt.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yvedp.cn/gtmgxsfelz.html

[C07] 把函数作为参数传入
来源：http://hz.guannengcc.top/gtcjlvcfwj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sufxvd.cn/gtjoluepvd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.mhx1999.top/gthvvmbrfn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhengqikj.top/gtqqlquqmw.html

TS:   arr.map(String)
来源：http://hz.gaohongyu789.top/gthmdluajv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shanyushiyangtech.top/gtqyltwlkt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gzhubu.top/gthnrgittx.html

Ruby: arr.map(&:upcase)
来源：http://hz.svipenyu.cn/gtbiwwvsqa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj20258.top/gtlpydrewi.html

[C08] 闭包
来源：http://hz.zhoulong.xyz/gtyvfwvnst.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.chenjidiqi.icu/gtziqqazyr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinqigufen.top/gtvwzwfxun.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtpxwwlfpb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtsgycvyob.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenzaomai.com/gttfckbgkz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hfpthk.cn/gtzjvgucfh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gotoacloud.top/gthmqiqptg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtbfbdyisx.html

[C09] 递归
来源：http://hz.cdnleiting.top/gtrzrvcbew.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daria6918.cn/gtdvxppdvx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yuxming.cn/gtybgzdcdp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinyuanbaomall.cn/gtsdvorqnd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hfpthk.cn/gtmibxhzha.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.haohaochexian.top/gtyzjwynhe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tianlin.xyz/gtpzpnvmjp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.aibaodan.cn/gtwtjlhmfj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhiwuduotai.top/gtkmxdpfwc.html

[C10] 变量作用域
来源：http://hz.guowangkeji.top/gthirztihi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.wangdashe.top/gtyttihrgo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yangfankeji.com/gtcdwcqmuy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinqigufen.top/gtzqddfaeq.html

TS:   同 JS
来源：http://hz.yvedp.cn/gtfxpmtuob.html

Java: 方法内为块级作用域
来源：http://hz.wangdashe.top/gtmzlvzioc.html

Go:   花括号块级作用域
来源：http://hz.ppjwa.cn/gtropociki.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenzaomai.com/gtddeytxbs.html

C#:   块级作用域
来源：http://hz.redwolf501.top/gtlbzqzsrp.html

[C11] 模块导入与导出
来源：http://hz.chenzaomai.com/gtffufmoff.html

Py:   from module import func
来源：http://hz.andypj.xyz/gtnaghcdmq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yonumen.top/gtqdtbpcuv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.9152youxi.cn/gtwxmqzyev.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhixingplan.top/gtgobzjidb.html

Java: import java.util.List;
来源：http://hz.yj20258.top/gtbocduzly.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhixingplan.top/gtzekvqxla.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.guowangkeji.top/gtreocvwkz.html

C#:   using System.Text;
来源：http://hz.jqgufenzy.top/gtmqtnztmp.html

[C12] 立即执行函数 IIFE
来源：http://hz.shanyushiyangtech.top/gtvenjenym.html

Py:   (lambda: print("run"))()
来源：http://hz.yj20258888.top/gtqvlmtksb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.svipenyu.cn/gteeubkemr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xinyue.icu/gtosacpdds.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sweek.top/gtkgzgvecq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.birdmap.top/gtwoqarnls.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhengqikj.top/gtyabgftjb.html

Ruby: -> { puts "run" }.call
来源：http://hz.nanxuanxn.top/gtomwcxyou.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daxiang520.top/gtfbjrpoma.html

[C13] 类型声明 / 类型注解
来源：http://hz.52xcode.cn/gtoandivcq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.havefunace.top/gtgcikfxur.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gtkevpvcuz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.haohaochexian.top/gtgedjygzu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shzxlz.cn/gturhbjmde.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtyjamiuur.html

Go:   func add(a, b int) int
来源：http://hz.cdnleiting.top/gtzbggawst.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhongyouzk.top/gtoqogtylo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yanxiufei.cn/gtijovozuc.html

[C14] 泛型函数
来源：http://hz.ydzc1.top/gtuebaadql.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ydjk.org.cn/gtklcltlmc.html

PHP:  // 无泛型
来源：http://hz.9152youxi.cn/gtyfgeyevg.html

JS:   // 无泛型
来源：http://hz.jqgufenzy.top/gtwmkvmeog.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hywenlv.cn/gthfrngico.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hnxiangtu.top/gtuniawmuu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.fzhhl.top/gtskvjacdg.html

Ruby: # 无泛型
来源：http://hz.hnxiangtu.top/gtfawoxidq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jyoumei.cn/gtxhshatca.html

[C15] 解构 / 展开参数
来源：http://hz.yongpay.top/gtvcnbjexd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgufenzy.top/gtnswxcpio.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hysaishi.cn/gtggfzygsv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtmlzgerzn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.guannengcc.top/gtgwtnvwto.html

Java: // 无解构
来源：http://hz.zhoulong.xyz/gtcpvipapd.html

Go:   // 无解构
来源：http://hz.yj20258.top/gtikoyenjq.html

Ruby: a, b = pair
来源：http://hz.birdmap.top/gtrzqwrmxc.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangtech.top/gtbsfxqukq.html

[C16] 函数 / 方法重载
来源：http://hz.smart0.xyz/gtzwrzruup.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.redwolf501.top/gtkrkuiosv.html

PHP:  // 无重载
来源：http://hz.daxiang520.top/gtmcogpbbc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cdnleiting.top/gtzrjpfpps.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cucudq.cn/gtjihpblkp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gotoacloud.top/gtpcouwwbk.html

Go:   // 无重载：用不同函数名
来源：http://hz.cucudq.cn/gtjnsnkbtp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhiwuduotai.top/gtyeunglbp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jqgufenzy.top/gtwvfclpqq.html

================================================================================
来源：http://hz.redwolf501.top/gtydctnihi.html

D. 数组 / 列表 / 集合
来源：http://hz.shangyingyoupin.top/gterxkibqd.html

================================================================================
来源：http://hz.xuanzx.com/gtunpejddk.html

[D01] 创建数组 / 列表
来源：http://hz.aizwys.cn/gtzzsrhifm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.andypj.xyz/gthtteftif.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nanxinkj.top/gtrogiujll.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigfzy.top/gtvgunaiqu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhaomingkeji.xyz/gtnpmrgaya.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhengqikj.top/gtehaaadxj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nanxuanxn.top/gtgzcrnfdb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cucudq.cn/gtwtvldtce.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.bjfxy.top/gtyuqqyfzg.html

[D02] 追加元素到末尾
来源：http://hz.zhijiandao.cn/gtofmxkgik.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhiwuduotai.top/gtekqwakgr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guannengcc.top/gtftnehbfn.html

JS:   arr.push(4);
来源：http://hz.jiagoushi.top/gtbcieplkc.html

TS:   arr.push(4);
来源：http://hz.jinqigfzy.top/gtqgvjrabj.html

Java: list.add(4);
来源：http://hz.shangyingyoupin.top/gtbiigqvzo.html

Go:   arr = append(arr, 4)
来源：http://hz.dashuyun.cn/gtsodzazsx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yvedp.cn/gtrtoywwhq.html

C#:   list.Add(4);
来源：http://hz.jqgufenzy.top/gttepmljhi.html

[D03] 在指定位置插入元素
来源：http://hz.sweek.top/gtkawqmvtt.html

Py:   arr.insert(0, 0)
来源：http://hz.hysaishi.cn/gtpkryohjb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nwbrower.top/gtcvsdpftw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ehwqpu.com/gtojjodvhn.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zycfv.cn/gtbxhlxisn.html

Java: list.add(0, 0);
来源：http://hz.sysykeji.top/gtlabmisqg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.havefunace.top/gtlubzegnz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.fzhhl.top/gthcusysga.html

C#:   list.Insert(0, 0);
来源：http://hz.iojbl.cn/gtrrbxyqqq.html

[D04] 删除元素
来源：http://hz.cqqwz.cn/gthjpfyulb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.kuanghao11.cn/gteahcvgjt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinyuanbaomall.cn/gtbkqzsmai.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sufxvd.cn/gtisutlyiu.html

TS:   arr.splice(0, 1);
来源：http://hz.ppjwa.cn/gtxjznxzcv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangshuangyany.cn/gtblwjodlu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.mhx1999.top/gtevywnljf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hysaishi.cn/gtfdplgmva.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xylfe.cn/gtscuftqbk.html

[D05] 访问与修改元素
来源：http://hz.yueranfly.top/gtfjaiyeti.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtwmmxvajx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sweek.top/gtrsxjriuy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cucudq.cn/gtqchidrqn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhongyouzk.top/gtquzjgkaj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.iojbl.cn/gtmuvouhpp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtvnnypokc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtcoiwmmgp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.pycfn.com/gtldncycsw.html

[D06] 数组长度
来源：http://hz.jiagoushi.top/gtyduwxfwz.html

Py:   len(arr)
来源：http://hz.yanxiufei.cn/gtqfttazjq.html

PHP:  count($arr);
来源：http://hz.xylfe.cn/gtjaolqnzs.html

JS:   arr.length
来源：http://hz.andypj.xyz/gtwnsxvxda.html

TS:   arr.length
来源：http://hz.nanxinkj.top/gtxsnqabtm.html

Java: list.size();
来源：http://hz.chenlongwang.top/gtinbauxlb.html

Go:   len(arr)
来源：http://hz.xuetiantiany.cn/gtwuxpqnvh.html

Ruby: arr.length; arr.size
来源：http://hz.chenzaomai.com/gtzhekpzxi.html

C#:   list.Count;
来源：http://hz.aibaodan.cn/gtmsxsyskb.html

[D07] 切片 / 取子数组
来源：http://hz.ydzc1.top/gtxqhkqffx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nwbrower.top/gthmuambwl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.wangdashe.top/gtkpfhgarn.html

JS:   arr.slice(1, 4);
来源：http://hz.cheryme.top/gtscbkpewv.html

TS:   arr.slice(1, 4);
来源：http://hz.yj20258.top/gtzijnzung.html

Java: list.subList(1, 4);
来源：http://hz.0kj1m.cn/gtzzcyggjb.html

Go:   arr[1:4]
来源：http://hz.hnxiangtu.top/gtlmtahlef.html

Ruby: arr[1, 3]
来源：http://hz.cucudq.cn/gtcryzshin.html

C#:   list.GetRange(1, 3);
来源：http://hz.316326.xyz/gtvgwwbtgb.html

[D08] 合并两个数组
来源：http://hz.guowangkeji.top/gttasfxwzx.html

Py:   a + b;  a.extend(b)
来源：http://hz.mhx1999.top/gthahmhxql.html

PHP:  array_merge($a, $b);
来源：http://hz.hongshengwenyu.top/gtegunzkkg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.birdmap.top/gtkvnkyite.html

TS:   [...a, ...b];
来源：http://hz.ydzc1.top/gtlzgnpizy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shzxlz.cn/gtjrilhdwv.html

Go:   append(a, b...)
来源：http://hz.haohaochexian.top/gtwmmysker.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj20258888.top/gtghjgztlo.html

C#:   a.Concat(b).ToList()
来源：http://hz.jqgfzy.top/gtoiwfmbvl.html

[D09] 排序（升序）
来源：http://hz.52xcode.cn/gtyvejtxqt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtloaoigyu.html

PHP:  sort($arr);
来源：http://hz.chenzaomai.com/gtunhrmpwm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tian-w.cn/gtfqkkaysv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jqgfzy.top/gthxlyjsfm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangdashe.top/gtgwszeayo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.pycfn.com/gtrzsiqyut.html

Ruby: arr.sort
来源：http://hz.havefunace.top/gtwyawxnsv.html

C#:   list.Sort();
来源：http://hz.hysaishi.cn/gtjnbubyqm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shanyushiyangkeji.top/gteuxorrqj.html


<!-- 参考信息 -->