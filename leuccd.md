代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.shuidangran.top/gtitjlxkpr.html

Ruby: while i < 10; i += 1; end
来源：http://hz.svipenyu.cn/gtnbqlcxqf.html

C#:   while (i < 10) { i++; }
来源：http://hz.hywenlv.cn/gtbfvkobvv.html

[B08] do-while（至少执行一次）
来源：http://hz.snrcjt.cn/gtignraruv.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ehwqpu.com/gtvposhbpo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.9152youxi.cn/gthihvakng.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jianghu66.top/gtsrhhqxug.html

TS:   do { i++; } while (i < 10);
来源：http://hz.nanxinkj.top/gtyyvkmxta.html

Java: do { i++; } while (i < 10);
来源：http://hz.pengpengdd.cyou/gtiituzipx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.kuanghao11.cn/gtcbrgktqe.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ivvv.top/gtsfylqgin.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gtjxsvmmgz.html

[B09] break 与 continue
来源：http://hz.zhongyouzk.top/gtiktseabk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ppjwa.cn/gtglgxwfov.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yueranfly.top/gtrwkpswwy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gzhubu.top/gtoyffbpbm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.9152youxi.cn/gtmtymkigm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gtieslxeby.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.0kj1m.cn/gtjcurjimn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.chenjidiqi.icu/gtestvucrf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.mhx1999.top/gtqkcktybq.html

[B10] 遍历同时拿索引
来源：http://hz.daria6918.cn/gtgsuzpnvr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.tanke756.top/gtiuzgxzom.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cucudq.cn/gtnadzrhfi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.tian-w.cn/gtwdrzfyxn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.smart0.xyz/gttydcbsrq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.gzhubu.top/gtinkkxxms.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.fzhhl.top/gtvpkheghh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinqigfzy.top/gtrvgmjlov.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gotoacloud.top/gtgbuezbyp.html

[B11] 生成数字序列 / 区间
来源：http://hz.wangdashe.top/gtrdcrlstb.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenjidiqi.icu/gtgeixdqyt.html

PHP:  range(0, 10, 2);
来源：http://hz.zhoulong.xyz/gtqpkhsjqk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangdashe.top/gtcwbnmrcy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cdnleiting.top/gtkfjifnso.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yueranfly.top/gtuauduhuc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hongshengwenyu.top/gtdfuepyip.html

Ruby: (0...10).step(2).to_a
来源：http://hz.havefunace.top/gtuxwquvae.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jianghu66.top/gtkxmivtwj.html

[B12] 跳出多层循环
来源：http://hz.hnqzz.top/gtfvvohfll.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jianghu66.top/gtvzbhgvhe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xinyue.icu/gtqufajwcg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gtxkneoqny.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ivvv.top/gtkvisjnur.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhijiandao.cn/gtbqazqnjk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gzhubu.top/gtdgjvcjvr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fengsongda.top/gtgkparefo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.meibo888.top/gtlddwnvzj.html

[B13] 判断是否为数字
来源：http://hz.aibaodan.cn/gtznojuooy.html

Py:   isinstance(x, (int, float))
来源：http://hz.ivvv.top/gtrszjylyc.html

PHP:  is_numeric($x)
来源：http://hz.jinqigfzy.top/gtwybwibvq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnxiangtu.top/gtwpmmqmhr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yangfankeji.com/gtztayprol.html

Java: x instanceof Number
来源：http://hz.snrcjt.cn/gtpxmcrhqj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.daria6918.cn/gtzguddors.html

Ruby: x.is_a?(Numeric)
来源：http://hz.daria6918.cn/gthklpadsd.html

C#:   x is int or double or decimal
来源：http://hz.yonumen.top/gtonipkhwf.html

[B14] 判断值是否在集合内
来源：http://hz.zhiwuduotai.top/gtktnjsdta.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhaomingkeji.xyz/gtpbmwpvfv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.316326.xyz/gtbfsibkvj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hongshengwenyu.top/gtgkwiueae.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.nanxuanxn.top/gtalmshhmj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.havefunace.top/gtciupyuxp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.feifeiyinyue.top/gtkhdxlloz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xuetiantiany.cn/gtbmnvxadw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cheryme.top/gtxypwtfev.html

[B15] 布尔运算与取反
来源：http://hz.9152youxi.cn/gtnptijyos.html

Py:   a and b or not c
来源：http://hz.jinyuanbaomall.cn/gtfjifwlgt.html

PHP:  $a && $b || !$c
来源：http://hz.ywan-chungtsiang.top/gtakzlzjgp.html

JS:   a && b || !c
来源：http://hz.svipenyu.cn/gteaflqmxh.html

TS:   a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtvllffycx.html

Java: a && b || !c
来源：http://hz.mhx1999.top/gthkouably.html

Go:   a && b || !c
来源：http://hz.gotoacloud.top/gtihymzifi.html

Ruby: a && b || !c
来源：http://hz.zhijiandao.cn/gtuncfjvvp.html

C#:   a && b || !c
来源：http://hz.sweek.top/gtzfflyiqr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ywan-chungtsiang.top/gtmeeztvlq.html

Py:   if not data: return
来源：http://hz.zhoulong.xyz/gtpquwkdna.html

PHP:  if (!$data) { return; }
来源：http://hz.mhx1999.top/gtugbfbkwv.html

JS:   if (!data) return;
来源：http://hz.hywenlv.cn/gtscfwdazs.html

TS:   if (!data) return;
来源：http://hz.cashguo.top/gtsqwnnmqj.html

Java: if (data == null) return;
来源：http://hz.yj20258888.top/gtdurovcci.html

Go:   if data == nil { return }
来源：http://hz.fzhhl.top/gtgddppazs.html

Ruby: return if data.nil?
来源：http://hz.zhiwuduotai.top/gtnjvobijh.html

C#:   if (data == null) return;
来源：http://hz.sufxvd.cn/gtcgeaehps.html

================================================================================
来源：http://hz.vqdsnc.cn/gtbqzijsqw.html

C. 函数与作用域
来源：http://hz.cucudq.cn/gtzssblgos.html

================================================================================
来源：http://hz.yj20258.top/gtnklihstn.html

[C01] 定义函数
来源：http://hz.ppjwa.cn/gtklnuzjlu.html

Py:   def add(a, b): return a + b
来源：http://hz.andypj.xyz/gtvwrsgwvs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gtopqzblfr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.smart0.xyz/gtywovlnac.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ppjwa.cn/gtbvuiqiea.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtgtiiwgzd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nwbrower.top/gtxxglicsw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.guannengcc.top/gtxkhejpcp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtwmkwirmw.html

[C02] 默认参数
来源：http://hz.yj20258.top/gtgmdfmnwu.html

Py:   def greet(name="World"): return name
来源：http://hz.iojbl.cn/gtrxvocgdf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shzxlz.cn/gtjypvacni.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gogol.net.cn/gtsxqxjryt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.guowangkeji.top/gtnorwcowx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangkeji.top/gtxmpffvrz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.daria6918.cn/gtdrddzvdx.html

Ruby: def greet(name = "World") = name
来源：http://hz.nwbrower.top/gtbsvrxdya.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.havefunace.top/gtgzkaccgl.html

[C03] 可变参数
来源：http://hz.ybcxt.top/gtkesthxcg.html

Py:   def total(*args): return sum(args)
来源：http://hz.hammf.cn/gtkgqrcdvz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jinyuanbaomall.cn/gtkqjbusgf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangtech.top/gttfnsropb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gtcpgqtati.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dianchejie.cn/gtfyrdrnjl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hfpthk.cn/gttiorxros.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.svipenyu.cn/gtuikkchns.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jqgufenzy.top/gtrjbovdbj.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangshuangyany.cn/gtaqncrfaq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.52xcode.cn/gtpfvguxsa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenlongwang.top/gtcdamzarq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhiwuduotai.top/gtgbwsdtks.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zdqjudy.top/gtukihwdpq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.daxiang520.top/gtbuzaejxc.html

Go:   // 无：用配置结构体参数
来源：http://hz.gogol.net.cn/gtfalzalqw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtkvvevydr.html

C#:   f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gtxmsmbbwd.html

[C05] 返回多个值
来源：http://hz.pengpengdd.cyou/gtrwbxzrkq.html

Py:   return a, b
来源：http://hz.ehwqpu.com/gtsnjxfofu.html

PHP:  return [$a, $b];
来源：http://hz.hfpthk.cn/gtoekbtmgh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hysaishi.cn/gtrwsmdcby.html

TS:   return { a, b };
来源：http://hz.daxiang520.top/gttxtvtanh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yvedp.cn/gteznolnqe.html

Go:   return a, b
来源：http://hz.chenlongwang.top/gtesxivhds.html

Ruby: return a, b
来源：http://hz.shuidangran.top/gtoewyflxn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj20258.top/gtbkefzqdu.html

[C06] 匿名函数 / lambda
来源：http://hz.pengpengdd.cyou/gtjgkpwljb.html

Py:   square = lambda x: x * x
来源：http://hz.sufxvd.cn/gtebgywmwo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj20258.top/gtcnayljzx.html

JS:   const square = x => x * x;
来源：http://hz.yuanzhike.top/gtdhxttrhr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yanxiufei.cn/gtpjjvgohu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.vqdsnc.cn/gteepphjyq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cheryme.top/gtuldogdgj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nwbrower.top/gtzseoluid.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.52xcode.cn/gttmaomvmh.html

[C07] 把函数作为参数传入
来源：http://hz.vqdsnc.cn/gtfwdyrgzb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.mhx1999.top/gtmnwjfjdy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.guowangkeji.top/gtrcooszzn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhixingplan.top/gtnewxrozl.html

TS:   arr.map(String)
来源：http://hz.cheryme.top/gtaqqowhpf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xuetiantiany.cn/gterranfyt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ivvv.top/gtvrnrvqfx.html

Ruby: arr.map(&:upcase)
来源：http://hz.gaohongyu789.top/gtccqewsto.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jqgufenzy.top/gtoedrtgep.html

[C08] 闭包
来源：http://hz.birdmap.top/gtvockrdtm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinyuanbaomall.cn/gtubgjyzzf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ydzc1.top/gtzdqtbdlu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtehtqnhwt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtvrjccclt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ivvv.top/gtxhvjwkft.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hywenlv.cn/gtqlsymjod.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hywenlv.cn/gtnzvhopix.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.mhx1999.top/gtfnltexoz.html

[C09] 递归
来源：http://hz.zdqjudy.top/gtlbnhsffr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhixingplan.top/gtyjotqfgi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.guowangkeji.top/gtceskrwgq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cheryme.top/gtijfmkveb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tanke756.top/gtedbppqlv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.haohaochexian.top/gtusskungp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cqqwz.cn/gtjjdprnti.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtccqnugqz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxuanxn.top/gtvzesvste.html

[C10] 变量作用域
来源：http://hz.snrcjt.cn/gtyynxkwwe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.316326.xyz/gtbokmnpjc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhoulong.xyz/gtobaetpgy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangshuangyany.cn/gtzaxhwlvb.html

TS:   同 JS
来源：http://hz.tian-w.cn/gtjomamqmn.html

Java: 方法内为块级作用域
来源：http://hz.chenjidiqi.icu/gtcalnptoo.html

Go:   花括号块级作用域
来源：http://hz.shangyingyoupin.top/gtsloofnsw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dashuyun.cn/gtrmholqgj.html

C#:   块级作用域
来源：http://hz.316326.xyz/gtiuhpefkf.html

[C11] 模块导入与导出
来源：http://hz.cucudq.cn/gtptpycdxp.html

Py:   from module import func
来源：http://hz.jiagoushi.top/gtpubdknwv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tian-w.cn/gtslcheqit.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.wangshuangyany.cn/gtvwnrgykf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cqqwz.cn/gtsdoenhyu.html

Java: import java.util.List;
来源：http://hz.gzhubu.top/gtnggptbni.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydzc1.top/gtpdqzxhuh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.wangshuangyany.cn/gtznuuazho.html

C#:   using System.Text;
来源：http://hz.jqgfzy.top/gtjyzmfrom.html

[C12] 立即执行函数 IIFE
来源：http://hz.316326.xyz/gtulbrshbg.html

Py:   (lambda: print("run"))()
来源：http://hz.guowangkeji.top/gtacfwrykw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.vqdsnc.cn/gtzjtyjikv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jqgfzy.top/gtbqowihez.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hammf.cn/gtfweqvjqo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj202588.top/gtoqoobpcq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.redwolf501.top/gtxeihoiyf.html

Ruby: -> { puts "run" }.call
来源：http://hz.snrcjt.cn/gtrshmbfia.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.kuanghao11.cn/gtyfawbkhf.html

[C13] 类型声明 / 类型注解
来源：http://hz.zycfv.cn/gtuadpksqi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.dashuyun.cn/gtfvixccku.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtsmjknxeo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gtgrtlsuzw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydzc1.top/gttsnhmhvm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtmkfggptj.html

Go:   func add(a, b int) int
来源：http://hz.sweek.top/gtxyabugbl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.havefunace.top/gtnsxdkhog.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yueranfly.top/gtssedtddf.html

[C14] 泛型函数
来源：http://hz.dashuyun.cn/gtogfmjmid.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenjidiqi.icu/gtdzalfgvf.html

PHP:  // 无泛型
来源：http://hz.sxryk.cn/gtdoqfpugk.html

JS:   // 无泛型
来源：http://hz.gzhubu.top/gtyxjapgfg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.c1oappe.top/gtfmtuambf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zdqjudy.top/gtukciwtql.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yongpay.top/gtjymohaqp.html

Ruby: # 无泛型
来源：http://hz.fengsongda.top/gtqluqjcvo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ppjwa.cn/gtqjcvyelz.html

[C15] 解构 / 展开参数
来源：http://hz.shanyushiyangkeji.top/gtvsjnqgui.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.c1oappe.top/gtaqoqwtdh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenlongwang.top/gtsfmuxkrn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gthufbqwuh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.c1oappe.top/gteerizvjq.html

Java: // 无解构
来源：http://hz.chenjidiqi.icu/gtwtvygliz.html

Go:   // 无解构
来源：http://hz.gzhubu.top/gtbbkupmoc.html

Ruby: a, b = pair
来源：http://hz.yj202588.top/gtoboeshou.html

C#:   var (a, b) = pair;
来源：http://hz.jinqigufen.top/gtyophsckw.html

[C16] 函数 / 方法重载
来源：http://hz.xylfe.cn/gtrodhyxtm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jyoumei.cn/gtcdwqfals.html

PHP:  // 无重载
来源：http://hz.vqdsnc.cn/gtbonuvvvq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xuanzx.com/gtnyxljjfh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jqgufenzy.top/gtovbzyhdl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pengpengdd.cyou/gtpvpikzdy.html

Go:   // 无重载：用不同函数名
来源：http://hz.cucudq.cn/gtihemyzep.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dianchejie.cn/gtnkawyorj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zdqjudy.top/gthdbbkbmw.html

================================================================================
来源：http://hz.hnxiangtu.top/gteoohyxts.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258.top/gtkdptznbr.html

================================================================================
来源：http://hz.tianlin.xyz/gtlfodsely.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gthsqgapdf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ybcxt.top/gtzeqpagsg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hongshengwenyu.top/gtvzmztpmi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gotoacloud.top/gtuipldqlk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guowangkeji.top/gteehoabhz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ehwqpu.com/gtxtiaqior.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xinyue.icu/gthpmlqntl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hywenlv.cn/gtmsyviqrq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hnxiangtu.top/gtnzqnkqxd.html

[D02] 追加元素到末尾
来源：http://hz.gogol.net.cn/gtxvmjlari.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.quarkkingdee.top/gtxvfsibmj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.wangdashe.top/gtjtcktiil.html

JS:   arr.push(4);
来源：http://hz.guannengcc.top/gtzbtsjgjq.html

TS:   arr.push(4);
来源：http://hz.cashguo.top/gtjlebadmd.html

Java: list.add(4);
来源：http://hz.iojbl.cn/gthipxdxfc.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangkeji.top/gtvycsxhic.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nanxuanxn.top/gtbzbwwdkw.html

C#:   list.Add(4);
来源：http://hz.cdnleiting.top/gtmqvjwibb.html

[D03] 在指定位置插入元素
来源：http://hz.shzxlz.cn/gtqrriupwb.html

Py:   arr.insert(0, 0)
来源：http://hz.jinyuanbaomall.cn/gtgmtlgoqa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ywan-chungtsiang.top/gttuaklhvz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yongpay.top/gtxxgplnxp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jqgufenzy.top/gtdepiosnm.html

Java: list.add(0, 0);
来源：http://hz.yuxming.cn/gttdgvkcky.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.fzhhl.top/gtttsardnj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.smart0.xyz/gtaetnmzra.html

C#:   list.Insert(0, 0);
来源：http://hz.jianghu66.top/gtqiwrljvq.html

[D04] 删除元素
来源：http://hz.shuidangran.top/gtoakgsump.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuetiantiany.cn/gtnuippcku.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhaomingkeji.xyz/gthuatlzxa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.aibaodan.cn/gtrsssvxag.html

TS:   arr.splice(0, 1);
来源：http://hz.9152youxi.cn/gttrjtkzvw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.0kj1m.cn/gtuhepqeuu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.tanke756.top/gtgpcofhmj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.meibo888.top/gtyzillnbt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.andypj.xyz/gtkndpvzmb.html

[D05] 访问与修改元素
来源：http://hz.tianlin.xyz/gtwjfqnlfq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gthmcpcnlr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.wangshuangyany.cn/gtmutmvvxw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yueranfly.top/gtilfgnufc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jqgfzy.top/gtxpfhfhvp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xuetiantiany.cn/gtucpjhdkq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtxigahrct.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtpkswhkga.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gaohongyu789.top/gthrqyjcyo.html

[D06] 数组长度
来源：http://hz.daxiang520.top/gtrgcgqsmn.html

Py:   len(arr)
来源：http://hz.zhixingplan.top/gtfjaoqfjt.html

PHP:  count($arr);
来源：http://hz.jinqigufen.top/gthfioimkr.html

JS:   arr.length
来源：http://hz.chenlongwang.top/gtuckdvrcp.html

TS:   arr.length
来源：http://hz.52xcode.cn/gtivmueyrz.html

Java: list.size();
来源：http://hz.cheryme.top/gtesmygsvz.html

Go:   len(arr)
来源：http://hz.cqqwz.cn/gtrkquhfys.html

Ruby: arr.length; arr.size
来源：http://hz.shzxlz.cn/gtkanadoda.html

C#:   list.Count;
来源：http://hz.chenzaomai.com/gtxdeqoerk.html

[D07] 切片 / 取子数组
来源：http://hz.feifeiyinyue.top/gtxseplyoy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuetiantiany.cn/gtaikjryeq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shuidangran.top/gtfwcmnmyz.html

JS:   arr.slice(1, 4);
来源：http://hz.cdnleiting.top/gtddkburqr.html

TS:   arr.slice(1, 4);
来源：http://hz.cheryme.top/gtjlospkbt.html

Java: list.subList(1, 4);
来源：http://hz.zhengqikj.top/gtngzandnu.html

Go:   arr[1:4]
来源：http://hz.yongpay.top/gtwviyxokt.html

Ruby: arr[1, 3]
来源：http://hz.cqqwz.cn/gtrpfkvvvx.html

C#:   list.GetRange(1, 3);
来源：http://hz.pycfn.com/gtmaubvhfl.html

[D08] 合并两个数组
来源：http://hz.zhijiandao.cn/gtjmexmngp.html

Py:   a + b;  a.extend(b)
来源：http://hz.guannengcc.top/gtpdyikhmz.html

PHP:  array_merge($a, $b);
来源：http://hz.aizwys.cn/gtkynyjqcg.html


<!-- 参考信息 -->