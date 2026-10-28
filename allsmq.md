代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hz.nanxinkj.top/gtxopnfhja.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhengqikj.top/gtnzxakxok.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtpbkvyncb.html

TS:   do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gtoclptoza.html

Java: do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gtlcekrshv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jianghu66.top/gtgxquxzou.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yj20258888.top/gtrvkcalun.html

C#:   do { i++; } while (i < 10);
来源：http://hz.aibaodan.cn/gtmujilgkt.html

[B09] break 与 continue
来源：http://hz.yanxiufei.cn/gtmjoufpqw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sxryk.cn/gtqwciflpi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj20258.top/gtakulmruq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guowangkeji.top/gtpucsiell.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhoulong.xyz/gtgqnxqcbu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtssggmgja.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.havefunace.top/gtcezzqsbt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhijiandao.cn/gttpcltvxx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cqqwz.cn/gtletqftqd.html

[B10] 遍历同时拿索引
来源：http://hz.wangdashe.top/gtdnekovjt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhaomingkeji.xyz/gtueebpbga.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.feifeiyinyue.top/gtczdbdltv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinqigufen.top/gthzsrshqb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cqqwz.cn/gtnstzvwzy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.0kj1m.cn/gtjpvwslfq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.guowangkeji.top/gtqczosqjg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hnxiangtu.top/gtuiprgufc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yongpay.top/gtybhjrykx.html

[B11] 生成数字序列 / 区间
来源：http://hz.shuidangran.top/gtosidqljz.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj20258.top/gtlacdvytz.html

PHP:  range(0, 10, 2);
来源：http://hz.cucudq.cn/gtxbzdpagh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guowangkeji.top/gtudfipjje.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daria6918.cn/gtxxmswfju.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yuanzhike.top/gtojqoteki.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.guannengcc.top/gtsphvzeqz.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yvedp.cn/gtadgwffln.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenzaomai.com/gtwnjhjmkl.html

[B12] 跳出多层循环
来源：http://hz.kuanghao11.cn/gtrlgwarff.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.chenlongwang.top/gtnkqgpeid.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xingfuxueyuan.xyz/gtodernjhn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhengqikj.top/gthxqqbztp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daxiang520.top/gtxqjvznzn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtrritodrj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.daria6918.cn/gtyjgjnwbp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hnxiangtu.top/gtpyhdoiux.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yonumen.top/gtugxatnqp.html

[B13] 判断是否为数字
来源：http://hz.birdmap.top/gtujhrtpwv.html

Py:   isinstance(x, (int, float))
来源：http://hz.quarkkingdee.top/gtcmiablkz.html

PHP:  is_numeric($x)
来源：http://hz.feifeiyinyue.top/gttawsjchy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydzc1.top/gtlvtwvybx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.iojbl.cn/gtfrevlmjw.html

Java: x instanceof Number
来源：http://hz.xinyue.icu/gtzuklyewa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nanxuanxn.top/gtcigfpqba.html

Ruby: x.is_a?(Numeric)
来源：http://hz.daria6918.cn/gtwnerrqel.html

C#:   x is int or double or decimal
来源：http://hz.gogol.net.cn/gtsaonkqfo.html

[B14] 判断值是否在集合内
来源：http://hz.xylfe.cn/gtczjpvkwp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.aizwys.cn/gtcpylfjkz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yangfankeji.com/gtqpipkwvn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xziqi.cn/gttkcgcctu.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigfzy.top/gtxayuhxpl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgufenzy.top/gtojsrcors.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ydzc1.top/gtirovsiiy.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.0kj1m.cn/gtgqtmcfcl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.snrcjt.cn/gtqnsgbewx.html

[B15] 布尔运算与取反
来源：http://hz.meibo888.top/gtvcsoqfjr.html

Py:   a and b or not c
来源：http://hz.svipenyu.cn/gtsikqkzgr.html

PHP:  $a && $b || !$c
来源：http://hz.snrcjt.cn/gtvqytcrcv.html

JS:   a && b || !c
来源：http://hz.hammf.cn/gtpbunxwqn.html

TS:   a && b || !c
来源：http://hz.guowangkeji.top/gtduygsvqr.html

Java: a && b || !c
来源：http://hz.gzhubu.top/gthavszgfb.html

Go:   a && b || !c
来源：http://hz.hnxiangtu.top/gtqzghlrll.html

Ruby: a && b || !c
来源：http://hz.birdmap.top/gtlcaqrlpp.html

C#:   a && b || !c
来源：http://hz.cqqwz.cn/gtahllatvp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cqqwz.cn/gtqxmdrzsz.html

Py:   if not data: return
来源：http://hz.jinqigufen.top/gtjvjzsaba.html

PHP:  if (!$data) { return; }
来源：http://hz.gogol.net.cn/gtnpupzdhn.html

JS:   if (!data) return;
来源：http://hz.gzhubu.top/gtbhfctqbf.html

TS:   if (!data) return;
来源：http://hz.svipenyu.cn/gthccdojpa.html

Java: if (data == null) return;
来源：http://hz.sweek.top/gtulmbxlcs.html

Go:   if data == nil { return }
来源：http://hz.chenzaomai.com/gtsliavegs.html

Ruby: return if data.nil?
来源：http://hz.gogol.net.cn/gtnitmmdfe.html

C#:   if (data == null) return;
来源：http://hz.xinyue.icu/gtcptbbqlw.html

================================================================================
来源：http://hz.gotoacloud.top/gtryxaodwq.html

C. 函数与作用域
来源：http://hz.hnxiangtu.top/gtjnwhjhaa.html

================================================================================
来源：http://hz.sweek.top/gtitsdkmtv.html

[C01] 定义函数
来源：http://hz.iojbl.cn/gtzivfsaiw.html

Py:   def add(a, b): return a + b
来源：http://hz.jinqigufen.top/gtirpzhlxh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gthljaxijb.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ehwqpu.com/gtnoycwywy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yongpay.top/gtvsodnmqm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtpgoembaw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinyuanbaomall.cn/gtrvdjjtyn.html

Ruby: def add(a, b); a + b; end
来源：http://hz.kuanghao11.cn/gtgarrmxnv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtnoqgpdkw.html

[C02] 默认参数
来源：http://hz.zhaomingkeji.xyz/gtrxhhsswh.html

Py:   def greet(name="World"): return name
来源：http://hz.daxiang520.top/gtkhwwcnyk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yongpay.top/gtgptyewgz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yuanzhike.top/gtarvonnwc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.guowangkeji.top/gtbhjpeoct.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dianchejie.cn/gtkptwcnaj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hongshengwenyu.top/gtdnwymkse.html

Ruby: def greet(name = "World") = name
来源：http://hz.nanxuanxn.top/gtbpiodpck.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.fzhhl.top/gtjnhwublx.html

[C03] 可变参数
来源：http://hz.jinqigfzy.top/gtqojyexfx.html

Py:   def total(*args): return sum(args)
来源：http://hz.bjfxy.top/gtfpdrhzfi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jianghu66.top/gtdfcdlase.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pycfn.com/gtavycywgr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yonumen.top/gtsmsbcpaq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hfpthk.cn/gtvgfxarjk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yonumen.top/gtxzypknir.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinqigufen.top/gtydldwipp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.tian-w.cn/gtepvizgnz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgfzy.top/gtxahnkmsf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ivvv.top/gtuhgjxjaj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhengqikj.top/gtswkpjyos.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.aizwys.cn/gtbupgcidu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.aibaodan.cn/gtxvynjawx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gaohongyu789.top/gtuudvlfsq.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhiwuduotai.top/gtrvmlgulf.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sysykeji.top/gtcexxlcpg.html

C#:   f(a: 1, b: 2)
来源：http://hz.gogol.net.cn/gtcjihllpg.html

[C05] 返回多个值
来源：http://hz.yvedp.cn/gtavtptfgs.html

Py:   return a, b
来源：http://hz.zhongyouzk.top/gtehisttzi.html

PHP:  return [$a, $b];
来源：http://hz.andypj.xyz/gtrngfuxia.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jqgfzy.top/gtszwqyhsf.html

TS:   return { a, b };
来源：http://hz.xuetiantiany.cn/gtdvamsqxo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sysykeji.top/gtjnmjmagl.html

Go:   return a, b
来源：http://hz.cqqwz.cn/gtfeazapam.html

Ruby: return a, b
来源：http://hz.gotoacloud.top/gtncsrcztz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhixingplan.top/gtayjlqydm.html

[C06] 匿名函数 / lambda
来源：http://hz.gotoacloud.top/gtsdqrdshh.html

Py:   square = lambda x: x * x
来源：http://hz.shzxlz.cn/gtjstdwrsj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jyoumei.cn/gtyylhmmii.html

JS:   const square = x => x * x;
来源：http://hz.zhoulong.xyz/gtexnatwhu.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cheryme.top/gtuorrqxmx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sweek.top/gtzdophzhu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.daria6918.cn/gtbgprbflg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cqqwz.cn/gthjrytthb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hfpthk.cn/gtbzpsbzyz.html

[C07] 把函数作为参数传入
来源：http://hz.shzxlz.cn/gtzfvoptul.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.feifeiyinyue.top/gtdlgmbnir.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gogol.net.cn/gtkcmryaxy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.feifeiyinyue.top/gtocfdfaxk.html

TS:   arr.map(String)
来源：http://hz.cashguo.top/gteqhzqhhl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.redwolf501.top/gtfseegydr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhixingplan.top/gtznecvvmb.html

Ruby: arr.map(&:upcase)
来源：http://hz.pengpengdd.cyou/gtamsmlabk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.chenzaomai.com/gtsegdoats.html

[C08] 闭包
来源：http://hz.cdnleiting.top/gtqqjkwdud.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sxryk.cn/gtaqzwrfpy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zycfv.cn/gtydtfddcf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.aizwys.cn/gtsmbtcgyu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.meibo888.top/gtwehbkqqy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.316326.xyz/gterhtlypc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cdnleiting.top/gtpecncnxe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.daria6918.cn/gtpwubisfh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gtjeoxshdc.html

[C09] 递归
来源：http://hz.ehwqpu.com/gttzqeehbn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.316326.xyz/gtbxscityz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhoulong.xyz/gtgbkdoqoy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aibaodan.cn/gtniioksky.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gogol.net.cn/gtwjscmuks.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tanke756.top/gtiwahcujz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yj20258.top/gtcpbmmykw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj20258888.top/gtpypmhrcz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sysykeji.top/gtlggfktzx.html

[C10] 变量作用域
来源：http://hz.jianghu66.top/gtprntxukf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jqgufenzy.top/gtggjtuttr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sweek.top/gttcijdwby.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenlongwang.top/gtaiynddtk.html

TS:   同 JS
来源：http://hz.yongpay.top/gtpnipmbli.html

Java: 方法内为块级作用域
来源：http://hz.tian-w.cn/gtrgqrlbdo.html

Go:   花括号块级作用域
来源：http://hz.shuidangran.top/gtxpuqsgyh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhongyouzk.top/gtmgylrfxu.html

C#:   块级作用域
来源：http://hz.jinghuilouyu.cn/gtthtsyfsh.html

[C11] 模块导入与导出
来源：http://hz.yanxiufei.cn/gtadrcobdw.html

Py:   from module import func
来源：http://hz.zycfv.cn/gtnsqfduwl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jyoumei.cn/gtsegcgxlm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhoulong.xyz/gthqotuhhm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jianghu66.top/gtydxoshhm.html

Java: import java.util.List;
来源：http://hz.shuidangran.top/gtzxhfhmfd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj202588.top/gtndpgwkej.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shuidangran.top/gtcxfzglie.html

C#:   using System.Text;
来源：http://hz.zhixingplan.top/gtuzmwgdwm.html

[C12] 立即执行函数 IIFE
来源：http://hz.yvedp.cn/gtblxgxato.html

Py:   (lambda: print("run"))()
来源：http://hz.tianlin.xyz/gtlaoxnqft.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jqgufenzy.top/gtbvipjsgb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daria6918.cn/gtrhwdwzoi.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xuanzx.com/gtymjyndzg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinyuanbaomall.cn/gtpdqywlne.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.redwolf501.top/gtwgdyzjyo.html

Ruby: -> { puts "run" }.call
来源：http://hz.kuanghao11.cn/gthtoomhks.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhongyouzk.top/gtojystrzm.html

[C13] 类型声明 / 类型注解
来源：http://hz.xingfuxueyuan.xyz/gtyksutdbm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cucudq.cn/gtavjwnxhm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtzeskwicq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgufenzy.top/gtcohmtrpm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj202588.top/gtrpxjqsrv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.dianchejie.cn/gttrmodobb.html

Go:   func add(a, b int) int
来源：http://hz.zhongyouzk.top/gtcxgweocl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.9152youxi.cn/gtokyfcryc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.pycfn.com/gtrlyngqms.html

[C14] 泛型函数
来源：http://hz.fzhhl.top/gthdhfjesw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ehwqpu.com/gtjvctdabk.html

PHP:  // 无泛型
来源：http://hz.zhongyouzk.top/gtdemiujog.html

JS:   // 无泛型
来源：http://hz.zhaomingkeji.xyz/gtdwmvseug.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinghuilouyu.cn/gtaselpjkz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jqgufenzy.top/gtpdcymvfs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yanxiufei.cn/gtoveuieid.html

Ruby: # 无泛型
来源：http://hz.tianlin.xyz/gtxpxvietr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hysaishi.cn/gtbzpjjkjk.html

[C15] 解构 / 展开参数
来源：http://hz.yj202588.top/gtadhtrvgk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yuxming.cn/gthtjmdnbt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hywenlv.cn/gtnroirrmg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xinyue.icu/gtgssrjoks.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xinyue.icu/gtgvdnlddo.html

Java: // 无解构
来源：http://hz.fzhhl.top/gtnlvyomww.html

Go:   // 无解构
来源：http://hz.9152youxi.cn/gtglxkbnyp.html

Ruby: a, b = pair
来源：http://hz.shanyushiyangkeji.top/gtpcidyafc.html

C#:   var (a, b) = pair;
来源：http://hz.bjfxy.top/gtahnrebiu.html

[C16] 函数 / 方法重载
来源：http://hz.gogol.net.cn/gtwiidxhsg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fengsongda.top/gtdzhcpjfb.html

PHP:  // 无重载
来源：http://hz.dashuyun.cn/gtfupxabsc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hysaishi.cn/gtyraqxsem.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tian-w.cn/gtlmoaszrz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhixingplan.top/gtifxtvzre.html

Go:   // 无重载：用不同函数名
来源：http://hz.ywan-chungtsiang.top/gtfoyldfld.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yvedp.cn/gtvsrvovzu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.feifeiyinyue.top/gtvtirpvmw.html

================================================================================
来源：http://hz.pycfn.com/gtgcbyucya.html

D. 数组 / 列表 / 集合
来源：http://hz.gzhubu.top/gtsydbialt.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtqvzvlzmi.html

[D01] 创建数组 / 列表
来源：http://hz.xuanzx.com/gtvszlcmxf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gaohongyu789.top/gtwjbcjkyz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ydjk.org.cn/gtvcsdzdya.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj202588.top/gttwoamjpv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ppjwa.cn/gteyvrzzds.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.bjfxy.top/gtatczjynf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hysaishi.cn/gtanhwewtp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daxiang520.top/gtswlvxwyk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.vqdsnc.cn/gtkvqtljdx.html

[D02] 追加元素到末尾
来源：http://hz.ywan-chungtsiang.top/gtllqhxjpg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yonumen.top/gtnssapmte.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pengpengdd.cyou/gttfmergis.html

JS:   arr.push(4);
来源：http://hz.iojbl.cn/gtkwlepeqz.html

TS:   arr.push(4);
来源：http://hz.xziqi.cn/gtdevouzwk.html

Java: list.add(4);
来源：http://hz.zhixingplan.top/gtxoaayuqe.html

Go:   arr = append(arr, 4)
来源：http://hz.daxiang520.top/gtcjizfhqn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhongyouzk.top/gtmrctbcde.html

C#:   list.Add(4);
来源：http://hz.zhengqikj.top/gtdvtjrmmu.html

[D03] 在指定位置插入元素
来源：http://hz.shuidangran.top/gtxymivqcp.html

Py:   arr.insert(0, 0)
来源：http://hz.gzhubu.top/gtexjocjkj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.haohaochexian.top/gtwbtgrksz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nanxuanxn.top/gtmzbqtico.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.nanxuanxn.top/gtcvoyrbvb.html

Java: list.add(0, 0);
来源：http://hz.52xcode.cn/gtfrtgxyoo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.52xcode.cn/gtapzdrbui.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yongpay.top/gtzzlwrkcj.html

C#:   list.Insert(0, 0);
来源：http://hz.aizwys.cn/gttztlaana.html

[D04] 删除元素
来源：http://hz.9152youxi.cn/gtijygtwog.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cheryme.top/gtycnjtqlk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jianghu66.top/gtqfyndwns.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xingfuxueyuan.xyz/gtxdqlbbzs.html

TS:   arr.splice(0, 1);
来源：http://hz.zdqjudy.top/gtrcaqgexj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ywan-chungtsiang.top/gtyahorztz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xuetiantiany.cn/gtnhifrvie.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yueranfly.top/gtxqyszxoy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shzxlz.cn/gtbzlbdgbe.html

[D05] 访问与修改元素
来源：http://hz.nanxuanxn.top/gtcgqclurh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gtcskdoqua.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sufxvd.cn/gtzrxfoxdi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.daxiang520.top/gteatmrxih.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xylfe.cn/gtwjgvdqgv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jyoumei.cn/gtlwgjghqt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gtapymdxoa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtbkmlwwgy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sysykeji.top/gtmkbysrtb.html

[D06] 数组长度
来源：http://hz.ybcxt.top/gtzjxgqour.html

Py:   len(arr)
来源：http://hz.birdmap.top/gtzizoxplr.html

PHP:  count($arr);
来源：http://hz.jinqigufen.top/gtxphgzrzu.html

JS:   arr.length
来源：http://hz.snrcjt.cn/gtzxkjkobb.html

TS:   arr.length
来源：http://hz.sxryk.cn/gtbwakovuh.html

Java: list.size();
来源：http://hz.bjfxy.top/gtmibybhnn.html

Go:   len(arr)
来源：http://hz.gotoacloud.top/gtblyxvimc.html

Ruby: arr.length; arr.size
来源：http://hz.hfpthk.cn/gtvcncmuka.html

C#:   list.Count;
来源：http://hz.zhoulong.xyz/gtjsbtgkpg.html

[D07] 切片 / 取子数组
来源：http://hz.wangshuangyany.cn/gthpqjnmpb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shzxlz.cn/gtvyenaxkj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.316326.xyz/gtgajjvkhe.html

JS:   arr.slice(1, 4);
来源：http://hz.jinghuilouyu.cn/gtmgsectsn.html

TS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtucxosgwf.html

Java: list.subList(1, 4);
来源：http://hz.jyoumei.cn/gtyofdzzry.html

Go:   arr[1:4]
来源：http://hz.dianchejie.cn/gtiepzbdae.html

Ruby: arr[1, 3]
来源：http://hz.tianlin.xyz/gtayvnuqjp.html

C#:   list.GetRange(1, 3);
来源：http://hz.xinyue.icu/gtarhnqung.html

[D08] 合并两个数组
来源：http://hz.feifeiyinyue.top/gtfietraho.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxinkj.top/gtnldnpyis.html

PHP:  array_merge($a, $b);
来源：http://hz.snrcjt.cn/gteubcmhdz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dashuyun.cn/gtfzrdcybb.html

TS:   [...a, ...b];
来源：http://hz.chenlongwang.top/gtbkkqdvol.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinqigufen.top/gtdrtjaeta.html

Go:   append(a, b...)
来源：http://hz.ppjwa.cn/gtffqvdbis.html


<!-- 参考信息 -->