代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.andypj.xyz/gtatgzssfc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.52xcode.cn/gtlwjrojaw.html

[B07] while 循环
来源：http://hz.jinqigfzy.top/gtanbtfkpd.html

Py:   while i < 10: i += 1
来源：http://hz.meibo888.top/gtdbjhmjah.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.gotoacloud.top/gtczolclyp.html

JS:   while (i < 10) { i++; }
来源：http://hz.guowangkeji.top/gtrkscsbmh.html

TS:   while (i < 10) { i++; }
来源：http://hz.yonumen.top/gtproojott.html

Java: while (i < 10) { i++; }
来源：http://hz.haohaochexian.top/gtrrsodccz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.52xcode.cn/gtocretdxt.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yj20258.top/gtxewmnygz.html

C#:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtwtipjdjg.html

[B08] do-while（至少执行一次）
来源：http://hz.svipenyu.cn/gtmgefwjfp.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinyuanbaomall.cn/gtmueazoud.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.pengpengdd.cyou/gtjqbqtkqz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtkywvyuna.html

TS:   do { i++; } while (i < 10);
来源：http://hz.0kj1m.cn/gthnvublpn.html

Java: do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gtbypiegwj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.316326.xyz/gtqkzyxzdv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.meibo888.top/gtyxiomxcq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtjxzraguv.html

[B09] break 与 continue
来源：http://hz.xinyue.icu/gtpcrftxst.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.iojbl.cn/gtvmxklmtk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.52xcode.cn/gtcuroxgds.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guowangkeji.top/gtmduvsbyn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtcxmlturn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuanzx.com/gtahhpiufg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinghuilouyu.cn/gtrdtiwxkl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ybcxt.top/gthtzimsgd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daxiang520.top/gtkmrvynpl.html

[B10] 遍历同时拿索引
来源：http://hz.aizwys.cn/gtetlcrpbl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xuanzx.com/gtfiykfrvh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yangfankeji.com/gtdyqebkcd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.guowangkeji.top/gtbkejiyjb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shanyushiyangtech.top/gtchbshhvg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhoulong.xyz/gtjdxrbaxm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yuanzhike.top/gtupkoexki.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.aibaodan.cn/gtekvntzxm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gaohongyu789.top/gtzplvxnuj.html

[B11] 生成数字序列 / 区间
来源：http://hz.c1oappe.top/gtbqvvkbls.html

Py:   list(range(0, 10, 2))
来源：http://hz.smart0.xyz/gtfixxwtqy.html

PHP:  range(0, 10, 2);
来源：http://hz.gaohongyu789.top/gtrackniqh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhoulong.xyz/gtrnapicgp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hammf.cn/gtvijfwcsf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.aizwys.cn/gtjigogfry.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.svipenyu.cn/gtypaagppn.html

Ruby: (0...10).step(2).to_a
来源：http://hz.fzhhl.top/gtpjpgyizz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.dianchejie.cn/gttetzjtnr.html

[B12] 跳出多层循环
来源：http://hz.9152youxi.cn/gtjcaxghev.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.birdmap.top/gtxrohxqdy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.aizwys.cn/gtxizrxlqk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtgbalvrqa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cdnleiting.top/gtfkeeteop.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gtntbnibaq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhengqikj.top/gtgzsccljq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.nanxuanxn.top/gtqcbzyplo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yueranfly.top/gtiujtqtrn.html

[B13] 判断是否为数字
来源：http://hz.hfpthk.cn/gtfbborlqi.html

Py:   isinstance(x, (int, float))
来源：http://hz.yonumen.top/gtmnpyevoj.html

PHP:  is_numeric($x)
来源：http://hz.chenjidiqi.icu/gtdpmqizss.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydjk.org.cn/gtqekjspkq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhixingplan.top/gtwmistazr.html

Java: x instanceof Number
来源：http://hz.yueranfly.top/gthbphaapq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.mhx1999.top/gtxlyddhrz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cashguo.top/gtnkzacgpg.html

C#:   x is int or double or decimal
来源：http://hz.zhengqikj.top/gtqtmzgwef.html

[B14] 判断值是否在集合内
来源：http://hz.ywan-chungtsiang.top/gtnklombfz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinghuilouyu.cn/gtcvozhowq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.daria6918.cn/gtiaqyeyat.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtummjjnks.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.birdmap.top/gtetydhjmc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hnqzz.top/gtdkeknzaf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gaohongyu789.top/gtwdcvcwnl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gzhubu.top/gtofjeuvyb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sysykeji.top/gtonwomoue.html

[B15] 布尔运算与取反
来源：http://hz.kuanghao11.cn/gtpyajsdpf.html

Py:   a and b or not c
来源：http://hz.zycfv.cn/gtnoafrqrh.html

PHP:  $a && $b || !$c
来源：http://hz.feifeiyinyue.top/gtzptfhgwv.html

JS:   a && b || !c
来源：http://hz.jqgfzy.top/gtfmfeelns.html

TS:   a && b || !c
来源：http://hz.yvedp.cn/gtlkcmtrqy.html

Java: a && b || !c
来源：http://hz.tian-w.cn/gtrndeaesd.html

Go:   a && b || !c
来源：http://hz.cqqwz.cn/gtpoksukfl.html

Ruby: a && b || !c
来源：http://hz.9152youxi.cn/gtxdbdondy.html

C#:   a && b || !c
来源：http://hz.meibo888.top/gtfhodscna.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xinyue.icu/gtzxlhombo.html

Py:   if not data: return
来源：http://hz.daxiang520.top/gttkkbpaqt.html

PHP:  if (!$data) { return; }
来源：http://hz.shangyingyoupin.top/gtgbtssqoe.html

JS:   if (!data) return;
来源：http://hz.gogol.net.cn/gtdukohwmg.html

TS:   if (!data) return;
来源：http://hz.gaohongyu789.top/gtirmqcnqq.html

Java: if (data == null) return;
来源：http://hz.havefunace.top/gttcobggse.html

Go:   if data == nil { return }
来源：http://hz.ehwqpu.com/gtdvrdgmyi.html

Ruby: return if data.nil?
来源：http://hz.yj20258888.top/gtfenmnwuc.html

C#:   if (data == null) return;
来源：http://hz.fzhhl.top/gthizywmpr.html

================================================================================
来源：http://hz.yangfankeji.com/gthwypxmyw.html

C. 函数与作用域
来源：http://hz.yueranfly.top/gtnhgrhftu.html

================================================================================
来源：http://hz.mhx1999.top/gtxejrrakn.html

[C01] 定义函数
来源：http://hz.tian-w.cn/gtymdqwjsa.html

Py:   def add(a, b): return a + b
来源：http://hz.havefunace.top/gtbjdgoabz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtgtcqauul.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.iojbl.cn/gtvgihtath.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zdqjudy.top/gtusxwcqea.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gtmzhkdceg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zycfv.cn/gttskwyqut.html

Ruby: def add(a, b); a + b; end
来源：http://hz.wangshuangyany.cn/gtpspnsrqb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gthuerrzfs.html

[C02] 默认参数
来源：http://hz.hnqzz.top/gtrwaurxiq.html

Py:   def greet(name="World"): return name
来源：http://hz.aibaodan.cn/gtdsdjgmbj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shanyushiyangtech.top/gtsqnolkkm.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jlsjyb.cn/gtmwjbqcrh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.mhx1999.top/gtheppwkvl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ydzc1.top/gtnsyvtirl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuanzhike.top/gtxtxucebr.html

Ruby: def greet(name = "World") = name
来源：http://hz.andypj.xyz/gtliivplpf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jiagoushi.top/gtnabzraoe.html

[C03] 可变参数
来源：http://hz.jyoumei.cn/gtpilkobts.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258.top/gthfxrnafr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shanyushiyangkeji.top/gtbqtzxzod.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtmgqgvbdw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gtsmjakywx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.9152youxi.cn/gtkdqmdsdl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cashguo.top/gtihjdjjdj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yueranfly.top/gtnnbtvemx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinyuanbaomall.cn/gtpwhvnmlg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yangfankeji.com/gtqzolnnfk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhengqikj.top/gtvtxlfnir.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhijiandao.cn/gtztrauuut.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xuanzx.com/gtifbaudtv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.tianlin.xyz/gtbqdrydde.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhengqikj.top/gtcwujmcwc.html

Go:   // 无：用配置结构体参数
来源：http://hz.hysaishi.cn/gtiwbrhfsk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jyoumei.cn/gtvmrqdysn.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtuympmpps.html

[C05] 返回多个值
来源：http://hz.ydjk.org.cn/gtveifoing.html

Py:   return a, b
来源：http://hz.vqdsnc.cn/gtwmcpaqdw.html

PHP:  return [$a, $b];
来源：http://hz.yj20258888.top/gtoalvpjyq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cdnleiting.top/gtdxskdntq.html

TS:   return { a, b };
来源：http://hz.yongpay.top/gtatohrqyt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.snrcjt.cn/gtmmpmljvw.html

Go:   return a, b
来源：http://hz.sysykeji.top/gtlcxrfler.html

Ruby: return a, b
来源：http://hz.yj20258888.top/gtemvjqjym.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jianghu66.top/gtjdzjtxwj.html

[C06] 匿名函数 / lambda
来源：http://hz.hysaishi.cn/gtiqrsykxt.html

Py:   square = lambda x: x * x
来源：http://hz.kuanghao11.cn/gthqodgrxw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj20258.top/gtccqmjpom.html

JS:   const square = x => x * x;
来源：http://hz.tianlin.xyz/gtvqhbxjwr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shanyushiyangtech.top/gthgzseuuy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhiwuduotai.top/gtmwezwkyj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gzhubu.top/gtfxcpsvkr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.gaohongyu789.top/gtwoodlxrh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tian-w.cn/gtqmsooken.html

[C07] 把函数作为参数传入
来源：http://hz.316326.xyz/gtgcvgmbsx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hnqzz.top/gtjolfyjcw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dashuyun.cn/gtenmpzoia.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.mhx1999.top/gtumcmfwzz.html

TS:   arr.map(String)
来源：http://hz.ydjk.org.cn/gttyiltqkr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hnxiangtu.top/gtqybkmeqw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xuetiantiany.cn/gtdmuzjxmo.html

Ruby: arr.map(&:upcase)
来源：http://hz.bjfxy.top/gtmrmovokn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhengqikj.top/gtcgatupyk.html

[C08] 闭包
来源：http://hz.daria6918.cn/gthdxkcjvt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.chenlongwang.top/gtntyfarry.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nanxuanxn.top/gttxucpvet.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ppjwa.cn/gtkmjfjgmh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gtaiiqfwvb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.dashuyun.cn/gttpeaemqa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ywan-chungtsiang.top/gthjfawcgi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.smart0.xyz/gtssfggrkr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhengqikj.top/gticatzijm.html

[C09] 递归
来源：http://hz.redwolf501.top/gtmoowgokr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.svipenyu.cn/gthjydwvcu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zdqjudy.top/gtuxhbhfgu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ivvv.top/gtnvwzqpre.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gthuafyquh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.andypj.xyz/gtecqqeegp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.nanxuanxn.top/gtbjjjfful.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.fengsongda.top/gtucxiyboi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangtech.top/gtbaqybtdi.html

[C10] 变量作用域
来源：http://hz.ydzc1.top/gtsfjvcnde.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daxiang520.top/gtcfsnimtn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jiagoushi.top/gtjnxkdajz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zdqjudy.top/gtjsinqkte.html

TS:   同 JS
来源：http://hz.yj20258.top/gtgcoszzir.html

Java: 方法内为块级作用域
来源：http://hz.9152youxi.cn/gttbicoqdg.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangtech.top/gtdluollyg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.fengsongda.top/gtzhtqlttn.html

C#:   块级作用域
来源：http://hz.sweek.top/gtlwnmjejk.html

[C11] 模块导入与导出
来源：http://hz.gaohongyu789.top/gtcmzcloyr.html

Py:   from module import func
来源：http://hz.andypj.xyz/gthgrucrkb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigfzy.top/gtcawabccp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shzxlz.cn/gtfqwhosjk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinghuilouyu.cn/gtjpahcneu.html

Java: import java.util.List;
来源：http://hz.sysykeji.top/gtgkdgfvdz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigufen.top/gtyistmsby.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.0kj1m.cn/gtfoisxwyf.html

C#:   using System.Text;
来源：http://hz.zycfv.cn/gtrccbhibe.html

[C12] 立即执行函数 IIFE
来源：http://hz.yongpay.top/gtdnqiyfmr.html

Py:   (lambda: print("run"))()
来源：http://hz.9152youxi.cn/gtiuqsqxbd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.vqdsnc.cn/gtdmzqggiq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtlgriuraz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jiagoushi.top/gtozdmxfcc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hammf.cn/gtklpwwbsx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yj20258.top/gtnwpawkur.html

Ruby: -> { puts "run" }.call
来源：http://hz.yongpay.top/gtwadzehrl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinqigufen.top/gtnlvcilqh.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gtxtakzjyh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhongyouzk.top/gttdpxbuot.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtlpiqhtla.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.fzhhl.top/gtspmjokwz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtgeonencf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtmnqzbvhc.html

Go:   func add(a, b int) int
来源：http://hz.cqqwz.cn/gtwnlsowlo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cdnleiting.top/gtjjqwicum.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.havefunace.top/gttozikiqu.html

[C14] 泛型函数
来源：http://hz.jqgfzy.top/gtjbctplgu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cheryme.top/gtlfthxzhe.html

PHP:  // 无泛型
来源：http://hz.hnqzz.top/gtzlpmbqjr.html

JS:   // 无泛型
来源：http://hz.ehwqpu.com/gtdflrorjf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.mhx1999.top/gtzaikbykx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xinyue.icu/gtvatbxkbf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.daxiang520.top/gtwbefzlyf.html

Ruby: # 无泛型
来源：http://hz.hfpthk.cn/gtllapktvg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xziqi.cn/gtcaimgamq.html

[C15] 解构 / 展开参数
来源：http://hz.andypj.xyz/gtytfcpuac.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ivvv.top/gtwnuikhat.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jianghu66.top/gtvsspawpc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtbmobvxkh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.pycfn.com/gtujrvkmed.html

Java: // 无解构
来源：http://hz.fzhhl.top/gthkizfyks.html

Go:   // 无解构
来源：http://hz.wangshuangyany.cn/gtaeiyauba.html

Ruby: a, b = pair
来源：http://hz.guowangkeji.top/gtdxvezqrq.html

C#:   var (a, b) = pair;
来源：http://hz.gogol.net.cn/gtvjemaxol.html

[C16] 函数 / 方法重载
来源：http://hz.xuanzx.com/gtlmckhueg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.andypj.xyz/gtrerlksji.html

PHP:  // 无重载
来源：http://hz.wangdashe.top/gtnxlebcaw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.guannengcc.top/gtlofwhxdh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.snrcjt.cn/gtuxbpioyf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sweek.top/gtqaaaades.html

Go:   // 无重载：用不同函数名
来源：http://hz.yangfankeji.com/gtozaittrz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhiwuduotai.top/gtlrccgsay.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhiwuduotai.top/gtriiufldg.html

================================================================================
来源：http://hz.zhoulong.xyz/gtiwtoamfx.html

D. 数组 / 列表 / 集合
来源：http://hz.zhijiandao.cn/gtbgvqobka.html

================================================================================
来源：http://hz.yonumen.top/gtnkbtspct.html

[D01] 创建数组 / 列表
来源：http://hz.cashguo.top/gteytczram.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.dianchejie.cn/gtetboxwkd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenlongwang.top/gtbiwqewkw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.kuanghao11.cn/gtsrketmog.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cheryme.top/gtvopqjxbc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jiagoushi.top/gtnuhywope.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.guowangkeji.top/gtljdmxtjz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.smart0.xyz/gtfwzjfsdn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.daria6918.cn/gtdysvyaty.html

[D02] 追加元素到末尾
来源：http://hz.shzxlz.cn/gtfptlisvg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jyoumei.cn/gtmhzmutjg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.tian-w.cn/gtxardhifm.html

JS:   arr.push(4);
来源：http://hz.zhongyouzk.top/gtjmfejato.html

TS:   arr.push(4);
来源：http://hz.jiagoushi.top/gtfieqxlam.html

Java: list.add(4);
来源：http://hz.daria6918.cn/gtirhcsyfv.html

Go:   arr = append(arr, 4)
来源：http://hz.xuanzx.com/gtjsjmlnes.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hnqzz.top/gttwsgobbd.html

C#:   list.Add(4);
来源：http://hz.dashuyun.cn/gtsjgwrmmj.html

[D03] 在指定位置插入元素
来源：http://hz.quarkkingdee.top/gtbhtrycyd.html

Py:   arr.insert(0, 0)
来源：http://hz.zycfv.cn/gtkhtymdna.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cashguo.top/gtaroyjyuw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhijiandao.cn/gtywqclkkt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.wangshuangyany.cn/gtoxnpippq.html

Java: list.add(0, 0);
来源：http://hz.pengpengdd.cyou/gtwqvrevol.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhiwuduotai.top/gtgbvvbblz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.feifeiyinyue.top/gtekyjiwap.html

C#:   list.Insert(0, 0);
来源：http://hz.jianghu66.top/gtomihrjuu.html

[D04] 删除元素
来源：http://hz.yanxiufei.cn/gtyfyqcjeo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.tianlin.xyz/gtxslvkbui.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jianghu66.top/gthjvidguy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.daria6918.cn/gteglvobmy.html

TS:   arr.splice(0, 1);
来源：http://hz.iojbl.cn/gtvmxvekux.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinyuanbaomall.cn/gtbilwsijr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cheryme.top/gtzvwjdyof.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yonumen.top/gteljodmpr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yueranfly.top/gtqqlmmkjc.html

[D05] 访问与修改元素
来源：http://hz.cucudq.cn/gtcuaygegm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xinyue.icu/gtmsaaizay.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guannengcc.top/gtdacngwdg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuanzx.com/gtzasqhxig.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.aizwys.cn/gtdheqwdzb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jqgfzy.top/gtfnqyeqsw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sxryk.cn/gtoklpouft.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zycfv.cn/gthrbgbwvp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxuanxn.top/gtusyggeab.html

[D06] 数组长度
来源：http://hz.tianlin.xyz/gtvigazxru.html

Py:   len(arr)
来源：http://hz.ybcxt.top/gttmzkjbym.html

PHP:  count($arr);
来源：http://hz.gzhubu.top/gtryajsmee.html

JS:   arr.length
来源：http://hz.havefunace.top/gtfrrfffoz.html

TS:   arr.length
来源：http://hz.gotoacloud.top/gtpzyslefr.html

Java: list.size();
来源：http://hz.ehwqpu.com/gtrywhguve.html

Go:   len(arr)
来源：http://hz.zhoulong.xyz/gtbcfyvskb.html

Ruby: arr.length; arr.size
来源：http://hz.jinghuilouyu.cn/gtewyvikil.html

C#:   list.Count;
来源：http://hz.snrcjt.cn/gtrmzqvrft.html

[D07] 切片 / 取子数组
来源：http://hz.meibo888.top/gteeddkmxr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhixingplan.top/gtcyvgnjpc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yongpay.top/gtjsfrotwp.html

JS:   arr.slice(1, 4);
来源：http://hz.xylfe.cn/gtyagrxpbw.html


<!-- 参考信息 -->