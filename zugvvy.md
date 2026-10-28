代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hz.pengpengdd.cyou/gtbwjudhbe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gzhubu.top/gtuumnwktj.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jianghu66.top/gttxfwkgsb.html

TS:   do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gttcsxpdqf.html

Java: do { i++; } while (i < 10);
来源：http://hz.sxryk.cn/gtvtnkrcto.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yj20258888.top/gtnvjtcpwf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.andypj.xyz/gtwxecugou.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhoulong.xyz/gtqtwtovcx.html

[B09] break 与 continue
来源：http://hz.dianchejie.cn/gtkpjavewl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yongpay.top/gtjmedpmik.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtdixwkjmf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtazmxjyud.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.svipenyu.cn/gtsgnupnkc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhijiandao.cn/gtldecqvfq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ehwqpu.com/gtcnsejald.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.quarkkingdee.top/gtoxsrusjc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtsfqrszzs.html

[B10] 遍历同时拿索引
来源：http://hz.shzxlz.cn/gthemljvhg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.dianchejie.cn/gtdnckkkpg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xinyue.icu/gtauarjvva.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinqigfzy.top/gtayjxevbc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.vqdsnc.cn/gtgnlwoctg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cheryme.top/gtathiqubu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hywenlv.cn/gtkltjvnqu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhijiandao.cn/gtdfmhinix.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigfzy.top/gthzazvezk.html

[B11] 生成数字序列 / 区间
来源：http://hz.tanke756.top/gtycmhydau.html

Py:   list(range(0, 10, 2))
来源：http://hz.guowangkeji.top/gtnlrpaayu.html

PHP:  range(0, 10, 2);
来源：http://hz.chenjidiqi.icu/gtqovplsde.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.316326.xyz/gttwddihef.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gtwimpvxez.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.redwolf501.top/gtmjiannlp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cqqwz.cn/gtzaosmjjm.html

Ruby: (0...10).step(2).to_a
来源：http://hz.0kj1m.cn/gtwyablpuy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hongshengwenyu.top/gtoswfaoul.html

[B12] 跳出多层循环
来源：http://hz.jianghu66.top/gtbotbywzf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.redwolf501.top/gtqbrtbcge.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinqigfzy.top/gtxwgqjbkx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.andypj.xyz/gtnejqrezp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zycfv.cn/gtguutjjnd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtmkihldwm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gzhubu.top/gtwcjxdchc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.0kj1m.cn/gtgfsbwlap.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.fengsongda.top/gtaxcaezex.html

[B13] 判断是否为数字
来源：http://hz.pycfn.com/gtwkcibncx.html

Py:   isinstance(x, (int, float))
来源：http://hz.aizwys.cn/gtjqfovdhs.html

PHP:  is_numeric($x)
来源：http://hz.tian-w.cn/gtqlfjyawy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgfzy.top/gtypkljhod.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yonumen.top/gthjrlvemc.html

Java: x instanceof Number
来源：http://hz.ydjk.org.cn/gtcxlpdvrn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.bjfxy.top/gtsrikrjog.html

Ruby: x.is_a?(Numeric)
来源：http://hz.fengsongda.top/gthhwdlzlm.html

C#:   x is int or double or decimal
来源：http://hz.daxiang520.top/gtxongmszx.html

[B14] 判断值是否在集合内
来源：http://hz.mhx1999.top/gttvocuppw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.316326.xyz/gtgmexsceg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.tanke756.top/gtpemkbufl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.tanke756.top/gtnksihvrm.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.havefunace.top/gtsktoqdzv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tian-w.cn/gtqfkwlxya.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guannengcc.top/gtvojknsjl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.meibo888.top/gthbqujbhh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hongshengwenyu.top/gtctpnpbcs.html

[B15] 布尔运算与取反
来源：http://hz.hywenlv.cn/gtqcokywug.html

Py:   a and b or not c
来源：http://hz.cqqwz.cn/gtiztetlpk.html

PHP:  $a && $b || !$c
来源：http://hz.chenzaomai.com/gtjysgsuhz.html

JS:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtvhtopxie.html

TS:   a && b || !c
来源：http://hz.hammf.cn/gtjpqwznle.html

Java: a && b || !c
来源：http://hz.yj20258888.top/gtnzyjdfle.html

Go:   a && b || !c
来源：http://hz.ydjk.org.cn/gthaioenjt.html

Ruby: a && b || !c
来源：http://hz.jianghu66.top/gtucfqwcma.html

C#:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtudwysgsg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.chenzaomai.com/gtxsbqzkoy.html

Py:   if not data: return
来源：http://hz.zhijiandao.cn/gtjkzsetgd.html

PHP:  if (!$data) { return; }
来源：http://hz.zhiwuduotai.top/gtwrphivoh.html

JS:   if (!data) return;
来源：http://hz.ydzc1.top/gtvvrowpfx.html

TS:   if (!data) return;
来源：http://hz.mhx1999.top/gtpdswwbpm.html

Java: if (data == null) return;
来源：http://hz.aibaodan.cn/gtazkyjdap.html

Go:   if data == nil { return }
来源：http://hz.chenjidiqi.icu/gtmoypfdqg.html

Ruby: return if data.nil?
来源：http://hz.iojbl.cn/gtcivwdhow.html

C#:   if (data == null) return;
来源：http://hz.chenjidiqi.icu/gtqmenxpta.html

================================================================================
来源：http://hz.yangfankeji.com/gtrcztkzxp.html

C. 函数与作用域
来源：http://hz.ywan-chungtsiang.top/gtmvngdeqw.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtdjulapfh.html

[C01] 定义函数
来源：http://hz.yonumen.top/gtksmwpaao.html

Py:   def add(a, b): return a + b
来源：http://hz.shanyushiyangtech.top/gtzacyedbo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtwjfopbre.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinqigfzy.top/gtkahkvunn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yongpay.top/gtzwbhafys.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtxhzugvby.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj20258888.top/gtjbvlaedt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xingfuxueyuan.xyz/gtirvarddw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtznahxqei.html

[C02] 默认参数
来源：http://hz.zdqjudy.top/gtsdvqhsgx.html

Py:   def greet(name="World"): return name
来源：http://hz.guowangkeji.top/gtboxqpgdr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.havefunace.top/gtnjpcgxdj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.daxiang520.top/gtentdcpzx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.pycfn.com/gtvmwnneud.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jiagoushi.top/gtpdilthut.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sufxvd.cn/gtmnqstydy.html

Ruby: def greet(name = "World") = name
来源：http://hz.wangdashe.top/gtibqzqxet.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.mhx1999.top/gtvqmpiaxb.html

[C03] 可变参数
来源：http://hz.jiagoushi.top/gtituiygtp.html

Py:   def total(*args): return sum(args)
来源：http://hz.xuanzx.com/gtgylrqqxx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.andypj.xyz/gtnudojabu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtxdsylkqj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ivvv.top/gtqrakzfqi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.birdmap.top/gtscxicxsb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hysaishi.cn/gtfpkssqsv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gaohongyu789.top/gtfornnaef.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dianchejie.cn/gtpgxnqbih.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ydjk.org.cn/gtldvmescx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yueranfly.top/gtpabmlbrj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ehwqpu.com/gtitkforhg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.bjfxy.top/gttufrgqhe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.svipenyu.cn/gthjzzwxhd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.svipenyu.cn/gtjshikulj.html

Go:   // 无：用配置结构体参数
来源：http://hz.aibaodan.cn/gtzwuyxkcx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gtzjdlxhnh.html

C#:   f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gtuzgtizmf.html

[C05] 返回多个值
来源：http://hz.guannengcc.top/gtxghbyzhr.html

Py:   return a, b
来源：http://hz.yongpay.top/gtrhnaggfx.html

PHP:  return [$a, $b];
来源：http://hz.aibaodan.cn/gtowfioasn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.feifeiyinyue.top/gtucojpsrc.html

TS:   return { a, b };
来源：http://hz.sufxvd.cn/gtgkrvcrqn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ehwqpu.com/gtsacmqxen.html

Go:   return a, b
来源：http://hz.ivvv.top/gtisisjqjm.html

Ruby: return a, b
来源：http://hz.quarkkingdee.top/gtnkmtzrge.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.shangyingyoupin.top/gttjoqkesj.html

[C06] 匿名函数 / lambda
来源：http://hz.quarkkingdee.top/gtuthvbxnm.html

Py:   square = lambda x: x * x
来源：http://hz.cheryme.top/gtrmodcccp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hnqzz.top/gtwwjmgkpk.html

JS:   const square = x => x * x;
来源：http://hz.gotoacloud.top/gtzuxwjpyi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.bjfxy.top/gthdnzhnjr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hammf.cn/gttovmghpi.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ydzc1.top/gtynhapsrl.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nanxinkj.top/gtzojvcedh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.svipenyu.cn/gtrughkart.html

[C07] 把函数作为参数传入
来源：http://hz.jiagoushi.top/gtngqkexuu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xingfuxueyuan.xyz/gtkdqkbtev.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhijiandao.cn/gtvqyxmiwn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shanyushiyangkeji.top/gtmzbhhyrv.html

TS:   arr.map(String)
来源：http://hz.vqdsnc.cn/gtldleppkj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.redwolf501.top/gtppylwbpi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sweek.top/gtminwwdpj.html

Ruby: arr.map(&:upcase)
来源：http://hz.haohaochexian.top/gthpclwwhw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ywan-chungtsiang.top/gtvoacobtt.html

[C08] 闭包
来源：http://hz.redwolf501.top/gtjaobaqip.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cqqwz.cn/gtgugeexll.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.0kj1m.cn/gthgkzuhpj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtlggvepec.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtdygxmgwp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.meibo888.top/gtbxexnzol.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhixingplan.top/gtqgtaaswy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hammf.cn/gtwhbhtbvo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sysykeji.top/gtuyculffn.html

[C09] 递归
来源：http://hz.cucudq.cn/gttbidaljk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.dianchejie.cn/gtjzabsllm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hammf.cn/gtxnkubpjq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gthyizaikt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gtxdgtcsqz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinyuanbaomall.cn/gtblmxpmbq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.havefunace.top/gtporcqlxq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xylfe.cn/gtrdsyfeqr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gotoacloud.top/gtdugqpsec.html

[C10] 变量作用域
来源：http://hz.xingfuxueyuan.xyz/gtoaftsoiu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhengqikj.top/gtvgkfprec.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yvedp.cn/gtnbeqwequ.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxinkj.top/gtumecowkm.html

TS:   同 JS
来源：http://hz.iojbl.cn/gtkyrnobai.html

Java: 方法内为块级作用域
来源：http://hz.guannengcc.top/gtpswrnkkn.html

Go:   花括号块级作用域
来源：http://hz.daxiang520.top/gtuzmdwhma.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ivvv.top/gtlbgvbsun.html

C#:   块级作用域
来源：http://hz.zycfv.cn/gthqnyjqdu.html

[C11] 模块导入与导出
来源：http://hz.zhoulong.xyz/gtxayecwyh.html

Py:   from module import func
来源：http://hz.haohaochexian.top/gtfkghwlhd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yuxming.cn/gthacgwfvp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.pengpengdd.cyou/gtultvexvi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jqgfzy.top/gtreqvuwaw.html

Java: import java.util.List;
来源：http://hz.jinyuanbaomall.cn/gtbggvajoj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hywenlv.cn/gtdrnmslor.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgufenzy.top/gtnblbtrmc.html

C#:   using System.Text;
来源：http://hz.bjfxy.top/gtrdispmok.html

[C12] 立即执行函数 IIFE
来源：http://hz.gzhubu.top/gtfqpbunbu.html

Py:   (lambda: print("run"))()
来源：http://hz.wangdashe.top/gtdsxbvoju.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ybcxt.top/gtpngidwiq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuanzx.com/gtevbqckdk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtzruyetsb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhiwuduotai.top/gthegamcvl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aibaodan.cn/gtrdqzvjvx.html

Ruby: -> { puts "run" }.call
来源：http://hz.yueranfly.top/gtocwtoxby.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gaohongyu789.top/gtehbcvmaq.html

[C13] 类型声明 / 类型注解
来源：http://hz.shangyingyoupin.top/gttsgvqupf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guannengcc.top/gthlhallmo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtgaffwwbk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangkeji.top/gtdgeyewcp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtusgizbet.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtmbnqhhbu.html

Go:   func add(a, b int) int
来源：http://hz.yonumen.top/gtxgnvabbc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinqigfzy.top/gtbzsgpweh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guowangkeji.top/gtkpjolgxk.html

[C14] 泛型函数
来源：http://hz.xinyue.icu/gteuygfxdn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.meibo888.top/gtazndxptd.html

PHP:  // 无泛型
来源：http://hz.kuanghao11.cn/gtidfixpbx.html

JS:   // 无泛型
来源：http://hz.nwbrower.top/gtuugkewoh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhengqikj.top/gtbkgcfjmc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sxryk.cn/gtmrizyjgn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.guannengcc.top/gtmdrzmwsm.html

Ruby: # 无泛型
来源：http://hz.sxryk.cn/gtzuhtnwuw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pycfn.com/gtqbozxrpt.html

[C15] 解构 / 展开参数
来源：http://hz.sufxvd.cn/gtshnpfkhl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cashguo.top/gtswgnqzyt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nanxuanxn.top/gthfdpnlfh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jlsjyb.cn/gtqkmmrekz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xuanzx.com/gtlsnxqrph.html

Java: // 无解构
来源：http://hz.dianchejie.cn/gtpqewksat.html

Go:   // 无解构
来源：http://hz.wangdashe.top/gthkguapug.html

Ruby: a, b = pair
来源：http://hz.zhiwuduotai.top/gtbakyzicw.html

C#:   var (a, b) = pair;
来源：http://hz.jinqigfzy.top/gtseropsfv.html

[C16] 函数 / 方法重载
来源：http://hz.hysaishi.cn/gteizjssvb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jianghu66.top/gttorebqzb.html

PHP:  // 无重载
来源：http://hz.sweek.top/gtwpbjfsju.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shangyingyoupin.top/gtorxuovzr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.mhx1999.top/gtspulpeat.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cucudq.cn/gthgbebtzs.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinyuanbaomall.cn/gtxbbqywea.html

Ruby: # 无重载：靠动态参数
来源：http://hz.smart0.xyz/gtqhjxezpo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinqigufen.top/gtduzpjhtm.html

================================================================================
来源：http://hz.ybcxt.top/gtopikbgex.html

D. 数组 / 列表 / 集合
来源：http://hz.xuetiantiany.cn/gtjbzvtzwv.html

================================================================================
来源：http://hz.snrcjt.cn/gtwhxxwwql.html

[D01] 创建数组 / 列表
来源：http://hz.jiagoushi.top/gtuurorjap.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xinyue.icu/gtkyjmepgr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cashguo.top/gtxurxetyl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aizwys.cn/gtkfptjsiu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.52xcode.cn/gtuxvcsewq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenlongwang.top/gtiyxdzcwa.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cheryme.top/gtlqsuound.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cqqwz.cn/gtrouckilf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sweek.top/gtlkynhsoy.html

[D02] 追加元素到末尾
来源：http://hz.zhijiandao.cn/gtciitucak.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jlsjyb.cn/gtxieceflz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xinyue.icu/gtpwurdhkb.html

JS:   arr.push(4);
来源：http://hz.ywan-chungtsiang.top/gtmmblhzny.html

TS:   arr.push(4);
来源：http://hz.xingfuxueyuan.xyz/gthwxzwumg.html

Java: list.add(4);
来源：http://hz.zhixingplan.top/gtxeefooaa.html

Go:   arr = append(arr, 4)
来源：http://hz.xziqi.cn/gtsbohgqhb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ybcxt.top/gtyyoujpez.html

C#:   list.Add(4);
来源：http://hz.hnqzz.top/gtewbhewqn.html

[D03] 在指定位置插入元素
来源：http://hz.zhixingplan.top/gtmjaflxts.html

Py:   arr.insert(0, 0)
来源：http://hz.yj20258.top/gtdyfqlldi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhongyouzk.top/gtecmksvlh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xuanzx.com/gtwovqyeal.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.svipenyu.cn/gtngoqnngd.html

Java: list.add(0, 0);
来源：http://hz.snrcjt.cn/gtfwhzuixi.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yanxiufei.cn/gtgujnzyts.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jianghu66.top/gtpnetelkz.html

C#:   list.Insert(0, 0);
来源：http://hz.chenjidiqi.icu/gtwmxkkphn.html

[D04] 删除元素
来源：http://hz.hysaishi.cn/gtpiwcxgqu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ehwqpu.com/gthpqbdpwo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tanke756.top/gtmnrcilnd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.dashuyun.cn/gtivzbqtct.html

TS:   arr.splice(0, 1);
来源：http://hz.shangyingyoupin.top/gtqsfdhhzz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shzxlz.cn/gtcvhqsblz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.daxiang520.top/gtrvoqgabe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yuxming.cn/gtjsgjtmfz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nanxinkj.top/gtniywrpct.html

[D05] 访问与修改元素
来源：http://hz.zhoulong.xyz/gthfckwoue.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtviahovtv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yonumen.top/gthysmjxvh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.mhx1999.top/gtyjkydfmb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj202588.top/gtacqcuvfl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nanxuanxn.top/gtjxrhbimk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtkmpftwwd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtjgnhdoam.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.dianchejie.cn/gtqzorvqbr.html

[D06] 数组长度
来源：http://hz.ppjwa.cn/gtyxtvrxes.html

Py:   len(arr)
来源：http://hz.sysykeji.top/gtkujwculu.html

PHP:  count($arr);
来源：http://hz.jinqigufen.top/gtvvqumuud.html

JS:   arr.length
来源：http://hz.hywenlv.cn/gtfzupqvjm.html

TS:   arr.length
来源：http://hz.gogol.net.cn/gtnetitush.html

Java: list.size();
来源：http://hz.andypj.xyz/gtjnfnnjpc.html

Go:   len(arr)
来源：http://hz.gzhubu.top/gtgctqwdvb.html

Ruby: arr.length; arr.size
来源：http://hz.yonumen.top/gtgmdjrfin.html

C#:   list.Count;
来源：http://hz.shanyushiyangtech.top/gtiewevpun.html

[D07] 切片 / 取子数组
来源：http://hz.xylfe.cn/gtwcblbaln.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cdnleiting.top/gtssjubsaa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jianghu66.top/gtmvwbvjub.html

JS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gtwenpmiir.html

TS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtundqnvol.html

Java: list.subList(1, 4);
来源：http://hz.xinyue.icu/gtrdotwkho.html

Go:   arr[1:4]
来源：http://hz.hongshengwenyu.top/gtqnwgrksq.html

Ruby: arr[1, 3]
来源：http://hz.yonumen.top/gtyuwabazc.html

C#:   list.GetRange(1, 3);
来源：http://hz.ywan-chungtsiang.top/gtkhemojgm.html

[D08] 合并两个数组
来源：http://hz.svipenyu.cn/gtzdvhnwyh.html

Py:   a + b;  a.extend(b)
来源：http://hz.ppjwa.cn/gtevemafaf.html

PHP:  array_merge($a, $b);
来源：http://hz.yanxiufei.cn/gtuixrqwbr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nanxuanxn.top/gtwsnefrix.html

TS:   [...a, ...b];
来源：http://hz.fengsongda.top/gtedvcvxhj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zycfv.cn/gtnhcvsewn.html

Go:   append(a, b...)
来源：http://hz.hysaishi.cn/gtnwbqzfwd.html


<!-- 参考信息 -->