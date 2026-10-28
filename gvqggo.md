代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hz.cucudq.cn/gtyqywtcea.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.wangdashe.top/gtepglvuqy.html

JS:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gtojmlpblt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.daria6918.cn/gtajsmezyz.html

Java: do { i++; } while (i < 10);
来源：http://hz.wangdashe.top/gtzjzpujhw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.shanyushiyangkeji.top/gtemzzpfaz.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ybcxt.top/gttqsiltpq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtcmifzkwh.html

[B09] break 与 continue
来源：http://hz.fengsongda.top/gtnjscjbux.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.52xcode.cn/gtubpoxsqu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.dashuyun.cn/gtbkzvnpbj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtjsqhsjpo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtdkxmqkon.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cqqwz.cn/gtucnrcdcj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.bjfxy.top/gtxrxihafc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.chenlongwang.top/gtciubxsyp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.birdmap.top/gtmedtygtj.html

[B10] 遍历同时拿索引
来源：http://hz.ehwqpu.com/gtbbjbelcr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.aibaodan.cn/gtdasattjc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yj202588.top/gtsjiteopj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.snrcjt.cn/gtsctpnnnl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.meibo888.top/gtjytvuxrp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.fzhhl.top/gtaghzphcq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.dianchejie.cn/gtkjftitgg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ppjwa.cn/gtufxnisxz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.tianlin.xyz/gttvlowgfu.html

[B11] 生成数字序列 / 区间
来源：http://hz.iojbl.cn/gtgqfanbsh.html

Py:   list(range(0, 10, 2))
来源：http://hz.yangfankeji.com/gtlpwxsmvw.html

PHP:  range(0, 10, 2);
来源：http://hz.daria6918.cn/gtxassmcpo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zycfv.cn/gtcknetgox.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtiswcvrix.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhaomingkeji.xyz/gteyigohdv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jqgfzy.top/gtdxywoxzd.html

Ruby: (0...10).step(2).to_a
来源：http://hz.fzhhl.top/gtqpeywdmq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.smart0.xyz/gtfmqmdvjv.html

[B12] 跳出多层循环
来源：http://hz.zhixingplan.top/gtkhhlbwky.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.c1oappe.top/gteiudzvwf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.quarkkingdee.top/gtqkwmvuqv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.52xcode.cn/gtwufdpdqo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtoincubyr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxinkj.top/gtltcaiuck.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhaomingkeji.xyz/gtrfhsllzc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.tianlin.xyz/gtdzfklbtw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.fengsongda.top/gttjgwyoxr.html

[B13] 判断是否为数字
来源：http://hz.316326.xyz/gtwgnhbbqf.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigfzy.top/gtcjhqlqco.html

PHP:  is_numeric($x)
来源：http://hz.bjfxy.top/gtqluuccdd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuanzx.com/gtvzrqhuok.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shanyushiyangkeji.top/gtqbzaokll.html

Java: x instanceof Number
来源：http://hz.zhongyouzk.top/gtkxjennex.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.feifeiyinyue.top/gtmvyfaxpl.html

Ruby: x.is_a?(Numeric)
来源：http://hz.gaohongyu789.top/gtxibilikh.html

C#:   x is int or double or decimal
来源：http://hz.yj20258.top/gtazyzahos.html

[B14] 判断值是否在集合内
来源：http://hz.zycfv.cn/gtjcmfiamj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gogol.net.cn/gtukupbbui.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gotoacloud.top/gtkqbffdml.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.9152youxi.cn/gtuznnzkvc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.mhx1999.top/gtdsswdqxl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhoulong.xyz/gtynouwmeu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xylfe.cn/gtnhcaeevb.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hfpthk.cn/gtiqgwhtmu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhoulong.xyz/gtlloiqplj.html

[B15] 布尔运算与取反
来源：http://hz.316326.xyz/gtupzwvszs.html

Py:   a and b or not c
来源：http://hz.gotoacloud.top/gtemlcdesr.html

PHP:  $a && $b || !$c
来源：http://hz.hammf.cn/gthcoszdrk.html

JS:   a && b || !c
来源：http://hz.wangdashe.top/gtfwznyuln.html

TS:   a && b || !c
来源：http://hz.kuanghao11.cn/gteagwjrfx.html

Java: a && b || !c
来源：http://hz.jinghuilouyu.cn/gtiwpprbhc.html

Go:   a && b || !c
来源：http://hz.zhixingplan.top/gthgmkdatz.html

Ruby: a && b || !c
来源：http://hz.andypj.xyz/gtzdekwysh.html

C#:   a && b || !c
来源：http://hz.aibaodan.cn/gtjvgodosk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sxryk.cn/gtkxrdznos.html

Py:   if not data: return
来源：http://hz.zhengqikj.top/gtgtpdnwja.html

PHP:  if (!$data) { return; }
来源：http://hz.yuxming.cn/gtqdsfzjmg.html

JS:   if (!data) return;
来源：http://hz.wangshuangyany.cn/gttwpjszxu.html

TS:   if (!data) return;
来源：http://hz.ehwqpu.com/gtbnzawinc.html

Java: if (data == null) return;
来源：http://hz.jiagoushi.top/gtparxikvq.html

Go:   if data == nil { return }
来源：http://hz.ywan-chungtsiang.top/gtzmamjwne.html

Ruby: return if data.nil?
来源：http://hz.yj20258888.top/gtasxqiukk.html

C#:   if (data == null) return;
来源：http://hz.chenzaomai.com/gtumjoeeuv.html

================================================================================
来源：http://hz.hammf.cn/gtmhrjkfpf.html

C. 函数与作用域
来源：http://hz.nwbrower.top/gtpzdralis.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmmcosize.html

[C01] 定义函数
来源：http://hz.jinqigufen.top/gtfnwpdqxu.html

Py:   def add(a, b): return a + b
来源：http://hz.mhx1999.top/gtgiqpecjx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nwbrower.top/gtreelbask.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cqqwz.cn/gtzwsrqrjr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sufxvd.cn/gtuzjshlbq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.mhx1999.top/gtarubrizx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guowangkeji.top/gtdkbgepwz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gzhubu.top/gtqxhgbycy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtsxghiwzv.html

[C02] 默认参数
来源：http://hz.mhx1999.top/gtrottoaut.html

Py:   def greet(name="World"): return name
来源：http://hz.zhiwuduotai.top/gtgommjgar.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.pengpengdd.cyou/gtxenwrzkg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yuanzhike.top/gtqmsrbqtj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gotoacloud.top/gtpwlkwicq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zycfv.cn/gtrkkbwetk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.9152youxi.cn/gtitmbtffj.html

Ruby: def greet(name = "World") = name
来源：http://hz.jiagoushi.top/gtinmmfglh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.andypj.xyz/gtkxdholfw.html

[C03] 可变参数
来源：http://hz.sweek.top/gteftilehr.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhengqikj.top/gtfglucrto.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ehwqpu.com/gtvfgnztjr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxinkj.top/gtkgekjqrs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guannengcc.top/gtqjxlbiiz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.tianlin.xyz/gtmmsogpfm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.0kj1m.cn/gtxeazqqeq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.fengsongda.top/gtdmarieav.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.c1oappe.top/gtkpelmhtb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hysaishi.cn/gtkkkygshu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tian-w.cn/gtdhagwqyi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj20258888.top/gtrvgwqhmy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtogfqakwc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xinyue.icu/gtulnxnleg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.daxiang520.top/gtyjclnaqn.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuxming.cn/gtbxddkkuw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtlicitsgz.html

C#:   f(a: 1, b: 2)
来源：http://hz.xylfe.cn/gtibsakyhn.html

[C05] 返回多个值
来源：http://hz.ybcxt.top/gthzvsfghg.html

Py:   return a, b
来源：http://hz.guowangkeji.top/gtdcyklekd.html

PHP:  return [$a, $b];
来源：http://hz.pengpengdd.cyou/gtqeneprem.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tanke756.top/gthaqmxqym.html

TS:   return { a, b };
来源：http://hz.mhx1999.top/gtkjljjphf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.feifeiyinyue.top/gtqjmeyxzx.html

Go:   return a, b
来源：http://hz.guannengcc.top/gtysrsbnto.html

Ruby: return a, b
来源：http://hz.zhongyouzk.top/gtzjtetagm.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dianchejie.cn/gttqwbxtiw.html

[C06] 匿名函数 / lambda
来源：http://hz.yj20258888.top/gtdzfbpwgj.html

Py:   square = lambda x: x * x
来源：http://hz.sufxvd.cn/gtetpcviwr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shzxlz.cn/gtiszgumld.html

JS:   const square = x => x * x;
来源：http://hz.shangyingyoupin.top/gtzyxntsxy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jyoumei.cn/gtsaimwwaw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.aizwys.cn/gtkocpzaez.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yanxiufei.cn/gtkubpoqkg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.iojbl.cn/gtdmrufhtt.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zycfv.cn/gtpczlihlj.html

[C07] 把函数作为参数传入
来源：http://hz.cheryme.top/gtupnezmod.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.316326.xyz/gtnluarrcu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zycfv.cn/gtdmntjvzp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yueranfly.top/gtbkqdmlcp.html

TS:   arr.map(String)
来源：http://hz.tian-w.cn/gteokmxadv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xylfe.cn/gtmiohgxrj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.nwbrower.top/gtsgjufjaa.html

Ruby: arr.map(&:upcase)
来源：http://hz.mhx1999.top/gtptihgumz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.chenlongwang.top/gtquzdhfld.html

[C08] 闭包
来源：http://hz.yj20258888.top/gtvmuvxzas.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yj20258.top/gtulbkumel.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tian-w.cn/gtihqwqtye.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtvhxkceye.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.mhx1999.top/gtccavzdzv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.quarkkingdee.top/gtvygjhhuj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.fengsongda.top/gtcjijpgcd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jianghu66.top/gtfqtpncox.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtfxbuzjro.html

[C09] 递归
来源：http://hz.xuetiantiany.cn/gtuuyuwsdx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jqgufenzy.top/gtimfixeue.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.wangshuangyany.cn/gtpkraqjmv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtmggjmrqw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fzhhl.top/gthsztbxhs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258.top/gtqznebmui.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenjidiqi.icu/gtrpeofnrn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinyuanbaomall.cn/gtthwysivi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydjk.org.cn/gtdflnwcbh.html

[C10] 变量作用域
来源：http://hz.zhengqikj.top/gtrnqsokae.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ybcxt.top/gtaxcxrntd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhixingplan.top/gtlffhrrdp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinqigfzy.top/gtjftbcqos.html

TS:   同 JS
来源：http://hz.jiagoushi.top/gtmeetnvyf.html

Java: 方法内为块级作用域
来源：http://hz.ydjk.org.cn/gtvuyizvee.html

Go:   花括号块级作用域
来源：http://hz.hfpthk.cn/gtcrsnvktr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.9152youxi.cn/gtwemlryex.html

C#:   块级作用域
来源：http://hz.shanyushiyangtech.top/gteoeyrpsr.html

[C11] 模块导入与导出
来源：http://hz.andypj.xyz/gthwinzrvj.html

Py:   from module import func
来源：http://hz.birdmap.top/gtbupttrpw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.chenjidiqi.icu/gtqnztenhn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.bjfxy.top/gtoaniaqgz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.pycfn.com/gtuntqipgz.html

Java: import java.util.List;
来源：http://hz.ybcxt.top/gtdqspavlv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jiagoushi.top/gtibbmlqub.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.52xcode.cn/gtsbbktyle.html

C#:   using System.Text;
来源：http://hz.cqqwz.cn/gtksskmaev.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinyuanbaomall.cn/gttkqbdqjk.html

Py:   (lambda: print("run"))()
来源：http://hz.sweek.top/gtvarlsygm.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zdqjudy.top/gtgudbiirp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhengqikj.top/gtiwbhjwuv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gthputwyxt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yvedp.cn/gtryvvbcpl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.pengpengdd.cyou/gtiqvwbeik.html

Ruby: -> { puts "run" }.call
来源：http://hz.yuxming.cn/gtxzjxonvs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daxiang520.top/gtwcasvlis.html

[C13] 类型声明 / 类型注解
来源：http://hz.hongshengwenyu.top/gtyzefnmwr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hnxiangtu.top/gtjejnabkc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtxraxtamn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pycfn.com/gtwhnlxvle.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dianchejie.cn/gtmanokgfg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gttcqdiidk.html

Go:   func add(a, b int) int
来源：http://hz.haohaochexian.top/gtvboatblm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fzhhl.top/gtoebpzcew.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daxiang520.top/gtccesfxyl.html

[C14] 泛型函数
来源：http://hz.yj202588.top/gtzfmydsuy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jiagoushi.top/gteyjesrka.html

PHP:  // 无泛型
来源：http://hz.ydzc1.top/gtrdzfgqnc.html

JS:   // 无泛型
来源：http://hz.chenlongwang.top/gtajqknhnl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.daxiang520.top/gtqqtwedjf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hnxiangtu.top/gthrrmitmo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shanyushiyangkeji.top/gtvuhhtmih.html

Ruby: # 无泛型
来源：http://hz.yvedp.cn/gtudrgzsdl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangshuangyany.cn/gtpwozltje.html

[C15] 解构 / 展开参数
来源：http://hz.haohaochexian.top/gtmyibgctw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.wangshuangyany.cn/gtidaoqlhu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj202588.top/gtjreynmge.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yanxiufei.cn/gtythlpgzt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenjidiqi.icu/gtkynkgcow.html

Java: // 无解构
来源：http://hz.ivvv.top/gtknrnazrt.html

Go:   // 无解构
来源：http://hz.redwolf501.top/gtjgodjznn.html

Ruby: a, b = pair
来源：http://hz.jiagoushi.top/gtzzvglxkn.html

C#:   var (a, b) = pair;
来源：http://hz.gzhubu.top/gteyauzcud.html

[C16] 函数 / 方法重载
来源：http://hz.yonumen.top/gtordgtyup.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xziqi.cn/gtgrnjwyko.html

PHP:  // 无重载
来源：http://hz.gotoacloud.top/gtyqgqtygw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ydzc1.top/gtmzgpbzyc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tian-w.cn/gtjhvjtwdw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cqqwz.cn/gtvypkhpje.html

Go:   // 无重载：用不同函数名
来源：http://hz.ydzc1.top/gtqnnvmahr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jlsjyb.cn/gtltrfkisc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xziqi.cn/gtaytdwhtf.html

================================================================================
来源：http://hz.daria6918.cn/gtrxujqsqq.html

D. 数组 / 列表 / 集合
来源：http://hz.cashguo.top/gtsxjegnkr.html

================================================================================
来源：http://hz.zhoulong.xyz/gtfdawbwwr.html

[D01] 创建数组 / 列表
来源：http://hz.kuanghao11.cn/gtwjuuitid.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangkeji.top/gtfmjravuq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.guannengcc.top/gtoffwkdwq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guowangkeji.top/gtknouxdih.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhaomingkeji.xyz/gtikpoxjyy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shzxlz.cn/gtldjkblug.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgufenzy.top/gtiwcsymyf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nwbrower.top/gtnawlbucs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.vqdsnc.cn/gtsgtkgist.html

[D02] 追加元素到末尾
来源：http://hz.c1oappe.top/gtueooormk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hongshengwenyu.top/gtfmkssogo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cheryme.top/gtprddcqmb.html

JS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtoxeabjch.html

TS:   arr.push(4);
来源：http://hz.jinyuanbaomall.cn/gtblfpqupl.html

Java: list.add(4);
来源：http://hz.cqqwz.cn/gtgrjpjhty.html

Go:   arr = append(arr, 4)
来源：http://hz.hywenlv.cn/gtwwycxtlx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.c1oappe.top/gtvcsqpawd.html

C#:   list.Add(4);
来源：http://hz.jyoumei.cn/gtbuzqhnxj.html

[D03] 在指定位置插入元素
来源：http://hz.zhijiandao.cn/gtebjosjhl.html

Py:   arr.insert(0, 0)
来源：http://hz.jqgfzy.top/gtrzpahzkh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenzaomai.com/gtrtiupwev.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhongyouzk.top/gtddxwfhsu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.dianchejie.cn/gtsbcoaxbv.html

Java: list.add(0, 0);
来源：http://hz.kuanghao11.cn/gtcpsabqfo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sweek.top/gtkcqnvlsv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.haohaochexian.top/gtcdtaamdu.html

C#:   list.Insert(0, 0);
来源：http://hz.hnqzz.top/gtmbikgkej.html

[D04] 删除元素
来源：http://hz.zhiwuduotai.top/gtbudnkpnc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.feifeiyinyue.top/gtujgxojsk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinyuanbaomall.cn/gtcultyxqb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.dianchejie.cn/gtycffzrmh.html

TS:   arr.splice(0, 1);
来源：http://hz.9152youxi.cn/gtzmsdsnva.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shzxlz.cn/gtkpojglex.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cucudq.cn/gtdlpkufrj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yvedp.cn/gtfhybzxbb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.haohaochexian.top/gtlfkoqxbv.html

[D05] 访问与修改元素
来源：http://hz.xuanzx.com/gtymodidxj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jqgufenzy.top/gtfofnnzlh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sysykeji.top/gtoindhpok.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cheryme.top/gtwwhxjdoi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.kuanghao11.cn/gtwpxyymyp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.haohaochexian.top/gtutlybfyq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jqgufenzy.top/gthuboqfdq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtkvakwffg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jianghu66.top/gtrlxutqnx.html

[D06] 数组长度
来源：http://hz.tanke756.top/gthhgaskoe.html

Py:   len(arr)
来源：http://hz.nanxuanxn.top/gtqcdshwgu.html

PHP:  count($arr);
来源：http://hz.vqdsnc.cn/gtpeklmyfx.html

JS:   arr.length
来源：http://hz.jyoumei.cn/gtcdclsskz.html

TS:   arr.length
来源：http://hz.zhiwuduotai.top/gtwzhdvjrd.html

Java: list.size();
来源：http://hz.havefunace.top/gtdlcdbijc.html

Go:   len(arr)
来源：http://hz.wangdashe.top/gtwnkdxsfi.html

Ruby: arr.length; arr.size
来源：http://hz.ppjwa.cn/gtrnrfzqlj.html

C#:   list.Count;
来源：http://hz.iojbl.cn/gtqspmecpd.html

[D07] 切片 / 取子数组
来源：http://hz.nanxinkj.top/gtbaufnwgg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigufen.top/gtkqlxpqdm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yvedp.cn/gttmszfkqi.html

JS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtbpmjakcs.html

TS:   arr.slice(1, 4);
来源：http://hz.hfpthk.cn/gtuevspjbq.html

Java: list.subList(1, 4);
来源：http://hz.chenzaomai.com/gtgccsijln.html

Go:   arr[1:4]
来源：http://hz.pengpengdd.cyou/gtoanzgkkb.html

Ruby: arr[1, 3]
来源：http://hz.cucudq.cn/gtnbwitkja.html

C#:   list.GetRange(1, 3);
来源：http://hz.jiagoushi.top/gtpeptichz.html

[D08] 合并两个数组
来源：http://hz.zhongyouzk.top/gtslfhktcv.html

Py:   a + b;  a.extend(b)
来源：http://hz.guannengcc.top/gtjyxjmsfy.html

PHP:  array_merge($a, $b);
来源：http://hz.yanxiufei.cn/gtfasiaeqc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenlongwang.top/gtljrsmyzu.html

TS:   [...a, ...b];
来源：http://hz.zhengqikj.top/gtkoxknjxy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yvedp.cn/gtsskatxef.html

Go:   append(a, b...)
来源：http://hz.iojbl.cn/gtarzwvmnj.html


<!-- 参考信息 -->