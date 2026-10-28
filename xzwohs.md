代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jyoumei.cn/gtelhdnizf.html

JS:   while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gtgemchluo.html

TS:   while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gtmgvcbtox.html

Java: while (i < 10) { i++; }
来源：http://hz.yueranfly.top/gtkisqiqlg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ehwqpu.com/gthmvwpvdj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zdqjudy.top/gtqgqwhzav.html

C#:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gthahxczoq.html

[B08] do-while（至少执行一次）
来源：http://hz.jinqigufen.top/gtpngtpdab.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.sxryk.cn/gtyslwsbya.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hnxiangtu.top/gtjclnqghy.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gtyrrzyjuf.html

TS:   do { i++; } while (i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtxdrfhczo.html

Java: do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtppunovca.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.svipenyu.cn/gtmjgrusyb.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.tanke756.top/gtikmkqllc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtsijdvqnw.html

[B09] break 与 continue
来源：http://hz.316326.xyz/gtcbevxqcs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shzxlz.cn/gtwllrvgdd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtrgprsebg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtaddmsvrs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj202588.top/gtzbvuxwuf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zycfv.cn/gtvsredgeo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cashguo.top/gtmcodkvqb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinqigufen.top/gtmqrutbzt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.c1oappe.top/gtxvhvnaue.html

[B10] 遍历同时拿索引
来源：http://hz.iojbl.cn/gtdwuxoejd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sxryk.cn/gtjjwvfsnq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xuanzx.com/gtbeyvvuug.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.dianchejie.cn/gthvencibp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.feifeiyinyue.top/gtidjkathi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hongshengwenyu.top/gteytuudus.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ydjk.org.cn/gtkgijwknl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cdnleiting.top/gtqrwlrjqb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hongshengwenyu.top/gtkemyacmr.html

[B11] 生成数字序列 / 区间
来源：http://hz.aibaodan.cn/gtqqyixzzl.html

Py:   list(range(0, 10, 2))
来源：http://hz.quarkkingdee.top/gtddamklub.html

PHP:  range(0, 10, 2);
来源：http://hz.gaohongyu789.top/gtobnbatmj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ppjwa.cn/gtbmripbks.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ydjk.org.cn/gtmaptowtq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shanyushiyangtech.top/gtswnptbuk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.feifeiyinyue.top/gttxhuqqwy.html

Ruby: (0...10).step(2).to_a
来源：http://hz.mhx1999.top/gtfqloavfq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.c1oappe.top/gtmtltkpbt.html

[B12] 跳出多层循环
来源：http://hz.xylfe.cn/gtzjpjhsol.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.dianchejie.cn/gtdcpmytnb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yj202588.top/gtrgrsotba.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtelcmjqyk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtiwgizpqe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtvndpnosl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhaomingkeji.xyz/gtcpfgooja.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhixingplan.top/gtoxlddexp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenlongwang.top/gtjcwqagev.html

[B13] 判断是否为数字
来源：http://hz.pengpengdd.cyou/gthmpzzfse.html

Py:   isinstance(x, (int, float))
来源：http://hz.tanke756.top/gtxhshwzce.html

PHP:  is_numeric($x)
来源：http://hz.aibaodan.cn/gtavhqhdla.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinghuilouyu.cn/gtngbjwzrc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guowangkeji.top/gtvlicfzus.html

Java: x instanceof Number
来源：http://hz.pengpengdd.cyou/gtroivddna.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuetiantiany.cn/gtunmopbct.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shangyingyoupin.top/gttgtjfquv.html

C#:   x is int or double or decimal
来源：http://hz.jqgfzy.top/gtayijysns.html

[B14] 判断值是否在集合内
来源：http://hz.jinqigufen.top/gtwzlabxju.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shanyushiyangkeji.top/gtlrnwmkxl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xuanzx.com/gtnntutyiq.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hfpthk.cn/gtbrjyhdwh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.pengpengdd.cyou/gtnfbejpwl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cheryme.top/gthxzozsat.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sysykeji.top/gtaxqvwvim.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jiagoushi.top/gtetsaaesf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.316326.xyz/gthlwhxpmm.html

[B15] 布尔运算与取反
来源：http://hz.cashguo.top/gtlznhzbfk.html

Py:   a and b or not c
来源：http://hz.zhengqikj.top/gtnpwhzrbq.html

PHP:  $a && $b || !$c
来源：http://hz.ehwqpu.com/gtnjtwhgsu.html

JS:   a && b || !c
来源：http://hz.yj20258888.top/gtxxfgchou.html

TS:   a && b || !c
来源：http://hz.cucudq.cn/gtdxaqvvex.html

Java: a && b || !c
来源：http://hz.svipenyu.cn/gtgswlrttu.html

Go:   a && b || !c
来源：http://hz.guannengcc.top/gtnhtrwmqo.html

Ruby: a && b || !c
来源：http://hz.ybcxt.top/gtgrapuawu.html

C#:   a && b || !c
来源：http://hz.jyoumei.cn/gtdmbokzrk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xylfe.cn/gtppmcnwvu.html

Py:   if not data: return
来源：http://hz.xingfuxueyuan.xyz/gtmaxavwkl.html

PHP:  if (!$data) { return; }
来源：http://hz.sxryk.cn/gtcrybzize.html

JS:   if (!data) return;
来源：http://hz.yangfankeji.com/gttipaakpo.html

TS:   if (!data) return;
来源：http://hz.hfpthk.cn/gtwijfrfib.html

Java: if (data == null) return;
来源：http://hz.316326.xyz/gtncvdwwom.html

Go:   if data == nil { return }
来源：http://hz.snrcjt.cn/gtaahkneaa.html

Ruby: return if data.nil?
来源：http://hz.hnxiangtu.top/gtfsxbgcea.html

C#:   if (data == null) return;
来源：http://hz.shangyingyoupin.top/gtrtdsudtr.html

================================================================================
来源：http://hz.yuanzhike.top/gtrppobfej.html

C. 函数与作用域
来源：http://hz.kuanghao11.cn/gtohflvbcp.html

================================================================================
来源：http://hz.yj20258888.top/gtgljrmgiw.html

[C01] 定义函数
来源：http://hz.sweek.top/gtzfjsmare.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxinkj.top/gtzshxszkj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtwraffuon.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tianlin.xyz/gtesorxqrd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yonumen.top/gtedggfirz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtyvwbkuis.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zycfv.cn/gtmgxsgkzi.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yangfankeji.com/gtaldmffvm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtwwncvckk.html

[C02] 默认参数
来源：http://hz.tanke756.top/gtqmfekzzi.html

Py:   def greet(name="World"): return name
来源：http://hz.nanxinkj.top/gtyebfgxdf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhongyouzk.top/gtutunkyqn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.quarkkingdee.top/gtwpcjoova.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.wangdashe.top/gtanxcezqw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinqigufen.top/gtquwlpguc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sufxvd.cn/gtoatazzfj.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhiwuduotai.top/gtkxisasrh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.dianchejie.cn/gtaudieeqa.html

[C03] 可变参数
来源：http://hz.yj20258888.top/gtplxkkpoh.html

Py:   def total(*args): return sum(args)
来源：http://hz.ivvv.top/gtnycareqv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnxiangtu.top/gtmlrgkgja.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xingfuxueyuan.xyz/gtartxwseq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xylfe.cn/gtznmvforc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhiwuduotai.top/gtgmxlchiw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.havefunace.top/gtyhgwqmrd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cheryme.top/gteochbesr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jyoumei.cn/gtgkgodojk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgufenzy.top/gtkjrmonma.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.iojbl.cn/gtqfvuzdoy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.daxiang520.top/gtwukhekdx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtqxqqdjyl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.meibo888.top/gtjbideoek.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hnxiangtu.top/gtfblomhsm.html

Go:   // 无：用配置结构体参数
来源：http://hz.jiagoushi.top/gtuvsivqzo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtsengihwj.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtsrbetjsy.html

[C05] 返回多个值
来源：http://hz.xuetiantiany.cn/gtguvonwwg.html

Py:   return a, b
来源：http://hz.zhixingplan.top/gtcfczfokk.html

PHP:  return [$a, $b];
来源：http://hz.hongshengwenyu.top/gtqwuvkfdv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hfpthk.cn/gtjprgwhdt.html

TS:   return { a, b };
来源：http://hz.dianchejie.cn/gtvyhzmkvk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.pycfn.com/gtuahbjdhi.html

Go:   return a, b
来源：http://hz.sweek.top/gtnfssyjsr.html

Ruby: return a, b
来源：http://hz.svipenyu.cn/gtnhzkwqbr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.svipenyu.cn/gthuiyecsd.html

[C06] 匿名函数 / lambda
来源：http://hz.svipenyu.cn/gtkmheyjnt.html

Py:   square = lambda x: x * x
来源：http://hz.cdnleiting.top/gthkxgvvtl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cheryme.top/gtxelpsrqb.html

JS:   const square = x => x * x;
来源：http://hz.yongpay.top/gtwbstfxnr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.daria6918.cn/gtegnngjpb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.316326.xyz/gtasvcnucq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zdqjudy.top/gtkanicnpk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.aizwys.cn/gtvuhwummc.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.pycfn.com/gthjkxeopg.html

[C07] 把函数作为参数传入
来源：http://hz.jianghu66.top/gtjxpmfulp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.havefunace.top/gtjojvjtup.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nwbrower.top/gtmugmqair.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yongpay.top/gtxxvvvonf.html

TS:   arr.map(String)
来源：http://hz.yj20258.top/gtslyebtnr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dashuyun.cn/gtgatersic.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shangyingyoupin.top/gtxouyddib.html

Ruby: arr.map(&:upcase)
来源：http://hz.dashuyun.cn/gtbclehbfx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ydzc1.top/gthoaociyr.html

[C08] 闭包
来源：http://hz.smart0.xyz/gtntigludy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hywenlv.cn/gtpzqqwryr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shzxlz.cn/gtzkkemdii.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj20258888.top/gtkfyvmlmh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.redwolf501.top/gtwotkzpfs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.wangdashe.top/gtpgdunljn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.pengpengdd.cyou/gtprpzafgu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hywenlv.cn/gteukafexj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gturxyyuhp.html

[C09] 递归
来源：http://hz.redwolf501.top/gtogojywoa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gogol.net.cn/gtdkpxhhrh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shuidangran.top/gttienzlaz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hysaishi.cn/gtnkmhjvor.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sweek.top/gthrkcoivj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.pycfn.com/gtzmwocukj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ywan-chungtsiang.top/gtnfbvqart.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.kuanghao11.cn/gtdgwfumnf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gotoacloud.top/gtdtrzmtox.html

[C10] 变量作用域
来源：http://hz.ydjk.org.cn/gtavuzabzg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daxiang520.top/gtaxxcbvgo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cqqwz.cn/gtgsmsnrzh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jianghu66.top/gttwuonpuk.html

TS:   同 JS
来源：http://hz.cdnleiting.top/gtrdeypmii.html

Java: 方法内为块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtreizguvu.html

Go:   花括号块级作用域
来源：http://hz.aizwys.cn/gtfwbnsazq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ppjwa.cn/gtvmlykmtl.html

C#:   块级作用域
来源：http://hz.gzhubu.top/gtjckxihzk.html

[C11] 模块导入与导出
来源：http://hz.chenjidiqi.icu/gtdymrbcok.html

Py:   from module import func
来源：http://hz.zdqjudy.top/gtdagyotnd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cheryme.top/gtfzwaxfgv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zdqjudy.top/gtbdtxkisz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gzhubu.top/gthnwjizlo.html

Java: import java.util.List;
来源：http://hz.yj20258.top/gtczwcevow.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ehwqpu.com/gtsfpubeug.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hammf.cn/gtkqcsdmks.html

C#:   using System.Text;
来源：http://hz.gaohongyu789.top/gtlqrltynt.html

[C12] 立即执行函数 IIFE
来源：http://hz.kuanghao11.cn/gtzedscsdi.html

Py:   (lambda: print("run"))()
来源：http://hz.mhx1999.top/gtjiydekoz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yvedp.cn/gtryemofzr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.aizwys.cn/gtiswtphru.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtxbnwajwx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.redwolf501.top/gtxeneivan.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jiagoushi.top/gtoxrgdwfq.html

Ruby: -> { puts "run" }.call
来源：http://hz.nanxinkj.top/gtlhskapzt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sufxvd.cn/gtvkroqxlf.html

[C13] 类型声明 / 类型注解
来源：http://hz.zycfv.cn/gtmimnemsm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhoulong.xyz/gtfqauamml.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gttggrhizo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yangfankeji.com/gtihsjjbmb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fengsongda.top/gtbveghdke.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtogdqlkmg.html

Go:   func add(a, b int) int
来源：http://hz.jyoumei.cn/gtcpjklxxa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gotoacloud.top/gtohlwfysx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.9152youxi.cn/gtuplqsbgn.html

[C14] 泛型函数
来源：http://hz.ydzc1.top/gtudymejtk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yanxiufei.cn/gtewwvraoh.html

PHP:  // 无泛型
来源：http://hz.hfpthk.cn/gtidtuyyje.html

JS:   // 无泛型
来源：http://hz.aibaodan.cn/gtueujvijv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cheryme.top/gthmlvzxre.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gzhubu.top/gtxwqgvmnp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.316326.xyz/gtceufjkvo.html

Ruby: # 无泛型
来源：http://hz.shuidangran.top/gtipdupehf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.vqdsnc.cn/gtssohzkdg.html

[C15] 解构 / 展开参数
来源：http://hz.yuanzhike.top/gtgozgvuii.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.svipenyu.cn/gtxvyyhusd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hfpthk.cn/gtwouxavfv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gtjeikpqoo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.guannengcc.top/gtmlsulhxs.html

Java: // 无解构
来源：http://hz.jqgfzy.top/gtkabsudzb.html

Go:   // 无解构
来源：http://hz.yuanzhike.top/gtckzndpgd.html

Ruby: a, b = pair
来源：http://hz.jinyuanbaomall.cn/gtzwggxdjb.html

C#:   var (a, b) = pair;
来源：http://hz.kuanghao11.cn/gtgwlilqml.html

[C16] 函数 / 方法重载
来源：http://hz.ydzc1.top/gtyxyfkcul.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xuanzx.com/gtihxuilns.html

PHP:  // 无重载
来源：http://hz.xuanzx.com/gtovqefovy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.kuanghao11.cn/gtadgrearl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shzxlz.cn/gtkmcuwkau.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhaomingkeji.xyz/gtqaxbxphm.html

Go:   // 无重载：用不同函数名
来源：http://hz.bjfxy.top/gtyripzvbb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hywenlv.cn/gteuuqjqts.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.52xcode.cn/gtxgbskjlo.html

================================================================================
来源：http://hz.jqgfzy.top/gtvnhpekqe.html

D. 数组 / 列表 / 集合
来源：http://hz.guowangkeji.top/gtuovjjrmm.html

================================================================================
来源：http://hz.jianghu66.top/gtjrulkgda.html

[D01] 创建数组 / 列表
来源：http://hz.yueranfly.top/gtjzpkqdvz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.svipenyu.cn/gtjkaxauxn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.c1oappe.top/gtntmynxhb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sufxvd.cn/gtyernngnv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jqgfzy.top/gtxpaawlev.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shanyushiyangkeji.top/gtbzthdcdz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daria6918.cn/gtpnmtzidm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenzaomai.com/gtnqosvipp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hysaishi.cn/gtadebxehd.html

[D02] 追加元素到末尾
来源：http://hz.feifeiyinyue.top/gthiuoimmg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cashguo.top/gtmbyvmisp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhijiandao.cn/gtetltrgzn.html

JS:   arr.push(4);
来源：http://hz.zhoulong.xyz/gtvweqdysf.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtgrzzynbv.html

Java: list.add(4);
来源：http://hz.gogol.net.cn/gtevuxfzud.html

Go:   arr = append(arr, 4)
来源：http://hz.gzhubu.top/gtziymfcgf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ppjwa.cn/gtbkdpsrus.html

C#:   list.Add(4);
来源：http://hz.kuanghao11.cn/gtktgtnoyh.html

[D03] 在指定位置插入元素
来源：http://hz.zhongyouzk.top/gtsnyjxbaa.html

Py:   arr.insert(0, 0)
来源：http://hz.cheryme.top/gtffhwsclz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jlsjyb.cn/gtchcmblrl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hysaishi.cn/gttasynpen.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yueranfly.top/gtwzjneiap.html

Java: list.add(0, 0);
来源：http://hz.wangdashe.top/gtucykqdpz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.dianchejie.cn/gtvwkaphzt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.mhx1999.top/gtmaazwxdw.html

C#:   list.Insert(0, 0);
来源：http://hz.smart0.xyz/gtcqyevnwd.html

[D04] 删除元素
来源：http://hz.svipenyu.cn/gtilyqaapu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ivvv.top/gtievxiezd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnxiangtu.top/gtkfwxstzu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.snrcjt.cn/gtibtxnoqj.html

TS:   arr.splice(0, 1);
来源：http://hz.zhiwuduotai.top/gtmisxacms.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ivvv.top/gteubislkd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.wangdashe.top/gtwcduusap.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jqgufenzy.top/gtraghqvyi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tianlin.xyz/gtlqyihhld.html

[D05] 访问与修改元素
来源：http://hz.shuidangran.top/gtzpewqmew.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gtycuihtwg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yongpay.top/gtglufasym.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jyoumei.cn/gtqymrmacl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuanzx.com/gtuxeqmchc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.pycfn.com/gtbpumirtk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gthhfnboax.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gtiexnyqog.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zdqjudy.top/gtqxeronir.html

[D06] 数组长度
来源：http://hz.xuanzx.com/gteysdpsdp.html

Py:   len(arr)
来源：http://hz.shzxlz.cn/gtqooadwnw.html

PHP:  count($arr);
来源：http://hz.xylfe.cn/gtmitvplcv.html

JS:   arr.length
来源：http://hz.shanyushiyangkeji.top/gtajabpvvi.html

TS:   arr.length
来源：http://hz.ywan-chungtsiang.top/gtmfonnyvh.html

Java: list.size();
来源：http://hz.yj20258.top/gteimsykhj.html

Go:   len(arr)
来源：http://hz.yueranfly.top/gtcrkqmfwo.html

Ruby: arr.length; arr.size
来源：http://hz.birdmap.top/gthkdpwtcd.html

C#:   list.Count;
来源：http://hz.shzxlz.cn/gtttmapojl.html

[D07] 切片 / 取子数组
来源：http://hz.birdmap.top/gtueejdgkt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shzxlz.cn/gtjlalyowc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhongyouzk.top/gtiwxbxauz.html

JS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gtvustuovv.html

TS:   arr.slice(1, 4);
来源：http://hz.yonumen.top/gtgaqypzrn.html

Java: list.subList(1, 4);
来源：http://hz.nwbrower.top/gtycgnltxe.html

Go:   arr[1:4]
来源：http://hz.vqdsnc.cn/gtnstpzvok.html

Ruby: arr[1, 3]
来源：http://hz.daria6918.cn/gtjxnueieo.html


<!-- 参考信息 -->