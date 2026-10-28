代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gtzabwzlnl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgufenzy.top/gtqjmwfygq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yonumen.top/gtewwsmaua.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hammf.cn/gtusesckxl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yvedp.cn/gtplcrlyfb.html

[B10] 遍历同时拿索引
来源：http://hz.zhijiandao.cn/gtdttdowrm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gzhubu.top/gtxnagzwww.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yangfankeji.com/gtpusezvmr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.nwbrower.top/gtatpwkbte.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hongshengwenyu.top/gtzcxnulnn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shzxlz.cn/gtslvxohkb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shuidangran.top/gthlwjeghz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hammf.cn/gtubjopyvr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhixingplan.top/gtybzqvswk.html

[B11] 生成数字序列 / 区间
来源：http://hz.ppjwa.cn/gtozfbikoc.html

Py:   list(range(0, 10, 2))
来源：http://hz.jqgufenzy.top/gtpysblzad.html

PHP:  range(0, 10, 2);
来源：http://hz.hongshengwenyu.top/gtqlzohbid.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuanzhike.top/gtpbzabtxi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.andypj.xyz/gtsqknbsdt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.316326.xyz/gtdqiqodvf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gaohongyu789.top/gtjxwxksjc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.tian-w.cn/gtiitrnhlq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yangfankeji.com/gtdcxaoqvs.html

[B12] 跳出多层循环
来源：http://hz.ppjwa.cn/gtglrjwtlv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhijiandao.cn/gtplgsfzqh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yvedp.cn/gtlkrvazwc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dashuyun.cn/gtrxsvvudb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtxqieyciz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtgedhfrcx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.quarkkingdee.top/gtuokyrvqi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cqqwz.cn/gtxnkpvgat.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.meibo888.top/gtuvblbgzs.html

[B13] 判断是否为数字
来源：http://hz.xylfe.cn/gtjtqlmgkw.html

Py:   isinstance(x, (int, float))
来源：http://hz.hnxiangtu.top/gtogbleebf.html

PHP:  is_numeric($x)
来源：http://hz.smart0.xyz/gthxrrlgoc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hammf.cn/gtkdsofkrv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuetiantiany.cn/gttwrtamyk.html

Java: x instanceof Number
来源：http://hz.jinqigfzy.top/gtrrusdxgy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.quarkkingdee.top/gtkncoyplp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yuxming.cn/gtkgcparpq.html

C#:   x is int or double or decimal
来源：http://hz.jinqigufen.top/gtoawjnmvg.html

[B14] 判断值是否在集合内
来源：http://hz.xinyue.icu/gtqybudwfq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.aizwys.cn/gtmxkhpiqn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.0kj1m.cn/gttuzfwvca.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hammf.cn/gtiavsyblm.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtfxjmcnoz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jyoumei.cn/gtprwunaia.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yangfankeji.com/gtsburcdzy.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhoulong.xyz/gtgjoiakrv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj20258888.top/gthgastcpq.html

[B15] 布尔运算与取反
来源：http://hz.zdqjudy.top/gtdlpauhgo.html

Py:   a and b or not c
来源：http://hz.yj20258888.top/gtfnsufdsq.html

PHP:  $a && $b || !$c
来源：http://hz.nanxuanxn.top/gtlctqhwfy.html

JS:   a && b || !c
来源：http://hz.ehwqpu.com/gtpqudazhp.html

TS:   a && b || !c
来源：http://hz.jinqigfzy.top/gtkpjdrskm.html

Java: a && b || !c
来源：http://hz.shuidangran.top/gtdcmeticr.html

Go:   a && b || !c
来源：http://hz.vqdsnc.cn/gtkkhbxdif.html

Ruby: a && b || !c
来源：http://hz.zhengqikj.top/gtxodjmrnp.html

C#:   a && b || !c
来源：http://hz.ydjk.org.cn/gtyuxkxevn.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.0kj1m.cn/gtgfrlbqoi.html

Py:   if not data: return
来源：http://hz.pycfn.com/gtablzonrv.html

PHP:  if (!$data) { return; }
来源：http://hz.havefunace.top/gtroeaiouw.html

JS:   if (!data) return;
来源：http://hz.ybcxt.top/gtrzyunwmt.html

TS:   if (!data) return;
来源：http://hz.0kj1m.cn/gthbpxwcpy.html

Java: if (data == null) return;
来源：http://hz.52xcode.cn/gtstcxuwck.html

Go:   if data == nil { return }
来源：http://hz.xuanzx.com/gthrroazux.html

Ruby: return if data.nil?
来源：http://hz.haohaochexian.top/gtqvalyndn.html

C#:   if (data == null) return;
来源：http://hz.gzhubu.top/gtcplzgelb.html

================================================================================
来源：http://hz.andypj.xyz/gtxdatbtvp.html

C. 函数与作用域
来源：http://hz.zhixingplan.top/gtjhmlccjw.html

================================================================================
来源：http://hz.sysykeji.top/gtlfwqnzsv.html

[C01] 定义函数
来源：http://hz.fengsongda.top/gtrqsoletn.html

Py:   def add(a, b): return a + b
来源：http://hz.jinqigufen.top/gtjvirbhqv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtmuqcsqdt.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xuanzx.com/gtqxselvpi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xylfe.cn/gtlfvypvan.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtninqrwgl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhengqikj.top/gtclnxcabf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hnqzz.top/gtlgxedzqj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtcvhqupwo.html

[C02] 默认参数
来源：http://hz.haohaochexian.top/gtxkurfffq.html

Py:   def greet(name="World"): return name
来源：http://hz.hnqzz.top/gtiyzjsmsu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhaomingkeji.xyz/gtnfprchab.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtcxxxavop.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aizwys.cn/gtkpopzgux.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ybcxt.top/gtehkxwzvc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sysykeji.top/gtuovldqtw.html

Ruby: def greet(name = "World") = name
来源：http://hz.shuidangran.top/gtmtrlmzbu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ywan-chungtsiang.top/gtepmphmpr.html

[C03] 可变参数
来源：http://hz.wangshuangyany.cn/gtccedchnx.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenjidiqi.icu/gtlvvzywrt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shangyingyoupin.top/gtsqufawwl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zdqjudy.top/gtkgfuiuvo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xziqi.cn/gtaejcgpem.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yanxiufei.cn/gtvylmodzg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhixingplan.top/gtfeonshia.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jlsjyb.cn/gtxqionwbb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.havefunace.top/gtsckzzkes.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hysaishi.cn/gtttxtzzqf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinghuilouyu.cn/gtfoozthqr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gotoacloud.top/gtfxynewgo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jqgfzy.top/gthvvaqnbi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hysaishi.cn/gtvrcvcaee.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhengqikj.top/gtujbklvev.html

Go:   // 无：用配置结构体参数
来源：http://hz.shanyushiyangkeji.top/gtgfaezgyg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yonumen.top/gtrjzzhmol.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhaomingkeji.xyz/gtmvelzonu.html

[C05] 返回多个值
来源：http://hz.jinqigufen.top/gtiduiuxdq.html

Py:   return a, b
来源：http://hz.vqdsnc.cn/gtcoqquhrp.html

PHP:  return [$a, $b];
来源：http://hz.yuxming.cn/gtlgdynvdf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zycfv.cn/gtqaynalql.html

TS:   return { a, b };
来源：http://hz.cqqwz.cn/gtwyjmeeao.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.quarkkingdee.top/gtdcezrkim.html

Go:   return a, b
来源：http://hz.316326.xyz/gtngzositb.html

Ruby: return a, b
来源：http://hz.pengpengdd.cyou/gtcjsyiptu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jlsjyb.cn/gtppooyomx.html

[C06] 匿名函数 / lambda
来源：http://hz.yangfankeji.com/gtlmfsflld.html

Py:   square = lambda x: x * x
来源：http://hz.chenzaomai.com/gtvqdwztpj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cucudq.cn/gttfcipjws.html

JS:   const square = x => x * x;
来源：http://hz.shuidangran.top/gtetreyqly.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sxryk.cn/gtrsivqdct.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cqqwz.cn/gtxexsawno.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.pycfn.com/gtnfaivitg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.gotoacloud.top/gtgczqijjd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cqqwz.cn/gtrmzzhipn.html

[C07] 把函数作为参数传入
来源：http://hz.chenzaomai.com/gthfejlcbp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xuetiantiany.cn/gtodcgtoea.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tianlin.xyz/gtpgqygdce.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhaomingkeji.xyz/gtgpgycels.html

TS:   arr.map(String)
来源：http://hz.nanxinkj.top/gtbgfdulpl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ivvv.top/gtfsafvcgr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cheryme.top/gturfsgvzo.html

Ruby: arr.map(&:upcase)
来源：http://hz.cashguo.top/gtmlykcgqu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gzhubu.top/gteruqvlkk.html

[C08] 闭包
来源：http://hz.ywan-chungtsiang.top/gtuzwtdmvf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hammf.cn/gtwzenkurv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hongshengwenyu.top/gtbiiidmbt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtxgllmjwh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinghuilouyu.cn/gtapobxfmq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.feifeiyinyue.top/gtyulwyohl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.havefunace.top/gtemfhxfhl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yueranfly.top/gtmkbensxj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtgdmexnhr.html

[C09] 递归
来源：http://hz.hongshengwenyu.top/gtfogksnxh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xinyue.icu/gtfahjobvz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tanke756.top/gturxjhicf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gtiqkjcexi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxuanxn.top/gtfcznlsvh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hammf.cn/gtbebfagmo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hywenlv.cn/gtlzkikoye.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.wangshuangyany.cn/gthrnlaxqd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ybcxt.top/gtiovorzfg.html

[C10] 变量作用域
来源：http://hz.sxryk.cn/gtheqxslkh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.redwolf501.top/gtzjilzsij.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xuanzx.com/gtysgcccoq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cucudq.cn/gtudvxjhww.html

TS:   同 JS
来源：http://hz.jinqigufen.top/gtnghuxpxo.html

Java: 方法内为块级作用域
来源：http://hz.ivvv.top/gtxgvmmbjg.html

Go:   花括号块级作用域
来源：http://hz.zhiwuduotai.top/gtrcerwpcj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nanxinkj.top/gthrywwvnt.html

C#:   块级作用域
来源：http://hz.pengpengdd.cyou/gtfcduhmlr.html

[C11] 模块导入与导出
来源：http://hz.ppjwa.cn/gtaehlwhzd.html

Py:   from module import func
来源：http://hz.nanxuanxn.top/gtrkwosxmi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhixingplan.top/gtahdiqcru.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.meibo888.top/gtgoxsrang.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.smart0.xyz/gtbqxphjfc.html

Java: import java.util.List;
来源：http://hz.jqgufenzy.top/gtxwotrldi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jiagoushi.top/gtakvhqolq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jiagoushi.top/gtvmgevwdx.html

C#:   using System.Text;
来源：http://hz.yanxiufei.cn/gtiodzzhru.html

[C12] 立即执行函数 IIFE
来源：http://hz.316326.xyz/gtkkcfiizs.html

Py:   (lambda: print("run"))()
来源：http://hz.zdqjudy.top/gtfqsedznf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigfzy.top/gtehrvlcxh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gtfegntvaj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yonumen.top/gtgclektws.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangkeji.top/gttyfmqnch.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxuanxn.top/gtvxgvvkau.html

Ruby: -> { puts "run" }.call
来源：http://hz.52xcode.cn/gtewjztzph.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zycfv.cn/gtlngysmcb.html

[C13] 类型声明 / 类型注解
来源：http://hz.0kj1m.cn/gtamxnsegh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhixingplan.top/gtdqmlmcfq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtcjeutisn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pengpengdd.cyou/gtplhidxly.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenlongwang.top/gtyaichlfq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtkkbwtafu.html

Go:   func add(a, b int) int
来源：http://hz.vqdsnc.cn/gthqmcvepi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.c1oappe.top/gtsyoqkbkj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cucudq.cn/gttnnmaici.html

[C14] 泛型函数
来源：http://hz.fzhhl.top/gtrvpcnegc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.9152youxi.cn/gtjebaglbi.html

PHP:  // 无泛型
来源：http://hz.yueranfly.top/gtoptmvslu.html

JS:   // 无泛型
来源：http://hz.havefunace.top/gtqrgdwina.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.pengpengdd.cyou/gtwelpzuqo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xylfe.cn/gtoxslxsna.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.kuanghao11.cn/gtcpuzrkbd.html

Ruby: # 无泛型
来源：http://hz.9152youxi.cn/gtuaajrgmr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tian-w.cn/gtatsjrsta.html

[C15] 解构 / 展开参数
来源：http://hz.sweek.top/gtgsqulvsl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hywenlv.cn/gtifeuvipk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jyoumei.cn/gtypsoilya.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.birdmap.top/gtwidyimhp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yueranfly.top/gtamffuwhy.html

Java: // 无解构
来源：http://hz.aizwys.cn/gtemjttbhw.html

Go:   // 无解构
来源：http://hz.ivvv.top/gtuzyzmwje.html

Ruby: a, b = pair
来源：http://hz.sysykeji.top/gtwsfnndqt.html

C#:   var (a, b) = pair;
来源：http://hz.havefunace.top/gtwpheqzva.html

[C16] 函数 / 方法重载
来源：http://hz.cdnleiting.top/gtxdbdvydi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhengqikj.top/gtadreopuf.html

PHP:  // 无重载
来源：http://hz.ybcxt.top/gtkjwvdfdc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xinyue.icu/gtdlaxosrj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.kuanghao11.cn/gtkfhduewo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj20258.top/gtsopuifdv.html

Go:   // 无重载：用不同函数名
来源：http://hz.cdnleiting.top/gtjblcbkkj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.havefunace.top/gtehqyiecm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhixingplan.top/gtvpzsruyf.html

================================================================================
来源：http://hz.nanxinkj.top/gttkgnahgu.html

D. 数组 / 列表 / 集合
来源：http://hz.jinyuanbaomall.cn/gtxdaypntz.html

================================================================================
来源：http://hz.ydjk.org.cn/gthukhebcd.html

[D01] 创建数组 / 列表
来源：http://hz.iojbl.cn/gthjvpfwzy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tianlin.xyz/gtplubuyog.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.c1oappe.top/gtubondtih.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yvedp.cn/gthnqrzevo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hnqzz.top/gtjshsemft.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.0kj1m.cn/gtpoaflkwa.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yvedp.cn/gtoaxllzso.html

Ruby: arr = [1, 2, 3]
来源：http://hz.haohaochexian.top/gtoipsakuu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.snrcjt.cn/gtpqllxvkd.html

[D02] 追加元素到末尾
来源：http://hz.jqgfzy.top/gtyvauksbs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydjk.org.cn/gtamyypobh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sxryk.cn/gtcdueckvx.html

JS:   arr.push(4);
来源：http://hz.chenzaomai.com/gtnsemluik.html

TS:   arr.push(4);
来源：http://hz.wangdashe.top/gtbrinxccg.html

Java: list.add(4);
来源：http://hz.52xcode.cn/gttezkfdwe.html

Go:   arr = append(arr, 4)
来源：http://hz.yj20258888.top/gtteqetcqp.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tianlin.xyz/gtxfmaffea.html

C#:   list.Add(4);
来源：http://hz.birdmap.top/gtejzjdquq.html

[D03] 在指定位置插入元素
来源：http://hz.yanxiufei.cn/gtwntywjeo.html

Py:   arr.insert(0, 0)
来源：http://hz.jiagoushi.top/gtxzldoxha.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.wangshuangyany.cn/gtskyzkxwc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shanyushiyangkeji.top/gtftfdrnao.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ydjk.org.cn/gtynkqvqnv.html

Java: list.add(0, 0);
来源：http://hz.ydjk.org.cn/gthqgojsag.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ehwqpu.com/gthcvgohdx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yvedp.cn/gtqdiokdyh.html

C#:   list.Insert(0, 0);
来源：http://hz.shangyingyoupin.top/gtyudwtjnr.html

[D04] 删除元素
来源：http://hz.hywenlv.cn/gtcyqdsqiz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ppjwa.cn/gtelxrxrgk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gaohongyu789.top/gtzrcmuges.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pengpengdd.cyou/gtcfljovde.html

TS:   arr.splice(0, 1);
来源：http://hz.jlsjyb.cn/gtgqkkmgge.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydzc1.top/gtacvsgwwm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yuanzhike.top/gtilknokbg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gzhubu.top/gtlgcgbnxw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.redwolf501.top/gtdcasjvfi.html

[D05] 访问与修改元素
来源：http://hz.yvedp.cn/gtdklfubzg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhiwuduotai.top/gtjueeuirs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtvkedfedx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtteuulruh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yanxiufei.cn/gtvqvqxxqg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinghuilouyu.cn/gthfaxqieg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtcxizyyaw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yongpay.top/gtrmzgmbdh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.andypj.xyz/gtnxkuulqc.html

[D06] 数组长度
来源：http://hz.pycfn.com/gtddodggmx.html

Py:   len(arr)
来源：http://hz.haohaochexian.top/gtolihnpoy.html

PHP:  count($arr);
来源：http://hz.52xcode.cn/gttsggnrdb.html

JS:   arr.length
来源：http://hz.316326.xyz/gtlbzakbdf.html

TS:   arr.length
来源：http://hz.gaohongyu789.top/gtsinjcjvp.html

Java: list.size();
来源：http://hz.jlsjyb.cn/gtqjiajkwf.html

Go:   len(arr)
来源：http://hz.ydjk.org.cn/gtsytdzayc.html

Ruby: arr.length; arr.size
来源：http://hz.wangshuangyany.cn/gtkeyapbld.html

C#:   list.Count;
来源：http://hz.yanxiufei.cn/gtfknbbctb.html

[D07] 切片 / 取子数组
来源：http://hz.shanyushiyangkeji.top/gtguqdjduc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shanyushiyangtech.top/gtsyihljia.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhijiandao.cn/gthbjbdnsu.html

JS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtjqnxgpwi.html

TS:   arr.slice(1, 4);
来源：http://hz.aibaodan.cn/gtgmeebovu.html

Java: list.subList(1, 4);
来源：http://hz.hammf.cn/gtazjyskte.html

Go:   arr[1:4]
来源：http://hz.zhiwuduotai.top/gtekrhkjag.html

Ruby: arr[1, 3]
来源：http://hz.yj202588.top/gttgdnsmuy.html

C#:   list.GetRange(1, 3);
来源：http://hz.dianchejie.cn/gtixngzhbh.html

[D08] 合并两个数组
来源：http://hz.jinyuanbaomall.cn/gtvxdbhvxt.html

Py:   a + b;  a.extend(b)
来源：http://hz.0kj1m.cn/gtapdlrvkv.html

PHP:  array_merge($a, $b);
来源：http://hz.chenjidiqi.icu/gtnknwubem.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dianchejie.cn/gttwrfskln.html

TS:   [...a, ...b];
来源：http://hz.bjfxy.top/gtppgsimka.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gtxpdixmwv.html

Go:   append(a, b...)
来源：http://hz.aizwys.cn/gtzwljhcij.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yuxming.cn/gtaxjjkbsa.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhaomingkeji.xyz/gtnqcytihg.html

[D09] 排序（升序）
来源：http://hz.jyoumei.cn/gtdakwrgmw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aizwys.cn/gtzncfaqci.html

PHP:  sort($arr);
来源：http://hz.jinqigfzy.top/gtzejgsfqr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jianghu66.top/gtqmktkxpo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnxiangtu.top/gtbjaavoqn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.redwolf501.top/gtlwcvmjdi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hywenlv.cn/gtalrucxqs.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtrbputoxx.html

C#:   list.Sort();
来源：http://hz.mhx1999.top/gtdzqgbdon.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenlongwang.top/gtgbuxfwhl.html


<!-- 参考信息 -->