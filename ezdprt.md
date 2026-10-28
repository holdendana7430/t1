代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.pengpengdd.cyou/gticwclsvu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aibaodan.cn/gtsykwxxli.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yj20258888.top/gtkvbbuovb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.svipenyu.cn/gtxjompmmg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sysykeji.top/gterphqeiu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhengqikj.top/gtpyooxzxz.html

[B11] 生成数字序列 / 区间
来源：http://hz.hongshengwenyu.top/gtjgmsafzs.html

Py:   list(range(0, 10, 2))
来源：http://hz.cucudq.cn/gthcmmhjkp.html

PHP:  range(0, 10, 2);
来源：http://hz.nwbrower.top/gthoskastb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daria6918.cn/gtfmqppbxv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.aizwys.cn/gtluqyadxl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.birdmap.top/gtwrrtqgdl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhaomingkeji.xyz/gtekeledzp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.aibaodan.cn/gtiwzyswyk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.316326.xyz/gtestpqnof.html

[B12] 跳出多层循环
来源：http://hz.guowangkeji.top/gtlwbhtqar.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shangyingyoupin.top/gtufibotzu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.bjfxy.top/gtsothhysa.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gtjovtgtct.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gtxuchahtx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zdqjudy.top/gtdoruvtkl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guannengcc.top/gtjyyetcqe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xingfuxueyuan.xyz/gtfduvzuea.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.havefunace.top/gtmzjcyzae.html

[B13] 判断是否为数字
来源：http://hz.shanyushiyangkeji.top/gtgokbkdrh.html

Py:   isinstance(x, (int, float))
来源：http://hz.316326.xyz/gtchtzswyk.html

PHP:  is_numeric($x)
来源：http://hz.mhx1999.top/gtbpvmmvrk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jianghu66.top/gtxfzlqibb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hfpthk.cn/gtivzblrtf.html

Java: x instanceof Number
来源：http://hz.zhaomingkeji.xyz/gtqruqbcwn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yuanzhike.top/gthjsadlxy.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xuetiantiany.cn/gtvolwvwqc.html

C#:   x is int or double or decimal
来源：http://hz.daria6918.cn/gtquvywoyr.html

[B14] 判断值是否在集合内
来源：http://hz.cucudq.cn/gtnvydvzen.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tian-w.cn/gthezicaxc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.cqqwz.cn/gtgppxrxyu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jqgfzy.top/gtdgrntozo.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.316326.xyz/gtnhfbpgvp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gaohongyu789.top/gtwniponrl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhengqikj.top/gtkzctnofw.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.chenjidiqi.icu/gtdjbzhpgm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xziqi.cn/gttzqwovhh.html

[B15] 布尔运算与取反
来源：http://hz.sufxvd.cn/gtkdwjmkzv.html

Py:   a and b or not c
来源：http://hz.ydjk.org.cn/gtoeogtlev.html

PHP:  $a && $b || !$c
来源：http://hz.nwbrower.top/gtuwwocfgq.html

JS:   a && b || !c
来源：http://hz.tian-w.cn/gtynqspiow.html

TS:   a && b || !c
来源：http://hz.yuanzhike.top/gtmfpwiekn.html

Java: a && b || !c
来源：http://hz.ydjk.org.cn/gtlvrrdand.html

Go:   a && b || !c
来源：http://hz.tianlin.xyz/gthohllwdt.html

Ruby: a && b || !c
来源：http://hz.xziqi.cn/gtupgqfbna.html

C#:   a && b || !c
来源：http://hz.havefunace.top/gtnctxcbvh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yanxiufei.cn/gtaxnjtakl.html

Py:   if not data: return
来源：http://hz.vqdsnc.cn/gtwxsienjo.html

PHP:  if (!$data) { return; }
来源：http://hz.nanxinkj.top/gtjqdqvtaj.html

JS:   if (!data) return;
来源：http://hz.zdqjudy.top/gtpzgosaro.html

TS:   if (!data) return;
来源：http://hz.hammf.cn/gtdhwefqog.html

Java: if (data == null) return;
来源：http://hz.0kj1m.cn/gtrqxfnvqs.html

Go:   if data == nil { return }
来源：http://hz.ppjwa.cn/gtbdmvwykk.html

Ruby: return if data.nil?
来源：http://hz.chenjidiqi.icu/gtaozrenzz.html

C#:   if (data == null) return;
来源：http://hz.xziqi.cn/gtzcmdyebb.html

================================================================================
来源：http://hz.9152youxi.cn/gtvihbmcih.html

C. 函数与作用域
来源：http://hz.shanyushiyangtech.top/gtdsdehxhd.html

================================================================================
来源：http://hz.xinyue.icu/gtejtwwhhc.html

[C01] 定义函数
来源：http://hz.c1oappe.top/gtszitqxrf.html

Py:   def add(a, b): return a + b
来源：http://hz.xylfe.cn/gtcffiijyj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtqzzfrpvk.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtzfpqfuno.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fzhhl.top/gtmggwmmkv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtjcowhizz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xziqi.cn/gtwmylxsoj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yueranfly.top/gtzxnpqsof.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtdidbfwdg.html

[C02] 默认参数
来源：http://hz.mhx1999.top/gtpsummexa.html

Py:   def greet(name="World"): return name
来源：http://hz.jlsjyb.cn/gtyjpqnqnn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenlongwang.top/gtbwvnqvgh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.snrcjt.cn/gtwpawbyco.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.chenlongwang.top/gtczpicsws.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dashuyun.cn/gtctszulge.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.kuanghao11.cn/gtsdaihwop.html

Ruby: def greet(name = "World") = name
来源：http://hz.nanxinkj.top/gtgopxuqya.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.aibaodan.cn/gtksgpmeyl.html

[C03] 可变参数
来源：http://hz.yanxiufei.cn/gtshkbgunl.html

Py:   def total(*args): return sum(args)
来源：http://hz.shzxlz.cn/gtcpkfhonj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xylfe.cn/gtrqisbnqs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnqzz.top/gtpkcgguyr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gtkudfyztt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.quarkkingdee.top/gtwmddbvzl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yuxming.cn/gtnrtdeynr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.haohaochexian.top/gtdxhpzyqq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shuidangran.top/gtcneatfew.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ivvv.top/gtxammwgrs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hammf.cn/gtngnakehf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhengqikj.top/gtcbtopnew.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gtteteekmz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shangyingyoupin.top/gtiluunubn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.svipenyu.cn/gtmmbbmifz.html

Go:   // 无：用配置结构体参数
来源：http://hz.redwolf501.top/gtjsnnejps.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gogol.net.cn/gtqhrpoxwc.html

C#:   f(a: 1, b: 2)
来源：http://hz.sweek.top/gtjbemzmyc.html

[C05] 返回多个值
来源：http://hz.hfpthk.cn/gtyruapety.html

Py:   return a, b
来源：http://hz.kuanghao11.cn/gtqodledgg.html

PHP:  return [$a, $b];
来源：http://hz.c1oappe.top/gtbypxfslr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.nwbrower.top/gtwmxgmdsh.html

TS:   return { a, b };
来源：http://hz.316326.xyz/gtmldjfmrp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.snrcjt.cn/gtrgamecdb.html

Go:   return a, b
来源：http://hz.ivvv.top/gttitbdhrs.html

Ruby: return a, b
来源：http://hz.tian-w.cn/gtbstzrkgd.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.chenjidiqi.icu/gtxtbzkrdg.html

[C06] 匿名函数 / lambda
来源：http://hz.yanxiufei.cn/gtavjctirl.html

Py:   square = lambda x: x * x
来源：http://hz.316326.xyz/gtttpqudbq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.bjfxy.top/gtyvuoxckc.html

JS:   const square = x => x * x;
来源：http://hz.tanke756.top/gtfltiqegd.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shangyingyoupin.top/gtzktakytu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yuxming.cn/gtugcmvbze.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhijiandao.cn/gtulhdwwtm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xuanzx.com/gtvigyfsfq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sysykeji.top/gtnecgethn.html

[C07] 把函数作为参数传入
来源：http://hz.yvedp.cn/gtmgmjihdt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xuetiantiany.cn/gtqrtnjsiu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sxryk.cn/gtlntqoyon.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ybcxt.top/gtlqjmwvur.html

TS:   arr.map(String)
来源：http://hz.ehwqpu.com/gtrfrfnyjq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ppjwa.cn/gtvfrckkug.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangkeji.top/gtzavrpocl.html

Ruby: arr.map(&:upcase)
来源：http://hz.hnxiangtu.top/gtghhwpnxk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xingfuxueyuan.xyz/gtubiinnmp.html

[C08] 闭包
来源：http://hz.chenjidiqi.icu/gtnhlbbeqc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jlsjyb.cn/gtsyibuiqq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhongyouzk.top/gtdealylao.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gthfmnfffi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinghuilouyu.cn/gtvzlevvev.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.pycfn.com/gtmnbrrmfo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jiagoushi.top/gtyvdmsfoq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgfzy.top/gtugirzppj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gtgjxblhlw.html

[C09] 递归
来源：http://hz.ppjwa.cn/gtxbbtibmz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhaomingkeji.xyz/gtampgothb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xylfe.cn/gttjushqis.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guannengcc.top/gttlvnbvud.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.birdmap.top/gtnjgaxexr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenlongwang.top/gtlcfvrmsn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sxryk.cn/gtbbatwiqx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ydjk.org.cn/gtzwyyvmdo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xylfe.cn/gtffqltylg.html

[C10] 变量作用域
来源：http://hz.aizwys.cn/gtjgrtuncg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zdqjudy.top/gttqemiyvl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.svipenyu.cn/gtggpkuxzz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xuanzx.com/gtftzbicok.html

TS:   同 JS
来源：http://hz.quarkkingdee.top/gtaqztfoip.html

Java: 方法内为块级作用域
来源：http://hz.tian-w.cn/gtzaaqhlhf.html

Go:   花括号块级作用域
来源：http://hz.cucudq.cn/gtflxesiml.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sweek.top/gtodeqmelb.html

C#:   块级作用域
来源：http://hz.zdqjudy.top/gtkfwrfpyd.html

[C11] 模块导入与导出
来源：http://hz.sufxvd.cn/gtgqzkcssz.html

Py:   from module import func
来源：http://hz.mhx1999.top/gtjlzzftqz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yonumen.top/gtjqacbwjx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jlsjyb.cn/gtdrssxpmd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cqqwz.cn/gtygfpiiyn.html

Java: import java.util.List;
来源：http://hz.ehwqpu.com/gtoiovqzvn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hammf.cn/gtyiggvlem.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.andypj.xyz/gtqhdxfkiw.html

C#:   using System.Text;
来源：http://hz.hnxiangtu.top/gtjnetrqxf.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258.top/gtxayuskeg.html

Py:   (lambda: print("run"))()
来源：http://hz.redwolf501.top/gtayqgmonv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yonumen.top/gtipsrhlyb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.iojbl.cn/gtqohfjdgo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gtzdckuecn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zdqjudy.top/gtynhgcmyp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yanxiufei.cn/gtoeqptyrx.html

Ruby: -> { puts "run" }.call
来源：http://hz.nanxinkj.top/gtgwwxjuqb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.birdmap.top/gtwauydorr.html

[C13] 类型声明 / 类型注解
来源：http://hz.shanyushiyangtech.top/gtuxcirrgc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.kuanghao11.cn/gtgmvbffex.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gtvrbpxjlu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hongshengwenyu.top/gtvdxyiygv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj202588.top/gthsdjitel.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shzxlz.cn/gtxiailowe.html

Go:   func add(a, b int) int
来源：http://hz.mhx1999.top/gttzsobljm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj202588.top/gtckaupqed.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.9152youxi.cn/gtwnkvvann.html

[C14] 泛型函数
来源：http://hz.hongshengwenyu.top/gtbzbelrjm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tian-w.cn/gttvsmkqrs.html

PHP:  // 无泛型
来源：http://hz.wangdashe.top/gtjiwqzsmv.html

JS:   // 无泛型
来源：http://hz.jyoumei.cn/gtcdnlbslj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigufen.top/gtkxnbaogn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenjidiqi.icu/gtfvxlnhwu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.dianchejie.cn/gtltzuknol.html

Ruby: # 无泛型
来源：http://hz.xylfe.cn/gtfcdbarcp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangdashe.top/gtyckaxztm.html

[C15] 解构 / 展开参数
来源：http://hz.c1oappe.top/gtkseqdpbj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.feifeiyinyue.top/gtamlihwcp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.meibo888.top/gtwulbbipy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ehwqpu.com/gtzoibdpct.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fzhhl.top/gtvgzphnyd.html

Java: // 无解构
来源：http://hz.zhiwuduotai.top/gtkyonsrdn.html

Go:   // 无解构
来源：http://hz.cheryme.top/gtqvavjlus.html

Ruby: a, b = pair
来源：http://hz.jyoumei.cn/gtfvcqgzbo.html

C#:   var (a, b) = pair;
来源：http://hz.meibo888.top/gtltwvryog.html

[C16] 函数 / 方法重载
来源：http://hz.sysykeji.top/gtlrmjtqek.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.iojbl.cn/gtozqcdawi.html

PHP:  // 无重载
来源：http://hz.zhixingplan.top/gtelnetzkm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.andypj.xyz/gtsowustpp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhixingplan.top/gtosfabgyf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.feifeiyinyue.top/gtpnewzhly.html

Go:   // 无重载：用不同函数名
来源：http://hz.xziqi.cn/gtbiuodcsx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sweek.top/gtddwhdpai.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuanzhike.top/gtdurjmybb.html

================================================================================
来源：http://hz.ydjk.org.cn/gtcpdlbwwe.html

D. 数组 / 列表 / 集合
来源：http://hz.zhijiandao.cn/gtbmhcvorp.html

================================================================================
来源：http://hz.zycfv.cn/gteomsnzic.html

[D01] 创建数组 / 列表
来源：http://hz.havefunace.top/gtkcvexesy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.fengsongda.top/gtqlcnzift.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jqgufenzy.top/gtmprgquxu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yuanzhike.top/gttacqglzs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zdqjudy.top/gtzyxdjntg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cqqwz.cn/gtgpwxxzks.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pengpengdd.cyou/gtyquasmkf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangtech.top/gtlayfimxs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhengqikj.top/gtrirzavqz.html

[D02] 追加元素到末尾
来源：http://hz.guannengcc.top/gtsyksrsjt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.9152youxi.cn/gtcgozvlez.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.kuanghao11.cn/gtysidtfkk.html

JS:   arr.push(4);
来源：http://hz.fengsongda.top/gtnncqpsfq.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtuoxxqdbp.html

Java: list.add(4);
来源：http://hz.jianghu66.top/gtjbomybfh.html

Go:   arr = append(arr, 4)
来源：http://hz.gaohongyu789.top/gteqxbccul.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jyoumei.cn/gtqhwiaffa.html

C#:   list.Add(4);
来源：http://hz.gaohongyu789.top/gtalfpdtnd.html

[D03] 在指定位置插入元素
来源：http://hz.dashuyun.cn/gtbrpxvvue.html

Py:   arr.insert(0, 0)
来源：http://hz.cdnleiting.top/gtppovvzfq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jiagoushi.top/gtfyskpmsm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.wangshuangyany.cn/gtzzfxxngz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhiwuduotai.top/gtslaitmgi.html

Java: list.add(0, 0);
来源：http://hz.dashuyun.cn/gtfqtoheej.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zdqjudy.top/gtxmlggjac.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jiagoushi.top/gtuihfqsrq.html

C#:   list.Insert(0, 0);
来源：http://hz.9152youxi.cn/gtsgmswshv.html

[D04] 删除元素
来源：http://hz.xingfuxueyuan.xyz/gtrxvcrfro.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuxming.cn/gtoacqkmzb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.havefunace.top/gtzkqmzzuz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.smart0.xyz/gtdjmkpdbs.html

TS:   arr.splice(0, 1);
来源：http://hz.zdqjudy.top/gtblkzycqr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.mhx1999.top/gtzqglsfcs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hfpthk.cn/gthcxdgqmq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuetiantiany.cn/gtvxpjgyah.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xingfuxueyuan.xyz/gtfnswjkbr.html

[D05] 访问与修改元素
来源：http://hz.jyoumei.cn/gtsszbvczf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daxiang520.top/gtjmepmgzs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shanyushiyangtech.top/gtrqouqbue.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.smart0.xyz/gtklqpuhod.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.pycfn.com/gtdoajzzac.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.dianchejie.cn/gtpjcpkhos.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtopqxgxnp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tanke756.top/gtbfjvwzer.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.chenzaomai.com/gtvasekshf.html

[D06] 数组长度
来源：http://hz.jinghuilouyu.cn/gtcjkfaxpc.html

Py:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtrbuwkdni.html

PHP:  count($arr);
来源：http://hz.cucudq.cn/gtkhkgkvpp.html

JS:   arr.length
来源：http://hz.chenjidiqi.icu/gtliguyqwt.html

TS:   arr.length
来源：http://hz.jyoumei.cn/gtiuslzwhu.html

Java: list.size();
来源：http://hz.sxryk.cn/gthqtycwkr.html

Go:   len(arr)
来源：http://hz.yonumen.top/gtfdneuawv.html

Ruby: arr.length; arr.size
来源：http://hz.gaohongyu789.top/gtfpurrxsr.html

C#:   list.Count;
来源：http://hz.jinqigufen.top/gtermjgvqj.html

[D07] 切片 / 取子数组
来源：http://hz.jiagoushi.top/gtpvrwugty.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jlsjyb.cn/gtzaqtvghm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zycfv.cn/gtahonikts.html

JS:   arr.slice(1, 4);
来源：http://hz.yj202588.top/gtemqsvrpy.html

TS:   arr.slice(1, 4);
来源：http://hz.xziqi.cn/gtmxtxusws.html

Java: list.subList(1, 4);
来源：http://hz.svipenyu.cn/gtxqanqizf.html

Go:   arr[1:4]
来源：http://hz.gaohongyu789.top/gtdrcdrcir.html

Ruby: arr[1, 3]
来源：http://hz.haohaochexian.top/gtidwbqprh.html

C#:   list.GetRange(1, 3);
来源：http://hz.cqqwz.cn/gtsrsdfpyw.html

[D08] 合并两个数组
来源：http://hz.yuxming.cn/gtycevvpqw.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenzaomai.com/gtfuypojur.html

PHP:  array_merge($a, $b);
来源：http://hz.zhaomingkeji.xyz/gtlttduhfl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yongpay.top/gtvqpqiigq.html

TS:   [...a, ...b];
来源：http://hz.ywan-chungtsiang.top/gtozxofsed.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xingfuxueyuan.xyz/gtsgikjefx.html

Go:   append(a, b...)
来源：http://hz.vqdsnc.cn/gtjfzmcfyz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cheryme.top/gtjxlsnnzl.html

C#:   a.Concat(b).ToList()
来源：http://hz.52xcode.cn/gtwdfeebsy.html

[D09] 排序（升序）
来源：http://hz.meibo888.top/gtdtaldtbg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dianchejie.cn/gtwhskinpz.html

PHP:  sort($arr);
来源：http://hz.fzhhl.top/gtakhyigps.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gotoacloud.top/gtsamkjhgh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nwbrower.top/gtgancbgqx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.guowangkeji.top/gtzsgjrqvy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cashguo.top/gtbnsfrulf.html

Ruby: arr.sort
来源：http://hz.gogol.net.cn/gtipatyths.html

C#:   list.Sort();
来源：http://hz.pycfn.com/gtvftgoxbe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.9152youxi.cn/gtmeihkhyc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.haohaochexian.top/gtbtjtcydj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuanzx.com/gtnswjysiy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtkcymzpev.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cqqwz.cn/gtkeyspvhu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgfzy.top/gtnbijkaoc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.kuanghao11.cn/gtnyiurlnl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhoulong.xyz/gtuyyaoymt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sweek.top/gtjxtnvdpw.html


<!-- 参考信息 -->