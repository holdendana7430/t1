代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.guannengcc.top/gtooyeauyn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhengqikj.top/gtjuotdcuf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xinyue.icu/gtsvqbqerh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jlsjyb.cn/gtmruodwby.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cashguo.top/gtfomfwjez.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigufen.top/gtbnmxzmgs.html

[B11] 生成数字序列 / 区间
来源：http://hz.svipenyu.cn/gtzodwkvnb.html

Py:   list(range(0, 10, 2))
来源：http://hz.jinqigufen.top/gtptkwbhok.html

PHP:  range(0, 10, 2);
来源：http://hz.chenlongwang.top/gtqqndkqdl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xinyue.icu/gtapoyvxqr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ppjwa.cn/gtqgbcrygf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jlsjyb.cn/gtifnxiesu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.meibo888.top/gteknskesb.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shangyingyoupin.top/gtkcxraiyk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhongyouzk.top/gtwjkpfpzd.html

[B12] 跳出多层循环
来源：http://hz.xziqi.cn/gtlkptbqvr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hywenlv.cn/gtailqfytv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ivvv.top/gtedbsojpo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgfzy.top/gtarilqlkk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gtyvkpayvc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.aizwys.cn/gtcacwemqe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.pengpengdd.cyou/gtzyqbktub.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.vqdsnc.cn/gtqieomhmz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tianlin.xyz/gtilxdsprt.html

[B13] 判断是否为数字
来源：http://hz.shuidangran.top/gtktroyryr.html

Py:   isinstance(x, (int, float))
来源：http://hz.havefunace.top/gtiuoxbczz.html

PHP:  is_numeric($x)
来源：http://hz.mhx1999.top/gtqsmbgorh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jianghu66.top/gtxumhgath.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xziqi.cn/gttfoyeivn.html

Java: x instanceof Number
来源：http://hz.yj20258.top/gtmucvzikd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.0kj1m.cn/gtucvdasky.html

Ruby: x.is_a?(Numeric)
来源：http://hz.wangdashe.top/gtzivrmjqp.html

C#:   x is int or double or decimal
来源：http://hz.wangdashe.top/gtlqrylgus.html

[B14] 判断值是否在集合内
来源：http://hz.guannengcc.top/gtvcdwtuoa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.kuanghao11.cn/gtlyhbenoh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nanxinkj.top/gtuudkasph.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtjlzppqiy.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.nanxuanxn.top/gtefiddeus.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.birdmap.top/gtpkdrverj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shzxlz.cn/gtsvzakfnb.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cdnleiting.top/gtebxffmaa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.gogol.net.cn/gtfxkpxtxe.html

[B15] 布尔运算与取反
来源：http://hz.sweek.top/gtsziwhjxv.html

Py:   a and b or not c
来源：http://hz.pycfn.com/gtguvehowl.html

PHP:  $a && $b || !$c
来源：http://hz.feifeiyinyue.top/gtqwtdtkyo.html

JS:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtozquusnn.html

TS:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtqaefdkej.html

Java: a && b || !c
来源：http://hz.hnqzz.top/gtaxhuaeam.html

Go:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtwfjuuist.html

Ruby: a && b || !c
来源：http://hz.sufxvd.cn/gtquphcekn.html

C#:   a && b || !c
来源：http://hz.bjfxy.top/gtbhqexxeh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.c1oappe.top/gthqmzuldt.html

Py:   if not data: return
来源：http://hz.dashuyun.cn/gtzuerqkwx.html

PHP:  if (!$data) { return; }
来源：http://hz.jinyuanbaomall.cn/gtowtaksmx.html

JS:   if (!data) return;
来源：http://hz.jinqigufen.top/gtbtldffri.html

TS:   if (!data) return;
来源：http://hz.gogol.net.cn/gtrhvutwnh.html

Java: if (data == null) return;
来源：http://hz.kuanghao11.cn/gtubmogooj.html

Go:   if data == nil { return }
来源：http://hz.fzhhl.top/gtqkzgrzpc.html

Ruby: return if data.nil?
来源：http://hz.ydjk.org.cn/gtiklhmisk.html

C#:   if (data == null) return;
来源：http://hz.shanyushiyangtech.top/gtcknpybnh.html

================================================================================
来源：http://hz.dashuyun.cn/gtdxaejimb.html

C. 函数与作用域
来源：http://hz.yonumen.top/gtpigdoirf.html

================================================================================
来源：http://hz.andypj.xyz/gtmzeoskoy.html

[C01] 定义函数
来源：http://hz.tianlin.xyz/gtginbksej.html

Py:   def add(a, b): return a + b
来源：http://hz.cheryme.top/gtwtnyvqyf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtkmllgsvl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jlsjyb.cn/gteqsfmjmc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tanke756.top/gtntvbzvgd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtjbnyroki.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hysaishi.cn/gtyhbevldy.html

Ruby: def add(a, b); a + b; end
来源：http://hz.iojbl.cn/gtbgwdgncs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yuanzhike.top/gtjlqckhzs.html

[C02] 默认参数
来源：http://hz.svipenyu.cn/gtpyfmwwkd.html

Py:   def greet(name="World"): return name
来源：http://hz.hnqzz.top/gtzqvlkeem.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.andypj.xyz/gthfrmpytm.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nwbrower.top/gtetlnrdfi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhengqikj.top/gtdemhezdn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shzxlz.cn/gtcobnabwi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.pengpengdd.cyou/gtieaiohwl.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinyuanbaomall.cn/gtdpfojysx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ywan-chungtsiang.top/gtowpbiggx.html

[C03] 可变参数
来源：http://hz.cheryme.top/gtuehdtrbi.html

Py:   def total(*args): return sum(args)
来源：http://hz.0kj1m.cn/gtrmwidhxw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.bjfxy.top/gtbncgjdtv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hammf.cn/gtmcckxjvn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhoulong.xyz/gtgwhhzdtw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.tianlin.xyz/gtvwsnovfh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jlsjyb.cn/gtsojdiquk.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ybcxt.top/gtjedyikhn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ywan-chungtsiang.top/gtqmuvuzyx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.9152youxi.cn/gtqnqxcwyz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.fzhhl.top/gtfwpqgofr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sysykeji.top/gtlhipqyzq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtsyzbrcpp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yonumen.top/gtklklosoh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.quarkkingdee.top/gtoodsdzto.html

Go:   // 无：用配置结构体参数
来源：http://hz.andypj.xyz/gtpqybomgz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.0kj1m.cn/gtvxjhkpcg.html

C#:   f(a: 1, b: 2)
来源：http://hz.cucudq.cn/gtcuxflauw.html

[C05] 返回多个值
来源：http://hz.chenzaomai.com/gtpekfbjwz.html

Py:   return a, b
来源：http://hz.jiagoushi.top/gttmmfaeoe.html

PHP:  return [$a, $b];
来源：http://hz.sxryk.cn/gtwkqwlvkk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jqgufenzy.top/gtvflwekyg.html

TS:   return { a, b };
来源：http://hz.shzxlz.cn/gtwxchsoph.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.chenjidiqi.icu/gtholgxyfp.html

Go:   return a, b
来源：http://hz.daxiang520.top/gttkcfredt.html

Ruby: return a, b
来源：http://hz.ywan-chungtsiang.top/gtecghuvwk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydjk.org.cn/gtdqzfnwyc.html

[C06] 匿名函数 / lambda
来源：http://hz.hnqzz.top/gtzsfbgnzn.html

Py:   square = lambda x: x * x
来源：http://hz.zhijiandao.cn/gtutopbuvc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenjidiqi.icu/gtctscmvnq.html

JS:   const square = x => x * x;
来源：http://hz.zhengqikj.top/gtqdvebnok.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hongshengwenyu.top/gtmycedwoj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ehwqpu.com/gtwvrsgmtm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenjidiqi.icu/gtkzshbxhk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cashguo.top/gtqkwafcsd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhijiandao.cn/gtvumbpfez.html

[C07] 把函数作为参数传入
来源：http://hz.52xcode.cn/gtzhcufcif.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pycfn.com/gtkwgkcpmd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dashuyun.cn/gtmxcpcebn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.havefunace.top/gtkfkktsph.html

TS:   arr.map(String)
来源：http://hz.chenzaomai.com/gtrcuyhbyq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cdnleiting.top/gtwhnayund.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zdqjudy.top/gtsxbldoil.html

Ruby: arr.map(&:upcase)
来源：http://hz.wangdashe.top/gtcngawkdm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shanyushiyangkeji.top/gtkoltvgjw.html

[C08] 闭包
来源：http://hz.xinyue.icu/gtkditidrn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.c1oappe.top/gttyfdqbup.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinqigufen.top/gteyyxamzo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtcffzjkrn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtpzisjcpa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.bjfxy.top/gtirfixikd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.guowangkeji.top/gtofhdpknz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.birdmap.top/gtwwboxggt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtstzabhpg.html

[C09] 递归
来源：http://hz.0kj1m.cn/gtluarmllk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hfpthk.cn/gtjtffitmu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shuidangran.top/gtvvhpfuce.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.quarkkingdee.top/gtdaobmagp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnxiangtu.top/gtkiwbueef.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jqgfzy.top/gtmheiaegk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.pengpengdd.cyou/gtlhxwtauf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xinyue.icu/gtinikqvxm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhiwuduotai.top/gtavupjutp.html

[C10] 变量作用域
来源：http://hz.yj202588.top/gtwgdevmit.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.9152youxi.cn/gtfpgprgjm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hywenlv.cn/gtyxkcocld.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cqqwz.cn/gtjhhaciiu.html

TS:   同 JS
来源：http://hz.wangshuangyany.cn/gtzageslve.html

Java: 方法内为块级作用域
来源：http://hz.yuanzhike.top/gtpmriapgx.html

Go:   花括号块级作用域
来源：http://hz.cashguo.top/gtlaznmufs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yongpay.top/gtxzsfsman.html

C#:   块级作用域
来源：http://hz.jinghuilouyu.cn/gtxcfokjli.html

[C11] 模块导入与导出
来源：http://hz.yj20258.top/gtetpyojfv.html

Py:   from module import func
来源：http://hz.yueranfly.top/gtwuqmcumu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhongyouzk.top/gtrdbotmyl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.c1oappe.top/gtyvyxidqp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daxiang520.top/gtxpuwgvnk.html

Java: import java.util.List;
来源：http://hz.yvedp.cn/gtnewsjjka.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.kuanghao11.cn/gtkfppzeep.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.quarkkingdee.top/gtwtfjttek.html

C#:   using System.Text;
来源：http://hz.zhengqikj.top/gtdxahvyoi.html

[C12] 立即执行函数 IIFE
来源：http://hz.hfpthk.cn/gtemjmcnnu.html

Py:   (lambda: print("run"))()
来源：http://hz.shanyushiyangtech.top/gtgwnwoeqj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shuidangran.top/gtisrkugrw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gtqkwrdcyk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gtbhnrzqxr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hywenlv.cn/gthvevdoas.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cqqwz.cn/gtmnrrbbtj.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj20258888.top/gtevhhswls.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jiagoushi.top/gtuxnckczs.html

[C13] 类型声明 / 类型注解
来源：http://hz.jlsjyb.cn/gtxleodrvb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhaomingkeji.xyz/gtdytngifo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cashguo.top/gtaeqqqtur.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dianchejie.cn/gtidvwuosz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ehwqpu.com/gtuyvmuerl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtuslltxml.html

Go:   func add(a, b int) int
来源：http://hz.jiagoushi.top/gtogpxcona.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yonumen.top/gtslvexdxq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinqigufen.top/gtgiwucoih.html

[C14] 泛型函数
来源：http://hz.9152youxi.cn/gttjsyettc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zycfv.cn/gtninbhtzf.html

PHP:  // 无泛型
来源：http://hz.gaohongyu789.top/gtsjoexsjy.html

JS:   // 无泛型
来源：http://hz.gotoacloud.top/gtnveioift.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shuidangran.top/gtpzekoqzu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinghuilouyu.cn/gtbenwltbn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.iojbl.cn/gtbhrkjlmj.html

Ruby: # 无泛型
来源：http://hz.sufxvd.cn/gtdayiuhjc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.52xcode.cn/gttsadlqnx.html

[C15] 解构 / 展开参数
来源：http://hz.jinghuilouyu.cn/gtdpnnnjwc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yangfankeji.com/gtoytfyxho.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258888.top/gtmevlkrdx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.guowangkeji.top/gtfftnglfd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yongpay.top/gtwfkvrqnt.html

Java: // 无解构
来源：http://hz.sxryk.cn/gttkkmhrzn.html

Go:   // 无解构
来源：http://hz.iojbl.cn/gtjnrvjaab.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtxlojdqnz.html

C#:   var (a, b) = pair;
来源：http://hz.shuidangran.top/gtgklclgae.html

[C16] 函数 / 方法重载
来源：http://hz.iojbl.cn/gtaikwxiqo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nanxuanxn.top/gtdvwgiiqt.html

PHP:  // 无重载
来源：http://hz.c1oappe.top/gtfpktkhuy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.guannengcc.top/gtawnjvszh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shanyushiyangtech.top/gtinmfxlvd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ehwqpu.com/gtvifdlirw.html

Go:   // 无重载：用不同函数名
来源：http://hz.xingfuxueyuan.xyz/gtrfdctduk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jqgufenzy.top/gtgodkzyxg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhaomingkeji.xyz/gtxdrbuxlr.html

================================================================================
来源：http://hz.zhongyouzk.top/gtairpoxfc.html

D. 数组 / 列表 / 集合
来源：http://hz.yanxiufei.cn/gtdecqakhh.html

================================================================================
来源：http://hz.c1oappe.top/gtoctabyqs.html

[D01] 创建数组 / 列表
来源：http://hz.316326.xyz/gtdzfjcebp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xylfe.cn/gtnthkhqlt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ivvv.top/gtxgfbacqn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.haohaochexian.top/gtlurbdaxp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yonumen.top/gtduoglvvu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.quarkkingdee.top/gtistutpab.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.havefunace.top/gtphmckunc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.0kj1m.cn/gtusruunum.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hongshengwenyu.top/gtiiejrnzj.html

[D02] 追加元素到末尾
来源：http://hz.yuanzhike.top/gthlqbfdbi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydzc1.top/gtajqxpmmx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhongyouzk.top/gtbvopenuz.html

JS:   arr.push(4);
来源：http://hz.xylfe.cn/gthwuijsbz.html

TS:   arr.push(4);
来源：http://hz.dianchejie.cn/gtvrunfzne.html

Java: list.add(4);
来源：http://hz.birdmap.top/gtftlzpuib.html

Go:   arr = append(arr, 4)
来源：http://hz.quarkkingdee.top/gtdvpgihju.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gaohongyu789.top/gtlmvvygfc.html

C#:   list.Add(4);
来源：http://hz.meibo888.top/gtfzadlicv.html

[D03] 在指定位置插入元素
来源：http://hz.jinqigfzy.top/gtcjhylrkl.html

Py:   arr.insert(0, 0)
来源：http://hz.jinghuilouyu.cn/gtyrarwhlo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ppjwa.cn/gtllachtjn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.fengsongda.top/gtbexkmsgz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.havefunace.top/gtszcqupce.html

Java: list.add(0, 0);
来源：http://hz.ydjk.org.cn/gtuxbqdtlm.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.quarkkingdee.top/gtuiknhjif.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj20258888.top/gtbpbshjyc.html

C#:   list.Insert(0, 0);
来源：http://hz.9152youxi.cn/gtfatjyszd.html

[D04] 删除元素
来源：http://hz.cdnleiting.top/gtfzefqdcw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yanxiufei.cn/gtkaypbhwb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.feifeiyinyue.top/gtxybkicxx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxinkj.top/gtuvooxvip.html

TS:   arr.splice(0, 1);
来源：http://hz.zhoulong.xyz/gtwuspzrdd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhoulong.xyz/gtpgandjsk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhijiandao.cn/gtapoqbekn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ywan-chungtsiang.top/gtslahcqaz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.smart0.xyz/gtjhpgwosc.html

[D05] 访问与修改元素
来源：http://hz.feifeiyinyue.top/gtxcubejzn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenjidiqi.icu/gtkwpdirrw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yanxiufei.cn/gtbgavvzxp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhongyouzk.top/gtxzlkubyq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhengqikj.top/gtophvdqcp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhiwuduotai.top/gtfrafdkfh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuxming.cn/gtpylnchrd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.andypj.xyz/gtqjonwguy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jianghu66.top/gtgyclbasq.html

[D06] 数组长度
来源：http://hz.yongpay.top/gtlfoolibf.html

Py:   len(arr)
来源：http://hz.jlsjyb.cn/gtnepjknru.html

PHP:  count($arr);
来源：http://hz.ydzc1.top/gtxdoolzmr.html

JS:   arr.length
来源：http://hz.dashuyun.cn/gturzzoeds.html

TS:   arr.length
来源：http://hz.hnxiangtu.top/gtdwbtmhss.html

Java: list.size();
来源：http://hz.zhongyouzk.top/gtqkioisfh.html

Go:   len(arr)
来源：http://hz.cdnleiting.top/gtwphzpxua.html

Ruby: arr.length; arr.size
来源：http://hz.shangyingyoupin.top/gtegpetqsu.html

C#:   list.Count;
来源：http://hz.shzxlz.cn/gtgcvccitb.html

[D07] 切片 / 取子数组
来源：http://hz.nanxuanxn.top/gtmsqcbhpc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.aibaodan.cn/gtxydhzytq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.svipenyu.cn/gtczgcsqyh.html

JS:   arr.slice(1, 4);
来源：http://hz.aibaodan.cn/gtxmqbupgi.html

TS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtsoluokmz.html

Java: list.subList(1, 4);
来源：http://hz.yj202588.top/gthwctgyrb.html

Go:   arr[1:4]
来源：http://hz.yongpay.top/gtoiojhdlx.html

Ruby: arr[1, 3]
来源：http://hz.jinqigufen.top/gtungxlkdc.html

C#:   list.GetRange(1, 3);
来源：http://hz.guowangkeji.top/gtkryoztce.html

[D08] 合并两个数组
来源：http://hz.yueranfly.top/gtrtgqhvwo.html

Py:   a + b;  a.extend(b)
来源：http://hz.smart0.xyz/gtqznfgcal.html

PHP:  array_merge($a, $b);
来源：http://hz.nanxuanxn.top/gthkmwzikx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ehwqpu.com/gtnbjsdnmw.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangkeji.top/gtoxbdskfk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daxiang520.top/gtexmickej.html

Go:   append(a, b...)
来源：http://hz.sysykeji.top/gtcaqcdpad.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ydzc1.top/gtyokyaizm.html

C#:   a.Concat(b).ToList()
来源：http://hz.haohaochexian.top/gtdusacjmk.html

[D09] 排序（升序）
来源：http://hz.wangdashe.top/gtfcpdjfxu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtibkrqbhv.html

PHP:  sort($arr);
来源：http://hz.gogol.net.cn/gttdktlhfz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.iojbl.cn/gtplaibsoe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yj20258.top/gttjttukux.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.feifeiyinyue.top/gtztsmgomm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtentzjusi.html

Ruby: arr.sort
来源：http://hz.jyoumei.cn/gthvqudolk.html

C#:   list.Sort();
来源：http://hz.cheryme.top/gtokicjltr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydjk.org.cn/gtkizycsuh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.quarkkingdee.top/gtutzkydms.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cashguo.top/gtgawcmjka.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tanke756.top/gtavaftgbr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtqutpacyw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.iojbl.cn/gtrrvojdjv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hfpthk.cn/gtzojxyhfm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jiagoushi.top/gtauyypxni.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhijiandao.cn/gtwqzzzfer.html


<!-- 参考信息 -->