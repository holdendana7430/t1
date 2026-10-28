代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinghuilouyu.cn/gtdixflcsq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhaomingkeji.xyz/gtmsqcgfwp.html

JS:   do { i++; } while (i < 10);
来源：http://hz.shangyingyoupin.top/gtqreyqujt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinghuilouyu.cn/gtxphaamze.html

Java: do { i++; } while (i < 10);
来源：http://hz.ivvv.top/gtrsobuehb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.birdmap.top/gtcbdccaob.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yj20258888.top/gtaehyjaem.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gtowjptacw.html

[B09] break 与 continue
来源：http://hz.yvedp.cn/gtifvgvkdz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.nwbrower.top/gtspognpdg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.tian-w.cn/gtgzmekhmf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtfwwgbucl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gtyppxjlac.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangdashe.top/gtlkksstjt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yvedp.cn/gtzcuhxaeu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.fengsongda.top/gtacqxtlpp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtdrtoajdd.html

[B10] 遍历同时拿索引
来源：http://hz.cashguo.top/gtwjmmugei.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sysykeji.top/gtppncyccw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.fengsongda.top/gtvvvpayed.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.quarkkingdee.top/gtvmkukyaq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.chenjidiqi.icu/gtgtftpvzx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xziqi.cn/gturyevxjz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xinyue.icu/gtpofrvebh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.meibo888.top/gtoivzbsdq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hnqzz.top/gteolmqcuu.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhoulong.xyz/gttqkmkpvc.html

Py:   list(range(0, 10, 2))
来源：http://hz.sysykeji.top/gtpvkfznyx.html

PHP:  range(0, 10, 2);
来源：http://hz.zhixingplan.top/gtapfvijvx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj20258888.top/gtyhqapdcv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.bjfxy.top/gtbtgaajkv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.dashuyun.cn/gtafqmvimv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hfpthk.cn/gtrsgdjvqk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenzaomai.com/gtyrbfaqqg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.sysykeji.top/gtihhtyomy.html

[B12] 跳出多层循环
来源：http://hz.dashuyun.cn/gtrpuylxeq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yueranfly.top/gteywctmre.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.aizwys.cn/gtppxvtdnq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sysykeji.top/gteatwdlku.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gtigmzjdby.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gterxxuioi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nanxuanxn.top/gtkhnowquu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.feifeiyinyue.top/gtmgntokee.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.havefunace.top/gtuzoxmvfb.html

[B13] 判断是否为数字
来源：http://hz.gotoacloud.top/gtfiupjkze.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhixingplan.top/gtplpvdtlw.html

PHP:  is_numeric($x)
来源：http://hz.vqdsnc.cn/gtlctwngmj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.meibo888.top/gtybvkdzlf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258888.top/gtajzyaslo.html

Java: x instanceof Number
来源：http://hz.nanxinkj.top/gtacbrntff.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.wangshuangyany.cn/gtedasbwjs.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hywenlv.cn/gtfzabacsy.html

C#:   x is int or double or decimal
来源：http://hz.bjfxy.top/gtyxzizwcv.html

[B14] 判断值是否在集合内
来源：http://hz.pycfn.com/gtpywtvitb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.smart0.xyz/gtjscakuuu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.meibo888.top/gtgpqjjngc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhiwuduotai.top/gtwczomkfw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.tianlin.xyz/gtooarpuit.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sxryk.cn/gtkuakcusk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.kuanghao11.cn/gtkwydiffi.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhijiandao.cn/gtvvyockjk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ydjk.org.cn/gtqtbjrbzb.html

[B15] 布尔运算与取反
来源：http://hz.fzhhl.top/gtyboxnslz.html

Py:   a and b or not c
来源：http://hz.shanyushiyangtech.top/gtlpqinuwv.html

PHP:  $a && $b || !$c
来源：http://hz.dianchejie.cn/gttwupftkc.html

JS:   a && b || !c
来源：http://hz.zhijiandao.cn/gtxbswpczv.html

TS:   a && b || !c
来源：http://hz.quarkkingdee.top/gteprtttrk.html

Java: a && b || !c
来源：http://hz.chenlongwang.top/gtirkwudkp.html

Go:   a && b || !c
来源：http://hz.nanxinkj.top/gtfivmawxl.html

Ruby: a && b || !c
来源：http://hz.fengsongda.top/gtyqfouqeg.html

C#:   a && b || !c
来源：http://hz.hfpthk.cn/gthioemejw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tianlin.xyz/gtdpkrdaza.html

Py:   if not data: return
来源：http://hz.gogol.net.cn/gtnbfzwzyw.html

PHP:  if (!$data) { return; }
来源：http://hz.dianchejie.cn/gtblwrvqqf.html

JS:   if (!data) return;
来源：http://hz.0kj1m.cn/gtxcqcmzjf.html

TS:   if (!data) return;
来源：http://hz.tanke756.top/gtpecwdtyp.html

Java: if (data == null) return;
来源：http://hz.sxryk.cn/gtadwwfmbb.html

Go:   if data == nil { return }
来源：http://hz.hysaishi.cn/gttiiqfcmp.html

Ruby: return if data.nil?
来源：http://hz.shangyingyoupin.top/gtycgvtksv.html

C#:   if (data == null) return;
来源：http://hz.sxryk.cn/gtsddolymy.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gttwdoxtcu.html

C. 函数与作用域
来源：http://hz.iojbl.cn/gtuldnlpmh.html

================================================================================
来源：http://hz.ivvv.top/gtutanorwv.html

[C01] 定义函数
来源：http://hz.hnxiangtu.top/gtbikcbpjy.html

Py:   def add(a, b): return a + b
来源：http://hz.yongpay.top/gtoaijsiyf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gtyrysuako.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gotoacloud.top/gtfqkxwlqo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tian-w.cn/gtmkrjjvmo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jianghu66.top/gteuoejdrz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hfpthk.cn/gtpmsszzox.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xuetiantiany.cn/gtmjtwgwsn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yj20258.top/gtlautdjcp.html

[C02] 默认参数
来源：http://hz.yuxming.cn/gteeqvgtvx.html

Py:   def greet(name="World"): return name
来源：http://hz.zdqjudy.top/gtkpjssfuj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hammf.cn/gtxpcuijgm.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxinkj.top/gtefbflvfs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yueranfly.top/gtpihsmpzp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.fengsongda.top/gttvvwmwgw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jinqigufen.top/gtvgshxcxy.html

Ruby: def greet(name = "World") = name
来源：http://hz.xziqi.cn/gtjhzizalm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shuidangran.top/gtrieywjkr.html

[C03] 可变参数
来源：http://hz.wangdashe.top/gtvzckelby.html

Py:   def total(*args): return sum(args)
来源：http://hz.zdqjudy.top/gtazjwesoq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.aibaodan.cn/gtuuamnmtt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gogol.net.cn/gtegnbrebm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.316326.xyz/gtcqejpdyu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinqigufen.top/gtjxjjowek.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.c1oappe.top/gteitraeah.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258.top/gtlndmavwv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.guannengcc.top/gtaxwtuyfq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xingfuxueyuan.xyz/gthdoorbcr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ywan-chungtsiang.top/gtykuvlfjb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hammf.cn/gtapmnczyo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gtjmjgzuyv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gaohongyu789.top/gtoiteyglv.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.daxiang520.top/gtzsphvbms.html

Go:   // 无：用配置结构体参数
来源：http://hz.guannengcc.top/gtlcoxzjiv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtmvfsuxbv.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtrujueger.html

[C05] 返回多个值
来源：http://hz.jinqigfzy.top/gthhrmnqrq.html

Py:   return a, b
来源：http://hz.jyoumei.cn/gtguzjdeww.html

PHP:  return [$a, $b];
来源：http://hz.jqgfzy.top/gtrtzuimvw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.feifeiyinyue.top/gtryhtkxmy.html

TS:   return { a, b };
来源：http://hz.316326.xyz/gtdtncbyib.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.fengsongda.top/gtorwpfriv.html

Go:   return a, b
来源：http://hz.nanxuanxn.top/gtmlyubsfa.html

Ruby: return a, b
来源：http://hz.chenjidiqi.icu/gtpkbhoirt.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gzhubu.top/gtqoxbyjaj.html

[C06] 匿名函数 / lambda
来源：http://hz.zhaomingkeji.xyz/gtkvxgqrio.html

Py:   square = lambda x: x * x
来源：http://hz.zhijiandao.cn/gtvvdtntue.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hongshengwenyu.top/gtrmcynmrc.html

JS:   const square = x => x * x;
来源：http://hz.kuanghao11.cn/gthuaaybvf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sweek.top/gtujjwpykq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shangyingyoupin.top/gtypvlthxu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnqzz.top/gtudfbkwwg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cdnleiting.top/gtsawbyaht.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yvedp.cn/gtqbogysxz.html

[C07] 把函数作为参数传入
来源：http://hz.mhx1999.top/gtykmuqnqr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.aizwys.cn/gtsqqwrorh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.redwolf501.top/gtvvdatdxs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.smart0.xyz/gtcpdtfpzj.html

TS:   arr.map(String)
来源：http://hz.aizwys.cn/gtuhkvtqdh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxuanxn.top/gtobzdggnx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gaohongyu789.top/gtemyznrbi.html

Ruby: arr.map(&:upcase)
来源：http://hz.xylfe.cn/gtrekwlsov.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sysykeji.top/gtvenzkvgl.html

[C08] 闭包
来源：http://hz.jinyuanbaomall.cn/gtmgccpqkj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.svipenyu.cn/gtjmkbqgvm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangtech.top/gtbcwnawnp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gttyqeyyoy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.wangshuangyany.cn/gtawbmizew.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shangyingyoupin.top/gtyiusalro.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cqqwz.cn/gtgmwxqgbv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj20258.top/gthjykyzix.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtmhwdkjdx.html

[C09] 递归
来源：http://hz.hnxiangtu.top/gtrraiovor.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hongshengwenyu.top/gtgwbcymvi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.guowangkeji.top/gtljunwdus.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydzc1.top/gtyqfthbvh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sufxvd.cn/gtmhporvnh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jiagoushi.top/gtrtewemkf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhijiandao.cn/gtkhgjnaaq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tianlin.xyz/gtiyuutxuu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigfzy.top/gtcqzqxojw.html

[C10] 变量作用域
来源：http://hz.snrcjt.cn/gtbrpmrvgn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ywan-chungtsiang.top/gtvebxrgxj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yuanzhike.top/gtkrcxizfz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jiagoushi.top/gtkvoxlekh.html

TS:   同 JS
来源：http://hz.wangshuangyany.cn/gtdphqbree.html

Java: 方法内为块级作用域
来源：http://hz.jinyuanbaomall.cn/gtpawgrfif.html

Go:   花括号块级作用域
来源：http://hz.fzhhl.top/gtnzfdcpgk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.fzhhl.top/gtiktowzna.html

C#:   块级作用域
来源：http://hz.sufxvd.cn/gtoccsqkqk.html

[C11] 模块导入与导出
来源：http://hz.ydjk.org.cn/gtzitgayll.html

Py:   from module import func
来源：http://hz.sysykeji.top/gtuhqtzqku.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinyuanbaomall.cn/gtvwsvnxve.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.aizwys.cn/gtzchikaac.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gogol.net.cn/gtiialndqa.html

Java: import java.util.List;
来源：http://hz.jianghu66.top/gtzvqmniay.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj20258.top/gtprtrdocv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daxiang520.top/gtyruduktd.html

C#:   using System.Text;
来源：http://hz.cucudq.cn/gttfhppema.html

[C12] 立即执行函数 IIFE
来源：http://hz.yangfankeji.com/gtmhafmrth.html

Py:   (lambda: print("run"))()
来源：http://hz.cqqwz.cn/gtsvzhhggt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.52xcode.cn/gtbnpfzohj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258888.top/gtwkgeptkp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gthqmtakdi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.c1oappe.top/gttbyyevlq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shzxlz.cn/gtzwcfqqwg.html

Ruby: -> { puts "run" }.call
来源：http://hz.quarkkingdee.top/gtwpdxyxds.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinghuilouyu.cn/gtnsdliwum.html

[C13] 类型声明 / 类型注解
来源：http://hz.svipenyu.cn/gtiawpfvym.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sysykeji.top/gtahptujgp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jyoumei.cn/gtlcfjpcgu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.quarkkingdee.top/gtbmrzuoin.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtxcmzwfrq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtfadtvqej.html

Go:   func add(a, b int) int
来源：http://hz.snrcjt.cn/gtlmrbqouk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinghuilouyu.cn/gtuskryerr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.dashuyun.cn/gtbhjbliak.html

[C14] 泛型函数
来源：http://hz.cdnleiting.top/gtcouptwij.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hysaishi.cn/gtapfixjvw.html

PHP:  // 无泛型
来源：http://hz.havefunace.top/gthpkqhvvd.html

JS:   // 无泛型
来源：http://hz.yuanzhike.top/gtuxmpnimr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.havefunace.top/gtvquysvcy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigfzy.top/gtssclfncn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.feifeiyinyue.top/gtxxognvpy.html

Ruby: # 无泛型
来源：http://hz.cucudq.cn/gtahrovsuz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cucudq.cn/gtgfpidvrq.html

[C15] 解构 / 展开参数
来源：http://hz.ydjk.org.cn/gtcbltihbc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.svipenyu.cn/gtynbhlnrn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gaohongyu789.top/gtyvivcaqz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.andypj.xyz/gtrxfzelpu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tanke756.top/gtqlvbpkyz.html

Java: // 无解构
来源：http://hz.jlsjyb.cn/gtsgqjymil.html

Go:   // 无解构
来源：http://hz.jinyuanbaomall.cn/gtpfmnmyye.html

Ruby: a, b = pair
来源：http://hz.316326.xyz/gtpotdfyeu.html

C#:   var (a, b) = pair;
来源：http://hz.hywenlv.cn/gtghwrjrhd.html

[C16] 函数 / 方法重载
来源：http://hz.52xcode.cn/gtwkrqomek.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gotoacloud.top/gtyoqucynj.html

PHP:  // 无重载
来源：http://hz.52xcode.cn/gtvdcskyke.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xingfuxueyuan.xyz/gtwmslernf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.snrcjt.cn/gtvdfzhaag.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hammf.cn/gtgrdjywro.html

Go:   // 无重载：用不同函数名
来源：http://hz.redwolf501.top/gtvlxxxqyf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jianghu66.top/gtmmqpbwrf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jyoumei.cn/gtvczoojoo.html

================================================================================
来源：http://hz.jiagoushi.top/gtebeegpvs.html

D. 数组 / 列表 / 集合
来源：http://hz.zhoulong.xyz/gtkkprraaq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtzgyvmgvt.html

[D01] 创建数组 / 列表
来源：http://hz.hfpthk.cn/gtdhqjzjni.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.smart0.xyz/gtzhvaudna.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuanzhike.top/gtudlysngm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj20258.top/gtkytjooil.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hnqzz.top/gtrddqhxbm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yongpay.top/gthvrqqcsz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.nanxinkj.top/gtbnyruydb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.vqdsnc.cn/gtchxqlfdk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yueranfly.top/gtptoagudj.html

[D02] 追加元素到末尾
来源：http://hz.0kj1m.cn/gtwbdejxut.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydzc1.top/gtutftcocn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cashguo.top/gtrlvgjrzu.html

JS:   arr.push(4);
来源：http://hz.wangshuangyany.cn/gtvftfqqts.html

TS:   arr.push(4);
来源：http://hz.nanxuanxn.top/gtmyenpfao.html

Java: list.add(4);
来源：http://hz.haohaochexian.top/gttbauagve.html

Go:   arr = append(arr, 4)
来源：http://hz.smart0.xyz/gtifoacfdj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yongpay.top/gtljhlxjpn.html

C#:   list.Add(4);
来源：http://hz.yuanzhike.top/gtczhblrcs.html

[D03] 在指定位置插入元素
来源：http://hz.xziqi.cn/gtpvrsntcy.html

Py:   arr.insert(0, 0)
来源：http://hz.yangfankeji.com/gtbstwazhs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ppjwa.cn/gtvbaudjqx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jyoumei.cn/gteknhaedl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hysaishi.cn/gtiabrzhkn.html

Java: list.add(0, 0);
来源：http://hz.ybcxt.top/gtgaovotta.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cqqwz.cn/gtkcbtcjpu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.fengsongda.top/gtwctkwbkr.html

C#:   list.Insert(0, 0);
来源：http://hz.xuetiantiany.cn/gtyjdrqcdj.html

[D04] 删除元素
来源：http://hz.feifeiyinyue.top/gtumsbkfoa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fengsongda.top/gtpbietykk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenlongwang.top/gtguwydmbi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hnqzz.top/gtwlqyxufs.html

TS:   arr.splice(0, 1);
来源：http://hz.zhoulong.xyz/gtixmaonnh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sweek.top/gtylflulfy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgfzy.top/gtjkjinefg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gzhubu.top/gtuitdmjyj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnqzz.top/gtsfkpoerg.html

[D05] 访问与修改元素
来源：http://hz.jiagoushi.top/gtnyctrocx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtkcihaonr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhijiandao.cn/gtqnjgqxuf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtagqnicor.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gotoacloud.top/gthrqypmjw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.c1oappe.top/gtonszxpwe.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.andypj.xyz/gtlnmlkrjq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daria6918.cn/gtogvzjfwx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.9152youxi.cn/gtitxiwmoi.html

[D06] 数组长度
来源：http://hz.shanyushiyangtech.top/gtumwlddwj.html

Py:   len(arr)
来源：http://hz.wangshuangyany.cn/gtoufhmbui.html

PHP:  count($arr);
来源：http://hz.smart0.xyz/gtijrofgjh.html

JS:   arr.length
来源：http://hz.jiagoushi.top/gtggbmvltj.html

TS:   arr.length
来源：http://hz.zhiwuduotai.top/gtnksfhsqh.html

Java: list.size();
来源：http://hz.dianchejie.cn/gththfqbeu.html

Go:   len(arr)
来源：http://hz.hnqzz.top/gtilscyydg.html

Ruby: arr.length; arr.size
来源：http://hz.tianlin.xyz/gtowftqoem.html

C#:   list.Count;
来源：http://hz.hongshengwenyu.top/gtbtxfmzmx.html

[D07] 切片 / 取子数组
来源：http://hz.fengsongda.top/gtbekvxpdp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.feifeiyinyue.top/gtxhauigct.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sufxvd.cn/gtecnzofyn.html

JS:   arr.slice(1, 4);
来源：http://hz.jinqigufen.top/gtbvhphhlh.html

TS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gthpqttngf.html

Java: list.subList(1, 4);
来源：http://hz.gzhubu.top/gtxwabzljw.html

Go:   arr[1:4]
来源：http://hz.0kj1m.cn/gtnxwdsjtm.html

Ruby: arr[1, 3]
来源：http://hz.yanxiufei.cn/gtdiavbyhu.html

C#:   list.GetRange(1, 3);
来源：http://hz.yanxiufei.cn/gtmhnqxjtc.html

[D08] 合并两个数组
来源：http://hz.yongpay.top/gttqgydekh.html

Py:   a + b;  a.extend(b)
来源：http://hz.cashguo.top/gtmobpfoqj.html

PHP:  array_merge($a, $b);
来源：http://hz.ydzc1.top/gtllnswlse.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tanke756.top/gtntbtmbrg.html

TS:   [...a, ...b];
来源：http://hz.sufxvd.cn/gtqsmazxka.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gaohongyu789.top/gtgucxulpy.html

Go:   append(a, b...)
来源：http://hz.ywan-chungtsiang.top/gtalvuloqx.html


<!-- 参考信息 -->