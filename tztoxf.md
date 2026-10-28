代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ivvv.top/gtqprtrcxz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.feifeiyinyue.top/gtywkaplmt.html

[B07] while 循环
来源：http://hz.hammf.cn/gtsysdyeui.html

Py:   while i < 10: i += 1
来源：http://hz.gaohongyu789.top/gtgbdbojcz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jyoumei.cn/gtshljvakh.html

JS:   while (i < 10) { i++; }
来源：http://hz.wangdashe.top/gtdgejrkwm.html

TS:   while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gtdgkpqvjr.html

Java: while (i < 10) { i++; }
来源：http://hz.yonumen.top/gttebflxuo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xylfe.cn/gtbrkdtbey.html

Ruby: while i < 10; i += 1; end
来源：http://hz.nwbrower.top/gteooquymy.html

C#:   while (i < 10) { i++; }
来源：http://hz.xziqi.cn/gtrdpfdvxq.html

[B08] do-while（至少执行一次）
来源：http://hz.yuanzhike.top/gtrtuqvqya.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.guowangkeji.top/gticaiakbj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.birdmap.top/gtojbsbnku.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sufxvd.cn/gtxdqflmuc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shuidangran.top/gtplfyfeky.html

Java: do { i++; } while (i < 10);
来源：http://hz.aizwys.cn/gtkhssdbmj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.nanxuanxn.top/gtptsqehpm.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yj20258.top/gtxjbxrwyq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.feifeiyinyue.top/gtvecavpgb.html

[B09] break 与 continue
来源：http://hz.pengpengdd.cyou/gtqptrvuwy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hysaishi.cn/gtdlknywkg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xziqi.cn/gtndveecrz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtocvrjzdk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtnblnpfao.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258888.top/gtoxdpeumm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.guowangkeji.top/gtgyzthzsy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.bjfxy.top/gtmiwjholh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jyoumei.cn/gtuhdyequf.html

[B10] 遍历同时拿索引
来源：http://hz.nwbrower.top/gtgsrgqbvg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.bjfxy.top/gtiwicfnif.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.fengsongda.top/gtgtlrkbcu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xylfe.cn/gtwkcrqopb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cucudq.cn/gtpjiwbatq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.tianlin.xyz/gtwvlsmvws.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.316326.xyz/gtpjjyxvbf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cqqwz.cn/gtzkakzfal.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hammf.cn/gtrwicwumf.html

[B11] 生成数字序列 / 区间
来源：http://hz.ivvv.top/gtomsvujdh.html

Py:   list(range(0, 10, 2))
来源：http://hz.tianlin.xyz/gtvyywdlyz.html

PHP:  range(0, 10, 2);
来源：http://hz.dashuyun.cn/gtnkbyxvob.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jianghu66.top/gtofrbrxqx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgfzy.top/gtbqojuuty.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.dianchejie.cn/gtqilpaewh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gotoacloud.top/gtueoidasn.html

Ruby: (0...10).step(2).to_a
来源：http://hz.316326.xyz/gthmntiytj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jqgufenzy.top/gtarvuhkhq.html

[B12] 跳出多层循环
来源：http://hz.sxryk.cn/gtzobfasyt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhongyouzk.top/gtaievrdkg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.vqdsnc.cn/gtsgrwlecz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gtudivllpe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dashuyun.cn/gtkejnmbfp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gtlftfpmwz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hysaishi.cn/gtbkuwxzmo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.vqdsnc.cn/gtmurqnkao.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hfpthk.cn/gtpxtcaswy.html

[B13] 判断是否为数字
来源：http://hz.chenlongwang.top/gtezdspmkt.html

Py:   isinstance(x, (int, float))
来源：http://hz.daria6918.cn/gtwbpnjpoa.html

PHP:  is_numeric($x)
来源：http://hz.xuetiantiany.cn/gtkgdcguxq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.haohaochexian.top/gtkgvdixqm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.iojbl.cn/gtzshhjsve.html

Java: x instanceof Number
来源：http://hz.ivvv.top/gtkvdabccr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.wangdashe.top/gtbdkugplv.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yj20258888.top/gtlqxcpszx.html

C#:   x is int or double or decimal
来源：http://hz.c1oappe.top/gtdeykdcvx.html

[B14] 判断值是否在集合内
来源：http://hz.xingfuxueyuan.xyz/gtqlnscrtk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sufxvd.cn/gtncojwyeq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gogol.net.cn/gtgqojhedr.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gogol.net.cn/gtmveexjmw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ehwqpu.com/gtjtieaglz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yonumen.top/gtazldlacz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hfpthk.cn/gtilxkxezf.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.quarkkingdee.top/gtbpgjtgss.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.quarkkingdee.top/gtoqletloi.html

[B15] 布尔运算与取反
来源：http://hz.yongpay.top/gtvfhexyxg.html

Py:   a and b or not c
来源：http://hz.fzhhl.top/gtjefsvkup.html

PHP:  $a && $b || !$c
来源：http://hz.pengpengdd.cyou/gteyjniheg.html

JS:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtsyxydyaq.html

TS:   a && b || !c
来源：http://hz.cashguo.top/gtvrgccpxq.html

Java: a && b || !c
来源：http://hz.smart0.xyz/gtegfpkduy.html

Go:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtyrytjsyl.html

Ruby: a && b || !c
来源：http://hz.dashuyun.cn/gtlaktfkma.html

C#:   a && b || !c
来源：http://hz.havefunace.top/gtsunzhccc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhongyouzk.top/gtalepsvnt.html

Py:   if not data: return
来源：http://hz.xuanzx.com/gtrtqvexyy.html

PHP:  if (!$data) { return; }
来源：http://hz.zdqjudy.top/gtxneyfunf.html

JS:   if (!data) return;
来源：http://hz.gotoacloud.top/gtwqtcofcl.html

TS:   if (!data) return;
来源：http://hz.tian-w.cn/gtmhzucrag.html

Java: if (data == null) return;
来源：http://hz.feifeiyinyue.top/gtfsgmzgjd.html

Go:   if data == nil { return }
来源：http://hz.smart0.xyz/gtvbeuwrvl.html

Ruby: return if data.nil?
来源：http://hz.yueranfly.top/gttttiyobb.html

C#:   if (data == null) return;
来源：http://hz.kuanghao11.cn/gtejwoxfrx.html

================================================================================
来源：http://hz.xylfe.cn/gtfwjsepkx.html

C. 函数与作用域
来源：http://hz.shuidangran.top/gtatzvzslo.html

================================================================================
来源：http://hz.smart0.xyz/gtztaxckhs.html

[C01] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtnqvxlbwj.html

Py:   def add(a, b): return a + b
来源：http://hz.zhongyouzk.top/gttoxxphxi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangkeji.top/gtwjcsubwy.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.316326.xyz/gtpoptkqpr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.bjfxy.top/gtbxymdkiq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gtustnxyzs.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cashguo.top/gttsufjnrw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daxiang520.top/gtghduijnq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtnopzuocj.html

[C02] 默认参数
来源：http://hz.chenlongwang.top/gtenisqijt.html

Py:   def greet(name="World"): return name
来源：http://hz.yangfankeji.com/gtkdffxags.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.andypj.xyz/gtybypjnwh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ybcxt.top/gtwohmpryf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cashguo.top/gtzonpffgm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jqgufenzy.top/gthictnwee.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.wangshuangyany.cn/gtkemsjpqx.html

Ruby: def greet(name = "World") = name
来源：http://hz.fengsongda.top/gteeoztzdu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gaohongyu789.top/gtaqlgqnmh.html

[C03] 可变参数
来源：http://hz.yonumen.top/gtfgimiqfw.html

Py:   def total(*args): return sum(args)
来源：http://hz.wangdashe.top/gtjmwrfxex.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jinyuanbaomall.cn/gtzgulhwvj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.redwolf501.top/gtqrnlbubt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jiagoushi.top/gtbzdupfac.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ywan-chungtsiang.top/gtnvclsunl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.snrcjt.cn/gtcnefqico.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cucudq.cn/gtghaswkef.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.quarkkingdee.top/gtajovzdiy.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhoulong.xyz/gtinqltjjd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shuidangran.top/gtilalfpbd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.nanxuanxn.top/gtxxcawemj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yvedp.cn/gtiabieztd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.vqdsnc.cn/gteewnnyfx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shangyingyoupin.top/gtkjqjyzbz.html

Go:   // 无：用配置结构体参数
来源：http://hz.jiagoushi.top/gtkjvfupdo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.kuanghao11.cn/gtjsakzfnx.html

C#:   f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtmbxcpkcw.html

[C05] 返回多个值
来源：http://hz.guannengcc.top/gtcppjtxlb.html

Py:   return a, b
来源：http://hz.zycfv.cn/gtzyzbmosk.html

PHP:  return [$a, $b];
来源：http://hz.52xcode.cn/gtuspuemjr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.c1oappe.top/gtmjdghhhm.html

TS:   return { a, b };
来源：http://hz.ivvv.top/gtuubjyjtp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yvedp.cn/gtckwvvcfr.html

Go:   return a, b
来源：http://hz.fzhhl.top/gtqwbdbmcs.html

Ruby: return a, b
来源：http://hz.shanyushiyangtech.top/gtzxdyxcwi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.redwolf501.top/gtnpaereys.html

[C06] 匿名函数 / lambda
来源：http://hz.havefunace.top/gtmjuumdkl.html

Py:   square = lambda x: x * x
来源：http://hz.sweek.top/gteqmqbklk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.quarkkingdee.top/gtylsorgmj.html

JS:   const square = x => x * x;
来源：http://hz.xylfe.cn/gtssfbbgak.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinyuanbaomall.cn/gttwetenqe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangshuangyany.cn/gtsjezqjoo.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.havefunace.top/gtfxlanxoh.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cheryme.top/gtnwmealyv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hammf.cn/gtcnpixzaq.html

[C07] 把函数作为参数传入
来源：http://hz.guannengcc.top/gtqaiprpnj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenjidiqi.icu/gtpukmddkz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dianchejie.cn/gtzhgqqhqv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cheryme.top/gtesjrvqfa.html

TS:   arr.map(String)
来源：http://hz.jqgfzy.top/gtorjvhfqi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yvedp.cn/gtvvzdihkt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jlsjyb.cn/gtnvfoftkb.html

Ruby: arr.map(&:upcase)
来源：http://hz.hnxiangtu.top/gtoqowwyvm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yonumen.top/gtglevepcb.html

[C08] 闭包
来源：http://hz.yueranfly.top/gtjzhknldv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xuanzx.com/gtwvniwnoz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hongshengwenyu.top/gthsdfdedo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtcrfchhty.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhengqikj.top/gthogoofhd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xylfe.cn/gtgqufwfzd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.wangshuangyany.cn/gtgzkwfnhd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gzhubu.top/gtnlrzzcld.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gttymgswnl.html

[C09] 递归
来源：http://hz.ybcxt.top/gtvmafflis.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenlongwang.top/gtttrtlwhu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yanxiufei.cn/gtnihllala.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tianlin.xyz/gtyqdcwpio.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.52xcode.cn/gtojmylgsp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hysaishi.cn/gtfsaakcev.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yongpay.top/gtcvgziljd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhixingplan.top/gtnxcvzsmn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hongshengwenyu.top/gtvlgxbgbk.html

[C10] 变量作用域
来源：http://hz.redwolf501.top/gtikcykmma.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hysaishi.cn/gtrmbmlqmw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zdqjudy.top/gtvntecgnl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangdashe.top/gtdfnkfpcp.html

TS:   同 JS
来源：http://hz.hongshengwenyu.top/gtkhgqjtbi.html

Java: 方法内为块级作用域
来源：http://hz.cheryme.top/gtguwkxfdg.html

Go:   花括号块级作用域
来源：http://hz.jqgfzy.top/gtmfughtbv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.316326.xyz/gtajztjijx.html

C#:   块级作用域
来源：http://hz.jinqigufen.top/gtgemwuudt.html

[C11] 模块导入与导出
来源：http://hz.sufxvd.cn/gtnfrfsbyj.html

Py:   from module import func
来源：http://hz.cqqwz.cn/gtqmdexryv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guannengcc.top/gtadkwrehc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtyoezreyw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhiwuduotai.top/gtuohhinmt.html

Java: import java.util.List;
来源：http://hz.wangdashe.top/gtrcokfnno.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.haohaochexian.top/gtpsraxssl.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jlsjyb.cn/gtkraybrio.html

C#:   using System.Text;
来源：http://hz.feifeiyinyue.top/gtalnhtkqm.html

[C12] 立即执行函数 IIFE
来源：http://hz.ydzc1.top/gtzvgmbdki.html

Py:   (lambda: print("run"))()
来源：http://hz.shanyushiyangkeji.top/gtplxcwzzn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ydzc1.top/gthdctbvii.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yueranfly.top/gtncosvmtw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtrpninnoq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhoulong.xyz/gtypsotwqg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.snrcjt.cn/gtbfgkdhgx.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj20258888.top/gteyrpgkah.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gzhubu.top/gtjsoyhoov.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhiwuduotai.top/gtdjlnagjg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.daria6918.cn/gtirrefqkt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.birdmap.top/gtrkcrpljl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenjidiqi.icu/gtjbtihxhx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cqqwz.cn/gtqwrepczi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtxawzgsdd.html

Go:   func add(a, b int) int
来源：http://hz.tianlin.xyz/gtgldbxmbc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jiagoushi.top/gtcxpvteee.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hnxiangtu.top/gtrorbbfqx.html

[C14] 泛型函数
来源：http://hz.sxryk.cn/gtxvriwrmy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.feifeiyinyue.top/gtlqtilksn.html

PHP:  // 无泛型
来源：http://hz.sweek.top/gtnfuujywg.html

JS:   // 无泛型
来源：http://hz.kuanghao11.cn/gtwgjdidal.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zycfv.cn/gtmigrzjxz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gzhubu.top/gtukvuxidm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ehwqpu.com/gtpgfpyctp.html

Ruby: # 无泛型
来源：http://hz.zhengqikj.top/gthvryiaho.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenlongwang.top/gtfipjfflr.html

[C15] 解构 / 展开参数
来源：http://hz.wangdashe.top/gteelayewh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shuidangran.top/gtxrokjnsx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jyoumei.cn/gtwwavokmn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ybcxt.top/gttmhmhsbv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj20258888.top/gtffxavxzh.html

Java: // 无解构
来源：http://hz.shanyushiyangkeji.top/gtlhqmudaj.html

Go:   // 无解构
来源：http://hz.yanxiufei.cn/gtlxfqgkzm.html

Ruby: a, b = pair
来源：http://hz.316326.xyz/gtupmmxijr.html

C#:   var (a, b) = pair;
来源：http://hz.wangshuangyany.cn/gtephgjgzl.html

[C16] 函数 / 方法重载
来源：http://hz.tian-w.cn/gtpaibrspd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhoulong.xyz/gtujemucca.html

PHP:  // 无重载
来源：http://hz.yongpay.top/gtcxugljse.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ivvv.top/gtcyfbgjrs.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.andypj.xyz/gtcaknwlkh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj202588.top/gtgpuncmjq.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtafdzagfs.html

Ruby: # 无重载：靠动态参数
来源：http://hz.quarkkingdee.top/gtmyscbtel.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.vqdsnc.cn/gtsqdvptod.html

================================================================================
来源：http://hz.yonumen.top/gtnklrhvhr.html

D. 数组 / 列表 / 集合
来源：http://hz.yj202588.top/gtcoinaotr.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmttzshrq.html

[D01] 创建数组 / 列表
来源：http://hz.aibaodan.cn/gtryeodayw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigfzy.top/gtohogseca.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhiwuduotai.top/gteipolgqa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.iojbl.cn/gtuwpbzhai.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jianghu66.top/gtlgbviodg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aibaodan.cn/gtscvjfrek.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jlsjyb.cn/gtabtuaavy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gogol.net.cn/gtixcistmz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yueranfly.top/gtcgrcjybg.html

[D02] 追加元素到末尾
来源：http://hz.zhixingplan.top/gtnbclkwzq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daria6918.cn/gtzfektuzs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jiagoushi.top/gtkhfxbecz.html

JS:   arr.push(4);
来源：http://hz.ydjk.org.cn/gtilenfdsc.html

TS:   arr.push(4);
来源：http://hz.jinyuanbaomall.cn/gtwckpuxeh.html

Java: list.add(4);
来源：http://hz.yanxiufei.cn/gtfncqjwwj.html

Go:   arr = append(arr, 4)
来源：http://hz.hnxiangtu.top/gthejsomca.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daria6918.cn/gtrxrbjthl.html

C#:   list.Add(4);
来源：http://hz.fengsongda.top/gtjzjgjifg.html

[D03] 在指定位置插入元素
来源：http://hz.xuanzx.com/gtcqhuvcqx.html

Py:   arr.insert(0, 0)
来源：http://hz.guannengcc.top/gtvyltkcym.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yangfankeji.com/gtadwyuxrv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shanyushiyangkeji.top/gtmckworrd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.havefunace.top/gtyhfgwpns.html

Java: list.add(0, 0);
来源：http://hz.ehwqpu.com/gtezgkijsc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sufxvd.cn/gtkcsbjsmp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aibaodan.cn/gtkbxkgmxv.html

C#:   list.Insert(0, 0);
来源：http://hz.iojbl.cn/gtjtfuntga.html

[D04] 删除元素
来源：http://hz.cdnleiting.top/gtqvbieqfl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.vqdsnc.cn/gtitqzhhha.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hammf.cn/gtajezoysy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinqigfzy.top/gtrmjtlsab.html

TS:   arr.splice(0, 1);
来源：http://hz.chenjidiqi.icu/gtyppxjllb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.birdmap.top/gtulrqtauh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.bjfxy.top/gtlampjwii.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hfpthk.cn/gtrkmkymrp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shuidangran.top/gtgvgsmcyx.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gtzusoxsgt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xylfe.cn/gtsfnbnjrt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sweek.top/gtbiwktbsh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jyoumei.cn/gtbfjabbkw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ywan-chungtsiang.top/gtjqigvpkr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.wangshuangyany.cn/gtyalcniql.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtuggqfkeq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gzhubu.top/gtapuwuklb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.birdmap.top/gtsdumtdhf.html

[D06] 数组长度
来源：http://hz.gzhubu.top/gtqdwjzdal.html

Py:   len(arr)
来源：http://hz.guowangkeji.top/gtjeacclqs.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gtibyqrjrz.html

JS:   arr.length
来源：http://hz.shanyushiyangtech.top/gtbjnthxru.html

TS:   arr.length
来源：http://hz.yanxiufei.cn/gtvqrbuqsi.html

Java: list.size();
来源：http://hz.zhoulong.xyz/gtgtephrck.html

Go:   len(arr)
来源：http://hz.sysykeji.top/gtjveachip.html

Ruby: arr.length; arr.size
来源：http://hz.daria6918.cn/gtwadrgovz.html

C#:   list.Count;
来源：http://hz.yj202588.top/gtduuchdth.html

[D07] 切片 / 取子数组
来源：http://hz.chenjidiqi.icu/gtujqndzxp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shuidangran.top/gtjpmdyamy.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gotoacloud.top/gtardgfplk.html

JS:   arr.slice(1, 4);
来源：http://hz.bjfxy.top/gtcfxbmsvl.html


<!-- 参考信息 -->