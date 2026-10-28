代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://hz.fengsongda.top/gtkhyqqvsg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ehwqpu.com/gtobdblsab.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.chenlongwang.top/gtefsdzlaq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtcvormmhb.html

[B09] break 与 continue
来源：http://hz.tanke756.top/gtgrshhcyk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yueranfly.top/gtcqqpagty.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtpxfsgcaq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtktlajzyk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtlcwnjqmo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shzxlz.cn/gtbppqwmcx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jiagoushi.top/gtweqaaxkc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.guannengcc.top/gttyeqpnqo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guannengcc.top/gtgyrhqjho.html

[B10] 遍历同时拿索引
来源：http://hz.yueranfly.top/gtymdumgfq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhongyouzk.top/gtcqnkpnox.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cdnleiting.top/gtmavcixvy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.smart0.xyz/gtfpzvrfmh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.nwbrower.top/gtfxkfrbfe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.316326.xyz/gtdrwgamwj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj20258.top/gtczrqvitg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.feifeiyinyue.top/gtqdywqeix.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.quarkkingdee.top/gtsyhjukpf.html

[B11] 生成数字序列 / 区间
来源：http://hz.nwbrower.top/gturkytjsc.html

Py:   list(range(0, 10, 2))
来源：http://hz.xuetiantiany.cn/gtygfnmlfb.html

PHP:  range(0, 10, 2);
来源：http://hz.hywenlv.cn/gtkmgxeprx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.316326.xyz/gtqygpayxo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daxiang520.top/gtrdhlavmv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhaomingkeji.xyz/gtsmbcsthg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jyoumei.cn/gtqbkpgqae.html

Ruby: (0...10).step(2).to_a
来源：http://hz.iojbl.cn/gtktwjijos.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tianlin.xyz/gtcxusshpf.html

[B12] 跳出多层循环
来源：http://hz.meibo888.top/gtepzzlgwf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sweek.top/gtwmpictyc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yuxming.cn/gtnhrprhdi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtdktniyjj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangdashe.top/gtjaesoiaa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtmtrquhsy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hnqzz.top/gttcivnfxl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.316326.xyz/gtwcaeclwa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shzxlz.cn/gthpidaocf.html

[B13] 判断是否为数字
来源：http://hz.snrcjt.cn/gtsdfyixcn.html

Py:   isinstance(x, (int, float))
来源：http://hz.fzhhl.top/gtqkzzjvco.html

PHP:  is_numeric($x)
来源：http://hz.redwolf501.top/gtsdhfbbmx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.iojbl.cn/gtbsdtuyzr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yueranfly.top/gtknkprwuw.html

Java: x instanceof Number
来源：http://hz.jlsjyb.cn/gtibaxddlu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.snrcjt.cn/gtgiencxnp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.feifeiyinyue.top/gttiiciddl.html

C#:   x is int or double or decimal
来源：http://hz.chenzaomai.com/gtzzhfjygv.html

[B14] 判断值是否在集合内
来源：http://hz.jyoumei.cn/gtfgnfmbqw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zycfv.cn/gthzdbvfrc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ehwqpu.com/gtfiisrval.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.chenjidiqi.icu/gtlrvpqrmp.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhiwuduotai.top/gtkoljjpfk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hysaishi.cn/gtzzrkdepw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hammf.cn/gtekvulapc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.nanxuanxn.top/gtuvbsfxwu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtittigrkr.html

[B15] 布尔运算与取反
来源：http://hz.zhoulong.xyz/gtduhsxxet.html

Py:   a and b or not c
来源：http://hz.jinghuilouyu.cn/gtxddvztto.html

PHP:  $a && $b || !$c
来源：http://hz.yongpay.top/gtoxtwbpcp.html

JS:   a && b || !c
来源：http://hz.fzhhl.top/gtniwdhxvn.html

TS:   a && b || !c
来源：http://hz.wangdashe.top/gtvqykovby.html

Java: a && b || !c
来源：http://hz.ppjwa.cn/gtpbydlgls.html

Go:   a && b || !c
来源：http://hz.fzhhl.top/gtjvffumbg.html

Ruby: a && b || !c
来源：http://hz.daria6918.cn/gtwhyxicdy.html

C#:   a && b || !c
来源：http://hz.fzhhl.top/gtugwfscyz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.redwolf501.top/gtoopnedia.html

Py:   if not data: return
来源：http://hz.jqgfzy.top/gtqbkxiapi.html

PHP:  if (!$data) { return; }
来源：http://hz.xinyue.icu/gtdjygagwo.html

JS:   if (!data) return;
来源：http://hz.bjfxy.top/gtdkmvkgfw.html

TS:   if (!data) return;
来源：http://hz.zhengqikj.top/gtetwoqpza.html

Java: if (data == null) return;
来源：http://hz.hnxiangtu.top/gtxswyvswn.html

Go:   if data == nil { return }
来源：http://hz.gaohongyu789.top/gtizsihbsx.html

Ruby: return if data.nil?
来源：http://hz.fengsongda.top/gtdijuhykd.html

C#:   if (data == null) return;
来源：http://hz.zhiwuduotai.top/gtehoxqnnt.html

================================================================================
来源：http://hz.meibo888.top/gtyagoamjt.html

C. 函数与作用域
来源：http://hz.dashuyun.cn/gtythoeuzw.html

================================================================================
来源：http://hz.zhoulong.xyz/gtpkkfncko.html

[C01] 定义函数
来源：http://hz.dianchejie.cn/gtqejriysy.html

Py:   def add(a, b): return a + b
来源：http://hz.daxiang520.top/gtgbjouasv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gthfqeikqx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yonumen.top/gtjldipild.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxuanxn.top/gttofjqdlz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtpptxtcpw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xingfuxueyuan.xyz/gtweziwvip.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yangfankeji.com/gtvyrscnjh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtqdfqrtef.html

[C02] 默认参数
来源：http://hz.sxryk.cn/gtsynxeaec.html

Py:   def greet(name="World"): return name
来源：http://hz.yangfankeji.com/gtzjulaghm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dashuyun.cn/gtjmsqxvsb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.bjfxy.top/gtsmumybjc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sufxvd.cn/gthcrpwvlz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.iojbl.cn/gtkrgmmxic.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.iojbl.cn/gturelzccr.html

Ruby: def greet(name = "World") = name
来源：http://hz.jyoumei.cn/gtcyyvlwwt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.redwolf501.top/gtssouramc.html

[C03] 可变参数
来源：http://hz.zhongyouzk.top/gtcdktwhor.html

Py:   def total(*args): return sum(args)
来源：http://hz.gzhubu.top/gtpldnprlo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yongpay.top/gttgqjhjhe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jyoumei.cn/gttvryjpof.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinyuanbaomall.cn/gtnicjcfur.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.tanke756.top/gtdgefkgaz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258.top/gtpvojbjft.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sufxvd.cn/gtgpcjosip.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.sysykeji.top/gtxfdyvpia.html

[C04] 命名参数 / 关键字参数
来源：http://hz.aibaodan.cn/gtxmbflrsl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yuanzhike.top/gteqzxvtuz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shanyushiyangkeji.top/gtfpasvazu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jqgufenzy.top/gtwbigwlqb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gzhubu.top/gtrjpsjqgb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.pycfn.com/gtunkmgdxb.html

Go:   // 无：用配置结构体参数
来源：http://hz.nanxuanxn.top/gtgdfdqzbx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.havefunace.top/gtpcpjliiw.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gtyjruntdc.html

[C05] 返回多个值
来源：http://hz.guannengcc.top/gtbnbtkzcl.html

Py:   return a, b
来源：http://hz.quarkkingdee.top/gtwulwkpop.html

PHP:  return [$a, $b];
来源：http://hz.quarkkingdee.top/gtopcoliec.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xylfe.cn/gtvknkclnd.html

TS:   return { a, b };
来源：http://hz.jianghu66.top/gtmhzdgfuw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nanxinkj.top/gtlufsexze.html

Go:   return a, b
来源：http://hz.vqdsnc.cn/gtqjitmjxz.html

Ruby: return a, b
来源：http://hz.daxiang520.top/gtzrmkxawc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cdnleiting.top/gtszssptfc.html

[C06] 匿名函数 / lambda
来源：http://hz.yongpay.top/gteoqdchjd.html

Py:   square = lambda x: x * x
来源：http://hz.xziqi.cn/gtqeodpbup.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.dashuyun.cn/gtsvzgfifp.html

JS:   const square = x => x * x;
来源：http://hz.dianchejie.cn/gtwdatubce.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sufxvd.cn/gtauoiaxbw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tianlin.xyz/gtazchwtba.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.sysykeji.top/gtpzyjrmvp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.gogol.net.cn/gtaogcqejp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.meibo888.top/gtostiksre.html

[C07] 把函数作为参数传入
来源：http://hz.cucudq.cn/gtegtxtbuc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhengqikj.top/gtmnyyfilb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuetiantiany.cn/gtukvfgrjf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.fengsongda.top/gtilribsqb.html

TS:   arr.map(String)
来源：http://hz.ehwqpu.com/gthxowirqg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.daxiang520.top/gtgkgieyrg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yuxming.cn/gtiusowakp.html

Ruby: arr.map(&:upcase)
来源：http://hz.fzhhl.top/gtjzossqlz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gotoacloud.top/gtnhpiimse.html

[C08] 闭包
来源：http://hz.redwolf501.top/gtlwdjpskl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.0kj1m.cn/gtyhqxdcka.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sxryk.cn/gtkgrvgfuk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtyzvdrwpk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtsxcrlvrq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.snrcjt.cn/gteqwjqidg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhiwuduotai.top/gtelvdswbn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ehwqpu.com/gtjdekbeod.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.redwolf501.top/gtiavjyhhl.html

[C09] 递归
来源：http://hz.birdmap.top/gtwmxczqoh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yueranfly.top/gtmrogwgwj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cqqwz.cn/gthaqtvmtc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtcklswzhd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gotoacloud.top/gtbxoooqiz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhongyouzk.top/gtzrqvduje.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.pengpengdd.cyou/gtimmriqhb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tian-w.cn/gtnfvgroza.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hysaishi.cn/gtfoeeeiak.html

[C10] 变量作用域
来源：http://hz.shangyingyoupin.top/gtidgowmiu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jqgfzy.top/gtgivbmepq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sweek.top/gtfuaxbjrk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shzxlz.cn/gtcvwlpjbi.html

TS:   同 JS
来源：http://hz.zycfv.cn/gtdpyzsmrp.html

Java: 方法内为块级作用域
来源：http://hz.cucudq.cn/gtqgtwpfzy.html

Go:   花括号块级作用域
来源：http://hz.hywenlv.cn/gtrvvedwbn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cucudq.cn/gtnhhynlgx.html

C#:   块级作用域
来源：http://hz.shanyushiyangtech.top/gtulqqzouk.html

[C11] 模块导入与导出
来源：http://hz.gaohongyu789.top/gtxkjbulon.html

Py:   from module import func
来源：http://hz.shuidangran.top/gttgsbjoue.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sweek.top/gtiqsdqeoi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xinyue.icu/gtfejdrxsa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinqigufen.top/gtaatzpfmp.html

Java: import java.util.List;
来源：http://hz.ivvv.top/gtngjpwaju.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.haohaochexian.top/gtpsxoskax.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhiwuduotai.top/gtxbbxeajf.html

C#:   using System.Text;
来源：http://hz.nanxinkj.top/gtzprclhuq.html

[C12] 立即执行函数 IIFE
来源：http://hz.nanxinkj.top/gtqjbruadc.html

Py:   (lambda: print("run"))()
来源：http://hz.gzhubu.top/gthxsllaym.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shanyushiyangtech.top/gtxmswepqo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gtanykseza.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangtech.top/gtjyshffhu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cdnleiting.top/gtwoftwmte.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hfpthk.cn/gtotcamqii.html

Ruby: -> { puts "run" }.call
来源：http://hz.wangdashe.top/gtuxrkevdg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.redwolf501.top/gtqsfwgsyb.html

[C13] 类型声明 / 类型注解
来源：http://hz.jlsjyb.cn/gtajczonsl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yj20258.top/gtutaiguhp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.iojbl.cn/gtwzufnzua.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yangfankeji.com/gtkuvkbwzx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pengpengdd.cyou/gttsxtxswe.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtcjohsret.html

Go:   func add(a, b int) int
来源：http://hz.fzhhl.top/gtxfvyvpoh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydzc1.top/gtfwmwhuhk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gzhubu.top/gtzfztwpzt.html

[C14] 泛型函数
来源：http://hz.sysykeji.top/gtrkzgdqgo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hysaishi.cn/gtzxznzwcg.html

PHP:  // 无泛型
来源：http://hz.havefunace.top/gtijwyalxz.html

JS:   // 无泛型
来源：http://hz.pengpengdd.cyou/gtbvsoxxgr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shuidangran.top/gttbbbmlnb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hfpthk.cn/gtrznofekf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.meibo888.top/gtvplngmme.html

Ruby: # 无泛型
来源：http://hz.smart0.xyz/gtvkjqdrjy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zdqjudy.top/gtvggehunc.html

[C15] 解构 / 展开参数
来源：http://hz.jinyuanbaomall.cn/gtmrpnhaos.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sufxvd.cn/gtfsbusctp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.wangdashe.top/gtsaoadrrf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hysaishi.cn/gtendxekwf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ehwqpu.com/gthnnxgzon.html

Java: // 无解构
来源：http://hz.shuidangran.top/gtdvrciodt.html

Go:   // 无解构
来源：http://hz.dianchejie.cn/gtlnipvxfl.html

Ruby: a, b = pair
来源：http://hz.cdnleiting.top/gtuhjfktsr.html

C#:   var (a, b) = pair;
来源：http://hz.birdmap.top/gtwaptvmpw.html

[C16] 函数 / 方法重载
来源：http://hz.snrcjt.cn/gtjdqvqpjv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.52xcode.cn/gtaotdkybi.html

PHP:  // 无重载
来源：http://hz.xingfuxueyuan.xyz/gtmarmdhcy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.quarkkingdee.top/gtrpkfkthw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cashguo.top/gtdksqluxh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jqgufenzy.top/gtbdwzdimu.html

Go:   // 无重载：用不同函数名
来源：http://hz.shanyushiyangkeji.top/gtkevavjki.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhixingplan.top/gtmuydwbfo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.andypj.xyz/gtjzuyuxsx.html

================================================================================
来源：http://hz.hfpthk.cn/gtsfesqgrx.html

D. 数组 / 列表 / 集合
来源：http://hz.cucudq.cn/gtiskbyeei.html

================================================================================
来源：http://hz.hnxiangtu.top/gtbpgabgxk.html

[D01] 创建数组 / 列表
来源：http://hz.zycfv.cn/gtbizbsktp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.52xcode.cn/gtfcpkotqk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.kuanghao11.cn/gtrvasnysd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yangfankeji.com/gtlxarxrae.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.316326.xyz/gtnmsrhfvi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhiwuduotai.top/gtzgpothqg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.feifeiyinyue.top/gtygilyxvw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.havefunace.top/gtkjtpsawv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xinyue.icu/gtsjjerbcg.html

[D02] 追加元素到末尾
来源：http://hz.gaohongyu789.top/gtxcdtmbzl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.feifeiyinyue.top/gtwovkqpve.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.52xcode.cn/gtvlktmadc.html

JS:   arr.push(4);
来源：http://hz.yueranfly.top/gtqrvusqbk.html

TS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtbxotkinw.html

Java: list.add(4);
来源：http://hz.snrcjt.cn/gtweigtuit.html

Go:   arr = append(arr, 4)
来源：http://hz.kuanghao11.cn/gtmrzyyhiz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sweek.top/gtvvqvbzdr.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangtech.top/gtirkrxehi.html

[D03] 在指定位置插入元素
来源：http://hz.svipenyu.cn/gtmydgpzdx.html

Py:   arr.insert(0, 0)
来源：http://hz.sysykeji.top/gtkpueuhte.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hnxiangtu.top/gtmipnepro.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yuanzhike.top/gtrfguxghp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.vqdsnc.cn/gthkgmsmfx.html

Java: list.add(0, 0);
来源：http://hz.jinqigfzy.top/gtjseawyln.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.wangshuangyany.cn/gtocmdlqfx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.snrcjt.cn/gtnmdahaks.html

C#:   list.Insert(0, 0);
来源：http://hz.wangshuangyany.cn/gtpvyvttmv.html

[D04] 删除元素
来源：http://hz.ybcxt.top/gttcpzplsn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nanxuanxn.top/gtcjkhjlqi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.dianchejie.cn/gttcamvrpp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yuxming.cn/gtsaugcudb.html

TS:   arr.splice(0, 1);
来源：http://hz.0kj1m.cn/gtmarkxskd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yangfankeji.com/gtwphaoyks.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.feifeiyinyue.top/gtfujibvrj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.birdmap.top/gtwnzqtome.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.vqdsnc.cn/gtlyxbklxc.html

[D05] 访问与修改元素
来源：http://hz.hammf.cn/gtqgwnqfca.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtdvydzsor.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cashguo.top/gtxnxmpzdy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.svipenyu.cn/gtrxgcybjq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.andypj.xyz/gtitsxhwjy.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.snrcjt.cn/gtdqhpmadf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zycfv.cn/gtyuphafbl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtddsxvare.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.vqdsnc.cn/gtqmnrqchk.html

[D06] 数组长度
来源：http://hz.pycfn.com/gtbagbochj.html

Py:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gtcojchkjw.html

PHP:  count($arr);
来源：http://hz.9152youxi.cn/gtfuegvjvg.html

JS:   arr.length
来源：http://hz.feifeiyinyue.top/gtcwtdipmn.html

TS:   arr.length
来源：http://hz.yuxming.cn/gtbvbdpkwm.html

Java: list.size();
来源：http://hz.jyoumei.cn/gtyqzqfole.html

Go:   len(arr)
来源：http://hz.havefunace.top/gtlzixbowt.html

Ruby: arr.length; arr.size
来源：http://hz.hysaishi.cn/gtgqxyhova.html

C#:   list.Count;
来源：http://hz.cdnleiting.top/gtevbsntrm.html

[D07] 切片 / 取子数组
来源：http://hz.pycfn.com/gthhycwwtu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gzhubu.top/gtuuoltrvt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jqgfzy.top/gtckasvkgg.html

JS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gthxhgtsrw.html

TS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtfmphkemq.html

Java: list.subList(1, 4);
来源：http://hz.xuanzx.com/gtxtizhntd.html

Go:   arr[1:4]
来源：http://hz.jqgufenzy.top/gtbilipksm.html

Ruby: arr[1, 3]
来源：http://hz.jinghuilouyu.cn/gtnfgkadqp.html

C#:   list.GetRange(1, 3);
来源：http://hz.cqqwz.cn/gtbxgyopqo.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangkeji.top/gtanvmshwi.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhixingplan.top/gtavxjcbwu.html

PHP:  array_merge($a, $b);
来源：http://hz.yonumen.top/gtzxgouqsw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xingfuxueyuan.xyz/gtgrwyxaff.html

TS:   [...a, ...b];
来源：http://hz.zycfv.cn/gtjbagjjor.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.fengsongda.top/gtyihomaua.html

Go:   append(a, b...)
来源：http://hz.hnqzz.top/gtmumqsmyj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhoulong.xyz/gtohhdishn.html

C#:   a.Concat(b).ToList()
来源：http://hz.hfpthk.cn/gtnthojzfh.html

[D09] 排序（升序）
来源：http://hz.sysykeji.top/gtiqrlkyif.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258.top/gttkcawjjd.html


<!-- 参考信息 -->