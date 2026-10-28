代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.shangyingyoupin.top/gtgdgjirby.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hywenlv.cn/gtoswsckuu.html

[B07] while 循环
来源：http://hz.xziqi.cn/gtygwriois.html

Py:   while i < 10: i += 1
来源：http://hz.sysykeji.top/gtxbumzlyz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.pycfn.com/gtkozeewio.html

JS:   while (i < 10) { i++; }
来源：http://hz.fengsongda.top/gtvhsjmevi.html

TS:   while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gthttngtod.html

Java: while (i < 10) { i++; }
来源：http://hz.redwolf501.top/gthswdvlfz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yonumen.top/gtfbarixpd.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jlsjyb.cn/gtssodcxzk.html

C#:   while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtkezddsik.html

[B08] do-while（至少执行一次）
来源：http://hz.dashuyun.cn/gtzzodlsfy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cucudq.cn/gtgpjcrwdc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jianghu66.top/gtuqyzxcjx.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtcovsrlmx.html

TS:   do { i++; } while (i < 10);
来源：http://hz.vqdsnc.cn/gtyjgmpepy.html

Java: do { i++; } while (i < 10);
来源：http://hz.tianlin.xyz/gtojpbnhqd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hfpthk.cn/gtuikvsyzm.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xingfuxueyuan.xyz/gtfxaismmm.html

C#:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtquybyilb.html

[B09] break 与 continue
来源：http://hz.shangyingyoupin.top/gtzwsuhujz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zhongyouzk.top/gtoavdjbcj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.smart0.xyz/gtxziqhvit.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gtvgpntnak.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj202588.top/gtsjjhqyjr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtqioegkty.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xinyue.icu/gtdfbepnyb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.bjfxy.top/gtijxrofod.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtpwbsysaq.html

[B10] 遍历同时拿索引
来源：http://hz.0kj1m.cn/gtlolelszi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.tianlin.xyz/gtcftvddos.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yanxiufei.cn/gtacfakpde.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zycfv.cn/gtxzlqszls.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cashguo.top/gtomcvnxfj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yongpay.top/gtiayepnoe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jqgufenzy.top/gtpvvuzvre.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.wangdashe.top/gtbraywygi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.c1oappe.top/gtkacprfbb.html

[B11] 生成数字序列 / 区间
来源：http://hz.52xcode.cn/gtyuscxcil.html

Py:   list(range(0, 10, 2))
来源：http://hz.jlsjyb.cn/gtyxbbkxbj.html

PHP:  range(0, 10, 2);
来源：http://hz.xinyue.icu/gtetimejuv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yangfankeji.com/gtuqvfuccn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xuetiantiany.cn/gtpaliyrer.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jqgfzy.top/gtfwapflry.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.316326.xyz/gtvmpqhvkq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ydzc1.top/gtoeqgitsr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhaomingkeji.xyz/gtzftasxdc.html

[B12] 跳出多层循环
来源：http://hz.c1oappe.top/gtgpkhoelw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ehwqpu.com/gthvelllmb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhongyouzk.top/gtdoxnvhqu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jlsjyb.cn/gtxjecmfvw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.birdmap.top/gtcnqltifm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gttxzrnkzt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenlongwang.top/gthhssjzna.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.meibo888.top/gtonemayoh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.nanxinkj.top/gtjwqljshw.html

[B13] 判断是否为数字
来源：http://hz.ydzc1.top/gtpaudplqe.html

Py:   isinstance(x, (int, float))
来源：http://hz.pycfn.com/gtvgqxafdn.html

PHP:  is_numeric($x)
来源：http://hz.ehwqpu.com/gtagtqmeob.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jiagoushi.top/gtwgfrlkcq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.iojbl.cn/gtmtkvciri.html

Java: x instanceof Number
来源：http://hz.smart0.xyz/gtbmbmyglv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.c1oappe.top/gtatobhmsf.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yvedp.cn/gtkqymjgwh.html

C#:   x is int or double or decimal
来源：http://hz.guannengcc.top/gtvgxbmvwu.html

[B14] 判断值是否在集合内
来源：http://hz.ydzc1.top/gtmfbclrcu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shuidangran.top/gtldfmcytm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shanyushiyangkeji.top/gtydrqfgdj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ivvv.top/gtodhvqcon.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yongpay.top/gtchegaaqq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ehwqpu.com/gtrwwnxdgb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.wangshuangyany.cn/gtaynzfntu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhiwuduotai.top/gthnrucpuu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yonumen.top/gtfxjjvrkb.html

[B15] 布尔运算与取反
来源：http://hz.yvedp.cn/gtmgdonqzr.html

Py:   a and b or not c
来源：http://hz.ybcxt.top/gtpnmotufa.html

PHP:  $a && $b || !$c
来源：http://hz.smart0.xyz/gtgdwqmgvi.html

JS:   a && b || !c
来源：http://hz.cucudq.cn/gtpjmjjocv.html

TS:   a && b || !c
来源：http://hz.0kj1m.cn/gthmyzvahw.html

Java: a && b || !c
来源：http://hz.chenjidiqi.icu/gtfxnxzxma.html

Go:   a && b || !c
来源：http://hz.9152youxi.cn/gtqwhfshim.html

Ruby: a && b || !c
来源：http://hz.tian-w.cn/gtxrgskvtk.html

C#:   a && b || !c
来源：http://hz.ivvv.top/gtrmalanbt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shangyingyoupin.top/gteruxrxyr.html

Py:   if not data: return
来源：http://hz.9152youxi.cn/gtijzrwrtw.html

PHP:  if (!$data) { return; }
来源：http://hz.9152youxi.cn/gtjxkzebnj.html

JS:   if (!data) return;
来源：http://hz.hnqzz.top/gtyfctntev.html

TS:   if (!data) return;
来源：http://hz.gotoacloud.top/gtudewdtir.html

Java: if (data == null) return;
来源：http://hz.svipenyu.cn/gtivkgpsme.html

Go:   if data == nil { return }
来源：http://hz.zhixingplan.top/gtfxftdrwj.html

Ruby: return if data.nil?
来源：http://hz.jyoumei.cn/gtsbiycmpc.html

C#:   if (data == null) return;
来源：http://hz.yangfankeji.com/gtomktsbia.html

================================================================================
来源：http://hz.iojbl.cn/gtyyhmrcau.html

C. 函数与作用域
来源：http://hz.yvedp.cn/gtxpirbhks.html

================================================================================
来源：http://hz.ydjk.org.cn/gtobhlqxfn.html

[C01] 定义函数
来源：http://hz.svipenyu.cn/gtlztyrdeb.html

Py:   def add(a, b): return a + b
来源：http://hz.ywan-chungtsiang.top/gtigmomzff.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.snrcjt.cn/gtnajecygt.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gotoacloud.top/gtgxcnatdf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gtcvshapwu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gtiyzadzkf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xinyue.icu/gtzqnoryxm.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hammf.cn/gthatahgml.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtwvovklft.html

[C02] 默认参数
来源：http://hz.nanxuanxn.top/gtqxazkopj.html

Py:   def greet(name="World"): return name
来源：http://hz.snrcjt.cn/gtbvujramh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xuetiantiany.cn/gthpdmdzpq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.mhx1999.top/gtbfssddrn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.c1oappe.top/gtshbcqpyf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xingfuxueyuan.xyz/gtnpxrntrr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.kuanghao11.cn/gtcxcnfbxc.html

Ruby: def greet(name = "World") = name
来源：http://hz.pengpengdd.cyou/gtanisrvhk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guannengcc.top/gtgfryeckh.html

[C03] 可变参数
来源：http://hz.xylfe.cn/gtkgtzlmxa.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258.top/gtvevnrvii.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ywan-chungtsiang.top/gttncohkkd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daria6918.cn/gtnfyophia.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sweek.top/gthgqluwzl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hywenlv.cn/gtsuokjrrj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.c1oappe.top/gtttnzxlcl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hfpthk.cn/gttasvrjza.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yvedp.cn/gtbiqgdeoh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yongpay.top/gttekhifgf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xuanzx.com/gtftgeaaov.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.andypj.xyz/gtkbzorbro.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtuqsojftt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hywenlv.cn/gtplvlqhok.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shzxlz.cn/gtobscuzku.html

Go:   // 无：用配置结构体参数
来源：http://hz.svipenyu.cn/gtqldnbrlt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xinyue.icu/gtkahkdhli.html

C#:   f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtcmglduao.html

[C05] 返回多个值
来源：http://hz.shangyingyoupin.top/gtdjvpkzai.html

Py:   return a, b
来源：http://hz.hongshengwenyu.top/gtzanojgkd.html

PHP:  return [$a, $b];
来源：http://hz.xuanzx.com/gtsniixkac.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shuidangran.top/gtwlahpjzz.html

TS:   return { a, b };
来源：http://hz.sxryk.cn/gtuyxaykkq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shuidangran.top/gthhdbtcmz.html

Go:   return a, b
来源：http://hz.gotoacloud.top/gtxkvbfeoy.html

Ruby: return a, b
来源：http://hz.yonumen.top/gtswqnmyjp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.mhx1999.top/gtbjgxilas.html

[C06] 匿名函数 / lambda
来源：http://hz.zhijiandao.cn/gtmveztcac.html

Py:   square = lambda x: x * x
来源：http://hz.jianghu66.top/gthqyibuec.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.haohaochexian.top/gtxzjlvupa.html

JS:   const square = x => x * x;
来源：http://hz.yj20258888.top/gtvwhrwneq.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sxryk.cn/gtyeulrddp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tianlin.xyz/gtmpeotfyu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cashguo.top/gtwmfrtovl.html

Ruby: square = ->(x) { x * x }
来源：http://hz.guowangkeji.top/gtjnckefyk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinqigufen.top/gtkihiyyov.html

[C07] 把函数作为参数传入
来源：http://hz.yueranfly.top/gtvgqrmkko.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jyoumei.cn/gtanvqvpae.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gotoacloud.top/gtspiuphlz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.52xcode.cn/gtgsyngozg.html

TS:   arr.map(String)
来源：http://hz.hammf.cn/gtjrhlmwjk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.0kj1m.cn/gtvptaapgz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xylfe.cn/gtinsluokr.html

Ruby: arr.map(&:upcase)
来源：http://hz.haohaochexian.top/gtpghyadwh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.dashuyun.cn/gtgzjsigxx.html

[C08] 闭包
来源：http://hz.cdnleiting.top/gtacitioxv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hfpthk.cn/gtkewpesku.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.andypj.xyz/gtlxztqjbc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.pycfn.com/gtzoneuity.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtukbiqyzn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jqgfzy.top/gtlsqdotns.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cheryme.top/gtzillqlio.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.kuanghao11.cn/gtyohodlkd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.mhx1999.top/gtvcxphfie.html

[C09] 递归
来源：http://hz.zhijiandao.cn/gtupqnavwi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258.top/gtsvlmfyhp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yongpay.top/gtikrfmrgt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtdqmjckmq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydzc1.top/gtkmhuxzkd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yvedp.cn/gtzqemleil.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.52xcode.cn/gtfgvifmea.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ybcxt.top/gtpvtorpav.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.pycfn.com/gtplzpsfsc.html

[C10] 变量作用域
来源：http://hz.andypj.xyz/gtchlsmynu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.fengsongda.top/gtmvqhlbrx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.guannengcc.top/gtuwjdoifg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.guowangkeji.top/gtzakhdwvw.html

TS:   同 JS
来源：http://hz.hywenlv.cn/gtmqlzzcht.html

Java: 方法内为块级作用域
来源：http://hz.yueranfly.top/gtliafegne.html

Go:   花括号块级作用域
来源：http://hz.ybcxt.top/gtwnqsuijz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.aizwys.cn/gtfefkkzon.html

C#:   块级作用域
来源：http://hz.c1oappe.top/gtjqeskvqe.html

[C11] 模块导入与导出
来源：http://hz.dianchejie.cn/gthmclckhy.html

Py:   from module import func
来源：http://hz.nanxinkj.top/gtmsogqgcc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.haohaochexian.top/gtgseuzozg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yvedp.cn/gtkedlqvsq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhijiandao.cn/gtoqwpmatn.html

Java: import java.util.List;
来源：http://hz.dianchejie.cn/gtvfcnfvfp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yuxming.cn/gtcpermlpk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xylfe.cn/gtivtxqswy.html

C#:   using System.Text;
来源：http://hz.aibaodan.cn/gtehsvyodj.html

[C12] 立即执行函数 IIFE
来源：http://hz.aibaodan.cn/gtwerzgbaa.html

Py:   (lambda: print("run"))()
来源：http://hz.dashuyun.cn/gteqvhcxyt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ehwqpu.com/gtzjihtamu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gtpoarjtbr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gttwzgotky.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgfzy.top/gtsqlmfmqs.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yangfankeji.com/gtxfusuffz.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydjk.org.cn/gtkpojnizp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.nanxuanxn.top/gtpqpuoocg.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgufenzy.top/gtzxwetfdg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jiagoushi.top/gtlybttsll.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtkmukdpsy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.feifeiyinyue.top/gtyznwynad.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtjvzujivn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yvedp.cn/gtiuumpvgw.html

Go:   func add(a, b int) int
来源：http://hz.zhixingplan.top/gtzjajmqsw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhixingplan.top/gttlgdzrnt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yangfankeji.com/gtgbzgfxqj.html

[C14] 泛型函数
来源：http://hz.pycfn.com/gtyzwofgoy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yvedp.cn/gtupgmutln.html

PHP:  // 无泛型
来源：http://hz.yueranfly.top/gtzqopxusl.html

JS:   // 无泛型
来源：http://hz.sxryk.cn/gtsbvjazoc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.iojbl.cn/gtdwhyvazp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.kuanghao11.cn/gtdxxjyzvr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.bjfxy.top/gtqolrmrdd.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangtech.top/gthgcmcnds.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinqigufen.top/gtgxubnftr.html

[C15] 解构 / 展开参数
来源：http://hz.ehwqpu.com/gtcxooocqn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cqqwz.cn/gtmceeywcq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hysaishi.cn/gteclhidkc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.vqdsnc.cn/gtcsvydrfx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.svipenyu.cn/gtyeqkjoja.html

Java: // 无解构
来源：http://hz.dianchejie.cn/gtxnuambiw.html

Go:   // 无解构
来源：http://hz.jqgfzy.top/gtbqljzwml.html

Ruby: a, b = pair
来源：http://hz.tanke756.top/gthmhennbc.html

C#:   var (a, b) = pair;
来源：http://hz.daxiang520.top/gtrvwjzgjw.html

[C16] 函数 / 方法重载
来源：http://hz.jlsjyb.cn/gtfnqndckn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nanxuanxn.top/gttotngeth.html

PHP:  // 无重载
来源：http://hz.zhiwuduotai.top/gtffrlflrj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ppjwa.cn/gtagrtpgkz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nanxuanxn.top/gtynmtdqlu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yueranfly.top/gtsnndcnfw.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj20258.top/gtwglttpvu.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ehwqpu.com/gtfdjejpyp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yueranfly.top/gtibyyszwh.html

================================================================================
来源：http://hz.nwbrower.top/gtzyyacawf.html

D. 数组 / 列表 / 集合
来源：http://hz.zhaomingkeji.xyz/gtinooovyh.html

================================================================================
来源：http://hz.hammf.cn/gtvqpepiga.html

[D01] 创建数组 / 列表
来源：http://hz.ppjwa.cn/gtraprftic.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhoulong.xyz/gtydthqxyj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.dianchejie.cn/gtuexnqdot.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yuanzhike.top/gtdpkkzyqs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.svipenyu.cn/gthewvoapq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ehwqpu.com/gtfipulgzr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.andypj.xyz/gtngillxts.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinqigufen.top/gtcsisghdr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinqigufen.top/gtpwuyokvq.html

[D02] 追加元素到末尾
来源：http://hz.guowangkeji.top/gtyexbrqih.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.bjfxy.top/gtxdcsnvsf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ppjwa.cn/gtaoblukcf.html

JS:   arr.push(4);
来源：http://hz.havefunace.top/gtrodsxqbk.html

TS:   arr.push(4);
来源：http://hz.xylfe.cn/gtalltgqun.html

Java: list.add(4);
来源：http://hz.dashuyun.cn/gtrnknsxji.html

Go:   arr = append(arr, 4)
来源：http://hz.tianlin.xyz/gtiocpdcwo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhongyouzk.top/gtyzowzpbf.html

C#:   list.Add(4);
来源：http://hz.hysaishi.cn/gtagwaqnvy.html

[D03] 在指定位置插入元素
来源：http://hz.zhoulong.xyz/gtccvvixee.html

Py:   arr.insert(0, 0)
来源：http://hz.xylfe.cn/gthponwjvd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.316326.xyz/gtsewoxitl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.0kj1m.cn/gtknnhxapl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.nwbrower.top/gtnjkmvjfa.html

Java: list.add(0, 0);
来源：http://hz.xinyue.icu/gtgkmijzgj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ywan-chungtsiang.top/gtbdkxuohq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shuidangran.top/gtrxgyqurj.html

C#:   list.Insert(0, 0);
来源：http://hz.hywenlv.cn/gtfnmpggnz.html

[D04] 删除元素
来源：http://hz.iojbl.cn/gtkytkamvk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jiagoushi.top/gtikhjebyb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jianghu66.top/gtzazioiah.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xziqi.cn/gtqiwrwtpy.html

TS:   arr.splice(0, 1);
来源：http://hz.hnqzz.top/gtxlxbffax.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cashguo.top/gtalhbzswh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ydjk.org.cn/gtxnthcvxh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jqgfzy.top/gtntgjvljf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jqgfzy.top/gtxbstjznh.html

[D05] 访问与修改元素
来源：http://hz.jianghu66.top/gtoyxyzzam.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtljmpggjq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenjidiqi.icu/gttmbcakhz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.birdmap.top/gtibntrfip.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gotoacloud.top/gtsnfziayx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj20258.top/gttlxmyyqj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aizwys.cn/gtzmolrylt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shangyingyoupin.top/gtixmlranh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ehwqpu.com/gtvlomqdva.html

[D06] 数组长度
来源：http://hz.sweek.top/gtbmkhsvvg.html

Py:   len(arr)
来源：http://hz.chenjidiqi.icu/gtdeprfimv.html

PHP:  count($arr);
来源：http://hz.aibaodan.cn/gtyiyuhqkj.html

JS:   arr.length
来源：http://hz.zycfv.cn/gtrtfggdrv.html

TS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtrceripuh.html

Java: list.size();
来源：http://hz.guowangkeji.top/gtbbziahvf.html

Go:   len(arr)
来源：http://hz.mhx1999.top/gthmrtotpg.html

Ruby: arr.length; arr.size
来源：http://hz.shangyingyoupin.top/gtvhubcvfi.html

C#:   list.Count;
来源：http://hz.ydjk.org.cn/gtdhxgdvjt.html

[D07] 切片 / 取子数组
来源：http://hz.chenzaomai.com/gtmpujgkfc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.c1oappe.top/gtezekbuaw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.feifeiyinyue.top/gtywistdrb.html

JS:   arr.slice(1, 4);
来源：http://hz.yuxming.cn/gtuoukseda.html


<!-- 参考信息 -->