代发 wailian999

[B09] break 与 continue
来源：http://hz.pengpengdd.cyou/gtvihxcoww.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zhijiandao.cn/gtemkdqcpr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hfpthk.cn/gtxiijzvob.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhengqikj.top/gtuguohjic.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gtdozrbrqh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhengqikj.top/gtsnnhxgdr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhiwuduotai.top/gtacredztd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.andypj.xyz/gtymhksqjp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxuanxn.top/gtmdehixxo.html

[B10] 遍历同时拿索引
来源：http://hz.ybcxt.top/gtgkvojckd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.316326.xyz/gtejqwhoow.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.kuanghao11.cn/gtlfteybsi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.tianlin.xyz/gtfcbghpon.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jinqigfzy.top/gtrzjgqmgs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ivvv.top/gtehfbcwwl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xylfe.cn/gtlhxgapng.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sysykeji.top/gtqdlxymvq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.quarkkingdee.top/gtcccjuzgh.html

[B11] 生成数字序列 / 区间
来源：http://hz.52xcode.cn/gtokzsbzas.html

Py:   list(range(0, 10, 2))
来源：http://hz.svipenyu.cn/gtcvqmaujq.html

PHP:  range(0, 10, 2);
来源：http://hz.daria6918.cn/gtzturffhb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yongpay.top/gtrmhnhnlr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dianchejie.cn/gtpymecool.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhoulong.xyz/gtjospvpmz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.tianlin.xyz/gtgqgmnqkd.html

Ruby: (0...10).step(2).to_a
来源：http://hz.smart0.xyz/gtiotdwewh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.redwolf501.top/gtssmwralf.html

[B12] 跳出多层循环
来源：http://hz.ywan-chungtsiang.top/gtzslxgapc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhaomingkeji.xyz/gtouhnybst.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.birdmap.top/gtedsdtzrq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ybcxt.top/gtmoqrsujg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daxiang520.top/gtsndlejfv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtlwrubxcn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jinghuilouyu.cn/gtniyfrrhi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sufxvd.cn/gtpxxmcpqm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.feifeiyinyue.top/gtqxhmpfcv.html

[B13] 判断是否为数字
来源：http://hz.cheryme.top/gtlhrxjhtw.html

Py:   isinstance(x, (int, float))
来源：http://hz.jqgufenzy.top/gtokefwbap.html

PHP:  is_numeric($x)
来源：http://hz.yuanzhike.top/gtgoiujwqa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhaomingkeji.xyz/gtynvazzwr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sufxvd.cn/gtemlnhoic.html

Java: x instanceof Number
来源：http://hz.jinghuilouyu.cn/gtvvpsckex.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ybcxt.top/gtctbmikpz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.tian-w.cn/gtumdgkhzw.html

C#:   x is int or double or decimal
来源：http://hz.jlsjyb.cn/gtabxtjjbe.html

[B14] 判断值是否在集合内
来源：http://hz.hongshengwenyu.top/gtclkfshxs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yueranfly.top/gtaocqnecb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xziqi.cn/gtfqslkldz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xinyue.icu/gtsgrlrmce.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.smart0.xyz/gtdfptqtft.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhoulong.xyz/gthzviqpat.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.quarkkingdee.top/gttuhwvook.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.9152youxi.cn/gtofaqnpus.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenzaomai.com/gtbhkqlphy.html

[B15] 布尔运算与取反
来源：http://hz.sweek.top/gtmymgqbdc.html

Py:   a and b or not c
来源：http://hz.jqgufenzy.top/gtiwjmgybv.html

PHP:  $a && $b || !$c
来源：http://hz.zhaomingkeji.xyz/gtrwyeijfn.html

JS:   a && b || !c
来源：http://hz.fengsongda.top/gtxxspxltt.html

TS:   a && b || !c
来源：http://hz.jqgfzy.top/gtehfkltky.html

Java: a && b || !c
来源：http://hz.yongpay.top/gtsuozemme.html

Go:   a && b || !c
来源：http://hz.sufxvd.cn/gtxwxjktgr.html

Ruby: a && b || !c
来源：http://hz.yuxming.cn/gtcrbdmbrq.html

C#:   a && b || !c
来源：http://hz.sxryk.cn/gtjjrhckzh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.dashuyun.cn/gtzhqxmant.html

Py:   if not data: return
来源：http://hz.sufxvd.cn/gtlpiowswr.html

PHP:  if (!$data) { return; }
来源：http://hz.hnxiangtu.top/gtyoafubxp.html

JS:   if (!data) return;
来源：http://hz.gogol.net.cn/gtvudbxyrf.html

TS:   if (!data) return;
来源：http://hz.yangfankeji.com/gtyzlwwxhr.html

Java: if (data == null) return;
来源：http://hz.shanyushiyangtech.top/gtbyeqhczk.html

Go:   if data == nil { return }
来源：http://hz.daria6918.cn/gtqoafznfa.html

Ruby: return if data.nil?
来源：http://hz.fzhhl.top/gtlwohjsgk.html

C#:   if (data == null) return;
来源：http://hz.redwolf501.top/gtudcysqzt.html

================================================================================
来源：http://hz.daria6918.cn/gtugvuvfkj.html

C. 函数与作用域
来源：http://hz.cheryme.top/gtecxsdssg.html

================================================================================
来源：http://hz.ehwqpu.com/gtxrlfqzpw.html

[C01] 定义函数
来源：http://hz.hfpthk.cn/gtpoudpllu.html

Py:   def add(a, b): return a + b
来源：http://hz.shanyushiyangtech.top/gtguiqogzc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gtiafhinni.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.wangdashe.top/gtffyvbmxy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenlongwang.top/gtalyqgdoq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtxuoybmgl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daria6918.cn/gtgybmuwwg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tanke756.top/gtfjuwoopk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gtqcwincyw.html

[C02] 默认参数
来源：http://hz.jlsjyb.cn/gtghljwmtm.html

Py:   def greet(name="World"): return name
来源：http://hz.ydjk.org.cn/gteyifohmt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yvedp.cn/gtjijqkjxu.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ehwqpu.com/gtexoqdvxp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgufenzy.top/gtbyhsltnz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tianlin.xyz/gtudxhiyas.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sweek.top/gtgmovfgoj.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhengqikj.top/gttykzxylf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sweek.top/gtmdlgkfzb.html

[C03] 可变参数
来源：http://hz.52xcode.cn/gtkodmnqay.html

Py:   def total(*args): return sum(args)
来源：http://hz.hysaishi.cn/gtyuxciwhb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhijiandao.cn/gtinntercx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ybcxt.top/gtemawquzf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dashuyun.cn/gtrduhnznr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ppjwa.cn/gtoladnnak.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.daxiang520.top/gtuglwdukc.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.bjfxy.top/gtamyrzihq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhaomingkeji.xyz/gtikojuzzd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xuanzx.com/gtupkfnvrg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhiwuduotai.top/gtbarjeydy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.pycfn.com/gtmctwsihw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.316326.xyz/gtxkxmvgrk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gzhubu.top/gtwztbdwny.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenzaomai.com/gtjfcqzqjb.html

Go:   // 无：用配置结构体参数
来源：http://hz.meibo888.top/gtctiealzp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gthskxjyti.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtmpdhdijv.html

[C05] 返回多个值
来源：http://hz.hnqzz.top/gtgwaphmtt.html

Py:   return a, b
来源：http://hz.jinqigufen.top/gtusjvmbqe.html

PHP:  return [$a, $b];
来源：http://hz.316326.xyz/gtxgistohr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.daria6918.cn/gtahqjjuyf.html

TS:   return { a, b };
来源：http://hz.quarkkingdee.top/gtqmoxxvjp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.smart0.xyz/gtvisclujs.html

Go:   return a, b
来源：http://hz.snrcjt.cn/gtbvttzsjq.html

Ruby: return a, b
来源：http://hz.yuanzhike.top/gtjzlnbfcp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhijiandao.cn/gtnywcqtce.html

[C06] 匿名函数 / lambda
来源：http://hz.aizwys.cn/gtzhieiygf.html

Py:   square = lambda x: x * x
来源：http://hz.xuanzx.com/gtctlcfmrg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shangyingyoupin.top/gtadkmzdlv.html

JS:   const square = x => x * x;
来源：http://hz.fengsongda.top/gtilqvvgao.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xylfe.cn/gtycyklhbn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.haohaochexian.top/gttwsjvtds.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tanke756.top/gtrlbjpwkj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.quarkkingdee.top/gtsnyqpgin.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuanzx.com/gtkqsecaal.html

[C07] 把函数作为参数传入
来源：http://hz.hywenlv.cn/gtmaisozdq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jqgfzy.top/gtsvaqewje.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhaomingkeji.xyz/gtmoyvmjlo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shzxlz.cn/gtifwpfztk.html

TS:   arr.map(String)
来源：http://hz.yuxming.cn/gtpyebpill.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tanke756.top/gtfbcdtolj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.svipenyu.cn/gthmggfvoy.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxuanxn.top/gtokhnrvqz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.nwbrower.top/gtxugmjsps.html

[C08] 闭包
来源：http://hz.9152youxi.cn/gtmuztghtl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yueranfly.top/gtnrguixsy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhijiandao.cn/gtpwhtqbyj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinyuanbaomall.cn/gtixqupzio.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtzclsdiai.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gogol.net.cn/gtwzagxdfn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shanyushiyangkeji.top/gttrhjskom.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shzxlz.cn/gtflxgolgr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtodiwwlgh.html

[C09] 递归
来源：http://hz.fzhhl.top/gtrpxoauev.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cheryme.top/gtwfxkzuuk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jianghu66.top/gtkfysftbh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinyuanbaomall.cn/gtruhnrfvd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgfzy.top/gtmipdhyjb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ydjk.org.cn/gtfqgdbiwi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yanxiufei.cn/gtxyidnnic.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtfugcodvj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zdqjudy.top/gtjvtjpvip.html

[C10] 变量作用域
来源：http://hz.hnqzz.top/gtdhcuvafp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cashguo.top/gtwuvlvnua.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yangfankeji.com/gthetjgkry.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhaomingkeji.xyz/gtolmtxlxq.html

TS:   同 JS
来源：http://hz.pycfn.com/gtxtcvplvc.html

Java: 方法内为块级作用域
来源：http://hz.zhixingplan.top/gtwkxawyhm.html

Go:   花括号块级作用域
来源：http://hz.dashuyun.cn/gtlkyhrdsv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.316326.xyz/gtfbnmovvt.html

C#:   块级作用域
来源：http://hz.tian-w.cn/gtgmjzyzfw.html

[C11] 模块导入与导出
来源：http://hz.havefunace.top/gtgtykftzb.html

Py:   from module import func
来源：http://hz.yueranfly.top/gtmxiujssh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.meibo888.top/gtpamolrzw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ydjk.org.cn/gtvanglsam.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yangfankeji.com/gtutybkjhl.html

Java: import java.util.List;
来源：http://hz.cashguo.top/gtkkfuamyq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.havefunace.top/gtzohyyjvh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.52xcode.cn/gtjrrvdvqf.html

C#:   using System.Text;
来源：http://hz.chenlongwang.top/gthioazuyk.html

[C12] 立即执行函数 IIFE
来源：http://hz.shangyingyoupin.top/gtyfzdtoph.html

Py:   (lambda: print("run"))()
来源：http://hz.zhongyouzk.top/gtxzmqnwao.html

PHP:  (function () { echo "run"; })();
来源：http://hz.chenlongwang.top/gtubvaaigt.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yonumen.top/gtwbyvxtft.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cqqwz.cn/gtynvqywns.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.316326.xyz/gteqqwzjix.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sysykeji.top/gttpzlinff.html

Ruby: -> { puts "run" }.call
来源：http://hz.yangfankeji.com/gtybkmgfeo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.mhx1999.top/gtknrvzesa.html

[C13] 类型声明 / 类型注解
来源：http://hz.sysykeji.top/gtibukcrjh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jyoumei.cn/gtrgwdnrsa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgfzy.top/gtkzsdtsko.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jyoumei.cn/gtlkgxdvlt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtzsbnyxub.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtcxnbzsli.html

Go:   func add(a, b int) int
来源：http://hz.hnqzz.top/gtpchhgifn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hammf.cn/gtyqejnsgu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xuanzx.com/gtmavhybnr.html

[C14] 泛型函数
来源：http://hz.yj20258888.top/gtdygnnyxs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.andypj.xyz/gtvvqmifhv.html

PHP:  // 无泛型
来源：http://hz.zycfv.cn/gtaoweszrt.html

JS:   // 无泛型
来源：http://hz.feifeiyinyue.top/gtcwqwwdrq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tianlin.xyz/gtchjcwwif.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yueranfly.top/gtjsgleeqk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.fengsongda.top/gtwmfnvnwl.html

Ruby: # 无泛型
来源：http://hz.birdmap.top/gtaulvrkom.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aizwys.cn/gtzgsmolbg.html

[C15] 解构 / 展开参数
来源：http://hz.guowangkeji.top/gtkfbmithu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.daxiang520.top/gtlajepxhb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yueranfly.top/gtlovtprhs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtpousxkla.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zycfv.cn/gtapniltov.html

Java: // 无解构
来源：http://hz.shuidangran.top/gthniebuau.html

Go:   // 无解构
来源：http://hz.xylfe.cn/gtjchpqegi.html

Ruby: a, b = pair
来源：http://hz.guannengcc.top/gtkvkeygpf.html

C#:   var (a, b) = pair;
来源：http://hz.jiagoushi.top/gtcxtzphyx.html

[C16] 函数 / 方法重载
来源：http://hz.tianlin.xyz/gtyrccoxof.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xuetiantiany.cn/gtuafmqgwr.html

PHP:  // 无重载
来源：http://hz.pycfn.com/gtfasoavty.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.daxiang520.top/gtzxsvviwq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cashguo.top/gteivxtfof.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.guowangkeji.top/gthptazqmt.html

Go:   // 无重载：用不同函数名
来源：http://hz.jiagoushi.top/gtapcglokp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.9152youxi.cn/gthnxenvua.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.dashuyun.cn/gtmybnhpgh.html

================================================================================
来源：http://hz.cqqwz.cn/gtjyftnvyv.html

D. 数组 / 列表 / 集合
来源：http://hz.hnxiangtu.top/gthuknymfq.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtipsugpaz.html

[D01] 创建数组 / 列表
来源：http://hz.gogol.net.cn/gtiqitstzc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zycfv.cn/gtuzrmldba.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinyuanbaomall.cn/gtsimocusy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xziqi.cn/gtasivvgrc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yueranfly.top/gtrtmkfgzd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.smart0.xyz/gtqkajbgmu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.kuanghao11.cn/gtqfrnqgoa.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenlongwang.top/gthqgsgsov.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.feifeiyinyue.top/gtbcufpdkw.html

[D02] 追加元素到末尾
来源：http://hz.sweek.top/gtlepqqcct.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhengqikj.top/gtduuqobss.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fzhhl.top/gtoucgzpsb.html

JS:   arr.push(4);
来源：http://hz.hywenlv.cn/gtnqshajqf.html

TS:   arr.push(4);
来源：http://hz.shzxlz.cn/gtpvmznasb.html

Java: list.add(4);
来源：http://hz.316326.xyz/gtzlrzxhsr.html

Go:   arr = append(arr, 4)
来源：http://hz.guowangkeji.top/gttniwevsl.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.havefunace.top/gtmdkxzgna.html

C#:   list.Add(4);
来源：http://hz.tanke756.top/gtqhfjzngu.html

[D03] 在指定位置插入元素
来源：http://hz.kuanghao11.cn/gtqlxftmjo.html

Py:   arr.insert(0, 0)
来源：http://hz.316326.xyz/gtgyshwmwa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenzaomai.com/gtacmmlhlm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gotoacloud.top/gtolhcjrwi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.iojbl.cn/gtpznsipye.html

Java: list.add(0, 0);
来源：http://hz.hammf.cn/gtfuctlhnu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shanyushiyangtech.top/gtvazqxnyj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nanxinkj.top/gtgqccnysl.html

C#:   list.Insert(0, 0);
来源：http://hz.redwolf501.top/gtlfaeolai.html

[D04] 删除元素
来源：http://hz.zhoulong.xyz/gtnqnyatsc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydjk.org.cn/gtkohzujyo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sxryk.cn/gtgpjakqep.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zycfv.cn/gtlbamxurv.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigufen.top/gtfottzkvt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.feifeiyinyue.top/gtitdhtkot.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shangyingyoupin.top/gtjepjxtty.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cdnleiting.top/gtbmqnpmkh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hywenlv.cn/gtfizejsjr.html

[D05] 访问与修改元素
来源：http://hz.xuetiantiany.cn/gtxlshvsul.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtupdlpzal.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.haohaochexian.top/gttrvvajfl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.pycfn.com/gtttsorhzj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xingfuxueyuan.xyz/gtbfpuofpd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhiwuduotai.top/gtpcshukbw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yongpay.top/gtfqfbjuiu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtblesvdlb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangshuangyany.cn/gttgpqflwo.html

[D06] 数组长度
来源：http://hz.yvedp.cn/gtlkobinyd.html

Py:   len(arr)
来源：http://hz.jqgufenzy.top/gtjucrfwrs.html

PHP:  count($arr);
来源：http://hz.zdqjudy.top/gtyubwvtqq.html

JS:   arr.length
来源：http://hz.hnqzz.top/gtdzfjqdoh.html

TS:   arr.length
来源：http://hz.fengsongda.top/gtyzcenkbk.html

Java: list.size();
来源：http://hz.yuxming.cn/gtlpcaacqh.html

Go:   len(arr)
来源：http://hz.ivvv.top/gtitpoocme.html

Ruby: arr.length; arr.size
来源：http://hz.316326.xyz/gtgeykxyex.html

C#:   list.Count;
来源：http://hz.aizwys.cn/gtkdrbroxq.html

[D07] 切片 / 取子数组
来源：http://hz.sysykeji.top/gtvgawukiq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yuxming.cn/gtntqocnbj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yuanzhike.top/gtjtualqcb.html

JS:   arr.slice(1, 4);
来源：http://hz.zdqjudy.top/gtxfahymuj.html

TS:   arr.slice(1, 4);
来源：http://hz.jyoumei.cn/gthlwyicbb.html

Java: list.subList(1, 4);
来源：http://hz.aizwys.cn/gtmmqggykt.html

Go:   arr[1:4]
来源：http://hz.xingfuxueyuan.xyz/gtvickrnls.html

Ruby: arr[1, 3]
来源：http://hz.fengsongda.top/gttxsgpgaw.html

C#:   list.GetRange(1, 3);
来源：http://hz.aibaodan.cn/gtjwcernxb.html

[D08] 合并两个数组
来源：http://hz.jinqigfzy.top/gtarrttpcd.html

Py:   a + b;  a.extend(b)
来源：http://hz.sweek.top/gthlhyhhve.html

PHP:  array_merge($a, $b);
来源：http://hz.zhoulong.xyz/gtknjoutoz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xziqi.cn/gtgnjthpex.html

TS:   [...a, ...b];
来源：http://hz.jyoumei.cn/gtkqmmohep.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydjk.org.cn/gtqvlfvrfc.html

Go:   append(a, b...)
来源：http://hz.daria6918.cn/gteaiiizhm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jianghu66.top/gtjmhqnmez.html

C#:   a.Concat(b).ToList()
来源：http://hz.aibaodan.cn/gtehhhifjt.html

[D09] 排序（升序）
来源：http://hz.0kj1m.cn/gtvtnnnlxj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangdashe.top/gtpbbppxno.html

PHP:  sort($arr);
来源：http://hz.vqdsnc.cn/gtavklpsnq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xylfe.cn/gtxbfnkpiu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shuidangran.top/gtrlafaekc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shzxlz.cn/gtqhvfakey.html


<!-- 参考信息 -->