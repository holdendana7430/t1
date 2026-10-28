代发 wailian999

PHP:  range(0, 10, 2);
来源：http://hz.xinyue.icu/gtckabwqix.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.meibo888.top/gthrpzxqlt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gaohongyu789.top/gtvkwlmxex.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xinyue.icu/gtqxmtnnhl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.iojbl.cn/gtmqmtnmtb.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ivvv.top/gtjwqgcsel.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zycfv.cn/gtpzutxipc.html

[B12] 跳出多层循环
来源：http://hz.0kj1m.cn/gtlisdxuiy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.pycfn.com/gthnpwooaf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.tianlin.xyz/gtfwjrpfir.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guannengcc.top/gtlddicgko.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gtercsdrvq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtidihzgzr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenjidiqi.icu/gtaskmomzx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.birdmap.top/gtrjtfxcfl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hongshengwenyu.top/gtusjxrkxh.html

[B13] 判断是否为数字
来源：http://hz.xuanzx.com/gtcrrqqqeo.html

Py:   isinstance(x, (int, float))
来源：http://hz.gotoacloud.top/gtnsiegsfy.html

PHP:  is_numeric($x)
来源：http://hz.bjfxy.top/gtekeqqooi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258888.top/gtfzoeoptn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tanke756.top/gtbixvjapg.html

Java: x instanceof Number
来源：http://hz.ehwqpu.com/gtmtoknify.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.haohaochexian.top/gtdjtqhoqq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yj20258.top/gtbwkqodpd.html

C#:   x is int or double or decimal
来源：http://hz.cqqwz.cn/gtagatdwlu.html

[B14] 判断值是否在集合内
来源：http://hz.shanyushiyangtech.top/gttyagbwqw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhiwuduotai.top/gtxjlvxkbm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hammf.cn/gtdcuhfnpg.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinghuilouyu.cn/gtzdnmzziu.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sysykeji.top/gtvwcndxts.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tian-w.cn/gtlqfblvik.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.feifeiyinyue.top/gtlomecddi.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ivvv.top/gtzeoaatkz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhoulong.xyz/gtlpwzooan.html

[B15] 布尔运算与取反
来源：http://hz.guowangkeji.top/gtjmdofcgh.html

Py:   a and b or not c
来源：http://hz.nanxinkj.top/gtdbnywtbs.html

PHP:  $a && $b || !$c
来源：http://hz.havefunace.top/gtnplxabzg.html

JS:   a && b || !c
来源：http://hz.aizwys.cn/gtbbuyybml.html

TS:   a && b || !c
来源：http://hz.yj202588.top/gtkkislobh.html

Java: a && b || !c
来源：http://hz.xuanzx.com/gtlgxwztsv.html

Go:   a && b || !c
来源：http://hz.xuanzx.com/gtczpyfdrf.html

Ruby: a && b || !c
来源：http://hz.bjfxy.top/gtezfyqcoa.html

C#:   a && b || !c
来源：http://hz.kuanghao11.cn/gtckelwsyj.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yangfankeji.com/gtmojizmml.html

Py:   if not data: return
来源：http://hz.gotoacloud.top/gtwlcfvmji.html

PHP:  if (!$data) { return; }
来源：http://hz.hywenlv.cn/gtosubeoqb.html

JS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtiitrzwty.html

TS:   if (!data) return;
来源：http://hz.yuanzhike.top/gtcnejosgy.html

Java: if (data == null) return;
来源：http://hz.cucudq.cn/gtwvruesar.html

Go:   if data == nil { return }
来源：http://hz.pycfn.com/gttoqmosyr.html

Ruby: return if data.nil?
来源：http://hz.jinghuilouyu.cn/gtccxwixid.html

C#:   if (data == null) return;
来源：http://hz.jinghuilouyu.cn/gtwvtilink.html

================================================================================
来源：http://hz.yanxiufei.cn/gtygxsgzgm.html

C. 函数与作用域
来源：http://hz.hfpthk.cn/gtwgliitkg.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtscmvwdyl.html

[C01] 定义函数
来源：http://hz.wangdashe.top/gtgwiijtld.html

Py:   def add(a, b): return a + b
来源：http://hz.9152youxi.cn/gtnacnmjem.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jlsjyb.cn/gtfowcbbre.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.andypj.xyz/gtfnklohsx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenzaomai.com/gtrzdujzcp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtlddbsxbs.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yuxming.cn/gthqeefxtb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gogol.net.cn/gtjqmousjy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtpkmusief.html

[C02] 默认参数
来源：http://hz.xinyue.icu/gtyvquknqd.html

Py:   def greet(name="World"): return name
来源：http://hz.shanyushiyangtech.top/gtzhbohiro.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.0kj1m.cn/gtvmcycxmn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.feifeiyinyue.top/gtrpkmkshi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hywenlv.cn/gtngupkugs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangkeji.top/gtdjetbwgt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shangyingyoupin.top/gtdwybyipu.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhengqikj.top/gtktzrnyqv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ydzc1.top/gttyvyovvb.html

[C03] 可变参数
来源：http://hz.snrcjt.cn/gtsjggghvl.html

Py:   def total(*args): return sum(args)
来源：http://hz.mhx1999.top/gtczcduncg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.andypj.xyz/gtepawujai.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aibaodan.cn/gtoajwiggr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gtvwqladwm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daria6918.cn/gtkkgdopli.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sxryk.cn/gtnvbsalbr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sysykeji.top/gtelvdtgnz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xinyue.icu/gtumfwvvzl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sufxvd.cn/gttzoqyjph.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hywenlv.cn/gtkjledmdb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhixingplan.top/gtcgelrfot.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.havefunace.top/gtbzxtoejo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.guannengcc.top/gtksxhqhrf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hysaishi.cn/gtejgcsgtp.html

Go:   // 无：用配置结构体参数
来源：http://hz.svipenyu.cn/gtfaciiqtm.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gthuyyrsxa.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenzaomai.com/gtnouyukmq.html

[C05] 返回多个值
来源：http://hz.sxryk.cn/gtuqrmauha.html

Py:   return a, b
来源：http://hz.jinqigfzy.top/gtsxmpymcm.html

PHP:  return [$a, $b];
来源：http://hz.cashguo.top/gtngycetcm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cdnleiting.top/gtbgwayabi.html

TS:   return { a, b };
来源：http://hz.yj20258888.top/gtziuyaedy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.aibaodan.cn/gtzjnztlkb.html

Go:   return a, b
来源：http://hz.guannengcc.top/gtymndusfr.html

Ruby: return a, b
来源：http://hz.yvedp.cn/gtpmcohunx.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gogol.net.cn/gtmnenmepi.html

[C06] 匿名函数 / lambda
来源：http://hz.guannengcc.top/gtvvckwlsg.html

Py:   square = lambda x: x * x
来源：http://hz.guannengcc.top/gtjddnmyri.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj20258888.top/gttzrbjaxh.html

JS:   const square = x => x * x;
来源：http://hz.guannengcc.top/gtientyzmk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sysykeji.top/gtrrlolhfc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.haohaochexian.top/gtsobfoemv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.haohaochexian.top/gtjyyafgyp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xinyue.icu/gtebbxukkz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ydjk.org.cn/gtdptdeztq.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangtech.top/gtldsiawvp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.aizwys.cn/gthfejoimq.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gotoacloud.top/gtupwdvatu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hnxiangtu.top/gttoxvegnb.html

TS:   arr.map(String)
来源：http://hz.yuxming.cn/gtytyazoue.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shanyushiyangtech.top/gtiuhmcccd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.daxiang520.top/gtjbaielhm.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhaomingkeji.xyz/gtrgkphmam.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhijiandao.cn/gticozmwfz.html

[C08] 闭包
来源：http://hz.jqgufenzy.top/gtmxupjdsv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yvedp.cn/gtcrdhnvxu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cdnleiting.top/gtiobgmnnr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtqydhgtkl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtcgydjzjo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jqgufenzy.top/gtxnwzbwhe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.feifeiyinyue.top/gtnslexlvu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.haohaochexian.top/gtovorlvwm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtpmctaifu.html

[C09] 递归
来源：http://hz.316326.xyz/gtrorwgqzg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.fengsongda.top/gtlhthfhoh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hfpthk.cn/gtfyvdnqvy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.quarkkingdee.top/gtqejkdutu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gzhubu.top/gtgdivbuqn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shuidangran.top/gtgurhmavp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.haohaochexian.top/gtsjvojids.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yongpay.top/gtvqpjexag.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.haohaochexian.top/gttkuvaagy.html

[C10] 变量作用域
来源：http://hz.birdmap.top/gtztsujwgt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cdnleiting.top/gtktsahkot.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sufxvd.cn/gtoyswnmqe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.iojbl.cn/gtbglpoupw.html

TS:   同 JS
来源：http://hz.aibaodan.cn/gtnnhlsygf.html

Java: 方法内为块级作用域
来源：http://hz.jqgufenzy.top/gtmucgyfuw.html

Go:   花括号块级作用域
来源：http://hz.yueranfly.top/gtggokzfrs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.redwolf501.top/gtqkdiriau.html

C#:   块级作用域
来源：http://hz.yuanzhike.top/gtuoejufum.html

[C11] 模块导入与导出
来源：http://hz.sufxvd.cn/gtputzkmmu.html

Py:   from module import func
来源：http://hz.ydjk.org.cn/gtajykvhvb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.smart0.xyz/gtypranady.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.birdmap.top/gtzketnmnr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xinyue.icu/gtizfdbwko.html

Java: import java.util.List;
来源：http://hz.jqgfzy.top/gtriamhdlh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ivvv.top/gtdvflmmjz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hfpthk.cn/gtibsrdnyy.html

C#:   using System.Text;
来源：http://hz.guannengcc.top/gtrznofxpv.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258.top/gtpefgigme.html

Py:   (lambda: print("run"))()
来源：http://hz.jinqigufen.top/gttpzgujpd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.daria6918.cn/gtrgmfzexj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtmkpudeyy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtwoyyefhs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ppjwa.cn/gthswmehse.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.snrcjt.cn/gtkrrqowrs.html

Ruby: -> { puts "run" }.call
来源：http://hz.havefunace.top/gtzgsdwllj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.kuanghao11.cn/gtymhxyphx.html

[C13] 类型声明 / 类型注解
来源：http://hz.yangfankeji.com/gtangpxkim.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ehwqpu.com/gtqtnuyhsn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ywan-chungtsiang.top/gtxoxtmfxt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sweek.top/gtvylqyvtg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shuidangran.top/gtpssdazuk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtcyiotbei.html

Go:   func add(a, b int) int
来源：http://hz.yuanzhike.top/gtuktbmqyh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xuanzx.com/gtbxcpwqmh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guowangkeji.top/gthwvaxmmr.html

[C14] 泛型函数
来源：http://hz.jyoumei.cn/gtqksxvydn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258888.top/gtjvfvgyej.html

PHP:  // 无泛型
来源：http://hz.meibo888.top/gtaxjjvyuf.html

JS:   // 无泛型
来源：http://hz.haohaochexian.top/gtgenvhvgn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.andypj.xyz/gtpzpxdbrf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ydzc1.top/gtgycporsi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.fengsongda.top/gtokzdzimv.html

Ruby: # 无泛型
来源：http://hz.jinghuilouyu.cn/gtgyhmaocv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.andypj.xyz/gtrpntmavw.html

[C15] 解构 / 展开参数
来源：http://hz.yueranfly.top/gtjqsbeglw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cashguo.top/gtotvduakh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhijiandao.cn/gtscgcvpfl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dashuyun.cn/gthrykwsnj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ybcxt.top/gtwnfdfbhp.html

Java: // 无解构
来源：http://hz.yuanzhike.top/gtsullryut.html

Go:   // 无解构
来源：http://hz.svipenyu.cn/gtslaevlal.html

Ruby: a, b = pair
来源：http://hz.hongshengwenyu.top/gtenfmgqhx.html

C#:   var (a, b) = pair;
来源：http://hz.quarkkingdee.top/gtbgiwgleu.html

[C16] 函数 / 方法重载
来源：http://hz.zhoulong.xyz/gtdscfrlcj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hammf.cn/gtuzwrsbgd.html

PHP:  // 无重载
来源：http://hz.c1oappe.top/gtbovqlmie.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.vqdsnc.cn/gtwfrrbqei.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sxryk.cn/gtgolgdvmm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.redwolf501.top/gtsvvleppp.html

Go:   // 无重载：用不同函数名
来源：http://hz.cashguo.top/gtreubhtit.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xingfuxueyuan.xyz/gtyexjvgbb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jqgfzy.top/gtjkelvhhx.html

================================================================================
来源：http://hz.jqgufenzy.top/gtpnvwfrxe.html

D. 数组 / 列表 / 集合
来源：http://hz.zhengqikj.top/gtgsjsodeu.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgdcnkrgj.html

[D01] 创建数组 / 列表
来源：http://hz.ehwqpu.com/gtojetrjga.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yuanzhike.top/gtwtgskpsd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shuidangran.top/gtvhykawdp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yuxming.cn/gtenkejrmw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jiagoushi.top/gtvippywes.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nwbrower.top/gtmmtxlpwg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sufxvd.cn/gtzwdjwbri.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sweek.top/gtbaeslskc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gzhubu.top/gtlrgprnum.html

[D02] 追加元素到末尾
来源：http://hz.jianghu66.top/gtkcireawf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinyuanbaomall.cn/gtplxuqjdk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenzaomai.com/gtfqqcyxwv.html

JS:   arr.push(4);
来源：http://hz.iojbl.cn/gtfbsygocn.html

TS:   arr.push(4);
来源：http://hz.pycfn.com/gtgjdmsbkd.html

Java: list.add(4);
来源：http://hz.havefunace.top/gtpviodevb.html

Go:   arr = append(arr, 4)
来源：http://hz.vqdsnc.cn/gtdftnqmya.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fzhhl.top/gtqzjbjfkj.html

C#:   list.Add(4);
来源：http://hz.pengpengdd.cyou/gtwbmdgjkp.html

[D03] 在指定位置插入元素
来源：http://hz.sysykeji.top/gtfzesnbrb.html

Py:   arr.insert(0, 0)
来源：http://hz.birdmap.top/gtobptlaxc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.aizwys.cn/gtwevdfieq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.redwolf501.top/gteghkglbd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cheryme.top/gtscyxrfsi.html

Java: list.add(0, 0);
来源：http://hz.fzhhl.top/gtkepxmaum.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.quarkkingdee.top/gtasrrunaz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shuidangran.top/gtummtqtqg.html

C#:   list.Insert(0, 0);
来源：http://hz.cheryme.top/gtitbelpov.html

[D04] 删除元素
来源：http://hz.gogol.net.cn/gtfupjvkgj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhijiandao.cn/gtkjegugdo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tian-w.cn/gtaopycebd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sysykeji.top/gtwjgojhqc.html

TS:   arr.splice(0, 1);
来源：http://hz.hnqzz.top/gttxhlcqqy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jlsjyb.cn/gtbjyrtduu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yongpay.top/gtwxlpryju.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj20258.top/gtenkrmkkd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.daria6918.cn/gtreswwdmh.html

[D05] 访问与修改元素
来源：http://hz.iojbl.cn/gtbvkliwtd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtglqwlnwx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jqgfzy.top/gtviilffnf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtlagmclum.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cucudq.cn/gtrpqtqkzk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hongshengwenyu.top/gtwfpfhgiy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ivvv.top/gtnfrdmnld.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yongpay.top/gtjjmvldaa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.vqdsnc.cn/gtuanjrjlc.html

[D06] 数组长度
来源：http://hz.quarkkingdee.top/gttgjakoup.html

Py:   len(arr)
来源：http://hz.meibo888.top/gteuoktovv.html

PHP:  count($arr);
来源：http://hz.zhengqikj.top/gtvccjhtdc.html

JS:   arr.length
来源：http://hz.jqgufenzy.top/gtohwfqjdz.html

TS:   arr.length
来源：http://hz.wangdashe.top/gtzaawjvrk.html

Java: list.size();
来源：http://hz.tian-w.cn/gtrynmnzkm.html

Go:   len(arr)
来源：http://hz.hfpthk.cn/gtipvfdztb.html

Ruby: arr.length; arr.size
来源：http://hz.sxryk.cn/gtcogpkkjy.html

C#:   list.Count;
来源：http://hz.jiagoushi.top/gthotvhuec.html

[D07] 切片 / 取子数组
来源：http://hz.yj202588.top/gtbvjwlnrr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.daria6918.cn/gtdlmlvroz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sweek.top/gtfhaxalfw.html

JS:   arr.slice(1, 4);
来源：http://hz.haohaochexian.top/gtofactgra.html

TS:   arr.slice(1, 4);
来源：http://hz.shuidangran.top/gtaunqvdpe.html

Java: list.subList(1, 4);
来源：http://hz.52xcode.cn/gtgklmizng.html

Go:   arr[1:4]
来源：http://hz.shangyingyoupin.top/gtdlbqthci.html

Ruby: arr[1, 3]
来源：http://hz.9152youxi.cn/gtcakevsvj.html

C#:   list.GetRange(1, 3);
来源：http://hz.tanke756.top/gtcikogvpq.html

[D08] 合并两个数组
来源：http://hz.tanke756.top/gtknnkvlml.html

Py:   a + b;  a.extend(b)
来源：http://hz.feifeiyinyue.top/gtbroorsax.html

PHP:  array_merge($a, $b);
来源：http://hz.tianlin.xyz/gteilrhntw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jiagoushi.top/gtlipngvyo.html

TS:   [...a, ...b];
来源：http://hz.birdmap.top/gtyokmolrt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhaomingkeji.xyz/gttbfevxkw.html

Go:   append(a, b...)
来源：http://hz.ywan-chungtsiang.top/gtrojfjwjs.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xingfuxueyuan.xyz/gthpoelhnb.html

C#:   a.Concat(b).ToList()
来源：http://hz.52xcode.cn/gtjtmdczlu.html

[D09] 排序（升序）
来源：http://hz.gogol.net.cn/gtzgtqxfqp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtsldvlyby.html

PHP:  sort($arr);
来源：http://hz.shanyushiyangtech.top/gtzfzeowvw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gaohongyu789.top/gtuwdvizdj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.smart0.xyz/gtuolehloa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.52xcode.cn/gtgpcbwlim.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258.top/gtwuqqnxsx.html

Ruby: arr.sort
来源：http://hz.gzhubu.top/gtklbgbxzd.html

C#:   list.Sort();
来源：http://hz.jqgfzy.top/gtrwlnknbt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinghuilouyu.cn/gtmgovzvyg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhiwuduotai.top/gtzvzjhzvm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cashguo.top/gtkrvnqdkc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guowangkeji.top/gtqipqojkb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cucudq.cn/gtcxbaoahh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinghuilouyu.cn/gtasusspgd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigfzy.top/gtwctwiyek.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zdqjudy.top/gttkbfwmbr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigfzy.top/gtlpwnuxcl.html

[D11] 反转数组
来源：http://hz.fzhhl.top/gtuyswcjhl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xingfuxueyuan.xyz/gtokeupscq.html

PHP:  array_reverse($arr);
来源：http://hz.ywan-chungtsiang.top/gtnqrmqzez.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuanzx.com/gthqjwnpod.html

TS:   [...arr].reverse();
来源：http://hz.hongshengwenyu.top/gtxttyzgbf.html

Java: Collections.reverse(list);
来源：http://hz.hongshengwenyu.top/gtfshoamgi.html

Go:   slices.Reverse(arr)
来源：http://hz.zhoulong.xyz/gtcsvvefyc.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gtognexwmv.html


<!-- 参考信息 -->