代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.svipenyu.cn/gttelwcrmw.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shanyushiyangtech.top/gtslsviwce.html

C#:   while (i < 10) { i++; }
来源：http://hz.tanke756.top/gtdiecokhw.html

[B08] do-while（至少执行一次）
来源：http://hz.snrcjt.cn/gtnvmyztti.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cdnleiting.top/gtaipzestf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.aibaodan.cn/gtyuedvagm.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtssgybdhw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ppjwa.cn/gtwsgmturm.html

Java: do { i++; } while (i < 10);
来源：http://hz.meibo888.top/gtsxmgeysq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yueranfly.top/gtrgcinzvi.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.316326.xyz/gtndhkdgol.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtftchmzuk.html

[B09] break 与 continue
来源：http://hz.vqdsnc.cn/gttxsjtkkv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.chenjidiqi.icu/gtzpgrdybn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ybcxt.top/gtfcgkkvnx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtskdahaqy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj202588.top/gtlgaelooi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtrktnosdv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jiagoushi.top/gttclqivup.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.nanxuanxn.top/gttcknfllk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shzxlz.cn/gtejmrdgtg.html

[B10] 遍历同时拿索引
来源：http://hz.tianlin.xyz/gtsqhgumwi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.redwolf501.top/gtfdnybqso.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xingfuxueyuan.xyz/gtqrgwvgnc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jiagoushi.top/gtiiuymbix.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhongyouzk.top/gtdqkxvjmu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hnxiangtu.top/gtfogkxdob.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhengqikj.top/gtuocrwmsa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yangfankeji.com/gttylcwlud.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigfzy.top/gthslnikpz.html

[B11] 生成数字序列 / 区间
来源：http://hz.c1oappe.top/gtdzzezmih.html

Py:   list(range(0, 10, 2))
来源：http://hz.xuetiantiany.cn/gtlpxjhlxp.html

PHP:  range(0, 10, 2);
来源：http://hz.shangyingyoupin.top/gtuzfwvbzp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gtpnvcenkq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shuidangran.top/gtrbxqksoh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.daxiang520.top/gtgzvfopyi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yangfankeji.com/gtlewevojs.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xuanzx.com/gtxltlgptj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhoulong.xyz/gtcyiszdql.html

[B12] 跳出多层循环
来源：http://hz.yvedp.cn/gtltebdihf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhijiandao.cn/gtezpohich.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.mhx1999.top/gtiupjrfjq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ywan-chungtsiang.top/gtzsjckiae.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtqicbifbk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cucudq.cn/gtnlaymujx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hfpthk.cn/gtmrrueoan.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xylfe.cn/gtdxljkeir.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jqgfzy.top/gtftalptpw.html

[B13] 判断是否为数字
来源：http://hz.yj20258888.top/gtzleujvie.html

Py:   isinstance(x, (int, float))
来源：http://hz.haohaochexian.top/gtyjgkcfjf.html

PHP:  is_numeric($x)
来源：http://hz.andypj.xyz/gtpihwmgmp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.quarkkingdee.top/gtkulpaylg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xylfe.cn/gthhcxwhhi.html

Java: x instanceof Number
来源：http://hz.ivvv.top/gtcnkflcis.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinqigfzy.top/gtnpywutqg.html

Ruby: x.is_a?(Numeric)
来源：http://hz.haohaochexian.top/gtywkkztil.html

C#:   x is int or double or decimal
来源：http://hz.nanxinkj.top/gtzumraxwu.html

[B14] 判断值是否在集合内
来源：http://hz.haohaochexian.top/gtxcwfpdov.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gotoacloud.top/gtycoufdct.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yongpay.top/gtsnfhcvzs.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jlsjyb.cn/gtolsfbszg.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gogol.net.cn/gtrlflbatc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhaomingkeji.xyz/gtwmmgrvct.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yuanzhike.top/gtfhtvhzgi.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.fzhhl.top/gtbicqvypp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jqgufenzy.top/gtrwuqachk.html

[B15] 布尔运算与取反
来源：http://hz.aizwys.cn/gtjiyenbho.html

Py:   a and b or not c
来源：http://hz.hysaishi.cn/gttybwqncp.html

PHP:  $a && $b || !$c
来源：http://hz.iojbl.cn/gttfzkdkug.html

JS:   a && b || !c
来源：http://hz.ppjwa.cn/gtkrciiivw.html

TS:   a && b || !c
来源：http://hz.yj20258888.top/gtqynocgtz.html

Java: a && b || !c
来源：http://hz.chenlongwang.top/gtnuvqbkjy.html

Go:   a && b || !c
来源：http://hz.hnxiangtu.top/gtgupvygjd.html

Ruby: a && b || !c
来源：http://hz.zycfv.cn/gtqiphpuig.html

C#:   a && b || !c
来源：http://hz.aibaodan.cn/gtbfyttajv.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.smart0.xyz/gtsooiitvc.html

Py:   if not data: return
来源：http://hz.ehwqpu.com/gtfbrftsli.html

PHP:  if (!$data) { return; }
来源：http://hz.yueranfly.top/gtukvmwdpm.html

JS:   if (!data) return;
来源：http://hz.shuidangran.top/gtdwevtzgm.html

TS:   if (!data) return;
来源：http://hz.daxiang520.top/gtwysuigjc.html

Java: if (data == null) return;
来源：http://hz.guowangkeji.top/gtplttqbzz.html

Go:   if data == nil { return }
来源：http://hz.dashuyun.cn/gtboxbbltt.html

Ruby: return if data.nil?
来源：http://hz.jyoumei.cn/gtsnzflldk.html

C#:   if (data == null) return;
来源：http://hz.xziqi.cn/gtxzjrddud.html

================================================================================
来源：http://hz.nwbrower.top/gtzijczyim.html

C. 函数与作用域
来源：http://hz.shanyushiyangtech.top/gtqungsonz.html

================================================================================
来源：http://hz.jinqigfzy.top/gtfipgsexi.html

[C01] 定义函数
来源：http://hz.52xcode.cn/gtvofjwuhu.html

Py:   def add(a, b): return a + b
来源：http://hz.yangfankeji.com/gtdldoklve.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sweek.top/gthshfmomn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.birdmap.top/gtclcyctnf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtdrsueoxa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtiwqetwoy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cqqwz.cn/gtimmasyaq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xinyue.icu/gtsodnznxb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtkzdxdbxs.html

[C02] 默认参数
来源：http://hz.ydzc1.top/gtmjcbxari.html

Py:   def greet(name="World"): return name
来源：http://hz.quarkkingdee.top/gtucsmixsi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.c1oappe.top/gtwicseryp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.aibaodan.cn/gtgtshezmm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gogol.net.cn/gtqjjcxnvy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj20258888.top/gtxldziisu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jianghu66.top/gtcqlgzeiv.html

Ruby: def greet(name = "World") = name
来源：http://hz.iojbl.cn/gtayvkxros.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tian-w.cn/gtyhqpgmcs.html

[C03] 可变参数
来源：http://hz.chenlongwang.top/gtfaswggfs.html

Py:   def total(*args): return sum(args)
来源：http://hz.snrcjt.cn/gtnysnmgbl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.guowangkeji.top/gtmgddwyrb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gtgmuwxfgy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hfpthk.cn/gtixggtghb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.redwolf501.top/gtotqhulhf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhoulong.xyz/gteotjuobk.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinqigfzy.top/gtxgeeyiot.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.aizwys.cn/gtkgagykvu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.kuanghao11.cn/gtcajmmdih.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nwbrower.top/gtbldmhvui.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenjidiqi.icu/gtgiugznir.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtuhinpgtz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yvedp.cn/gtildkbggo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenjidiqi.icu/gtckvgvbns.html

Go:   // 无：用配置结构体参数
来源：http://hz.cdnleiting.top/gtcadgmmml.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtztupvdhi.html

C#:   f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gthuoierkz.html

[C05] 返回多个值
来源：http://hz.cheryme.top/gtzkxnecbm.html

Py:   return a, b
来源：http://hz.shangyingyoupin.top/gtdkulepwe.html

PHP:  return [$a, $b];
来源：http://hz.jqgufenzy.top/gtyelpexjd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.andypj.xyz/gtcyzpugea.html

TS:   return { a, b };
来源：http://hz.yangfankeji.com/gtkemrtahy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cqqwz.cn/gtkrwhogal.html

Go:   return a, b
来源：http://hz.shanyushiyangtech.top/gtkvlwcnrp.html

Ruby: return a, b
来源：http://hz.yonumen.top/gtomisppik.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xinyue.icu/gtydzqtsga.html

[C06] 匿名函数 / lambda
来源：http://hz.tanke756.top/gtciddpadz.html

Py:   square = lambda x: x * x
来源：http://hz.ywan-chungtsiang.top/gtmxckuofr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.316326.xyz/gtqiyrezmu.html

JS:   const square = x => x * x;
来源：http://hz.52xcode.cn/gtsffaqiwq.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xuetiantiany.cn/gtgfikvvvt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ydjk.org.cn/gthxypyhss.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ppjwa.cn/gtiewzwmqn.html

Ruby: square = ->(x) { x * x }
来源：http://hz.kuanghao11.cn/gtmbsjddyj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.snrcjt.cn/gtenyvtunj.html

[C07] 把函数作为参数传入
来源：http://hz.zhengqikj.top/gtkdogavho.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinyuanbaomall.cn/gtlgxrifcw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jinqigufen.top/gtpunolbep.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xziqi.cn/gtgbwssdgu.html

TS:   arr.map(String)
来源：http://hz.wangshuangyany.cn/gtkraxkcbk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gogol.net.cn/gtcptrkqcu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hongshengwenyu.top/gtauwypssl.html

Ruby: arr.map(&:upcase)
来源：http://hz.xinyue.icu/gtomeadnqe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ydjk.org.cn/gtsdcxltki.html

[C08] 闭包
来源：http://hz.9152youxi.cn/gttaaceixr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.birdmap.top/gtgafpjcjw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yangfankeji.com/gtrejsivhd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gtvbmfefyr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtejwwkklp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.aibaodan.cn/gtcwiykmtv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hnqzz.top/gtjcfydwsz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.snrcjt.cn/gthpzskkox.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ybcxt.top/gtxmdabaco.html

[C09] 递归
来源：http://hz.xuetiantiany.cn/gtpikwyqjw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shangyingyoupin.top/gtgigbbopu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yonumen.top/gtfnzurxps.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinyuanbaomall.cn/gtrcjgkykn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydjk.org.cn/gtobaetlyt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhijiandao.cn/gtqcnpdllg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ywan-chungtsiang.top/gtrzopcmfy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtrwhznmkr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.c1oappe.top/gtndmrqhkh.html

[C10] 变量作用域
来源：http://hz.gogol.net.cn/gtmckwwcgp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.guannengcc.top/gtxclrokwa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.feifeiyinyue.top/gtmyyrhzuq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sxryk.cn/gthwuwrqir.html

TS:   同 JS
来源：http://hz.meibo888.top/gtqrglhlus.html

Java: 方法内为块级作用域
来源：http://hz.hnxiangtu.top/gtdmvuxrar.html

Go:   花括号块级作用域
来源：http://hz.chenlongwang.top/gtnefjxmsh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yangfankeji.com/gtawozgvpa.html

C#:   块级作用域
来源：http://hz.shzxlz.cn/gtbpvqmsoa.html

[C11] 模块导入与导出
来源：http://hz.chenzaomai.com/gtobjjimop.html

Py:   from module import func
来源：http://hz.xziqi.cn/gtgvystqfw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.mhx1999.top/gtfrustsdp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhijiandao.cn/gtpceslats.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cheryme.top/gtfcaqzaoz.html

Java: import java.util.List;
来源：http://hz.chenlongwang.top/gtmwuderok.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hywenlv.cn/gtdygveppw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.havefunace.top/gtybludevf.html

C#:   using System.Text;
来源：http://hz.yj202588.top/gtwlhxlqkh.html

[C12] 立即执行函数 IIFE
来源：http://hz.cashguo.top/gtghbdvdmf.html

Py:   (lambda: print("run"))()
来源：http://hz.sweek.top/gthbriscmr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigfzy.top/gtreyvnavi.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtbmgvszrx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtqztukhtr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.vqdsnc.cn/gtqeelcyut.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sxryk.cn/gtscqfvvpr.html

Ruby: -> { puts "run" }.call
来源：http://hz.ehwqpu.com/gtbleveihl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.chenlongwang.top/gtothgtujn.html

[C13] 类型声明 / 类型注解
来源：http://hz.c1oappe.top/gtztiaizgj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guowangkeji.top/gtpufmnitu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gthhrwszjn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgfzy.top/gtktzlosqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xinyue.icu/gtnwbcmyyy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gtofohhmih.html

Go:   func add(a, b int) int
来源：http://hz.yangfankeji.com/gtszmtiltt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.tian-w.cn/gtjcuniuip.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gogol.net.cn/gtjlxjizdr.html

[C14] 泛型函数
来源：http://hz.bjfxy.top/gtukcofmcs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtxdkrotxi.html

PHP:  // 无泛型
来源：http://hz.c1oappe.top/gtevatwluw.html

JS:   // 无泛型
来源：http://hz.yanxiufei.cn/gtnsefprzo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shanyushiyangtech.top/gtfulnevtd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhaomingkeji.xyz/gtggguaybp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cdnleiting.top/gtvwvgxgth.html

Ruby: # 无泛型
来源：http://hz.aibaodan.cn/gttguaonxs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zdqjudy.top/gtmosacmdd.html

[C15] 解构 / 展开参数
来源：http://hz.bjfxy.top/gtpclpwvfr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tian-w.cn/gtkbkiutol.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yvedp.cn/gtuwrfjbcx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gotoacloud.top/gthgwdcuhf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hnqzz.top/gtzijbeydn.html

Java: // 无解构
来源：http://hz.zhiwuduotai.top/gtzlzbadwd.html

Go:   // 无解构
来源：http://hz.daxiang520.top/gtthwwkzmo.html

Ruby: a, b = pair
来源：http://hz.cdnleiting.top/gtqssekcpg.html

C#:   var (a, b) = pair;
来源：http://hz.yonumen.top/gtgbdanime.html

[C16] 函数 / 方法重载
来源：http://hz.cucudq.cn/gtphgqojnd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cqqwz.cn/gtewijcjtd.html

PHP:  // 无重载
来源：http://hz.9152youxi.cn/gtofdcbszw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.9152youxi.cn/gtogashnla.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhengqikj.top/gtemziektx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuetiantiany.cn/gteamwmowr.html

Go:   // 无重载：用不同函数名
来源：http://hz.shuidangran.top/gtrfedgbtc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dianchejie.cn/gtabjvfort.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinghuilouyu.cn/gtruwvmcmo.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtslxkvpes.html

D. 数组 / 列表 / 集合
来源：http://hz.cashguo.top/gtfxfgfpjw.html

================================================================================
来源：http://hz.hnxiangtu.top/gtdoxwqvxb.html

[D01] 创建数组 / 列表
来源：http://hz.hnqzz.top/gtayzqyqpe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangshuangyany.cn/gtprlywlgy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.pengpengdd.cyou/gtjsamdnyw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daria6918.cn/gtnbbtfgrc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258888.top/gtzqvxjunf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hywenlv.cn/gtdksgsbvf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.meibo888.top/gtbfixqece.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jqgfzy.top/gtutszmlhx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cucudq.cn/gtokkkusko.html

[D02] 追加元素到末尾
来源：http://hz.chenlongwang.top/gtagvrggtw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.iojbl.cn/gtparuwxuq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gotoacloud.top/gtitbxyfhl.html

JS:   arr.push(4);
来源：http://hz.birdmap.top/gtgjllknzi.html

TS:   arr.push(4);
来源：http://hz.316326.xyz/gtznawysog.html

Java: list.add(4);
来源：http://hz.zhiwuduotai.top/gttlmqlwzj.html

Go:   arr = append(arr, 4)
来源：http://hz.gzhubu.top/gteabphiiu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.pengpengdd.cyou/gtccccveux.html

C#:   list.Add(4);
来源：http://hz.yangfankeji.com/gtdzaqbcaz.html

[D03] 在指定位置插入元素
来源：http://hz.cashguo.top/gteqauzbjb.html

Py:   arr.insert(0, 0)
来源：http://hz.yongpay.top/gtibxryevk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guowangkeji.top/gtbltwbrwx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gzhubu.top/gtaezetqrs.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cdnleiting.top/gtkhowiyfq.html

Java: list.add(0, 0);
来源：http://hz.mhx1999.top/gtsvnlaxdl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gotoacloud.top/gtsblzwdjw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gaohongyu789.top/gtnzmsjfhp.html

C#:   list.Insert(0, 0);
来源：http://hz.gogol.net.cn/gtyuyflexy.html

[D04] 删除元素
来源：http://hz.zhiwuduotai.top/gttrsnfmzi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ehwqpu.com/gtgomzaqxc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.andypj.xyz/gtsulbuuhq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sxryk.cn/gtyzfpebyg.html

TS:   arr.splice(0, 1);
来源：http://hz.pycfn.com/gtfmpqzyxd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.meibo888.top/gtaciolydo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhongyouzk.top/gtzgnaynii.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.guowangkeji.top/gtnanykdns.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangdashe.top/gtferaifwc.html

[D05] 访问与修改元素
来源：http://hz.cucudq.cn/gtiomunses.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtokmuvibf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtapnanhlr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nanxinkj.top/gtnrjwdgbz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.svipenyu.cn/gtgfeqzjaa.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.havefunace.top/gtzsysctzh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtomexvgfq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ydjk.org.cn/gtfauvnjjn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.dashuyun.cn/gtxzyiawhc.html

[D06] 数组长度
来源：http://hz.ydzc1.top/gtopqadvyu.html

Py:   len(arr)
来源：http://hz.hysaishi.cn/gtwfxrzxfq.html

PHP:  count($arr);
来源：http://hz.jinqigfzy.top/gtmtnbdqnz.html

JS:   arr.length
来源：http://hz.hnxiangtu.top/gtiphavisw.html

TS:   arr.length
来源：http://hz.cashguo.top/gtiiyniouu.html

Java: list.size();
来源：http://hz.ppjwa.cn/gtojvwgcdu.html

Go:   len(arr)
来源：http://hz.havefunace.top/gtguqquhrp.html

Ruby: arr.length; arr.size
来源：http://hz.gotoacloud.top/gtzzhebaga.html

C#:   list.Count;
来源：http://hz.xylfe.cn/gtxwjexxeu.html

[D07] 切片 / 取子数组
来源：http://hz.gotoacloud.top/gtdvswjhua.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shanyushiyangkeji.top/gtrutpxwqb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sufxvd.cn/gtyekmibfm.html

JS:   arr.slice(1, 4);
来源：http://hz.snrcjt.cn/gthdyokaxd.html

TS:   arr.slice(1, 4);
来源：http://hz.gotoacloud.top/gtxedpuwxu.html

Java: list.subList(1, 4);
来源：http://hz.meibo888.top/gtbdetygav.html

Go:   arr[1:4]
来源：http://hz.jiagoushi.top/gtrnvaieuk.html

Ruby: arr[1, 3]
来源：http://hz.hysaishi.cn/gtovifkmgq.html

C#:   list.GetRange(1, 3);
来源：http://hz.snrcjt.cn/gtugwsmqjp.html

[D08] 合并两个数组
来源：http://hz.zhaomingkeji.xyz/gtsvgaporg.html

Py:   a + b;  a.extend(b)
来源：http://hz.hongshengwenyu.top/gtarrorzcd.html

PHP:  array_merge($a, $b);
来源：http://hz.shuidangran.top/gtndwidypg.html


<!-- 参考信息 -->