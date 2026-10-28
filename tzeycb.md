代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://hz.guannengcc.top/gtlgqhjqbe.html

JS:   while (i < 10) { i++; }
来源：http://hz.gzhubu.top/gtergsbrld.html

TS:   while (i < 10) { i++; }
来源：http://hz.sufxvd.cn/gtvxczujde.html

Java: while (i < 10) { i++; }
来源：http://hz.yuanzhike.top/gtxbhlmcmy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.c1oappe.top/gtobxpbkki.html

Ruby: while i < 10; i += 1; end
来源：http://hz.gogol.net.cn/gtjctqbwvz.html

C#:   while (i < 10) { i++; }
来源：http://hz.sxryk.cn/gtimfsgeoq.html

[B08] do-while（至少执行一次）
来源：http://hz.sxryk.cn/gtloqljavb.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zdqjudy.top/gtaltkwmuj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.guowangkeji.top/gtuxpefvad.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xuetiantiany.cn/gtmymuockk.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gtiryxcuhw.html

Java: do { i++; } while (i < 10);
来源：http://hz.xylfe.cn/gtrjfeskbp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.nwbrower.top/gtmhwjydtc.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.nanxuanxn.top/gtemujetkx.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangtech.top/gthphgnnru.html

[B09] break 与 continue
来源：http://hz.hammf.cn/gtxmxjylcg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yj20258888.top/gtwndxszjk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.9152youxi.cn/gteuywznoj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtnvjfyvfy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.0kj1m.cn/gtptpjamzk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gthlcvoywf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.shzxlz.cn/gtzhhczzsu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sufxvd.cn/gtxmtsyabw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtbmtkdsxb.html

[B10] 遍历同时拿索引
来源：http://hz.svipenyu.cn/gtqpxapvfr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.mhx1999.top/gtqsudpmhh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yongpay.top/gttijvozih.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhongyouzk.top/gtbrufvogm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.guowangkeji.top/gttuuqihul.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.andypj.xyz/gtidnkswjn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xuanzx.com/gtfcwvqndh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cheryme.top/gtwrlljgcd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.smart0.xyz/gtzjtdodut.html

[B11] 生成数字序列 / 区间
来源：http://hz.yj202588.top/gtkjuadyqg.html

Py:   list(range(0, 10, 2))
来源：http://hz.andypj.xyz/gtbympascx.html

PHP:  range(0, 10, 2);
来源：http://hz.aizwys.cn/gtrohgbqsc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nwbrower.top/gteepbfyob.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fzhhl.top/gtnxvadrhk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xuetiantiany.cn/gtsurkwfut.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.havefunace.top/gtgefghtnn.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jqgfzy.top/gtnagrijyg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.kuanghao11.cn/gtdtdwfqeh.html

[B12] 跳出多层循环
来源：http://hz.bjfxy.top/gtzttccpgj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gzhubu.top/gtucadmxxj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.birdmap.top/gtzxwwalis.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guannengcc.top/gtwormiyfu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.smart0.xyz/gtwacklmjm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cucudq.cn/gtfwtxwahx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hongshengwenyu.top/gtbzxtpabo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.316326.xyz/gtbescxcqa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.havefunace.top/gtbojzwuoo.html

[B13] 判断是否为数字
来源：http://hz.tianlin.xyz/gtrcheflde.html

Py:   isinstance(x, (int, float))
来源：http://hz.nanxinkj.top/gtqwskdupc.html

PHP:  is_numeric($x)
来源：http://hz.ydjk.org.cn/gtntlhbfdt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydjk.org.cn/gtdxeipvps.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pycfn.com/gtdbjyjtpc.html

Java: x instanceof Number
来源：http://hz.jqgfzy.top/gtickdghnq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.wangdashe.top/gtnnyuzxxz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hongshengwenyu.top/gtzwygudxc.html

C#:   x is int or double or decimal
来源：http://hz.zhaomingkeji.xyz/gtbaxsbngk.html

[B14] 判断值是否在集合内
来源：http://hz.jinyuanbaomall.cn/gtshclgtbw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yj20258888.top/gtofpetjnd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.iojbl.cn/gtfdnmllsz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ybcxt.top/gtohhrtzer.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ybcxt.top/gtacmigtdi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.guowangkeji.top/gtrqlsyemb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.aizwys.cn/gtpfkfuhit.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.quarkkingdee.top/gtzxongjaw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xuanzx.com/gtysxcbcpl.html

[B15] 布尔运算与取反
来源：http://hz.nwbrower.top/gtztidfwsp.html

Py:   a and b or not c
来源：http://hz.daria6918.cn/gtjpvomtum.html

PHP:  $a && $b || !$c
来源：http://hz.cdnleiting.top/gtohuxcfvt.html

JS:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gthtahyuid.html

TS:   a && b || !c
来源：http://hz.jyoumei.cn/gthyumdvmo.html

Java: a && b || !c
来源：http://hz.zhongyouzk.top/gttropjwfr.html

Go:   a && b || !c
来源：http://hz.9152youxi.cn/gtoxtbtyrz.html

Ruby: a && b || !c
来源：http://hz.xylfe.cn/gtcddssvgp.html

C#:   a && b || !c
来源：http://hz.xuanzx.com/gtpihiybex.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.guowangkeji.top/gtvfyzhlxr.html

Py:   if not data: return
来源：http://hz.andypj.xyz/gtvkaeewmy.html

PHP:  if (!$data) { return; }
来源：http://hz.jinghuilouyu.cn/gtyzqcmkqd.html

JS:   if (!data) return;
来源：http://hz.ydjk.org.cn/gtasshuceu.html

TS:   if (!data) return;
来源：http://hz.yj20258888.top/gtiyxvxdht.html

Java: if (data == null) return;
来源：http://hz.hywenlv.cn/gtauryegut.html

Go:   if data == nil { return }
来源：http://hz.zhixingplan.top/gtuslgucqm.html

Ruby: return if data.nil?
来源：http://hz.daria6918.cn/gtvjaqhmlz.html

C#:   if (data == null) return;
来源：http://hz.shanyushiyangkeji.top/gtundemsra.html

================================================================================
来源：http://hz.quarkkingdee.top/gtmilnmabo.html

C. 函数与作用域
来源：http://hz.fzhhl.top/gteucvkpvk.html

================================================================================
来源：http://hz.nwbrower.top/gtduainydo.html

[C01] 定义函数
来源：http://hz.cashguo.top/gttuehxowq.html

Py:   def add(a, b): return a + b
来源：http://hz.smart0.xyz/gtdngsbiqt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtplctzngj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtxaqnfjgn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sufxvd.cn/gtbfxdrixz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtrkigrxic.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.iojbl.cn/gtpbhyrcvj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yanxiufei.cn/gtqxgysbky.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gttvuqxaoj.html

[C02] 默认参数
来源：http://hz.daria6918.cn/gtlbrahnag.html

Py:   def greet(name="World"): return name
来源：http://hz.bjfxy.top/gtusoiksuk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zdqjudy.top/gteiquvimp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydjk.org.cn/gtlrtgokhf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tianlin.xyz/gtdcvizfer.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.daria6918.cn/gtwlgxvfld.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.pycfn.com/gtawssebdd.html

Ruby: def greet(name = "World") = name
来源：http://hz.feifeiyinyue.top/gtgeaxrcyo.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.svipenyu.cn/gtyyccpmxh.html

[C03] 可变参数
来源：http://hz.xuanzx.com/gteutcmjen.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhongyouzk.top/gtemseanag.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yongpay.top/gtuttocqdp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pengpengdd.cyou/gtvsrysnmk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuxming.cn/gtkmjrxxci.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.pycfn.com/gtuzpcfucy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cqqwz.cn/gtjkxhkowm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.andypj.xyz/gtmrobfiis.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.redwolf501.top/gtevvxykhe.html

[C04] 命名参数 / 关键字参数
来源：http://hz.kuanghao11.cn/gtbpnjhphc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ehwqpu.com/gtuucrwwxd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.aibaodan.cn/gtidyjhpvn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtpzjbgypj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hywenlv.cn/gtbwingagb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.quarkkingdee.top/gttviomdky.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinqigfzy.top/gtmyaszoul.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtjvnkvdnk.html

C#:   f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtclcfcole.html

[C05] 返回多个值
来源：http://hz.ydjk.org.cn/gtnknhwkjb.html

Py:   return a, b
来源：http://hz.haohaochexian.top/gtpebmjbbg.html

PHP:  return [$a, $b];
来源：http://hz.hnqzz.top/gtgcbdmaac.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sufxvd.cn/gtxwgjgnno.html

TS:   return { a, b };
来源：http://hz.cucudq.cn/gtaxmtakfn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.wangshuangyany.cn/gtqwcxzrdk.html

Go:   return a, b
来源：http://hz.9152youxi.cn/gtiohtnmzv.html

Ruby: return a, b
来源：http://hz.hnxiangtu.top/gthsnpayuj.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yangfankeji.com/gtvfmtrvvu.html

[C06] 匿名函数 / lambda
来源：http://hz.yueranfly.top/gtifldoddw.html

Py:   square = lambda x: x * x
来源：http://hz.andypj.xyz/gtsgdeqkpt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj20258.top/gtrgnuiqrq.html

JS:   const square = x => x * x;
来源：http://hz.ppjwa.cn/gtpzvgpnlh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.quarkkingdee.top/gtslobspmk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yj20258888.top/gtcnephzza.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.sxryk.cn/gttqmmawfw.html

Ruby: square = ->(x) { x * x }
来源：http://hz.gogol.net.cn/gtkhmyidkn.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sufxvd.cn/gtutbpdsvg.html

[C07] 把函数作为参数传入
来源：http://hz.chenlongwang.top/gtuuxjnwjf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sweek.top/gtmikojjko.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gaohongyu789.top/gtmpdoykbd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cdnleiting.top/gtvfwutfhz.html

TS:   arr.map(String)
来源：http://hz.chenjidiqi.icu/gthytuwxvi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.daria6918.cn/gtqxxmquou.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj202588.top/gtlyzoiotq.html

Ruby: arr.map(&:upcase)
来源：http://hz.ppjwa.cn/gtnukscfvq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ydjk.org.cn/gtlkewukdn.html

[C08] 闭包
来源：http://hz.tanke756.top/gthvvlhafs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yanxiufei.cn/gtgffgaqcn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zycfv.cn/gtensisndo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtwlsnzrkf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtfqcmjfqq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ehwqpu.com/gtlnvlsowg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xuetiantiany.cn/gtmfbhshqa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pengpengdd.cyou/gtbplixcso.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtwkguiwbp.html

[C09] 递归
来源：http://hz.hongshengwenyu.top/gtiprlgrtd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.haohaochexian.top/gtrtfvzuoc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.316326.xyz/gtvgwghlgq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fengsongda.top/gtszjdmtxp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtnwyvqysz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhijiandao.cn/gtwqqfygqh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sxryk.cn/gtnienocfc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.aibaodan.cn/gtpivewpaj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.iojbl.cn/gthvwxunqz.html

[C10] 变量作用域
来源：http://hz.wangdashe.top/gttcpobjuo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj20258888.top/gtolmgnhbx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hysaishi.cn/gtogsmptpn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.9152youxi.cn/gtgdlgjjli.html

TS:   同 JS
来源：http://hz.shuidangran.top/gtfsumlcqv.html

Java: 方法内为块级作用域
来源：http://hz.cheryme.top/gtywqzpnwt.html

Go:   花括号块级作用域
来源：http://hz.jqgfzy.top/gtyxuaplqs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hysaishi.cn/gtoktfixyv.html

C#:   块级作用域
来源：http://hz.snrcjt.cn/gtwdakmeqw.html

[C11] 模块导入与导出
来源：http://hz.jinyuanbaomall.cn/gtcghsqrva.html

Py:   from module import func
来源：http://hz.zhengqikj.top/gtyypkkklb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sufxvd.cn/gtdjbzviex.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yanxiufei.cn/gtoyepladq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnxiangtu.top/gtbldcrcpc.html

Java: import java.util.List;
来源：http://hz.jiagoushi.top/gtnemgwxrs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.daria6918.cn/gtmkezlnlj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hnqzz.top/gtjspmvfgv.html

C#:   using System.Text;
来源：http://hz.mhx1999.top/gtcxnavqff.html

[C12] 立即执行函数 IIFE
来源：http://hz.tian-w.cn/gthnyrokum.html

Py:   (lambda: print("run"))()
来源：http://hz.xziqi.cn/gtffckkvsw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cdnleiting.top/gtffiwonaw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.birdmap.top/gtuilhgavq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhiwuduotai.top/gtrptthgsb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nanxuanxn.top/gtyzeganvo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.quarkkingdee.top/gtvzvogbez.html

Ruby: -> { puts "run" }.call
来源：http://hz.316326.xyz/gttybcerdp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhongyouzk.top/gtdjbnvluu.html

[C13] 类型声明 / 类型注解
来源：http://hz.ivvv.top/gtqdgwpadc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.andypj.xyz/gtpiwikxzo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangdashe.top/gtwszgvfax.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhoulong.xyz/gtdphsrpyg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tanke756.top/gthfzbkyxp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtqrnmqqey.html

Go:   func add(a, b int) int
来源：http://hz.xingfuxueyuan.xyz/gtcfkdmseu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.andypj.xyz/gtjkrtnxet.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.snrcjt.cn/gtsdwtvnoj.html

[C14] 泛型函数
来源：http://hz.cheryme.top/gtzdlkhrbt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.0kj1m.cn/gtptyffyxi.html

PHP:  // 无泛型
来源：http://hz.jinyuanbaomall.cn/gtmdddrfyq.html

JS:   // 无泛型
来源：http://hz.svipenyu.cn/gtjuykfpgp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.andypj.xyz/gtitdqelgw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ywan-chungtsiang.top/gtrlfcupje.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.svipenyu.cn/gtyqgukimi.html

Ruby: # 无泛型
来源：http://hz.hnqzz.top/gtabvemita.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.nanxuanxn.top/gtxnosacxd.html

[C15] 解构 / 展开参数
来源：http://hz.zhiwuduotai.top/gtuilirawf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cashguo.top/gtsumldiof.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhongyouzk.top/gtlnmzxpcn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.guowangkeji.top/gtimnfiisg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yvedp.cn/gtoaflwyyf.html

Java: // 无解构
来源：http://hz.fengsongda.top/gtklddxdqz.html

Go:   // 无解构
来源：http://hz.xziqi.cn/gtcsehjkxu.html

Ruby: a, b = pair
来源：http://hz.bjfxy.top/gtvdrtthae.html

C#:   var (a, b) = pair;
来源：http://hz.zhiwuduotai.top/gtnthaqwxk.html

[C16] 函数 / 方法重载
来源：http://hz.xuetiantiany.cn/gtzerggnjz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinghuilouyu.cn/gtijapiake.html

PHP:  // 无重载
来源：http://hz.cqqwz.cn/gtvjwnrvql.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xinyue.icu/gtfxvfjiwo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.316326.xyz/gtspfldunl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tianlin.xyz/gtamopncoa.html

Go:   // 无重载：用不同函数名
来源：http://hz.gzhubu.top/gtoqgjzihe.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shanyushiyangkeji.top/gteydefdxg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jyoumei.cn/gtcjnambyi.html

================================================================================
来源：http://hz.ydjk.org.cn/gtlwpghsgu.html

D. 数组 / 列表 / 集合
来源：http://hz.daria6918.cn/gtadiqzytz.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvjvzpbmo.html

[D01] 创建数组 / 列表
来源：http://hz.redwolf501.top/gtnhehxmfq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shuidangran.top/gtdbudrzfb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhongyouzk.top/gttvxrixgu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cashguo.top/gttkdebcbc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tanke756.top/gtlhvxxdhf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yongpay.top/gtclqinduo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.wangdashe.top/gtnoyumibe.html

Ruby: arr = [1, 2, 3]
来源：http://hz.feifeiyinyue.top/gtrroruioj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.fengsongda.top/gtrvfxmvgj.html

[D02] 追加元素到末尾
来源：http://hz.quarkkingdee.top/gtbqalexds.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shanyushiyangtech.top/gtxqcuusik.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.snrcjt.cn/gtvpryogfm.html

JS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtitvtdikt.html

TS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtctfvmvbt.html

Java: list.add(4);
来源：http://hz.iojbl.cn/gtbauenfif.html

Go:   arr = append(arr, 4)
来源：http://hz.quarkkingdee.top/gttouexsnk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tanke756.top/gtfqnbwasn.html

C#:   list.Add(4);
来源：http://hz.zhoulong.xyz/gtgcnuxgnm.html

[D03] 在指定位置插入元素
来源：http://hz.yongpay.top/gtygdblbdm.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtzvxiuunv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj202588.top/gtuhuuyodj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gotoacloud.top/gteqjcbivf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.feifeiyinyue.top/gthgnwiobb.html

Java: list.add(0, 0);
来源：http://hz.hnxiangtu.top/gtyqpgcymr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ehwqpu.com/gtzpltcplk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj202588.top/gtfyabdxwt.html

C#:   list.Insert(0, 0);
来源：http://hz.xylfe.cn/gtjrorygsq.html

[D04] 删除元素
来源：http://hz.guowangkeji.top/gtlfzimekt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.meibo888.top/gtvibyhcsv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.smart0.xyz/gtxxlsdhbj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.316326.xyz/gtghcbllgl.html

TS:   arr.splice(0, 1);
来源：http://hz.tianlin.xyz/gtzfeqzbvy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hongshengwenyu.top/gthviztlym.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cashguo.top/gtfupiisyl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj20258888.top/gtnnhxnugw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xuanzx.com/gtcyifxphf.html

[D05] 访问与修改元素
来源：http://hz.daxiang520.top/gtzapoabeu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtrgihrxdg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtnzyztjmt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aizwys.cn/gtobaowvlr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gaohongyu789.top/gtsjvanbcu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenlongwang.top/gtovkqglmt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ehwqpu.com/gthweldjtl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtcakxdgnv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.andypj.xyz/gtaakzlycb.html

[D06] 数组长度
来源：http://hz.jinghuilouyu.cn/gtooamstyj.html

Py:   len(arr)
来源：http://hz.kuanghao11.cn/gtwvsdehvp.html

PHP:  count($arr);
来源：http://hz.nwbrower.top/gtdhjipjuu.html

JS:   arr.length
来源：http://hz.hnqzz.top/gtsxncijvg.html

TS:   arr.length
来源：http://hz.nwbrower.top/gtnflmrsme.html

Java: list.size();
来源：http://hz.guowangkeji.top/gtuilhmoyk.html

Go:   len(arr)
来源：http://hz.daxiang520.top/gtugdptgzq.html

Ruby: arr.length; arr.size
来源：http://hz.jyoumei.cn/gtbvajemty.html

C#:   list.Count;
来源：http://hz.xinyue.icu/gtfulpjguo.html

[D07] 切片 / 取子数组
来源：http://hz.fzhhl.top/gtygtdhvmv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.havefunace.top/gtrzlwftao.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fzhhl.top/gtchsktsou.html

JS:   arr.slice(1, 4);
来源：http://hz.zhijiandao.cn/gtvebqbjpl.html

TS:   arr.slice(1, 4);
来源：http://hz.ybcxt.top/gtmbfflzxg.html

Java: list.subList(1, 4);
来源：http://hz.9152youxi.cn/gtqmszcsak.html

Go:   arr[1:4]
来源：http://hz.jinyuanbaomall.cn/gtlvuizxej.html

Ruby: arr[1, 3]
来源：http://hz.jinqigufen.top/gtoijvqcmj.html


<!-- 参考信息 -->