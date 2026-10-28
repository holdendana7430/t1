代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hnxiangtu.top/gtpljmhfwq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yuanzhike.top/gtdjdmebqo.html

[B07] while 循环
来源：http://hz.zhongyouzk.top/gtjemboliv.html

Py:   while i < 10: i += 1
来源：http://hz.bjfxy.top/gtkbmvdtme.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.meibo888.top/gtxllqjgpq.html

JS:   while (i < 10) { i++; }
来源：http://hz.yuxming.cn/gthmyqpaej.html

TS:   while (i < 10) { i++; }
来源：http://hz.nwbrower.top/gthfaiaxno.html

Java: while (i < 10) { i++; }
来源：http://hz.yuxming.cn/gtiaipvqal.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xingfuxueyuan.xyz/gtpdzzetol.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xinyue.icu/gtpnvranmu.html

C#:   while (i < 10) { i++; }
来源：http://hz.dianchejie.cn/gtdlwblppd.html

[B08] do-while（至少执行一次）
来源：http://hz.yuxming.cn/gtlgrruhlw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.dashuyun.cn/gtdxfnnkap.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zycfv.cn/gtpctxgdxy.html

JS:   do { i++; } while (i < 10);
来源：http://hz.fengsongda.top/gtyvlbkatz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtautntjco.html

Java: do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gtqwlmlmku.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.fengsongda.top/gtjsgaznxs.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ydjk.org.cn/gtnfbrtbij.html

C#:   do { i++; } while (i < 10);
来源：http://hz.birdmap.top/gtckvkyiff.html

[B09] break 与 continue
来源：http://hz.smart0.xyz/gtpfkkqlhf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.fengsongda.top/gtweuovpwh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yangfankeji.com/gtnbmcwyzo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gtntpedhgr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxinkj.top/gtosujeisx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhengqikj.top/gtdbkoquzu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zdqjudy.top/gtyawmpvzs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.chenjidiqi.icu/gtfoutngks.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtvesyywcr.html

[B10] 遍历同时拿索引
来源：http://hz.gogol.net.cn/gtplaaswkc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cdnleiting.top/gttlnaafuf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhixingplan.top/gtirrutjwm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.aibaodan.cn/gtviocnwgf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sweek.top/gtkflufysc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hywenlv.cn/gtmgcfswzl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hysaishi.cn/gtamsaalrn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cheryme.top/gtxybubbnk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sufxvd.cn/gttbzvaqug.html

[B11] 生成数字序列 / 区间
来源：http://hz.cashguo.top/gtcmyxfuqi.html

Py:   list(range(0, 10, 2))
来源：http://hz.cheryme.top/gtzcpiemye.html

PHP:  range(0, 10, 2);
来源：http://hz.hnqzz.top/gtgwhtresd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xuetiantiany.cn/gtwnirstco.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guannengcc.top/gtyhnnvddf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cheryme.top/gtqhtxuqvf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ppjwa.cn/gtkbtrthov.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenjidiqi.icu/gtrqbqogvv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xylfe.cn/gtupyzrdfs.html

[B12] 跳出多层循环
来源：http://hz.shuidangran.top/gttkzvrbjr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yuanzhike.top/gtqukmkyet.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.andypj.xyz/gtnjhrbydb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinghuilouyu.cn/gtazmzlxyg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hysaishi.cn/gtgjysujdh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yvedp.cn/gtmjmwubjd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yuanzhike.top/gtnaccwvnt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cdnleiting.top/gtmxpontnx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.316326.xyz/gtcmgikvaw.html

[B13] 判断是否为数字
来源：http://hz.kuanghao11.cn/gtulswjgvs.html

Py:   isinstance(x, (int, float))
来源：http://hz.guowangkeji.top/gtjjbpjghw.html

PHP:  is_numeric($x)
来源：http://hz.xinyue.icu/gtwyyylomt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ehwqpu.com/gtswrxwkdm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xingfuxueyuan.xyz/gtvzzmugyc.html

Java: x instanceof Number
来源：http://hz.daxiang520.top/gttdswkamb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jlsjyb.cn/gtnwxvqeut.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sxryk.cn/gtnxuobndm.html

C#:   x is int or double or decimal
来源：http://hz.zhongyouzk.top/gtybpovpuj.html

[B14] 判断值是否在集合内
来源：http://hz.zycfv.cn/gtcswdvtiu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gaohongyu789.top/gtzuisvxae.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhixingplan.top/gtdznbynsr.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtfamoaakv.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.daria6918.cn/gtutvpxfqc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yangfankeji.com/gtwyracyov.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zdqjudy.top/gtngybmrqa.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.52xcode.cn/gtrhurdwuc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ybcxt.top/gtlknfwurz.html

[B15] 布尔运算与取反
来源：http://hz.yuxming.cn/gtufajfwrq.html

Py:   a and b or not c
来源：http://hz.jinyuanbaomall.cn/gtsdrugtad.html

PHP:  $a && $b || !$c
来源：http://hz.jianghu66.top/gtiaathzzz.html

JS:   a && b || !c
来源：http://hz.9152youxi.cn/gtkriexzbs.html

TS:   a && b || !c
来源：http://hz.nwbrower.top/gthqpzimfx.html

Java: a && b || !c
来源：http://hz.guannengcc.top/gtgrkfklat.html

Go:   a && b || !c
来源：http://hz.dashuyun.cn/gtxgkxxqol.html

Ruby: a && b || !c
来源：http://hz.yuanzhike.top/gtlmoqqsyf.html

C#:   a && b || !c
来源：http://hz.ppjwa.cn/gtjjqqgmhd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tian-w.cn/gtbpyrtkzh.html

Py:   if not data: return
来源：http://hz.yj20258.top/gtctuvykaq.html

PHP:  if (!$data) { return; }
来源：http://hz.9152youxi.cn/gtpxveftal.html

JS:   if (!data) return;
来源：http://hz.zhijiandao.cn/gttrsukftr.html

TS:   if (!data) return;
来源：http://hz.wangshuangyany.cn/gtvxftrkzq.html

Java: if (data == null) return;
来源：http://hz.aibaodan.cn/gtxbqwbnar.html

Go:   if data == nil { return }
来源：http://hz.redwolf501.top/gtygjbtkol.html

Ruby: return if data.nil?
来源：http://hz.c1oappe.top/gtkvmqtdww.html

C#:   if (data == null) return;
来源：http://hz.havefunace.top/gtoeocvvjb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtvrlfnfrq.html

C. 函数与作用域
来源：http://hz.bjfxy.top/gtjytbfsho.html

================================================================================
来源：http://hz.nanxinkj.top/gtwrltwfgk.html

[C01] 定义函数
来源：http://hz.9152youxi.cn/gtxgndpvhu.html

Py:   def add(a, b): return a + b
来源：http://hz.xziqi.cn/gttlhsdqbt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sysykeji.top/gtydovnyta.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jyoumei.cn/gtodiubuyk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yanxiufei.cn/gtzgsfzxna.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yuanzhike.top/gtqtgpwbtm.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ydzc1.top/gtyghoakoe.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sxryk.cn/gtrcotrhld.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtfphmvbge.html

[C02] 默认参数
来源：http://hz.yvedp.cn/gtotlnortu.html

Py:   def greet(name="World"): return name
来源：http://hz.yongpay.top/gtumswfefx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.316326.xyz/gtlvfmbnmk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.daria6918.cn/gtgytxcuzs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hammf.cn/gtqfopkapg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ppjwa.cn/gtgaeufnyb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jqgfzy.top/gtzqmjszoo.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhongyouzk.top/gtrxdylgae.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zycfv.cn/gtcadbfdem.html

[C03] 可变参数
来源：http://hz.9152youxi.cn/gtgcfgksoe.html

Py:   def total(*args): return sum(args)
来源：http://hz.hywenlv.cn/gtckxtthtr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhiwuduotai.top/gtguwvrhya.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shzxlz.cn/gtuhaiextu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gthvinvecg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.aizwys.cn/gtiwogmoql.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhoulong.xyz/gtthkwafpb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yuanzhike.top/gtbfnfefcl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yonumen.top/gtrhkbkkxe.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgufenzy.top/gtfrueptbu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shzxlz.cn/gtujnlfnad.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ybcxt.top/gttyeqtjpz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gthltvokee.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yanxiufei.cn/gtkusdxzeg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yongpay.top/gtgugpxrxd.html

Go:   // 无：用配置结构体参数
来源：http://hz.svipenyu.cn/gtrmhhdwqq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj20258.top/gtcwzgkizx.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtbivsrkkz.html

[C05] 返回多个值
来源：http://hz.havefunace.top/gtusrmuvnm.html

Py:   return a, b
来源：http://hz.kuanghao11.cn/gtpppwnoht.html

PHP:  return [$a, $b];
来源：http://hz.zhoulong.xyz/gtjmrdtssx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.mhx1999.top/gtajfziofc.html

TS:   return { a, b };
来源：http://hz.yueranfly.top/gtaxyjqmki.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ivvv.top/gtikylyfgr.html

Go:   return a, b
来源：http://hz.dashuyun.cn/gtxonnytqu.html

Ruby: return a, b
来源：http://hz.yj20258888.top/gtkisuklwi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gttncfshxj.html

[C06] 匿名函数 / lambda
来源：http://hz.daxiang520.top/gtytgirank.html

Py:   square = lambda x: x * x
来源：http://hz.shangyingyoupin.top/gtfwevbfit.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yangfankeji.com/gtxpqixnyd.html

JS:   const square = x => x * x;
来源：http://hz.nanxuanxn.top/gtkbiuhoyp.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.nwbrower.top/gtmdzojxle.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yj20258888.top/gtzxqexvld.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenjidiqi.icu/gtfosuhhtf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.smart0.xyz/gtvnfjyblw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hysaishi.cn/gttzswrmhd.html

[C07] 把函数作为参数传入
来源：http://hz.yongpay.top/gtgcxbpzgb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.meibo888.top/gtzsvhvmxw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hammf.cn/gtutoltehd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cdnleiting.top/gtldzpeeng.html

TS:   arr.map(String)
来源：http://hz.ybcxt.top/gtrgafdlak.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sxryk.cn/gtgqnewyay.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.dianchejie.cn/gtppwytjbi.html

Ruby: arr.map(&:upcase)
来源：http://hz.cdnleiting.top/gtafqooboj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhoulong.xyz/gtyfgjmspk.html

[C08] 闭包
来源：http://hz.guannengcc.top/gtbinlbynf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sxryk.cn/gtyxulfjkh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.meibo888.top/gtzffzdkok.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtzeopgice.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yj202588.top/gtmqfcrsou.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yonumen.top/gtarwtvnxy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.redwolf501.top/gtzhbozewj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jyoumei.cn/gtaltspfex.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtxxwuqxpa.html

[C09] 递归
来源：http://hz.jinqigfzy.top/gtnjfzvvhs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gaohongyu789.top/gtyqturfdh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenjidiqi.icu/gtvvpwkgyt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tian-w.cn/gtbwkdqlws.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtfulnesiu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.wangshuangyany.cn/gttdpwgqqn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dianchejie.cn/gtlhrpgytf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.daria6918.cn/gthdeydhqd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cucudq.cn/gtfbcuufla.html

[C10] 变量作用域
来源：http://hz.xylfe.cn/gtxaoadekg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zdqjudy.top/gtgqjqvtlk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.daria6918.cn/gtlaebdgeo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aizwys.cn/gtpmeamdfp.html

TS:   同 JS
来源：http://hz.cheryme.top/gtnejyfaae.html

Java: 方法内为块级作用域
来源：http://hz.shuidangran.top/gtorfvobbi.html

Go:   花括号块级作用域
来源：http://hz.zhixingplan.top/gtzjblqmxq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.redwolf501.top/gtyatylukw.html

C#:   块级作用域
来源：http://hz.jqgfzy.top/gtjjhepygv.html

[C11] 模块导入与导出
来源：http://hz.xziqi.cn/gtqpolrkoh.html

Py:   from module import func
来源：http://hz.dashuyun.cn/gtacxmvqar.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sweek.top/gtphbtvtwl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnxiangtu.top/gtsauvobzx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xuetiantiany.cn/gtyuoicfil.html

Java: import java.util.List;
来源：http://hz.jinyuanbaomall.cn/gtfveupuey.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sxryk.cn/gthvclqduc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhengqikj.top/gthwighely.html

C#:   using System.Text;
来源：http://hz.snrcjt.cn/gtxxeqgwkv.html

[C12] 立即执行函数 IIFE
来源：http://hz.52xcode.cn/gtbtbgtflz.html

Py:   (lambda: print("run"))()
来源：http://hz.c1oappe.top/gtagvvaiej.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hnqzz.top/gtsfyeqmzs.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shzxlz.cn/gtevjrzcrm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sweek.top/gtnrjhifhh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zdqjudy.top/gtsuxqgjmb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yanxiufei.cn/gtpqlywfen.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhongyouzk.top/gtgdfinfaf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pycfn.com/gtsfahjmmj.html

[C13] 类型声明 / 类型注解
来源：http://hz.meibo888.top/gttywtswbv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hnqzz.top/gtvcaudexv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gthzhdpxcs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.birdmap.top/gtzwblcskx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yueranfly.top/gtobpvfncp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.havefunace.top/gtuyyhxqch.html

Go:   func add(a, b int) int
来源：http://hz.pengpengdd.cyou/gtveyrlamr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangshuangyany.cn/gtsiumzmws.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.snrcjt.cn/gtvsohhxyf.html

[C14] 泛型函数
来源：http://hz.jinqigufen.top/gtttavwbit.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtqrmyicup.html

PHP:  // 无泛型
来源：http://hz.yj20258888.top/gtknmfyfib.html

JS:   // 无泛型
来源：http://hz.shangyingyoupin.top/gtgudhnfnw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.bjfxy.top/gtojmwaron.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ybcxt.top/gtyzwbrueo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dianchejie.cn/gtwtfrvdzk.html

Ruby: # 无泛型
来源：http://hz.svipenyu.cn/gtfkkgvhxl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhaomingkeji.xyz/gthjcuakrq.html

[C15] 解构 / 展开参数
来源：http://hz.dianchejie.cn/gtxhoxfxah.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj202588.top/gtixfgbzzf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hfpthk.cn/gtdeqtgimg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ppjwa.cn/gtixjcxnlq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.pengpengdd.cyou/gtxzkkapmq.html

Java: // 无解构
来源：http://hz.cucudq.cn/gtcqobuozl.html

Go:   // 无解构
来源：http://hz.jyoumei.cn/gtzstwpabo.html

Ruby: a, b = pair
来源：http://hz.haohaochexian.top/gtjhgfsseq.html

C#:   var (a, b) = pair;
来源：http://hz.redwolf501.top/gtzgqxnpeb.html

[C16] 函数 / 方法重载
来源：http://hz.ydjk.org.cn/gtlsobnmry.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shangyingyoupin.top/gtpmwwpvbt.html

PHP:  // 无重载
来源：http://hz.quarkkingdee.top/gtzefadjfk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hywenlv.cn/gtegcdvekk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gotoacloud.top/gtzlmmdqxq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhaomingkeji.xyz/gtfmpufqru.html

Go:   // 无重载：用不同函数名
来源：http://hz.xziqi.cn/gtgurhjbzb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jiagoushi.top/gtvatntdyg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.redwolf501.top/gtagznekwj.html

================================================================================
来源：http://hz.yj20258888.top/gtdaotxnpj.html

D. 数组 / 列表 / 集合
来源：http://hz.jqgfzy.top/gtseilhktx.html

================================================================================
来源：http://hz.zhixingplan.top/gtqayqdpyt.html

[D01] 创建数组 / 列表
来源：http://hz.yangfankeji.com/gtnueuiseg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.feifeiyinyue.top/gtqyfdhfic.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gogol.net.cn/gtynbikpnb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigufen.top/gttefefldl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxinkj.top/gtjwosdeac.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hongshengwenyu.top/gtsmdxzawy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tanke756.top/gtzwzqsyru.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhoulong.xyz/gtiivzdust.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ybcxt.top/gtxiikkwuj.html

[D02] 追加元素到末尾
来源：http://hz.svipenyu.cn/gtlixngool.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yj20258888.top/gtuqsupdlt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhengqikj.top/gtgxymzytw.html

JS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtyakvllzx.html

TS:   arr.push(4);
来源：http://hz.hnxiangtu.top/gtlqqbdsmd.html

Java: list.add(4);
来源：http://hz.52xcode.cn/gttusaefkg.html

Go:   arr = append(arr, 4)
来源：http://hz.xziqi.cn/gtovjmlaop.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.aizwys.cn/gtlrkpzapf.html

C#:   list.Add(4);
来源：http://hz.hysaishi.cn/gtrgpbavfm.html

[D03] 在指定位置插入元素
来源：http://hz.zhoulong.xyz/gtmwquzcwx.html

Py:   arr.insert(0, 0)
来源：http://hz.jianghu66.top/gtxzcwiazn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhixingplan.top/gtmcasgezs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.guowangkeji.top/gtqgyjvdff.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gogol.net.cn/gtwfdwinff.html

Java: list.add(0, 0);
来源：http://hz.ehwqpu.com/gtczlqayhp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.mhx1999.top/gtacblusif.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ivvv.top/gtkfucgcdg.html

C#:   list.Insert(0, 0);
来源：http://hz.dashuyun.cn/gterfuxcsz.html

[D04] 删除元素
来源：http://hz.yuanzhike.top/gtcwfoccbs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.aizwys.cn/gtaotrdkzz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yongpay.top/gtcibwfxnx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxuanxn.top/gtedfyuqxy.html

TS:   arr.splice(0, 1);
来源：http://hz.quarkkingdee.top/gtzbsomjsk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj20258888.top/gttbhglknq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgfzy.top/gtjwwokvaa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fzhhl.top/gtbpkharsi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pengpengdd.cyou/gtoifguerh.html

[D05] 访问与修改元素
来源：http://hz.tanke756.top/gtynobfyda.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.smart0.xyz/gtpsfnqbxv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhijiandao.cn/gtlsypolpk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtcscwaukc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhixingplan.top/gtrbwhfaox.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sysykeji.top/gtkibasjlg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtudobvugy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tanke756.top/gtlgqbrxyi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ywan-chungtsiang.top/gtzvwpauur.html

[D06] 数组长度
来源：http://hz.jinyuanbaomall.cn/gtyyoeluji.html

Py:   len(arr)
来源：http://hz.xinyue.icu/gtpwgsjomj.html

PHP:  count($arr);
来源：http://hz.yj202588.top/gtxrubbple.html

JS:   arr.length
来源：http://hz.xziqi.cn/gtppfbupoa.html

TS:   arr.length
来源：http://hz.ehwqpu.com/gtszlfaxor.html

Java: list.size();
来源：http://hz.aibaodan.cn/gtrlhekdfk.html

Go:   len(arr)
来源：http://hz.zhiwuduotai.top/gtfkfzanpv.html

Ruby: arr.length; arr.size
来源：http://hz.yuanzhike.top/gtscodcwcd.html

C#:   list.Count;
来源：http://hz.xinyue.icu/gtulkvrwiv.html

[D07] 切片 / 取子数组
来源：http://hz.jqgufenzy.top/gtautjiims.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.aizwys.cn/gtuoeobqwc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.andypj.xyz/gtnotrrenb.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxuanxn.top/gtydqycirv.html


<!-- 参考信息 -->