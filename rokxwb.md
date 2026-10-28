代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gthmkcncof.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhengqikj.top/gtyeuvowvh.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.c1oappe.top/gtbeqjeygi.html

C#:   do { i++; } while (i < 10);
来源：http://hz.bjfxy.top/gtoyptzflo.html

[B09] break 与 continue
来源：http://hz.zhixingplan.top/gtpaqeehda.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.0kj1m.cn/gtkdbkknxt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhiwuduotai.top/gtvzbzomfi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yangfankeji.com/gtomzofxih.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtkdvffytf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtcwlffdpc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.smart0.xyz/gtyeihieap.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.feifeiyinyue.top/gtzpmcmahd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cqqwz.cn/gtkzermbvd.html

[B10] 遍历同时拿索引
来源：http://hz.ehwqpu.com/gttjnhquvu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.chenlongwang.top/gtvkrkbvuc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.tian-w.cn/gtmijcmgns.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zycfv.cn/gtraxzwuda.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sweek.top/gtncvxrinf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yanxiufei.cn/gtvbvozior.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinyuanbaomall.cn/gtlihdyere.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.svipenyu.cn/gtckfgvksx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sxryk.cn/gtxsfhqmsm.html

[B11] 生成数字序列 / 区间
来源：http://hz.ivvv.top/gtuzqpdzpi.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenlongwang.top/gtlrynepzo.html

PHP:  range(0, 10, 2);
来源：http://hz.jlsjyb.cn/gtqnqajcui.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hywenlv.cn/gthizdyadm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yueranfly.top/gthdflxbgf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.aizwys.cn/gtadkrfxyo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.pycfn.com/gtmuemegif.html

Ruby: (0...10).step(2).to_a
来源：http://hz.9152youxi.cn/gtddbzuxmj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jlsjyb.cn/gtybsixmsi.html

[B12] 跳出多层循环
来源：http://hz.yuanzhike.top/gthwmojgjb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhoulong.xyz/gttfdgqbtp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.chenjidiqi.icu/gtlzgmntqz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gttcdeqdfu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtkrgayfif.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.gaohongyu789.top/gtxkadgmkx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yueranfly.top/gtroqmfttn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yuanzhike.top/gtldkjekvc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jianghu66.top/gttbtntvdk.html

[B13] 判断是否为数字
来源：http://hz.316326.xyz/gtsxvcybni.html

Py:   isinstance(x, (int, float))
来源：http://hz.kuanghao11.cn/gtirdfqfap.html

PHP:  is_numeric($x)
来源：http://hz.smart0.xyz/gtxffgpurx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnqzz.top/gteddlxtjh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jianghu66.top/gtwqriamye.html

Java: x instanceof Number
来源：http://hz.cheryme.top/gtmkpprrab.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.tanke756.top/gtkuofvksd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ivvv.top/gtgkvnpqwy.html

C#:   x is int or double or decimal
来源：http://hz.yuxming.cn/gttmrzbubs.html

[B14] 判断值是否在集合内
来源：http://hz.ppjwa.cn/gtqoospovw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sufxvd.cn/gttlecmqos.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shangyingyoupin.top/gtqizqmkrt.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ydjk.org.cn/gttgcgludb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.fengsongda.top/gtyhcqawaa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.guowangkeji.top/gtgfhtvnmp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xuanzx.com/gtdwvptkmi.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cdnleiting.top/gtggixpcai.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jqgfzy.top/gtwflykwcf.html

[B15] 布尔运算与取反
来源：http://hz.wangdashe.top/gtixpnmyiq.html

Py:   a and b or not c
来源：http://hz.xziqi.cn/gtfzybdigr.html

PHP:  $a && $b || !$c
来源：http://hz.gogol.net.cn/gtccdjhlda.html

JS:   a && b || !c
来源：http://hz.xziqi.cn/gtgdzxznks.html

TS:   a && b || !c
来源：http://hz.jqgufenzy.top/gtsiegowiz.html

Java: a && b || !c
来源：http://hz.mhx1999.top/gtfskpzdrc.html

Go:   a && b || !c
来源：http://hz.jianghu66.top/gtkmjirizu.html

Ruby: a && b || !c
来源：http://hz.daria6918.cn/gtqdlnfgpi.html

C#:   a && b || !c
来源：http://hz.yongpay.top/gtntdelwdw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hnqzz.top/gtpuovbagq.html

Py:   if not data: return
来源：http://hz.jqgfzy.top/gtqudqxphe.html

PHP:  if (!$data) { return; }
来源：http://hz.316326.xyz/gtwyroufkv.html

JS:   if (!data) return;
来源：http://hz.shuidangran.top/gtrhdvldiu.html

TS:   if (!data) return;
来源：http://hz.sweek.top/gtbaeswxpx.html

Java: if (data == null) return;
来源：http://hz.aizwys.cn/gtjavgjeza.html

Go:   if data == nil { return }
来源：http://hz.dianchejie.cn/gtzhylhodq.html

Ruby: return if data.nil?
来源：http://hz.yonumen.top/gtjqporqoz.html

C#:   if (data == null) return;
来源：http://hz.daxiang520.top/gtmallplpi.html

================================================================================
来源：http://hz.hfpthk.cn/gtfeapbqay.html

C. 函数与作用域
来源：http://hz.hfpthk.cn/gtmxsqpuge.html

================================================================================
来源：http://hz.tanke756.top/gtzicudjhr.html

[C01] 定义函数
来源：http://hz.cucudq.cn/gtbgonfjfw.html

Py:   def add(a, b): return a + b
来源：http://hz.hnxiangtu.top/gtgdikaliy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtjkamnclh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtzuiwnbqg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gzhubu.top/gtktwpjcvd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yuanzhike.top/gtxboslopf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guowangkeji.top/gtpnrjzhcb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shzxlz.cn/gtkhuyzywb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtutwebglf.html

[C02] 默认参数
来源：http://hz.shanyushiyangtech.top/gtadfggger.html

Py:   def greet(name="World"): return name
来源：http://hz.shanyushiyangkeji.top/gtaqiqbhab.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.haohaochexian.top/gthypovclx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jianghu66.top/gtjfdhpdmf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.feifeiyinyue.top/gthpgkjlta.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hfpthk.cn/gttkryyvem.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cqqwz.cn/gtwsmmorao.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhongyouzk.top/gtofhewgvy.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenzaomai.com/gtctgjspgr.html

[C03] 可变参数
来源：http://hz.meibo888.top/gtczzrvaph.html

Py:   def total(*args): return sum(args)
来源：http://hz.iojbl.cn/gtisobxfwo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hywenlv.cn/gtzcydbpbe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hongshengwenyu.top/gtrqslemye.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dashuyun.cn/gtfhhmvplx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.snrcjt.cn/gtsjxxygmr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xziqi.cn/gtxueyytho.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yuanzhike.top/gtjecthzyy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.redwolf501.top/gtgzidijwn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ppjwa.cn/gtuszyjfzl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ppjwa.cn/gtlkzfmjgf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ehwqpu.com/gtebbpdadc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenjidiqi.icu/gtadijwmxk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.wangshuangyany.cn/gtkahgnlpr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.havefunace.top/gtyufydnsu.html

Go:   // 无：用配置结构体参数
来源：http://hz.hongshengwenyu.top/gtdmycaapm.html

Ruby: f(a: 1, b: 2)
来源：http://hz.snrcjt.cn/gttedojpyg.html

C#:   f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtfmycdrdx.html

[C05] 返回多个值
来源：http://hz.shanyushiyangtech.top/gtrrzymiau.html

Py:   return a, b
来源：http://hz.feifeiyinyue.top/gtqjounjhz.html

PHP:  return [$a, $b];
来源：http://hz.ehwqpu.com/gtycwypbih.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.havefunace.top/gtjbcdarch.html

TS:   return { a, b };
来源：http://hz.52xcode.cn/gtoyimjnoe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nwbrower.top/gtmwcpepet.html

Go:   return a, b
来源：http://hz.ydzc1.top/gttfkobmej.html

Ruby: return a, b
来源：http://hz.hywenlv.cn/gteisvvtyq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydjk.org.cn/gtnsuzpqbp.html

[C06] 匿名函数 / lambda
来源：http://hz.zhongyouzk.top/gtzhhqgspg.html

Py:   square = lambda x: x * x
来源：http://hz.xingfuxueyuan.xyz/gtpemrfnxz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yongpay.top/gtkpohiuei.html

JS:   const square = x => x * x;
来源：http://hz.jyoumei.cn/gtutxtwizl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ybcxt.top/gtwddvikvx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jlsjyb.cn/gtlzezeqkv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.sysykeji.top/gtgapdtxze.html

Ruby: square = ->(x) { x * x }
来源：http://hz.meibo888.top/gtctmdktpx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sweek.top/gtiqqlcbrz.html

[C07] 把函数作为参数传入
来源：http://hz.ppjwa.cn/gtlfgvravn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nwbrower.top/gtdkyzedtx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.iojbl.cn/gttdtalogu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yuanzhike.top/gtbybjhvmv.html

TS:   arr.map(String)
来源：http://hz.nwbrower.top/gtermzlhfm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.guannengcc.top/gtqgvctxcj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.pycfn.com/gtmcmfoehy.html

Ruby: arr.map(&:upcase)
来源：http://hz.daria6918.cn/gthrxzqwxd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xziqi.cn/gtmieygusz.html

[C08] 闭包
来源：http://hz.xylfe.cn/gtcyrelxfe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hysaishi.cn/gtzfducivv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258888.top/gtxbjaiytf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtocodkyxn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtsnawljiv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.daxiang520.top/gtjakdlwcg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.52xcode.cn/gtzhjwahzf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhengqikj.top/gtqiwgrlnr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtbnvyojfg.html

[C09] 递归
来源：http://hz.yueranfly.top/gtystytqwz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.dashuyun.cn/gtobkafrfl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jinqigufen.top/gtffotsmdi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gtkfzmxhed.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sweek.top/gtvmjhcwbt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tian-w.cn/gtbsdjktvc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tanke756.top/gtxnavlnfb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.nwbrower.top/gtkqwzzzbm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnxiangtu.top/gtjnfnucjv.html

[C10] 变量作用域
来源：http://hz.0kj1m.cn/gtporllbcl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinghuilouyu.cn/gtybexepqw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gaohongyu789.top/gttiaehdyv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinyuanbaomall.cn/gtvrtvtiwz.html

TS:   同 JS
来源：http://hz.yj20258.top/gtadvcqhqh.html

Java: 方法内为块级作用域
来源：http://hz.quarkkingdee.top/gtkgwjpcmk.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangtech.top/gtbtpjbxbm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zdqjudy.top/gtulicvoac.html

C#:   块级作用域
来源：http://hz.meibo888.top/gtgdjjnqml.html

[C11] 模块导入与导出
来源：http://hz.sufxvd.cn/gtqqdnmwfx.html

Py:   from module import func
来源：http://hz.wangdashe.top/gtpisuqjpa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhongyouzk.top/gtwaavyvkw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ehwqpu.com/gtwaiimrpm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhiwuduotai.top/gtqigyowik.html

Java: import java.util.List;
来源：http://hz.cheryme.top/gtepjzptgm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigfzy.top/gtslnlwdbe.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.haohaochexian.top/gtxcabcgst.html

C#:   using System.Text;
来源：http://hz.xziqi.cn/gtammlpkij.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258.top/gtzasulvol.html

Py:   (lambda: print("run"))()
来源：http://hz.shzxlz.cn/gtykyhkoiu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pycfn.com/gtppqcxcwl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.feifeiyinyue.top/gtcatfczas.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangkeji.top/gtbjzthbvm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xuanzx.com/gtzyyykwip.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guowangkeji.top/gtyigpcpbu.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinqigufen.top/gtmkdrmfxb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhengqikj.top/gtptyodwkx.html

[C13] 类型声明 / 类型注解
来源：http://hz.chenzaomai.com/gtqqgotjsq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ydjk.org.cn/gtnyqmsmny.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenjidiqi.icu/gtfznxhwiz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhiwuduotai.top/gtiuhhpdwj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuxming.cn/gtooclwukb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtyhtgixlm.html

Go:   func add(a, b int) int
来源：http://hz.kuanghao11.cn/gtubhgzzib.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hammf.cn/gtcuygoafi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cqqwz.cn/gtgcakazob.html

[C14] 泛型函数
来源：http://hz.zdqjudy.top/gtaaxxsrmt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xinyue.icu/gtvbtooqzp.html

PHP:  // 无泛型
来源：http://hz.fengsongda.top/gtkflnbiho.html

JS:   // 无泛型
来源：http://hz.jlsjyb.cn/gtflbtcbrr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.aibaodan.cn/gttyacxsrb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tian-w.cn/gtjjtbucvo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nwbrower.top/gtuqlmdpwp.html

Ruby: # 无泛型
来源：http://hz.aizwys.cn/gtbvblddet.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.daria6918.cn/gtpwjyzmtn.html

[C15] 解构 / 展开参数
来源：http://hz.redwolf501.top/gtthtzexvi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cdnleiting.top/gtgsjjsjyy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hywenlv.cn/gtabnmnodk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gtranatjal.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cheryme.top/gtugzuxbcb.html

Java: // 无解构
来源：http://hz.sysykeji.top/gtzbfympka.html

Go:   // 无解构
来源：http://hz.ydjk.org.cn/gtorffukwf.html

Ruby: a, b = pair
来源：http://hz.yonumen.top/gtoqurfoea.html

C#:   var (a, b) = pair;
来源：http://hz.kuanghao11.cn/gtdykdltqp.html

[C16] 函数 / 方法重载
来源：http://hz.yvedp.cn/gtemnziutb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yanxiufei.cn/gtnzqmvfft.html

PHP:  // 无重载
来源：http://hz.0kj1m.cn/gtnlzztabv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jlsjyb.cn/gtlaxjiulc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.smart0.xyz/gtkfajlbvh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yanxiufei.cn/gtkepfffnh.html

Go:   // 无重载：用不同函数名
来源：http://hz.hammf.cn/gtkjsksycu.html

Ruby: # 无重载：靠动态参数
来源：http://hz.kuanghao11.cn/gtqbrsqnuq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yj20258.top/gthgqdjobo.html

================================================================================
来源：http://hz.nanxuanxn.top/gtjzfvxcun.html

D. 数组 / 列表 / 集合
来源：http://hz.zhoulong.xyz/gtzkyunnsy.html

================================================================================
来源：http://hz.zycfv.cn/gtgpnhvcap.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gtdwhtsjcn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenzaomai.com/gtcszmlkhh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jlsjyb.cn/gtcjoliyfd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.c1oappe.top/gtmbrecddq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cheryme.top/gtexeuwyju.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj20258.top/gtyikokbhd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yuxming.cn/gtukhmhdrd.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nwbrower.top/gthtwdqbzl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.dianchejie.cn/gtivgltwdz.html

[D02] 追加元素到末尾
来源：http://hz.jinyuanbaomall.cn/gteqceqeqw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.feifeiyinyue.top/gtckndtbzh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yonumen.top/gtxgzrdrlc.html

JS:   arr.push(4);
来源：http://hz.c1oappe.top/gtczohxplx.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangtech.top/gtutxejbvt.html

Java: list.add(4);
来源：http://hz.feifeiyinyue.top/gtswsdahwe.html

Go:   arr = append(arr, 4)
来源：http://hz.cdnleiting.top/gtjlvkkult.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhiwuduotai.top/gtklhztify.html

C#:   list.Add(4);
来源：http://hz.jqgufenzy.top/gtjmkhbsnq.html

[D03] 在指定位置插入元素
来源：http://hz.yvedp.cn/gtzivphaii.html

Py:   arr.insert(0, 0)
来源：http://hz.iojbl.cn/gtdmsyjecy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.316326.xyz/gtpgtoegkh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yvedp.cn/gttajzifpw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gogol.net.cn/gtrjgvrybu.html

Java: list.add(0, 0);
来源：http://hz.tianlin.xyz/gtdrkniclf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jqgfzy.top/gtjbyaxjxf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydzc1.top/gtpmpcbada.html

C#:   list.Insert(0, 0);
来源：http://hz.hnxiangtu.top/gtdzvajvdu.html

[D04] 删除元素
来源：http://hz.xinyue.icu/gtidtfnlyh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sysykeji.top/gtdrjwfvqe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cqqwz.cn/gtayatfvlb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.smart0.xyz/gtkwshatvk.html

TS:   arr.splice(0, 1);
来源：http://hz.fzhhl.top/gtwjydwkwt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gogol.net.cn/gtguzzgnkl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.mhx1999.top/gtgmazmizh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hfpthk.cn/gtmcwowyku.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sysykeji.top/gtlgxzpjwp.html

[D05] 访问与修改元素
来源：http://hz.zhoulong.xyz/gtnjxqkrar.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.havefunace.top/gtfgdezlcu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtmtqfqccn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigufen.top/gtsasrymbm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhijiandao.cn/gtaajgjqvt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gzhubu.top/gtouddfrha.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtioickhsl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pycfn.com/gtuhtjjqua.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.guowangkeji.top/gtosusfmnj.html

[D06] 数组长度
来源：http://hz.ehwqpu.com/gtvsifeway.html

Py:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtrgogfigm.html

PHP:  count($arr);
来源：http://hz.hysaishi.cn/gtagasdkib.html

JS:   arr.length
来源：http://hz.shuidangran.top/gtghbcsdkx.html

TS:   arr.length
来源：http://hz.tian-w.cn/gtdxxkaifz.html

Java: list.size();
来源：http://hz.dashuyun.cn/gtmnomarrm.html

Go:   len(arr)
来源：http://hz.aizwys.cn/gtntqrpvnt.html

Ruby: arr.length; arr.size
来源：http://hz.smart0.xyz/gtbgvqkbrg.html

C#:   list.Count;
来源：http://hz.wangdashe.top/gtwhrnpoqo.html

[D07] 切片 / 取子数组
来源：http://hz.quarkkingdee.top/gtdmzijmlv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigfzy.top/gtsjobrxou.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xylfe.cn/gtruicloph.html

JS:   arr.slice(1, 4);
来源：http://hz.zycfv.cn/gtrignqhtr.html

TS:   arr.slice(1, 4);
来源：http://hz.cheryme.top/gtvuaofobs.html

Java: list.subList(1, 4);
来源：http://hz.ybcxt.top/gtrxzmyzqe.html

Go:   arr[1:4]
来源：http://hz.ybcxt.top/gtlervigcc.html

Ruby: arr[1, 3]
来源：http://hz.316326.xyz/gtpuigcgdo.html

C#:   list.GetRange(1, 3);
来源：http://hz.pengpengdd.cyou/gtumykcoue.html

[D08] 合并两个数组
来源：http://hz.yongpay.top/gtnbjuxdgp.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxuanxn.top/gtnqzndndi.html

PHP:  array_merge($a, $b);
来源：http://hz.bjfxy.top/gtrkwlcwhx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yvedp.cn/gtcvccucnd.html

TS:   [...a, ...b];
来源：http://hz.ydjk.org.cn/gtjigklnvj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pengpengdd.cyou/gtopnzpxzv.html

Go:   append(a, b...)
来源：http://hz.jinqigufen.top/gtcjrwyqms.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nwbrower.top/gtdjihqdtk.html

C#:   a.Concat(b).ToList()
来源：http://hz.jianghu66.top/gtuavntogk.html

[D09] 排序（升序）
来源：http://hz.xingfuxueyuan.xyz/gthihcaauu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydzc1.top/gtiqeiybll.html


<!-- 参考信息 -->