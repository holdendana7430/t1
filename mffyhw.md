代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://hz.chenjidiqi.icu/gtsojeyoyt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ydzc1.top/gtuljzahzq.html

JS:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gttqcufxeq.html

TS:   do { i++; } while (i < 10);
来源：http://hz.wangdashe.top/gtmgtcbqra.html

Java: do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtagxnnmzp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.aizwys.cn/gtbkscyabr.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.tanke756.top/gttrdkwogi.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtqxvwgqmc.html

[B09] break 与 continue
来源：http://hz.vqdsnc.cn/gtdisejdup.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.mhx1999.top/gtudizjdaq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj202588.top/gtlywmrqsg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jianghu66.top/gteojoxhfi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gthxggtmvr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jianghu66.top/gtesycuouu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hnxiangtu.top/gtfleuwoso.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinyuanbaomall.cn/gtldraxkxh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gthxfpmlyd.html

[B10] 遍历同时拿索引
来源：http://hz.yj20258888.top/gtoztcqkcf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shanyushiyangtech.top/gtmrqhfqys.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.quarkkingdee.top/gtugqvqdge.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.cdnleiting.top/gtumgtzqxs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.tanke756.top/gtilvxuqxu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.quarkkingdee.top/gtdfwhgywg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhiwuduotai.top/gtavcuekbk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yvedp.cn/gtbgschkqb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.havefunace.top/gtevuptxlz.html

[B11] 生成数字序列 / 区间
来源：http://hz.nwbrower.top/gtleldmugj.html

Py:   list(range(0, 10, 2))
来源：http://hz.nanxinkj.top/gteqeqxfip.html

PHP:  range(0, 10, 2);
来源：http://hz.ywan-chungtsiang.top/gtaqqmqsqj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.feifeiyinyue.top/gtpfklfbed.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cdnleiting.top/gtnsyntcnf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ywan-chungtsiang.top/gtqmyeuphh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xuanzx.com/gtfmgktdja.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhoulong.xyz/gtfggjaoob.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.havefunace.top/gtdbdepnac.html

[B12] 跳出多层循环
来源：http://hz.zycfv.cn/gtcwgrkfwk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yuanzhike.top/gtqobgklee.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shuidangran.top/gtlvxsiuxc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pycfn.com/gtrpxwjjel.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zycfv.cn/gtywrfaotb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtlycjqnnf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yangfankeji.com/gtldygqnva.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jinyuanbaomall.cn/gtphadshgi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.haohaochexian.top/gtnraxfyfi.html

[B13] 判断是否为数字
来源：http://hz.hysaishi.cn/gtnaccravi.html

Py:   isinstance(x, (int, float))
来源：http://hz.shanyushiyangkeji.top/gtwaembgas.html

PHP:  is_numeric($x)
来源：http://hz.redwolf501.top/gtxxfrgbek.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.9152youxi.cn/gtqjpjicjb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tian-w.cn/gtdfntnexp.html

Java: x instanceof Number
来源：http://hz.yuxming.cn/gthbhsaszl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.fzhhl.top/gtzhawrccq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.aizwys.cn/gtkyjyfmfv.html

C#:   x is int or double or decimal
来源：http://hz.feifeiyinyue.top/gthcrosgew.html

[B14] 判断值是否在集合内
来源：http://hz.yonumen.top/gtkdxatsxm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cheryme.top/gtbouwuyrm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.daxiang520.top/gtjursqhwb.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hnxiangtu.top/gtpdbjwtfy.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.iojbl.cn/gtpoidupyb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sysykeji.top/gtuhytwdqp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sysykeji.top/gtjxrsovlg.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shzxlz.cn/gtayxbasny.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cucudq.cn/gtjoaggqdd.html

[B15] 布尔运算与取反
来源：http://hz.yonumen.top/gtoquleaul.html

Py:   a and b or not c
来源：http://hz.xingfuxueyuan.xyz/gtebvptsse.html

PHP:  $a && $b || !$c
来源：http://hz.9152youxi.cn/gtcdtzqhzx.html

JS:   a && b || !c
来源：http://hz.aibaodan.cn/gtharhhtzy.html

TS:   a && b || !c
来源：http://hz.iojbl.cn/gtqxvgqhjj.html

Java: a && b || !c
来源：http://hz.kuanghao11.cn/gtmotolqyk.html

Go:   a && b || !c
来源：http://hz.guannengcc.top/gtbynxudwk.html

Ruby: a && b || !c
来源：http://hz.fengsongda.top/gtwjkegkjn.html

C#:   a && b || !c
来源：http://hz.hammf.cn/gtazfwsafg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhijiandao.cn/gtttzsgfkq.html

Py:   if not data: return
来源：http://hz.tian-w.cn/gtviggxkru.html

PHP:  if (!$data) { return; }
来源：http://hz.yanxiufei.cn/gtumkugvgy.html

JS:   if (!data) return;
来源：http://hz.pycfn.com/gtsxodjrcc.html

TS:   if (!data) return;
来源：http://hz.jiagoushi.top/gtszopadql.html

Java: if (data == null) return;
来源：http://hz.meibo888.top/gtqlhsbuko.html

Go:   if data == nil { return }
来源：http://hz.jiagoushi.top/gtzwzfjwaz.html

Ruby: return if data.nil?
来源：http://hz.xuetiantiany.cn/gtyaflpxlx.html

C#:   if (data == null) return;
来源：http://hz.tianlin.xyz/gtrgocqmjb.html

================================================================================
来源：http://hz.daria6918.cn/gtwdaqsvju.html

C. 函数与作用域
来源：http://hz.zhoulong.xyz/gtukttwglf.html

================================================================================
来源：http://hz.aibaodan.cn/gtxgqgvhtf.html

[C01] 定义函数
来源：http://hz.quarkkingdee.top/gtzawxwgjs.html

Py:   def add(a, b): return a + b
来源：http://hz.aizwys.cn/gtnqkspgsz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gtdmixivue.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtfrxxyffp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tian-w.cn/gtssmbbpfi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtxsgfpzbv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.kuanghao11.cn/gtnjhnaojh.html

Ruby: def add(a, b); a + b; end
来源：http://hz.dianchejie.cn/gtyhjngqvi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.iojbl.cn/gtforkxsed.html

[C02] 默认参数
来源：http://hz.xylfe.cn/gtkuvyfdbk.html

Py:   def greet(name="World"): return name
来源：http://hz.gogol.net.cn/gtzlramgig.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fengsongda.top/gtaukfwtzf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.fengsongda.top/gtzgmmjozb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.c1oappe.top/gtsqgwitcz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hysaishi.cn/gtgtkhtceu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hysaishi.cn/gtndhhxmsm.html

Ruby: def greet(name = "World") = name
来源：http://hz.guannengcc.top/gtwfnpsddt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ehwqpu.com/gtokhdoztj.html

[C03] 可变参数
来源：http://hz.zhixingplan.top/gtczootlqi.html

Py:   def total(*args): return sum(args)
来源：http://hz.xuanzx.com/gthpomqabf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yanxiufei.cn/gtqqqeeerf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dashuyun.cn/gtdtyplssj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinyuanbaomall.cn/gthpfjioqi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.aizwys.cn/gtvailuino.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shanyushiyangkeji.top/gtbxzoagpe.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gogol.net.cn/gtmjwagler.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.redwolf501.top/gtypzadbkf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuanzhike.top/gtkvkbeoos.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xuetiantiany.cn/gtskcbngqk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj202588.top/gtxtmvshtc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gteurrynaw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.vqdsnc.cn/gtapchhvfy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jlsjyb.cn/gtswmagffj.html

Go:   // 无：用配置结构体参数
来源：http://hz.chenlongwang.top/gtypkelwup.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtcqfrtypu.html

C#:   f(a: 1, b: 2)
来源：http://hz.cucudq.cn/gtzpwgwagw.html

[C05] 返回多个值
来源：http://hz.zhengqikj.top/gthwsfkser.html

Py:   return a, b
来源：http://hz.gotoacloud.top/gtyzjtzfov.html

PHP:  return [$a, $b];
来源：http://hz.yanxiufei.cn/gtwnkvunsl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.smart0.xyz/gtpzamvayr.html

TS:   return { a, b };
来源：http://hz.gotoacloud.top/gtrhkzsbsl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangkeji.top/gtbghqjyaw.html

Go:   return a, b
来源：http://hz.9152youxi.cn/gtfltifqsq.html

Ruby: return a, b
来源：http://hz.dianchejie.cn/gtgtccbpwq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.birdmap.top/gtdibeweir.html

[C06] 匿名函数 / lambda
来源：http://hz.hfpthk.cn/gtbdyhojro.html

Py:   square = lambda x: x * x
来源：http://hz.yueranfly.top/gtcikzrgxm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ybcxt.top/gtgkqbenqh.html

JS:   const square = x => x * x;
来源：http://hz.chenlongwang.top/gtipbniyaq.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinqigfzy.top/gttowejyud.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenzaomai.com/gtusotdcna.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yj202588.top/gtpvtjjndr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.fzhhl.top/gtxwqipuuh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yanxiufei.cn/gttjiwkedt.html

[C07] 把函数作为参数传入
来源：http://hz.xuanzx.com/gtndlqxhja.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhengqikj.top/gtqffknqpw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj202588.top/gtqycutgdh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinqigufen.top/gtnqxjjsnq.html

TS:   arr.map(String)
来源：http://hz.sweek.top/gtpxonqjbs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhengqikj.top/gtucompucm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258.top/gtifmivckv.html

Ruby: arr.map(&:upcase)
来源：http://hz.yueranfly.top/gtwglbopfa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.smart0.xyz/gtqkaiqxkk.html

[C08] 闭包
来源：http://hz.zhixingplan.top/gtyhxqwqjs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cashguo.top/gtnrnbgqye.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenzaomai.com/gteaovdhuu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gtybgsmcng.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gtqkkdzaty.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.dashuyun.cn/gtvrbimfns.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.quarkkingdee.top/gtaueakhqu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cheryme.top/gtspwdotzj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtjdrghbqk.html

[C09] 递归
来源：http://hz.vqdsnc.cn/gtwmybzrsi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenlongwang.top/gtcwyvdkzo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gogol.net.cn/gtoqkrtoni.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jlsjyb.cn/gtjnrwweus.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinyuanbaomall.cn/gtldmwxcgm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yanxiufei.cn/gtvuukdaar.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jianghu66.top/gtsuhiflkq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shzxlz.cn/gttewsqkvo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gaohongyu789.top/gtfbzfgyfu.html

[C10] 变量作用域
来源：http://hz.tanke756.top/gtrbemnwij.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.9152youxi.cn/gtyhyqpoom.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shanyushiyangtech.top/gtyvdfgppe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yj20258.top/gtarppdlbd.html

TS:   同 JS
来源：http://hz.yj202588.top/gtipwdviuv.html

Java: 方法内为块级作用域
来源：http://hz.nwbrower.top/gtrtyowxeq.html

Go:   花括号块级作用域
来源：http://hz.hfpthk.cn/gtciwzwfbe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hfpthk.cn/gtkoqxgsdn.html

C#:   块级作用域
来源：http://hz.jinqigfzy.top/gthhubnpfv.html

[C11] 模块导入与导出
来源：http://hz.haohaochexian.top/gtmeaqkagi.html

Py:   from module import func
来源：http://hz.jinyuanbaomall.cn/gtwcqlkyxf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jyoumei.cn/gtjvjjvqmj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnxiangtu.top/gtklzgtegz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zycfv.cn/gtcvdoemqa.html

Java: import java.util.List;
来源：http://hz.havefunace.top/gtatftjyls.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.52xcode.cn/gtmhxerwff.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.birdmap.top/gtqqvpujtq.html

C#:   using System.Text;
来源：http://hz.nanxuanxn.top/gtdymxgjpb.html

[C12] 立即执行函数 IIFE
来源：http://hz.nwbrower.top/gtjrwybtkz.html

Py:   (lambda: print("run"))()
来源：http://hz.jinqigufen.top/gtcyvlzqeg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jqgfzy.top/gtmcbjmqdr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtnnagrexb.html

TS:   (() => { console.log("run"); })();
来源：http://hz.0kj1m.cn/gtmugurnce.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.aibaodan.cn/gtqfjmkpcr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.andypj.xyz/gtrerddzna.html

Ruby: -> { puts "run" }.call
来源：http://hz.pycfn.com/gttqwaqysj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yongpay.top/gtajxguecu.html

[C13] 类型声明 / 类型注解
来源：http://hz.316326.xyz/gtqehekcfk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hnxiangtu.top/gtxabppjyp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.iojbl.cn/gtwcftsswk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ybcxt.top/gtqsshaltm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zycfv.cn/gtkfumnhmt.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtkckkbaos.html

Go:   func add(a, b int) int
来源：http://hz.meibo888.top/gtfbpduicb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.52xcode.cn/gtgemncgho.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydzc1.top/gtvhyrxbay.html

[C14] 泛型函数
来源：http://hz.vqdsnc.cn/gtoatbpmnc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yangfankeji.com/gtspfseunl.html

PHP:  // 无泛型
来源：http://hz.gogol.net.cn/gtxahnjuus.html

JS:   // 无泛型
来源：http://hz.jianghu66.top/gttpmeawhe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shuidangran.top/gttkaiinof.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.haohaochexian.top/gtbnqsmwwq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hongshengwenyu.top/gtcpdweqab.html

Ruby: # 无泛型
来源：http://hz.yvedp.cn/gttnstwqem.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj20258.top/gtjgdipdtd.html

[C15] 解构 / 展开参数
来源：http://hz.pycfn.com/gtbpcyciyw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigufen.top/gtwqllfctj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.snrcjt.cn/gtjnksmqqw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.fzhhl.top/gtcbmfkcxg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinqigufen.top/gtrlsrotmd.html

Java: // 无解构
来源：http://hz.iojbl.cn/gtdizehoae.html

Go:   // 无解构
来源：http://hz.cucudq.cn/gtoltsolyg.html

Ruby: a, b = pair
来源：http://hz.cheryme.top/gtxbeltcta.html

C#:   var (a, b) = pair;
来源：http://hz.guannengcc.top/gtjrvhkeab.html

[C16] 函数 / 方法重载
来源：http://hz.aibaodan.cn/gtgyhseclt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenzaomai.com/gtcqqgaxnv.html

PHP:  // 无重载
来源：http://hz.svipenyu.cn/gtsxyjnurl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yuanzhike.top/gtgggugtdv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinghuilouyu.cn/gtytsdvvzr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sufxvd.cn/gtcwvunrwo.html

Go:   // 无重载：用不同函数名
来源：http://hz.yuanzhike.top/gtfmgissfg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuxming.cn/gtbhwigdhv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhijiandao.cn/gtowhrndnd.html

================================================================================
来源：http://hz.havefunace.top/gtaglgfocm.html

D. 数组 / 列表 / 集合
来源：http://hz.hongshengwenyu.top/gtpszsxlzq.html

================================================================================
来源：http://hz.dianchejie.cn/gtaajcjmkz.html

[D01] 创建数组 / 列表
来源：http://hz.xinyue.icu/gtnouvchaq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jianghu66.top/gtirlswwzd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.feifeiyinyue.top/gtmnbmjmqr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guannengcc.top/gtvjroogqn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258.top/gthckzjldg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zycfv.cn/gtfmpxibnt.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xinyue.icu/gtirizyuav.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhaomingkeji.xyz/gtowxlcdyq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhengqikj.top/gtixgbvcfj.html

[D02] 追加元素到末尾
来源：http://hz.daxiang520.top/gtujopmfpj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shanyushiyangkeji.top/gtiqixfomb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yj202588.top/gtizrucmuy.html

JS:   arr.push(4);
来源：http://hz.0kj1m.cn/gtsgzurwwl.html

TS:   arr.push(4);
来源：http://hz.ehwqpu.com/gtrznzhrdr.html

Java: list.add(4);
来源：http://hz.xinyue.icu/gtowvrhdbt.html

Go:   arr = append(arr, 4)
来源：http://hz.snrcjt.cn/gtjkmesndn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhoulong.xyz/gtedriqyws.html

C#:   list.Add(4);
来源：http://hz.guowangkeji.top/gthatvjsxy.html

[D03] 在指定位置插入元素
来源：http://hz.zhijiandao.cn/gtvyqmrjtw.html

Py:   arr.insert(0, 0)
来源：http://hz.wangdashe.top/gtwjrirbau.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shuidangran.top/gtqhvwxscs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hysaishi.cn/gtthamienm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shuidangran.top/gtwimryuja.html

Java: list.add(0, 0);
来源：http://hz.daxiang520.top/gtiskxbomn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.0kj1m.cn/gtsinmkchk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinqigufen.top/gtqsvqkwty.html

C#:   list.Insert(0, 0);
来源：http://hz.guannengcc.top/gtbjjxhnzf.html

[D04] 删除元素
来源：http://hz.yongpay.top/gtzodjolvx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cucudq.cn/gtekisagap.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zycfv.cn/gtlpvvglqb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sweek.top/gtmmhvtjro.html

TS:   arr.splice(0, 1);
来源：http://hz.hnqzz.top/gteguadaws.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ivvv.top/gttrtzzqba.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hammf.cn/gtqqwobsxf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangtech.top/gtegzzbeqs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tianlin.xyz/gtmkrsaqil.html

[D05] 访问与修改元素
来源：http://hz.yj20258.top/gtuyuexzom.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtrzmivnco.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.0kj1m.cn/gtpbzuffyc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.kuanghao11.cn/gtupwttxwd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangkeji.top/gttxfflkht.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hnxiangtu.top/gtyekocimb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtckdwsewx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guannengcc.top/gtpzzmtjic.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hnqzz.top/gtsufadybu.html

[D06] 数组长度
来源：http://hz.yanxiufei.cn/gtchfepjpo.html

Py:   len(arr)
来源：http://hz.sxryk.cn/gtxmylrwku.html

PHP:  count($arr);
来源：http://hz.sxryk.cn/gtxtjwxqxs.html

JS:   arr.length
来源：http://hz.52xcode.cn/gtzqqgahxy.html

TS:   arr.length
来源：http://hz.dashuyun.cn/gtblpgrkye.html

Java: list.size();
来源：http://hz.feifeiyinyue.top/gtcyauhrxg.html

Go:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gtuoprqvau.html

Ruby: arr.length; arr.size
来源：http://hz.ywan-chungtsiang.top/gtqvhhiiik.html

C#:   list.Count;
来源：http://hz.feifeiyinyue.top/gtztjbnhie.html

[D07] 切片 / 取子数组
来源：http://hz.sysykeji.top/gtfzksngmp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hammf.cn/gtvsiaroto.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtgayvujlq.html

JS:   arr.slice(1, 4);
来源：http://hz.zhijiandao.cn/gtnfaskvoa.html

TS:   arr.slice(1, 4);
来源：http://hz.chenlongwang.top/gtahzbciin.html

Java: list.subList(1, 4);
来源：http://hz.fengsongda.top/gtckjslaxm.html

Go:   arr[1:4]
来源：http://hz.quarkkingdee.top/gtwwjoerai.html

Ruby: arr[1, 3]
来源：http://hz.yj20258888.top/gtaygkksig.html

C#:   list.GetRange(1, 3);
来源：http://hz.9152youxi.cn/gtyfouxznr.html

[D08] 合并两个数组
来源：http://hz.feifeiyinyue.top/gtsvppjxqb.html

Py:   a + b;  a.extend(b)
来源：http://hz.cucudq.cn/gtwosroqwn.html

PHP:  array_merge($a, $b);
来源：http://hz.redwolf501.top/gthnxxbrmc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cashguo.top/gtfrllqkov.html

TS:   [...a, ...b];
来源：http://hz.wangshuangyany.cn/gtyefhifyp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jiagoushi.top/gtasyexnht.html

Go:   append(a, b...)
来源：http://hz.ybcxt.top/gtxbtgwkxw.html


<!-- 参考信息 -->