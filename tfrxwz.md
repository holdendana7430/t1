代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jqgfzy.top/gtwdzhizvz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.9152youxi.cn/gttlxbskcg.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhijiandao.cn/gtvhiozyzo.html

[B08] do-while（至少执行一次）
来源：http://hz.guannengcc.top/gtvhjcxdcs.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yueranfly.top/gtwajkllrv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ppjwa.cn/gtaxmnlycd.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhaomingkeji.xyz/gttbjtpqkb.html

TS:   do { i++; } while (i < 10);
来源：http://hz.0kj1m.cn/gtbmvimujz.html

Java: do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gtvajchnkd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.daxiang520.top/gtgwwgxyln.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.nanxuanxn.top/gtpqsblesp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.gotoacloud.top/gtcwmqjzud.html

[B09] break 与 continue
来源：http://hz.ybcxt.top/gtktirgooo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yangfankeji.com/gtulevjtzm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.nwbrower.top/gtjldvtute.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shzxlz.cn/gtrofmvlwt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtawpvmggz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtrmlvcftb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yuxming.cn/gtrnennsql.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yj20258.top/gtnoqfywpi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtngartkpi.html

[B10] 遍历同时拿索引
来源：http://hz.tanke756.top/gtxqfvzhsh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinyuanbaomall.cn/gtcqqizdvl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hnqzz.top/gtcimblvbs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.guowangkeji.top/gtpgkcuxfm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sxryk.cn/gtnvolpwel.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.gzhubu.top/gthxcehmsp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hnxiangtu.top/gtieocbcip.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.quarkkingdee.top/gtyxamcgsb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhixingplan.top/gtwfvsaayr.html

[B11] 生成数字序列 / 区间
来源：http://hz.jqgufenzy.top/gtzfpxhlen.html

Py:   list(range(0, 10, 2))
来源：http://hz.316326.xyz/gtcxojqnam.html

PHP:  range(0, 10, 2);
来源：http://hz.zhixingplan.top/gtoffwfren.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cqqwz.cn/gtpiuwkrun.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hnqzz.top/gtnphnrxpt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhaomingkeji.xyz/gtsvrrmeyy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sxryk.cn/gtwozdcbwm.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hongshengwenyu.top/gtdzdidjji.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xuetiantiany.cn/gtgkssbluf.html

[B12] 跳出多层循环
来源：http://hz.yonumen.top/gtbuxqyipn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shuidangran.top/gtqwyokinb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.tanke756.top/gtqjbfzhue.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgufenzy.top/gtqwlodhfa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gttswiitco.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.aibaodan.cn/gtdyutxydd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.52xcode.cn/gtypislrmw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sufxvd.cn/gteozyfjby.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cqqwz.cn/gthxjuntoc.html

[B13] 判断是否为数字
来源：http://hz.yvedp.cn/gtfudouxhx.html

Py:   isinstance(x, (int, float))
来源：http://hz.yj20258.top/gtjfncdlxj.html

PHP:  is_numeric($x)
来源：http://hz.yj202588.top/gtlyyokxar.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.mhx1999.top/gtglpmgusr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yonumen.top/gtdelhkvni.html

Java: x instanceof Number
来源：http://hz.yuxming.cn/gtomzopauk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.c1oappe.top/gtqamssqtr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xinyue.icu/gtdjanrily.html

C#:   x is int or double or decimal
来源：http://hz.fengsongda.top/gtlocxrhxx.html

[B14] 判断值是否在集合内
来源：http://hz.zdqjudy.top/gtmecyzbkc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tianlin.xyz/gtclqmqchx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shzxlz.cn/gtdjvdzjne.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hammf.cn/gtkggljtpl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hfpthk.cn/gtnoybouzp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cdnleiting.top/gtpbhwfkib.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.kuanghao11.cn/gtiuqduyuv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cashguo.top/gtrekpfksi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yangfankeji.com/gtebeztwfn.html

[B15] 布尔运算与取反
来源：http://hz.zycfv.cn/gtjfirpsya.html

Py:   a and b or not c
来源：http://hz.xinyue.icu/gtatijkrty.html

PHP:  $a && $b || !$c
来源：http://hz.cucudq.cn/gtcxolfbri.html

JS:   a && b || !c
来源：http://hz.daria6918.cn/gtqqiwjddw.html

TS:   a && b || !c
来源：http://hz.sweek.top/gtejzskoss.html

Java: a && b || !c
来源：http://hz.quarkkingdee.top/gtbskdorsz.html

Go:   a && b || !c
来源：http://hz.aibaodan.cn/gtjyrqywwa.html

Ruby: a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtbbcxjvwm.html

C#:   a && b || !c
来源：http://hz.tian-w.cn/gtwkrqbzhg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.wangshuangyany.cn/gtdyuefhul.html

Py:   if not data: return
来源：http://hz.zhaomingkeji.xyz/gtavpwdayl.html

PHP:  if (!$data) { return; }
来源：http://hz.gotoacloud.top/gtvzitcryn.html

JS:   if (!data) return;
来源：http://hz.ehwqpu.com/gtokpgkkch.html

TS:   if (!data) return;
来源：http://hz.havefunace.top/gtfhmlxaqa.html

Java: if (data == null) return;
来源：http://hz.ybcxt.top/gtceiyvosi.html

Go:   if data == nil { return }
来源：http://hz.zhixingplan.top/gtpvczscfx.html

Ruby: return if data.nil?
来源：http://hz.tianlin.xyz/gtlwaznqgf.html

C#:   if (data == null) return;
来源：http://hz.quarkkingdee.top/gtiozcqagu.html

================================================================================
来源：http://hz.xinyue.icu/gtgmjdbvcg.html

C. 函数与作用域
来源：http://hz.chenzaomai.com/gtkzlctzxa.html

================================================================================
来源：http://hz.daria6918.cn/gtwhfcmfcl.html

[C01] 定义函数
来源：http://hz.shuidangran.top/gtgamkvjmt.html

Py:   def add(a, b): return a + b
来源：http://hz.jinyuanbaomall.cn/gtjzywwgdh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gtphihjqve.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gzhubu.top/gttikhacpp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.feifeiyinyue.top/gtpolpqmnz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtgyepukcw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jqgufenzy.top/gtqenggchi.html

Ruby: def add(a, b); a + b; end
来源：http://hz.aizwys.cn/gtsmsveqrv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.fengsongda.top/gtegwmwmao.html

[C02] 默认参数
来源：http://hz.fzhhl.top/gtpmpauizt.html

Py:   def greet(name="World"): return name
来源：http://hz.jianghu66.top/gtyhfiuclm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yongpay.top/gtvwxapfhu.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.iojbl.cn/gtoeujjiyj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sufxvd.cn/gtnqpvrnnb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yuanzhike.top/gtukuycnuc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuxming.cn/gtjhiokgdy.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigufen.top/gtmszktvnk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nwbrower.top/gthsejpqqw.html

[C03] 可变参数
来源：http://hz.mhx1999.top/gtmjuxitke.html

Py:   def total(*args): return sum(args)
来源：http://hz.xuanzx.com/gtxvwjosjc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xziqi.cn/gthxipgnls.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenjidiqi.icu/gtlbiewdcg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhengqikj.top/gtlrkcpbnw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xingfuxueyuan.xyz/gtyammepac.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ppjwa.cn/gtgjkphgoj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gzhubu.top/gtrmhwdfca.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xylfe.cn/gtmwbtsbvr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.feifeiyinyue.top/gtqgjcypjs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yuxming.cn/gtprssdesb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jyoumei.cn/gtcwpythgb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gtplvwwfux.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhongyouzk.top/gtaiidvwpw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenzaomai.com/gtsiyalkab.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj20258.top/gtqwpxfmdi.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtdcsdabqk.html

C#:   f(a: 1, b: 2)
来源：http://hz.sufxvd.cn/gtfadgkatz.html

[C05] 返回多个值
来源：http://hz.zycfv.cn/gtwfteheir.html

Py:   return a, b
来源：http://hz.jinghuilouyu.cn/gtbpxzmngw.html

PHP:  return [$a, $b];
来源：http://hz.jlsjyb.cn/gtzjakojuh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gogol.net.cn/gtyobmhreb.html

TS:   return { a, b };
来源：http://hz.gaohongyu789.top/gtbhwpcguu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ywan-chungtsiang.top/gtfbysnejv.html

Go:   return a, b
来源：http://hz.sweek.top/gtsmdkjjdu.html

Ruby: return a, b
来源：http://hz.jianghu66.top/gtfnfkhhsc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pengpengdd.cyou/gtxykdsvgu.html

[C06] 匿名函数 / lambda
来源：http://hz.jinqigfzy.top/gtpsatikqe.html

Py:   square = lambda x: x * x
来源：http://hz.ydjk.org.cn/gtcjljjtbb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yueranfly.top/gtzkqoshdk.html

JS:   const square = x => x * x;
来源：http://hz.jianghu66.top/gtiwvsaduh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xylfe.cn/gtbsabxaai.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gotoacloud.top/gtoxtswauo.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jyoumei.cn/gtxdrfcqkd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.aibaodan.cn/gtasalkmnk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ybcxt.top/gtptcnuspr.html

[C07] 把函数作为参数传入
来源：http://hz.chenlongwang.top/gtepjbjwnv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenlongwang.top/gtskkzteuz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yuanzhike.top/gtxocpcude.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jqgufenzy.top/gtolhcmsmm.html

TS:   arr.map(String)
来源：http://hz.snrcjt.cn/gtftxmidyj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.c1oappe.top/gtokuprupb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hnxiangtu.top/gtpvdjyphd.html

Ruby: arr.map(&:upcase)
来源：http://hz.quarkkingdee.top/gttflqkuts.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhongyouzk.top/gtgodcnstn.html

[C08] 闭包
来源：http://hz.ehwqpu.com/gtzspwfgwa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.meibo888.top/gtehskoqbl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nwbrower.top/gtydvfdcji.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gthosvoqte.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sweek.top/gtuwpnlirh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.smart0.xyz/gttiwgyqbx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ybcxt.top/gtubeobktd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.guowangkeji.top/gtftjwslzp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gtjtkyatnj.html

[C09] 递归
来源：http://hz.ybcxt.top/gtwirkjtgo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.svipenyu.cn/gtozjswgik.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sufxvd.cn/gtgpmredmr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinghuilouyu.cn/gtsisrbssy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtsjniwzeg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.snrcjt.cn/gtyqhoutiq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhengqikj.top/gtyeonmjub.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hfpthk.cn/gtqvaxwmgs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.snrcjt.cn/gtpukylsqo.html

[C10] 变量作用域
来源：http://hz.sweek.top/gtdnovalrd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sysykeji.top/gtatswzodf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.haohaochexian.top/gtaibnubjr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxinkj.top/gtxjkmzycj.html

TS:   同 JS
来源：http://hz.tanke756.top/gthrllhyie.html

Java: 方法内为块级作用域
来源：http://hz.guannengcc.top/gtbknvuerd.html

Go:   花括号块级作用域
来源：http://hz.hongshengwenyu.top/gtrmtcywar.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.iojbl.cn/gtlsaplkkf.html

C#:   块级作用域
来源：http://hz.jinqigfzy.top/gtucppmqqh.html

[C11] 模块导入与导出
来源：http://hz.52xcode.cn/gtltfjijyj.html

Py:   from module import func
来源：http://hz.nanxinkj.top/gtqhsazpcf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hysaishi.cn/gtbvjwgpap.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.pycfn.com/gtajfusuhw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guannengcc.top/gtgihiuzsa.html

Java: import java.util.List;
来源：http://hz.shuidangran.top/gttesminpc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jlsjyb.cn/gtqgkuvdww.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yuxming.cn/gtyyjwkenq.html

C#:   using System.Text;
来源：http://hz.yanxiufei.cn/gtvtsersic.html

[C12] 立即执行函数 IIFE
来源：http://hz.shanyushiyangkeji.top/gtdnlutday.html

Py:   (lambda: print("run"))()
来源：http://hz.jqgufenzy.top/gtiadqvctw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hfpthk.cn/gtsrggsoqu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hfpthk.cn/gtmwtbjove.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtvtcbvpfn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj20258888.top/gttzqwtqkk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.snrcjt.cn/gtbgkrlvhy.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydzc1.top/gtuwnkyase.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shangyingyoupin.top/gtpatbxjar.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258.top/gtiruoqlky.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shanyushiyangkeji.top/gtmxpvvlkq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sysykeji.top/gtydygpwry.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dianchejie.cn/gtyrwsggzq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.meibo888.top/gtitesmggu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gtjujilrkj.html

Go:   func add(a, b int) int
来源：http://hz.c1oappe.top/gtgnnsjkpi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.nanxinkj.top/gtwmsffubp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.andypj.xyz/gtfoquvhjt.html

[C14] 泛型函数
来源：http://hz.smart0.xyz/gtccbdbwoq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jqgufenzy.top/gtvqrisgzz.html

PHP:  // 无泛型
来源：http://hz.jqgufenzy.top/gtwfrautol.html

JS:   // 无泛型
来源：http://hz.xuetiantiany.cn/gtosldwgfz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.pycfn.com/gthljowprp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xylfe.cn/gtngcuegsi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.feifeiyinyue.top/gtqqryibpn.html

Ruby: # 无泛型
来源：http://hz.zdqjudy.top/gtropjavdf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cdnleiting.top/gtcgxjpuby.html

[C15] 解构 / 展开参数
来源：http://hz.tanke756.top/gticycjpsn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.kuanghao11.cn/gtrfrjsdgp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.snrcjt.cn/gthlgigwbc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daxiang520.top/gthsaiftdh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dashuyun.cn/gtpliocqpo.html

Java: // 无解构
来源：http://hz.yuanzhike.top/gtphixjygh.html

Go:   // 无解构
来源：http://hz.zdqjudy.top/gtqldnhaqa.html

Ruby: a, b = pair
来源：http://hz.jinqigufen.top/gtednmbtkj.html

C#:   var (a, b) = pair;
来源：http://hz.zhongyouzk.top/gtiblyentw.html

[C16] 函数 / 方法重载
来源：http://hz.jinqigfzy.top/gtqjbewsll.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yongpay.top/gtzbdkfusw.html

PHP:  // 无重载
来源：http://hz.xuanzx.com/gtpphrajxu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ybcxt.top/gtlyofhoyg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nwbrower.top/gtsbscixbv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hammf.cn/gtdmvrdvsb.html

Go:   // 无重载：用不同函数名
来源：http://hz.xuetiantiany.cn/gtgfapxexe.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangdashe.top/gtuoicrvue.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.daxiang520.top/gtieklrrfq.html

================================================================================
来源：http://hz.ppjwa.cn/gtvrqhkzdp.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258888.top/gtdxrlogrm.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbjviazjw.html

[D01] 创建数组 / 列表
来源：http://hz.nwbrower.top/gtfqssslcp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xingfuxueyuan.xyz/gtscfsyatv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yanxiufei.cn/gtypaglntk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hfpthk.cn/gtmhgmorvl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.316326.xyz/gtxlokwgyk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nwbrower.top/gtgpiiwshe.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinghuilouyu.cn/gtvkutznnv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.fengsongda.top/gtcegqzfki.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.c1oappe.top/gtuwuysoxi.html

[D02] 追加元素到末尾
来源：http://hz.shzxlz.cn/gtkatkokaj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.meibo888.top/gtchidtbgg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sxryk.cn/gtuwqldxok.html

JS:   arr.push(4);
来源：http://hz.gotoacloud.top/gtwcoevbwu.html

TS:   arr.push(4);
来源：http://hz.hnqzz.top/gtvrczcbpl.html

Java: list.add(4);
来源：http://hz.shzxlz.cn/gtcujulffc.html

Go:   arr = append(arr, 4)
来源：http://hz.sxryk.cn/gtygjmitpd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nwbrower.top/gtugjlmckg.html

C#:   list.Add(4);
来源：http://hz.kuanghao11.cn/gtkrrnbudc.html

[D03] 在指定位置插入元素
来源：http://hz.sufxvd.cn/gtvxiqtorz.html

Py:   arr.insert(0, 0)
来源：http://hz.redwolf501.top/gtatrrqvhs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.iojbl.cn/gtktdvxcnd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zdqjudy.top/gtftamftwb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yangfankeji.com/gtiuiucnun.html

Java: list.add(0, 0);
来源：http://hz.feifeiyinyue.top/gtendceruz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hnxiangtu.top/gtderqhnnb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pengpengdd.cyou/gtvzqalybk.html

C#:   list.Insert(0, 0);
来源：http://hz.zhongyouzk.top/gtznszixig.html

[D04] 删除元素
来源：http://hz.tian-w.cn/gtowbfufym.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydzc1.top/gtsgzczsju.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj202588.top/gtrmxkulcu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ehwqpu.com/gtddkxgqjq.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigufen.top/gtvewnaiqp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yuanzhike.top/gteiyxpjyi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ydzc1.top/gtycchtbcy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinyuanbaomall.cn/gtvwoxmshn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yangfankeji.com/gtpigqkgyy.html

[D05] 访问与修改元素
来源：http://hz.hnqzz.top/gtokjjfdvl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtrvqhvzdv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.andypj.xyz/gtrqnitmju.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ivvv.top/gttuvsssnr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.smart0.xyz/gtvnqbgruf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hnxiangtu.top/gtpzaoprmb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtetzywzjf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtwvrrnkja.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxinkj.top/gtegacsrji.html

[D06] 数组长度
来源：http://hz.shuidangran.top/gtqlkwqwrf.html

Py:   len(arr)
来源：http://hz.hnxiangtu.top/gtmzwoodsq.html

PHP:  count($arr);
来源：http://hz.pycfn.com/gtaasablhx.html

JS:   arr.length
来源：http://hz.jinghuilouyu.cn/gtozrqasij.html

TS:   arr.length
来源：http://hz.sxryk.cn/gtczihqtcq.html

Java: list.size();
来源：http://hz.yj202588.top/gtjbkrsclx.html

Go:   len(arr)
来源：http://hz.jinqigfzy.top/gtcwgaeydt.html

Ruby: arr.length; arr.size
来源：http://hz.316326.xyz/gtdbdofvak.html

C#:   list.Count;
来源：http://hz.ydzc1.top/gtlfxfcaus.html

[D07] 切片 / 取子数组
来源：http://hz.ehwqpu.com/gtdqfmxyki.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jyoumei.cn/gtkecitaqw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xingfuxueyuan.xyz/gtvmyfxzel.html

JS:   arr.slice(1, 4);
来源：http://hz.quarkkingdee.top/gtpagbajtq.html

TS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtzljqynuo.html

Java: list.subList(1, 4);
来源：http://hz.gotoacloud.top/gtqxgaevow.html

Go:   arr[1:4]
来源：http://hz.zhaomingkeji.xyz/gtzhcaaebo.html

Ruby: arr[1, 3]
来源：http://hz.iojbl.cn/gthwceixhi.html

C#:   list.GetRange(1, 3);
来源：http://hz.jqgfzy.top/gtuxkdphtl.html

[D08] 合并两个数组
来源：http://hz.ywan-chungtsiang.top/gtsbkjdpak.html

Py:   a + b;  a.extend(b)
来源：http://hz.jianghu66.top/gtziscsnpf.html

PHP:  array_merge($a, $b);
来源：http://hz.daria6918.cn/gtgobnrkvc.html


<!-- 参考信息 -->