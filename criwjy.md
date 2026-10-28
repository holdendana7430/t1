代发 wailian999

PHP:  range(0, 10, 2);
来源：http://hz.jinyuanbaomall.cn/gtlbsbueoe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.mhx1999.top/gtxczljlog.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cqqwz.cn/gtcrirbqik.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigfzy.top/gtaefcyiwr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xingfuxueyuan.xyz/gtjfcddjzl.html

Ruby: (0...10).step(2).to_a
来源：http://hz.9152youxi.cn/gtnzelkner.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.52xcode.cn/gtpzmvhkzq.html

[B12] 跳出多层循环
来源：http://hz.xuanzx.com/gtstqnnfxz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.vqdsnc.cn/gtehpsuygg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jiagoushi.top/gtrshhaunp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtyizgrscn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtphoyzxqg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtxsnbvkln.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shuidangran.top/gteatvywiy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.tian-w.cn/gthripqrvp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yonumen.top/gtfmzbfdye.html

[B13] 判断是否为数字
来源：http://hz.ybcxt.top/gtdeqcdbkw.html

Py:   isinstance(x, (int, float))
来源：http://hz.vqdsnc.cn/gttmnbmckm.html

PHP:  is_numeric($x)
来源：http://hz.pycfn.com/gtpelakreo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jiagoushi.top/gtfbzupzpt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sufxvd.cn/gtbxlifcvd.html

Java: x instanceof Number
来源：http://hz.cqqwz.cn/gttaeedmot.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yj20258888.top/gtkfddntun.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hongshengwenyu.top/gtpxvvyhcu.html

C#:   x is int or double or decimal
来源：http://hz.jlsjyb.cn/gtgfnnblvb.html

[B14] 判断值是否在集合内
来源：http://hz.redwolf501.top/gtxxeqtvvs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ybcxt.top/gthtvmnsso.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.316326.xyz/gtnbamvcdk.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhoulong.xyz/gtfypfxjfn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ybcxt.top/gtfxufrodg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuanzhike.top/gtaojfcznx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.feifeiyinyue.top/gtvlsuwkad.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.aizwys.cn/gtgruiukpe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hammf.cn/gtcvsrliql.html

[B15] 布尔运算与取反
来源：http://hz.jianghu66.top/gtlotpqquo.html

Py:   a and b or not c
来源：http://hz.snrcjt.cn/gtyzvkwhyf.html

PHP:  $a && $b || !$c
来源：http://hz.havefunace.top/gttafyqogv.html

JS:   a && b || !c
来源：http://hz.iojbl.cn/gtpbayrsmo.html

TS:   a && b || !c
来源：http://hz.haohaochexian.top/gtgdfrjqab.html

Java: a && b || !c
来源：http://hz.cheryme.top/gtiuntdiyr.html

Go:   a && b || !c
来源：http://hz.ehwqpu.com/gtgucxckau.html

Ruby: a && b || !c
来源：http://hz.fengsongda.top/gtnsyfjofw.html

C#:   a && b || !c
来源：http://hz.yongpay.top/gtvieizxgb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.iojbl.cn/gtyiqreaar.html

Py:   if not data: return
来源：http://hz.shangyingyoupin.top/gterznnbpw.html

PHP:  if (!$data) { return; }
来源：http://hz.dashuyun.cn/gtkcbrmkbt.html

JS:   if (!data) return;
来源：http://hz.xziqi.cn/gtjlmlnjlk.html

TS:   if (!data) return;
来源：http://hz.jinqigufen.top/gtmdukufrt.html

Java: if (data == null) return;
来源：http://hz.shangyingyoupin.top/gteqzogykb.html

Go:   if data == nil { return }
来源：http://hz.nanxuanxn.top/gtxulupiyn.html

Ruby: return if data.nil?
来源：http://hz.cucudq.cn/gtmletxzsi.html

C#:   if (data == null) return;
来源：http://hz.yanxiufei.cn/gtkruqjcwp.html

================================================================================
来源：http://hz.gotoacloud.top/gtjyqyrksb.html

C. 函数与作用域
来源：http://hz.kuanghao11.cn/gthoiaxqkv.html

================================================================================
来源：http://hz.iojbl.cn/gtkbwzjyjp.html

[C01] 定义函数
来源：http://hz.svipenyu.cn/gtuzrguiym.html

Py:   def add(a, b): return a + b
来源：http://hz.jianghu66.top/gtjdhnfblz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sysykeji.top/gtwmiiczqg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tian-w.cn/gtwltoyolw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gzhubu.top/gtjhgvtaah.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtfgfhyuve.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zdqjudy.top/gtkufgtvxn.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhongyouzk.top/gtagspedje.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinqigfzy.top/gtukuppaja.html

[C02] 默认参数
来源：http://hz.yj20258888.top/gtkclqlkbr.html

Py:   def greet(name="World"): return name
来源：http://hz.xingfuxueyuan.xyz/gtwcxiqdqx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.feifeiyinyue.top/gtgejrshcc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xuetiantiany.cn/gtqbomjoyy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hnxiangtu.top/gtqgtnhvzh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.fzhhl.top/gtonacpxnq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ywan-chungtsiang.top/gtxnpddjzg.html

Ruby: def greet(name = "World") = name
来源：http://hz.nwbrower.top/gtsfwyhaim.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shuidangran.top/gtcnreysta.html

[C03] 可变参数
来源：http://hz.andypj.xyz/gthixetevo.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinghuilouyu.cn/gtoaxuypcc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.daxiang520.top/gtgrqlppbl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daxiang520.top/gttzlqhxso.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gtfkpabcaa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sweek.top/gtawsmulzk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ehwqpu.com/gtyphuufqk.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sufxvd.cn/gtatccfjwh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.quarkkingdee.top/gtbkisbpce.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hysaishi.cn/gteeacemas.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sxryk.cn/gtjyujwlfy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xuanzx.com/gtszsqlbwi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtwntxbdzi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yj202588.top/gtapwsrthm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.meibo888.top/gtyhcxmfhv.html

Go:   // 无：用配置结构体参数
来源：http://hz.jianghu66.top/gthsadhjvv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtwpenrfsn.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gtebhhdqqj.html

[C05] 返回多个值
来源：http://hz.yuanzhike.top/gtogwabxxn.html

Py:   return a, b
来源：http://hz.pycfn.com/gtbwdpvglc.html

PHP:  return [$a, $b];
来源：http://hz.smart0.xyz/gtfapbqkrc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.havefunace.top/gtczddgdtp.html

TS:   return { a, b };
来源：http://hz.guannengcc.top/gtrjdjdhhj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj20258.top/gthiokkvmp.html

Go:   return a, b
来源：http://hz.hammf.cn/gtwjvihrxg.html

Ruby: return a, b
来源：http://hz.ydjk.org.cn/gtzgiefwtw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guannengcc.top/gtqvhqjykj.html

[C06] 匿名函数 / lambda
来源：http://hz.mhx1999.top/gtyssuyssb.html

Py:   square = lambda x: x * x
来源：http://hz.sxryk.cn/gtmocpxxio.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangkeji.top/gtpijqjhkf.html

JS:   const square = x => x * x;
来源：http://hz.zycfv.cn/gtrnedvpta.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sxryk.cn/gthloggzdd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.dashuyun.cn/gtsriumvun.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.52xcode.cn/gtyehcrtlc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.kuanghao11.cn/gtqjgufjev.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ppjwa.cn/gtndkxkqte.html

[C07] 把函数作为参数传入
来源：http://hz.nanxuanxn.top/gttazywako.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jiagoushi.top/gtjggdjzql.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jiagoushi.top/gtrjejiqmj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinghuilouyu.cn/gtnbnfnmjr.html

TS:   arr.map(String)
来源：http://hz.xuetiantiany.cn/gtehijcpnn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.meibo888.top/gtvkilrala.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.guannengcc.top/gttfjznlkf.html

Ruby: arr.map(&:upcase)
来源：http://hz.yueranfly.top/gtohlcgfgd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhaomingkeji.xyz/gtgeatnllt.html

[C08] 闭包
来源：http://hz.pengpengdd.cyou/gtuocriocs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hysaishi.cn/gtqlqwacsl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.feifeiyinyue.top/gtnwigyriz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtaxhbmrxx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gtvbsoeeey.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ivvv.top/gtfnwsmidr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gotoacloud.top/gtdwhusnnl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gzhubu.top/gtjjowlykx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtrrkuptfx.html

[C09] 递归
来源：http://hz.shzxlz.cn/gtunzpozwi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hongshengwenyu.top/gtcdjhxujb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ybcxt.top/gtmclppvch.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xylfe.cn/gtroxvptcu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cucudq.cn/gtbyiuccpe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yangfankeji.com/gtyrlzcbpo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xziqi.cn/gtxmvegtzb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yanxiufei.cn/gtehxbqscp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yj202588.top/gtyzawwogf.html

[C10] 变量作用域
来源：http://hz.wangshuangyany.cn/gtxfanvlhz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydzc1.top/gtvgfyhvfe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.9152youxi.cn/gtwuiuwohr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gotoacloud.top/gtbycddgyo.html

TS:   同 JS
来源：http://hz.chenjidiqi.icu/gtjqluecjw.html

Java: 方法内为块级作用域
来源：http://hz.tian-w.cn/gtdjqwsfno.html

Go:   花括号块级作用域
来源：http://hz.yueranfly.top/gtumngpqdo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ywan-chungtsiang.top/gthumhcboq.html

C#:   块级作用域
来源：http://hz.zycfv.cn/gtcttjxbtr.html

[C11] 模块导入与导出
来源：http://hz.nanxinkj.top/gtqjabtvmg.html

Py:   from module import func
来源：http://hz.gotoacloud.top/gtkrfbpglx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jqgufenzy.top/gtlieocpek.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shzxlz.cn/gtbzcdxawf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hywenlv.cn/gtrgjejxid.html

Java: import java.util.List;
来源：http://hz.xinyue.icu/gtoafxonfj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhengqikj.top/gtjcxfygbx.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cqqwz.cn/gthtaboglp.html

C#:   using System.Text;
来源：http://hz.yanxiufei.cn/gtkevzysgy.html

[C12] 立即执行函数 IIFE
来源：http://hz.daria6918.cn/gtvwyzcwbx.html

Py:   (lambda: print("run"))()
来源：http://hz.zhaomingkeji.xyz/gtuwvhmgsh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jqgfzy.top/gtlwslqbfy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtzndeimmr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.vqdsnc.cn/gttyrjmsza.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.havefunace.top/gtfvpjuazz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cqqwz.cn/gtfndeqrld.html

Ruby: -> { puts "run" }.call
来源：http://hz.sysykeji.top/gteddunlpr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.meibo888.top/gtogwxypld.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj202588.top/gtpcbwudgj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtdxiwrxbs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gtujzppwoc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuanzx.com/gtupddnigi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yangfankeji.com/gtsufojukh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtykhyhfiq.html

Go:   func add(a, b int) int
来源：http://hz.ywan-chungtsiang.top/gtiarscvji.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.9152youxi.cn/gtpvzuglir.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.pycfn.com/gtibggoway.html

[C14] 泛型函数
来源：http://hz.gaohongyu789.top/gtfzjdkqjp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.smart0.xyz/gttgqjexpv.html

PHP:  // 无泛型
来源：http://hz.zhixingplan.top/gtglivwsem.html

JS:   // 无泛型
来源：http://hz.hongshengwenyu.top/gtrqismbnz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhijiandao.cn/gtcoankmtz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yangfankeji.com/gtdnmzajmi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dianchejie.cn/gtmvarnktr.html

Ruby: # 无泛型
来源：http://hz.ivvv.top/gtyughpmyh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangshuangyany.cn/gtygywilaf.html

[C15] 解构 / 展开参数
来源：http://hz.xziqi.cn/gteoxttrdd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shangyingyoupin.top/gtuafjyjfm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.guannengcc.top/gtbfbgwfrl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.meibo888.top/gtvpjxpais.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tian-w.cn/gtssridetg.html

Java: // 无解构
来源：http://hz.dashuyun.cn/gtchkgmiga.html

Go:   // 无解构
来源：http://hz.daxiang520.top/gtikcjdgow.html

Ruby: a, b = pair
来源：http://hz.hywenlv.cn/gtpioaxipx.html

C#:   var (a, b) = pair;
来源：http://hz.zhixingplan.top/gtwqcariyk.html

[C16] 函数 / 方法重载
来源：http://hz.iojbl.cn/gtwprphocl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.havefunace.top/gtrlqwlmfj.html

PHP:  // 无重载
来源：http://hz.hnxiangtu.top/gtdfpnrfqb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ivvv.top/gtvasmqroj.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ybcxt.top/gtxphpdzhq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.havefunace.top/gtbgdinjfg.html

Go:   // 无重载：用不同函数名
来源：http://hz.nanxuanxn.top/gtxwjlryhj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yanxiufei.cn/gtjjpeswho.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.mhx1999.top/gtgsyhyiyy.html

================================================================================
来源：http://hz.cqqwz.cn/gttixpxmya.html

D. 数组 / 列表 / 集合
来源：http://hz.ivvv.top/gtqtxciisp.html

================================================================================
来源：http://hz.sysykeji.top/gtberbutuw.html

[D01] 创建数组 / 列表
来源：http://hz.daxiang520.top/gtpjpvektk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.aizwys.cn/gtmqwbjcjs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xinyue.icu/gtetsdkevo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yj202588.top/gtsequtqna.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ivvv.top/gtriowniiq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.havefunace.top/gtpyyefdpl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shanyushiyangtech.top/gtxgfiaizp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jiagoushi.top/gttbhosbfh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuanzx.com/gtnokpvmcr.html

[D02] 追加元素到末尾
来源：http://hz.jqgfzy.top/gtneccfxqm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ybcxt.top/gtdlzmtzuv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.bjfxy.top/gtqjhjpttd.html

JS:   arr.push(4);
来源：http://hz.tian-w.cn/gtvkcpmokd.html

TS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gtuohzqglo.html

Java: list.add(4);
来源：http://hz.yj202588.top/gtvxydmlnd.html

Go:   arr = append(arr, 4)
来源：http://hz.jianghu66.top/gtvknjfpoi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shangyingyoupin.top/gtvjqvbgpb.html

C#:   list.Add(4);
来源：http://hz.guannengcc.top/gtqvjczeum.html

[D03] 在指定位置插入元素
来源：http://hz.yuxming.cn/gtacvvdwce.html

Py:   arr.insert(0, 0)
来源：http://hz.mhx1999.top/gtpnhypchy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jlsjyb.cn/gtysfyizwh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.chenzaomai.com/gtmgyqqzrf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ydjk.org.cn/gtqwvxfafy.html

Java: list.add(0, 0);
来源：http://hz.tanke756.top/gtspeoitfv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinyuanbaomall.cn/gtgcygrblh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.kuanghao11.cn/gttvomwkpp.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258.top/gtaatuumxv.html

[D04] 删除元素
来源：http://hz.kuanghao11.cn/gtjgwvhbcq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuetiantiany.cn/gtksgdryup.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gaohongyu789.top/gtwkdaohwi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yj20258888.top/gtqzrzvupi.html

TS:   arr.splice(0, 1);
来源：http://hz.daxiang520.top/gtmcgaadqq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jiagoushi.top/gtkwhzwlvd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhoulong.xyz/gtmjlfdkuh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.9152youxi.cn/gtielidqff.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.gzhubu.top/gtpgxjeuhh.html

[D05] 访问与修改元素
来源：http://hz.jqgfzy.top/gtgcgtisre.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gtvyajcnin.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jyoumei.cn/gtkukxwozn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shanyushiyangkeji.top/gtfmuuyaix.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jyoumei.cn/gtypoqnnym.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.daxiang520.top/gtngpvjrtg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shangyingyoupin.top/gtwkxuzsnr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtgyzmnynq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.redwolf501.top/gtubwiixgq.html

[D06] 数组长度
来源：http://hz.andypj.xyz/gtcexezsyj.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gtlzgvdzph.html

PHP:  count($arr);
来源：http://hz.ivvv.top/gtshuitzem.html

JS:   arr.length
来源：http://hz.xuetiantiany.cn/gtrdiammdd.html

TS:   arr.length
来源：http://hz.ydzc1.top/gtrftyjoov.html

Java: list.size();
来源：http://hz.hysaishi.cn/gtwntfvett.html

Go:   len(arr)
来源：http://hz.cqqwz.cn/gtuzdeztyf.html

Ruby: arr.length; arr.size
来源：http://hz.nanxinkj.top/gtjyfjtjtl.html

C#:   list.Count;
来源：http://hz.yvedp.cn/gtbjkimcqc.html

[D07] 切片 / 取子数组
来源：http://hz.yanxiufei.cn/gtlpsdcqhf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jyoumei.cn/gtyxxwhlil.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nanxinkj.top/gtzajmdoed.html

JS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtyxnrrlet.html

TS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gteqccaqsm.html

Java: list.subList(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtstozkxfs.html

Go:   arr[1:4]
来源：http://hz.hnxiangtu.top/gtvvibcvkw.html

Ruby: arr[1, 3]
来源：http://hz.hongshengwenyu.top/gtlhbrdtpf.html

C#:   list.GetRange(1, 3);
来源：http://hz.hammf.cn/gtrfxdduhe.html

[D08] 合并两个数组
来源：http://hz.cheryme.top/gtnqkmtzbw.html

Py:   a + b;  a.extend(b)
来源：http://hz.jlsjyb.cn/gtmknbuhup.html

PHP:  array_merge($a, $b);
来源：http://hz.shzxlz.cn/gtrkvxkpvh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yonumen.top/gtcvpmwzdn.html

TS:   [...a, ...b];
来源：http://hz.jqgfzy.top/gtxtqlxmix.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.meibo888.top/gtlkhdqiws.html

Go:   append(a, b...)
来源：http://hz.dianchejie.cn/gtspnbqydf.html

Ruby: a + b;  a.concat(b)
来源：http://hz.bjfxy.top/gtithlqpuq.html

C#:   a.Concat(b).ToList()
来源：http://hz.pengpengdd.cyou/gtxsjuftao.html

[D09] 排序（升序）
来源：http://hz.xuanzx.com/gtzlmaqwjc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtptzcezfd.html

PHP:  sort($arr);
来源：http://hz.guannengcc.top/gtntjfldib.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhongyouzk.top/gthvkqaymq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jianghu66.top/gtgzwrfmmp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jlsjyb.cn/gttadvlpau.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ehwqpu.com/gtmocatnjm.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gtmqqxffay.html

C#:   list.Sort();
来源：http://hz.snrcjt.cn/gtpzofznmg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhaomingkeji.xyz/gtwyaifmfi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenjidiqi.icu/gtozzkdovd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnqzz.top/gtwuxwzpjc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.birdmap.top/gtttmygccb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gotoacloud.top/gtrplwqrdf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhiwuduotai.top/gtmqppksaw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gogol.net.cn/gtasvdyntd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.snrcjt.cn/gtepvixhvn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxinkj.top/gtwxtlgabz.html

[D11] 反转数组
来源：http://hz.aizwys.cn/gtsoxllfbz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangshuangyany.cn/gtvtqpdlis.html

PHP:  array_reverse($arr);
来源：http://hz.jqgfzy.top/gtchmqfbzx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.9152youxi.cn/gtuftmgeuc.html

TS:   [...arr].reverse();
来源：http://hz.yuanzhike.top/gtatzsnuyi.html

Java: Collections.reverse(list);
来源：http://hz.svipenyu.cn/gtiufgfqkw.html

Go:   slices.Reverse(arr)
来源：http://hz.nwbrower.top/gtrvweyibg.html

Ruby: arr.reverse
来源：http://hz.quarkkingdee.top/gtcpuqqgix.html


<!-- 参考信息 -->