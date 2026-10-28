代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtuyzbmypy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ivvv.top/gtbnutsvtc.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ywan-chungtsiang.top/gtteawwgal.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gttvkhdfjb.html

[B09] break 与 continue
来源：http://hz.sysykeji.top/gtdsprfinx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ivvv.top/gteajudvlr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtupnsetdg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.birdmap.top/gtgswimfhq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxuanxn.top/gthzlbsjfo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtqkauqhzn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ivvv.top/gttjsbufzv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jqgufenzy.top/gtuwnslohs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nwbrower.top/gtcwrhdcfm.html

[B10] 遍历同时拿索引
来源：http://hz.chenzaomai.com/gtmxhtxvho.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.dashuyun.cn/gtmdpphkwa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yuanzhike.top/gtlsndfapk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jianghu66.top/gtaerdnwxt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xingfuxueyuan.xyz/gthptplhzf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yvedp.cn/gttyyripzh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.dianchejie.cn/gtrjrqwmbi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ppjwa.cn/gtwoldtmtq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gogol.net.cn/gthituwfsp.html

[B11] 生成数字序列 / 区间
来源：http://hz.yuanzhike.top/gtictxnsxb.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhixingplan.top/gtylexqqew.html

PHP:  range(0, 10, 2);
来源：http://hz.zhengqikj.top/gtmckbduwf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shzxlz.cn/gthxnhtjzk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fzhhl.top/gtzbbgmzsz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xuanzx.com/gttbgtkhje.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ppjwa.cn/gtcxalvesk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shanyushiyangtech.top/gtshubsuyk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.dianchejie.cn/gtyxbrxbus.html

[B12] 跳出多层循环
来源：http://hz.hongshengwenyu.top/gticyfcrtp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nanxuanxn.top/gtlszhyyfw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sxryk.cn/gtsuqzogat.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daxiang520.top/gtgiuvnhza.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgufenzy.top/gtktqwgzfj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gtrtuegkoy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.feifeiyinyue.top/gtjpzjkgfs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.quarkkingdee.top/gtbnwcqsip.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yuanzhike.top/gtfmiqxsqt.html

[B13] 判断是否为数字
来源：http://hz.fengsongda.top/gtkltvtpgr.html

Py:   isinstance(x, (int, float))
来源：http://hz.shanyushiyangtech.top/gtfrgtunuk.html

PHP:  is_numeric($x)
来源：http://hz.zhongyouzk.top/gtynxxhpyp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.andypj.xyz/gtwmwibrdn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.meibo888.top/gttwubcdei.html

Java: x instanceof Number
来源：http://hz.ivvv.top/gtnwfqmnba.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.gogol.net.cn/gtyoksyjcw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.pycfn.com/gtnmtfaqlu.html

C#:   x is int or double or decimal
来源：http://hz.ywan-chungtsiang.top/gtazofmrat.html

[B14] 判断值是否在集合内
来源：http://hz.jinyuanbaomall.cn/gttdenaudu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jqgfzy.top/gtrxvocnyv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.feifeiyinyue.top/gtwslfuqlx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yongpay.top/gtbrokgjoo.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.birdmap.top/gtdmiiftbv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.feifeiyinyue.top/gtxqlusoxo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guowangkeji.top/gtvyezctjf.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.andypj.xyz/gtskallgni.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.quarkkingdee.top/gtnjcoqltf.html

[B15] 布尔运算与取反
来源：http://hz.gaohongyu789.top/gtkhnpoaid.html

Py:   a and b or not c
来源：http://hz.iojbl.cn/gtuhtvhqjm.html

PHP:  $a && $b || !$c
来源：http://hz.yonumen.top/gtonbaylei.html

JS:   a && b || !c
来源：http://hz.chenzaomai.com/gtjgiaxmov.html

TS:   a && b || !c
来源：http://hz.yongpay.top/gtxmrpxwyj.html

Java: a && b || !c
来源：http://hz.ppjwa.cn/gtpvxpvnmm.html

Go:   a && b || !c
来源：http://hz.jyoumei.cn/gtzfewbxbg.html

Ruby: a && b || !c
来源：http://hz.ydzc1.top/gtqftqnxbi.html

C#:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtwmlrkvyn.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shanyushiyangkeji.top/gtjuyghxxd.html

Py:   if not data: return
来源：http://hz.xuanzx.com/gtnmatyiol.html

PHP:  if (!$data) { return; }
来源：http://hz.iojbl.cn/gtcnllfyyh.html

JS:   if (!data) return;
来源：http://hz.mhx1999.top/gtdmkuqxns.html

TS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtfskjgrdx.html

Java: if (data == null) return;
来源：http://hz.yanxiufei.cn/gtvyhsynkz.html

Go:   if data == nil { return }
来源：http://hz.vqdsnc.cn/gtonvumopi.html

Ruby: return if data.nil?
来源：http://hz.feifeiyinyue.top/gtnxdqdcnz.html

C#:   if (data == null) return;
来源：http://hz.jinghuilouyu.cn/gthswnqspd.html

================================================================================
来源：http://hz.ydzc1.top/gtljpebnxb.html

C. 函数与作用域
来源：http://hz.zhijiandao.cn/gtqbszhzig.html

================================================================================
来源：http://hz.zdqjudy.top/gtnsfumkie.html

[C01] 定义函数
来源：http://hz.haohaochexian.top/gtoumqshfa.html

Py:   def add(a, b): return a + b
来源：http://hz.pengpengdd.cyou/gttrtteohn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydzc1.top/gtztsbfoac.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hammf.cn/gtkasuvjfp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.smart0.xyz/gtkofetsix.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhixingplan.top/gtqnglvgfx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.vqdsnc.cn/gtqtzwjulu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.quarkkingdee.top/gtnibubrmf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.mhx1999.top/gtnhsrkyyp.html

[C02] 默认参数
来源：http://hz.redwolf501.top/gtadadfdvy.html

Py:   def greet(name="World"): return name
来源：http://hz.zhiwuduotai.top/gtfsuiksor.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hywenlv.cn/gtjvdwlfvx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jianghu66.top/gtlafstzsx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ivvv.top/gtldlweghw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tanke756.top/gtvwjjceta.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nwbrower.top/gtjkptgqcb.html

Ruby: def greet(name = "World") = name
来源：http://hz.0kj1m.cn/gtbfroibvv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shangyingyoupin.top/gtkqbpwdyj.html

[C03] 可变参数
来源：http://hz.jianghu66.top/gtevdeovsv.html

Py:   def total(*args): return sum(args)
来源：http://hz.hongshengwenyu.top/gtvcpdmise.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jinqigufen.top/gtelqopblm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenzaomai.com/gtlwdthdtq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xingfuxueyuan.xyz/gtolbjsdzl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.chenzaomai.com/gtvjgjuhxg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cdnleiting.top/gtavdyqlvz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yuanzhike.top/gtolrhptsj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnxiangtu.top/gtxxbmlnki.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuxming.cn/gtjkiqnwxn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhiwuduotai.top/gtbmkahdot.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.smart0.xyz/gtmwmmobow.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sysykeji.top/gtjmaxgjzy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shuidangran.top/gtyocxnuuv.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhongyouzk.top/gtoafwmtan.html

Go:   // 无：用配置结构体参数
来源：http://hz.yangfankeji.com/gtomsuifio.html

Ruby: f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gtptckimye.html

C#:   f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtrsqhwdhi.html

[C05] 返回多个值
来源：http://hz.bjfxy.top/gtwtnhulbb.html

Py:   return a, b
来源：http://hz.haohaochexian.top/gtubokbeow.html

PHP:  return [$a, $b];
来源：http://hz.nanxinkj.top/gtxzckcndt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xylfe.cn/gthftbytji.html

TS:   return { a, b };
来源：http://hz.shzxlz.cn/gtfeujozia.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gotoacloud.top/gtepnqtndj.html

Go:   return a, b
来源：http://hz.zhengqikj.top/gtmjpigmhz.html

Ruby: return a, b
来源：http://hz.guowangkeji.top/gtalsfocjg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.nwbrower.top/gtqzkfmsba.html

[C06] 匿名函数 / lambda
来源：http://hz.smart0.xyz/gtqpfhnbll.html

Py:   square = lambda x: x * x
来源：http://hz.yueranfly.top/gtqsrcsfnc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hfpthk.cn/gtouxwusrf.html

JS:   const square = x => x * x;
来源：http://hz.0kj1m.cn/gtlmelhnxx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sxryk.cn/gthlzikyya.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jlsjyb.cn/gtuzlppmbb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xingfuxueyuan.xyz/gtmahdpezt.html

Ruby: square = ->(x) { x * x }
来源：http://hz.feifeiyinyue.top/gtkdiowayw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gaohongyu789.top/gtkkxtfpjy.html

[C07] 把函数作为参数传入
来源：http://hz.jqgfzy.top/gtumdtfwad.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yanxiufei.cn/gtlhpdzfhm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nwbrower.top/gtjttcttfl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.gzhubu.top/gtmxgfkwhv.html

TS:   arr.map(String)
来源：http://hz.meibo888.top/gtwbamyeck.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.daria6918.cn/gthagdnnrt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.fzhhl.top/gteijjqtfp.html

Ruby: arr.map(&:upcase)
来源：http://hz.tanke756.top/gtocmbkywo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xuanzx.com/gtsgfpmdhp.html

[C08] 闭包
来源：http://hz.xingfuxueyuan.xyz/gteacavnmf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.tian-w.cn/gtejfoxvsr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.nanxinkj.top/gtiyrolqoi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shangyingyoupin.top/gtoduysphc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gtbxgtuzzg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cheryme.top/gtenwnitka.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ppjwa.cn/gtuqkgyjea.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj202588.top/gtbuteypsr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtfgkoyktn.html

[C09] 递归
来源：http://hz.tianlin.xyz/gtddvacghg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.tian-w.cn/gthojlffds.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ydjk.org.cn/gtvbseoknd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.birdmap.top/gthiyhrpzl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnqzz.top/gtuaxuqjxv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.52xcode.cn/gtulxxvhtp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.haohaochexian.top/gtnadvjgrh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhijiandao.cn/gtfdhsillg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.c1oappe.top/gthkmxufht.html

[C10] 变量作用域
来源：http://hz.hywenlv.cn/gtoawuffzm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hysaishi.cn/gtioilvvzz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cashguo.top/gtqszraugy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yueranfly.top/gtlttzrqca.html

TS:   同 JS
来源：http://hz.gzhubu.top/gtmmdppgdb.html

Java: 方法内为块级作用域
来源：http://hz.cdnleiting.top/gtaxyuckdx.html

Go:   花括号块级作用域
来源：http://hz.sxryk.cn/gtixzqdmdv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.shangyingyoupin.top/gtatbuqaxz.html

C#:   块级作用域
来源：http://hz.cdnleiting.top/gtkgbwvhtu.html

[C11] 模块导入与导出
来源：http://hz.c1oappe.top/gthwtmsere.html

Py:   from module import func
来源：http://hz.ivvv.top/gtxgpcjizb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yvedp.cn/gtdwwgvlxo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xylfe.cn/gtbwscyfvp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guannengcc.top/gtfqvbntod.html

Java: import java.util.List;
来源：http://hz.wangshuangyany.cn/gtjjozntsv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.chenlongwang.top/gtpcgsusmn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigfzy.top/gtxfzmjphs.html

C#:   using System.Text;
来源：http://hz.hnqzz.top/gtpvgyrytn.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhiwuduotai.top/gtiygoqfzv.html

Py:   (lambda: print("run"))()
来源：http://hz.sweek.top/gtdmswhhcq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.smart0.xyz/gtucabwdmm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yueranfly.top/gtpqzkwwnh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ydzc1.top/gtohwlnbbz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hysaishi.cn/gtzfvutcut.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.feifeiyinyue.top/gtagegkugs.html

Ruby: -> { puts "run" }.call
来源：http://hz.cqqwz.cn/gtyrskdxnn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinyuanbaomall.cn/gtldzfuskk.html

[C13] 类型声明 / 类型注解
来源：http://hz.shuidangran.top/gtsajeidgt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangdashe.top/gtbphoxvxp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtotugvfzd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ywan-chungtsiang.top/gtmvmwkijb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gtakjtimmr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtncxgxntq.html

Go:   func add(a, b int) int
来源：http://hz.yvedp.cn/gtpvjesmgo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shanyushiyangkeji.top/gtzwdcmtcx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinqigfzy.top/gtjspuqtfp.html

[C14] 泛型函数
来源：http://hz.fzhhl.top/gtjnchquuh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhoulong.xyz/gtndjzahaj.html

PHP:  // 无泛型
来源：http://hz.chenlongwang.top/gthtljltiy.html

JS:   // 无泛型
来源：http://hz.redwolf501.top/gtgtkuspja.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zycfv.cn/gtorapowrn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gzhubu.top/gtfebdrtrx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.haohaochexian.top/gtiunwcfbv.html

Ruby: # 无泛型
来源：http://hz.ydzc1.top/gtffpwfxuo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ybcxt.top/gtvuwdvhue.html

[C15] 解构 / 展开参数
来源：http://hz.ppjwa.cn/gtmlukksdx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fzhhl.top/gtbgdguzac.html

PHP:  [$a, $b] = $pair;
来源：http://hz.snrcjt.cn/gtbfenjuyu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.316326.xyz/gtvvzllxgi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cashguo.top/gtlazralas.html

Java: // 无解构
来源：http://hz.pycfn.com/gtcinbcdbc.html

Go:   // 无解构
来源：http://hz.ywan-chungtsiang.top/gtvigyxwab.html

Ruby: a, b = pair
来源：http://hz.zhaomingkeji.xyz/gtapvlbmwo.html

C#:   var (a, b) = pair;
来源：http://hz.fzhhl.top/gtijczcbuq.html

[C16] 函数 / 方法重载
来源：http://hz.iojbl.cn/gtlnidderx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jyoumei.cn/gtwxgzlhbo.html

PHP:  // 无重载
来源：http://hz.shanyushiyangkeji.top/gtalrtfbpj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.0kj1m.cn/gtvhqsqthi.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cdnleiting.top/gtsjeaervd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sysykeji.top/gtjnrqqflp.html

Go:   // 无重载：用不同函数名
来源：http://hz.shangyingyoupin.top/gtvoqwabkc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gotoacloud.top/gthuxnfjea.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.andypj.xyz/gtfumtenqq.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtzwyfphgl.html

D. 数组 / 列表 / 集合
来源：http://hz.shuidangran.top/gthzjchghv.html

================================================================================
来源：http://hz.yonumen.top/gtcpssdpbd.html

[D01] 创建数组 / 列表
来源：http://hz.aizwys.cn/gtqguwqggw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.feifeiyinyue.top/gtgsymfrow.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhoulong.xyz/gtsqfoeydt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aizwys.cn/gtywvjuqik.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.dianchejie.cn/gtqzsbuvcf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuetiantiany.cn/gtaqevvkey.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.316326.xyz/gtlrvtcewn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daxiang520.top/gtivwgwaws.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shangyingyoupin.top/gttmhlflwq.html

[D02] 追加元素到末尾
来源：http://hz.yj20258888.top/gtwebakamn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cashguo.top/gtyeiahzre.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pycfn.com/gttwftkvei.html

JS:   arr.push(4);
来源：http://hz.jinqigufen.top/gtnkncuxjl.html

TS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtyruzyqam.html

Java: list.add(4);
来源：http://hz.yj20258.top/gtutdyfyqs.html

Go:   arr = append(arr, 4)
来源：http://hz.hysaishi.cn/gtxxawgpph.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tanke756.top/gtdkjhlqds.html

C#:   list.Add(4);
来源：http://hz.yonumen.top/gtlneviquq.html

[D03] 在指定位置插入元素
来源：http://hz.tanke756.top/gtvvmdsjxg.html

Py:   arr.insert(0, 0)
来源：http://hz.yonumen.top/gthlibybbg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ydzc1.top/gtdwtxzjjx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jyoumei.cn/gtnptdcpws.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258.top/gtsqxwbhmf.html

Java: list.add(0, 0);
来源：http://hz.jqgufenzy.top/gtbzcmojfe.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.316326.xyz/gtrywmpbnr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yanxiufei.cn/gtcjsfxklm.html

C#:   list.Insert(0, 0);
来源：http://hz.zhixingplan.top/gtpkvqufti.html

[D04] 删除元素
来源：http://hz.yj20258888.top/gtwrgfkcxz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhoulong.xyz/gtcuxqhnvc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.quarkkingdee.top/gtpxrtxchb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xuanzx.com/gttvtbvsmn.html

TS:   arr.splice(0, 1);
来源：http://hz.kuanghao11.cn/gttbeidbpn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhiwuduotai.top/gtkqbklkzp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sweek.top/gtbwvlurwb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinyuanbaomall.cn/gtvjugobxr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gogol.net.cn/gtuzlatlkz.html

[D05] 访问与修改元素
来源：http://hz.xylfe.cn/gtiapeqtaw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtygjltwiy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtfwglvjce.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hywenlv.cn/gtlrswopla.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.fengsongda.top/gtmrlemtiz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenjidiqi.icu/gtjcctkjia.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cheryme.top/gtiaszvrjb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtwmufuiwc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuetiantiany.cn/gtkohefbgo.html

[D06] 数组长度
来源：http://hz.birdmap.top/gtjwjcgfih.html

Py:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtjzgtqbtd.html

PHP:  count($arr);
来源：http://hz.daria6918.cn/gtjirvocem.html

JS:   arr.length
来源：http://hz.vqdsnc.cn/gtogpxaonq.html

TS:   arr.length
来源：http://hz.wangshuangyany.cn/gtqanntqbs.html

Java: list.size();
来源：http://hz.ybcxt.top/gtttywquja.html

Go:   len(arr)
来源：http://hz.zhongyouzk.top/gtfpxfbukd.html

Ruby: arr.length; arr.size
来源：http://hz.bjfxy.top/gtbfcwzjuk.html

C#:   list.Count;
来源：http://hz.tianlin.xyz/gtvmzqhhbk.html

[D07] 切片 / 取子数组
来源：http://hz.jianghu66.top/gtwiwygzvm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ppjwa.cn/gtrkppcjlg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ivvv.top/gtwuwidaen.html

JS:   arr.slice(1, 4);
来源：http://hz.hysaishi.cn/gtijaxptei.html

TS:   arr.slice(1, 4);
来源：http://hz.0kj1m.cn/gtsmmexnzm.html

Java: list.subList(1, 4);
来源：http://hz.52xcode.cn/gtngehxeyo.html

Go:   arr[1:4]
来源：http://hz.daxiang520.top/gtdgeatgid.html

Ruby: arr[1, 3]
来源：http://hz.jinqigufen.top/gtglwjpegz.html

C#:   list.GetRange(1, 3);
来源：http://hz.jiagoushi.top/gtubltmkqv.html

[D08] 合并两个数组
来源：http://hz.tianlin.xyz/gtvphamkwb.html

Py:   a + b;  a.extend(b)
来源：http://hz.jqgfzy.top/gtzlziyoli.html

PHP:  array_merge($a, $b);
来源：http://hz.hysaishi.cn/gtgnkoovkz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.guannengcc.top/gtzuymsovs.html

TS:   [...a, ...b];
来源：http://hz.zdqjudy.top/gtcrviwgtm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.52xcode.cn/gtkignnylz.html

Go:   append(a, b...)
来源：http://hz.zhixingplan.top/gteaoflpwg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zycfv.cn/gtzzsuftgw.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhaomingkeji.xyz/gtqmrqbcri.html

[D09] 排序（升序）
来源：http://hz.kuanghao11.cn/gtdscdtika.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tanke756.top/gtydmzcejp.html


<!-- 参考信息 -->