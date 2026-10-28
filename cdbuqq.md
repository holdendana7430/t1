代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gtrpgyxonb.html

[B10] 遍历同时拿索引
来源：http://hz.gogol.net.cn/gtdksvwyle.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sxryk.cn/gtykyugfyk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ydjk.org.cn/gthdihhfok.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.sufxvd.cn/gtfzpmuzvq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yvedp.cn/gtzbhjvjgz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shanyushiyangkeji.top/gtmnmifhkw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cashguo.top/gtdrswyhzd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhixingplan.top/gtnwjrzipy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hnqzz.top/gtfcxcwbsn.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinqigfzy.top/gthneorzhd.html

Py:   list(range(0, 10, 2))
来源：http://hz.kuanghao11.cn/gtjsmultmn.html

PHP:  range(0, 10, 2);
来源：http://hz.sweek.top/gtppidsqtr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhaomingkeji.xyz/gtccxgzulq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hnqzz.top/gtcaworzmz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xuetiantiany.cn/gthqcksosa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.dianchejie.cn/gtznonwuig.html

Ruby: (0...10).step(2).to_a
来源：http://hz.havefunace.top/gtbzqrovlh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.52xcode.cn/gtjdaogopy.html

[B12] 跳出多层循环
来源：http://hz.yonumen.top/gtyzorydnx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jinyuanbaomall.cn/gtfrhdkegk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhengqikj.top/gtfpznnipi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtnhvsuptm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tian-w.cn/gtjhdzpkbl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gtbqfpbezi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.sweek.top/gtgjqxwbzu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hnqzz.top/gtjuogqbfk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.fzhhl.top/gtblugznhy.html

[B13] 判断是否为数字
来源：http://hz.zhaomingkeji.xyz/gtftxvufhl.html

Py:   isinstance(x, (int, float))
来源：http://hz.ywan-chungtsiang.top/gtlvzsayrw.html

PHP:  is_numeric($x)
来源：http://hz.feifeiyinyue.top/gtvyuudfth.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.316326.xyz/gtavhbbskf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hywenlv.cn/gtpyebtand.html

Java: x instanceof Number
来源：http://hz.cqqwz.cn/gtmsujszzl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shanyushiyangkeji.top/gtxnweqoez.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ehwqpu.com/gtiyyzjiwv.html

C#:   x is int or double or decimal
来源：http://hz.cheryme.top/gthegfrxgv.html

[B14] 判断值是否在集合内
来源：http://hz.jinghuilouyu.cn/gtiftsxsbr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.havefunace.top/gtkvxbdneo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ppjwa.cn/gtsgpdnxmd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.iojbl.cn/gtmyiptxts.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.redwolf501.top/gtiklsmwrc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ehwqpu.com/gtyaqovdbi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hysaishi.cn/gtvpkvasxd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.aibaodan.cn/gtylwttpse.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.vqdsnc.cn/gtdhqgykvj.html

[B15] 布尔运算与取反
来源：http://hz.shangyingyoupin.top/gtrfsejkrd.html

Py:   a and b or not c
来源：http://hz.wangshuangyany.cn/gtubyzmtfb.html

PHP:  $a && $b || !$c
来源：http://hz.tianlin.xyz/gtpwxtpimo.html

JS:   a && b || !c
来源：http://hz.birdmap.top/gtmicapxle.html

TS:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtkamhtucr.html

Java: a && b || !c
来源：http://hz.yuanzhike.top/gttbqaehmc.html

Go:   a && b || !c
来源：http://hz.tian-w.cn/gttkypgeyj.html

Ruby: a && b || !c
来源：http://hz.jiagoushi.top/gtnqhvdgfv.html

C#:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtzgghxnam.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zycfv.cn/gtswmsztzl.html

Py:   if not data: return
来源：http://hz.aizwys.cn/gttspfysxh.html

PHP:  if (!$data) { return; }
来源：http://hz.shanyushiyangkeji.top/gtymtlgusu.html

JS:   if (!data) return;
来源：http://hz.fengsongda.top/gtxoejvgpl.html

TS:   if (!data) return;
来源：http://hz.jyoumei.cn/gthxbpumly.html

Java: if (data == null) return;
来源：http://hz.redwolf501.top/gtyzsfkhiw.html

Go:   if data == nil { return }
来源：http://hz.52xcode.cn/gtmhrhpnux.html

Ruby: return if data.nil?
来源：http://hz.shanyushiyangkeji.top/gtfjuxtinn.html

C#:   if (data == null) return;
来源：http://hz.feifeiyinyue.top/gtgxcqjimb.html

================================================================================
来源：http://hz.hfpthk.cn/gtfwhfllyo.html

C. 函数与作用域
来源：http://hz.yj20258.top/gtnognumuq.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtmxztmexz.html

[C01] 定义函数
来源：http://hz.yj202588.top/gtpyygulkl.html

Py:   def add(a, b): return a + b
来源：http://hz.jqgufenzy.top/gtqavpbwxh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xylfe.cn/gtngxubeza.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pycfn.com/gtkaqomcjj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.birdmap.top/gtsmayiacq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yuanzhike.top/gtqkbyozrw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guowangkeji.top/gtmcqbasif.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gzhubu.top/gtugndjhbx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtoqojylli.html

[C02] 默认参数
来源：http://hz.meibo888.top/gtsbguhfam.html

Py:   def greet(name="World"): return name
来源：http://hz.nanxuanxn.top/gtfjrkcvlh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yanxiufei.cn/gtyhowvpuw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cucudq.cn/gtednloftn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xylfe.cn/gtbmvvlidt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jianghu66.top/gtzvzheeqx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.vqdsnc.cn/gtlmvhbocp.html

Ruby: def greet(name = "World") = name
来源：http://hz.chenzaomai.com/gtcjqwhest.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhiwuduotai.top/gtwkcuofnc.html

[C03] 可变参数
来源：http://hz.zhaomingkeji.xyz/gtayvrctzp.html

Py:   def total(*args): return sum(args)
来源：http://hz.gzhubu.top/gtrvfjpqdj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ehwqpu.com/gtgkhehqpt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xylfe.cn/gtpdljubfu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinyuanbaomall.cn/gtsqatjjgc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ydzc1.top/gtonrkpxkz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.pycfn.com/gtfdzejhcl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yvedp.cn/gtcpvkxebi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydjk.org.cn/gtwifnyswm.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sysykeji.top/gtwzculvcg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xylfe.cn/gtjeqfbuom.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.smart0.xyz/gtnubkvsyq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nwbrower.top/gtvurviqzl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xuanzx.com/gtgyrinavq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.vqdsnc.cn/gtihwmyojs.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinghuilouyu.cn/gtiachhvqz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtcxkmhsvl.html

C#:   f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gtumwhvxoo.html

[C05] 返回多个值
来源：http://hz.snrcjt.cn/gtinvfuqbb.html

Py:   return a, b
来源：http://hz.jianghu66.top/gthldijccw.html

PHP:  return [$a, $b];
来源：http://hz.sweek.top/gtfjsudkkq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.wangshuangyany.cn/gtxiharblw.html

TS:   return { a, b };
来源：http://hz.yueranfly.top/gtnykldwjw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yueranfly.top/gtkyekqdth.html

Go:   return a, b
来源：http://hz.cashguo.top/gthdbzpbaj.html

Ruby: return a, b
来源：http://hz.ivvv.top/gtclkkfllp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.birdmap.top/gtzutqdzvl.html

[C06] 匿名函数 / lambda
来源：http://hz.chenjidiqi.icu/gtjqrzfpjf.html

Py:   square = lambda x: x * x
来源：http://hz.quarkkingdee.top/gtpgokrjot.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sxryk.cn/gtvenzdizo.html

JS:   const square = x => x * x;
来源：http://hz.havefunace.top/gtzyqspcej.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xuanzx.com/gtpjdpdybj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shanyushiyangtech.top/gtjkwggtsp.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cdnleiting.top/gtjkidmxzj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xylfe.cn/gtetokqyen.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ehwqpu.com/gtagqgetpl.html

[C07] 把函数作为参数传入
来源：http://hz.cashguo.top/gtdrycjewz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.52xcode.cn/gtbghdspbg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tanke756.top/gtilcdzkvm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhijiandao.cn/gtfuoeally.html

TS:   arr.map(String)
来源：http://hz.fengsongda.top/gtalrdtnbu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shzxlz.cn/gtrzdiuaie.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hnqzz.top/gtkfqzrbhi.html

Ruby: arr.map(&:upcase)
来源：http://hz.quarkkingdee.top/gtgmaksyhp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.havefunace.top/gtlrblerqx.html

[C08] 闭包
来源：http://hz.andypj.xyz/gtlghjyhbx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.feifeiyinyue.top/gtfhfuolqe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinghuilouyu.cn/gtovkbevfv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj20258888.top/gtngzfdwxw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtbbnpzglt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jqgufenzy.top/gtlxcdoqil.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jqgfzy.top/gtornchhyj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.feifeiyinyue.top/gtajongcik.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gthmencggv.html

[C09] 递归
来源：http://hz.zhengqikj.top/gtygtcjuna.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.vqdsnc.cn/gtcheaalmn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.haohaochexian.top/gtkmdglxyk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jlsjyb.cn/gtmldgpnmv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jiagoushi.top/gtgajssqan.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tian-w.cn/gtawvlddfm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jlsjyb.cn/gtyxeqpuxp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jqgfzy.top/gtzsjcttdi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.fengsongda.top/gtvznkxkbt.html

[C10] 变量作用域
来源：http://hz.zycfv.cn/gtmtwblugw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jlsjyb.cn/gtoowtayiz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.kuanghao11.cn/gtaaajckqv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinqigfzy.top/gtqhjmdxat.html

TS:   同 JS
来源：http://hz.yanxiufei.cn/gttvsteash.html

Java: 方法内为块级作用域
来源：http://hz.gotoacloud.top/gthskrxugs.html

Go:   花括号块级作用域
来源：http://hz.jianghu66.top/gtnryhmsvj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.feifeiyinyue.top/gtzpuzcnmp.html

C#:   块级作用域
来源：http://hz.zhengqikj.top/gtslmhxykw.html

[C11] 模块导入与导出
来源：http://hz.ivvv.top/gtlspusxdv.html

Py:   from module import func
来源：http://hz.zycfv.cn/gtmjelasii.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gogol.net.cn/gtnwqcbggs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xuetiantiany.cn/gtesxkdbqe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.c1oappe.top/gtpoecrlru.html

Java: import java.util.List;
来源：http://hz.fzhhl.top/gtetfplohx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yuanzhike.top/gtnmgcztjn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhiwuduotai.top/gtidhvtasp.html

C#:   using System.Text;
来源：http://hz.gaohongyu789.top/gtxamysrwu.html

[C12] 立即执行函数 IIFE
来源：http://hz.shzxlz.cn/gtgmddcwpp.html

Py:   (lambda: print("run"))()
来源：http://hz.jinyuanbaomall.cn/gtcgtmpcev.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jqgfzy.top/gtsyenzubl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtdqulidpm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtxsgccnaa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xinyue.icu/gtljsgfigv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydzc1.top/gtnezkdigq.html

Ruby: -> { puts "run" }.call
来源：http://hz.jqgufenzy.top/gtuituqfmd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258888.top/gtithzbwlx.html

[C13] 类型声明 / 类型注解
来源：http://hz.svipenyu.cn/gtcyilpgwr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtffrkzucd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtirepmavr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pengpengdd.cyou/gtdcgjhwaz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gtzhgfyulb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gteftxnauf.html

Go:   func add(a, b int) int
来源：http://hz.haohaochexian.top/gtqdlbrpsb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinghuilouyu.cn/gthorfomub.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.bjfxy.top/gthbcmngxa.html

[C14] 泛型函数
来源：http://hz.bjfxy.top/gtycfjmisd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hysaishi.cn/gtpicevyxb.html

PHP:  // 无泛型
来源：http://hz.bjfxy.top/gtquywkzql.html

JS:   // 无泛型
来源：http://hz.chenlongwang.top/gtgvhssyvs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dashuyun.cn/gtkhfpbnlg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.fzhhl.top/gtunkvsjqe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shangyingyoupin.top/gtohepgvhv.html

Ruby: # 无泛型
来源：http://hz.shuidangran.top/gttqojdyzt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinghuilouyu.cn/gteftdxkvs.html

[C15] 解构 / 展开参数
来源：http://hz.yuanzhike.top/gtlfnktgyk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhaomingkeji.xyz/gtqzafmsqd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cucudq.cn/gtxzzlmftc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ivvv.top/gtulscmumm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hongshengwenyu.top/gtnwdiubpi.html

Java: // 无解构
来源：http://hz.cqqwz.cn/gtgouggnbh.html

Go:   // 无解构
来源：http://hz.xinyue.icu/gtwxxyhsre.html

Ruby: a, b = pair
来源：http://hz.gzhubu.top/gtbzpihcvx.html

C#:   var (a, b) = pair;
来源：http://hz.hongshengwenyu.top/gthbnhymgd.html

[C16] 函数 / 方法重载
来源：http://hz.vqdsnc.cn/gtzlfjsfgg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.c1oappe.top/gthmlfqkkq.html

PHP:  // 无重载
来源：http://hz.xziqi.cn/gtgsevxrmz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hywenlv.cn/gthbzjfggc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.aizwys.cn/gtrxqogmuo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.kuanghao11.cn/gtyeffkdnp.html

Go:   // 无重载：用不同函数名
来源：http://hz.yonumen.top/gtehlabdou.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dianchejie.cn/gtobrmlref.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jiagoushi.top/gtpwlxcndj.html

================================================================================
来源：http://hz.meibo888.top/gtfftvkkot.html

D. 数组 / 列表 / 集合
来源：http://hz.hnqzz.top/gttphexexw.html

================================================================================
来源：http://hz.tian-w.cn/gtaohejlkw.html

[D01] 创建数组 / 列表
来源：http://hz.ydzc1.top/gthvxhgqsk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhaomingkeji.xyz/gtguzodnuq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.snrcjt.cn/gtounagzdt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hnqzz.top/gttqlzdyga.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhiwuduotai.top/gteypngqpz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nwbrower.top/gtjidtxofk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yvedp.cn/gtqaxewpaw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hammf.cn/gtkdejyhzx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xylfe.cn/gtrlukizis.html

[D02] 追加元素到末尾
来源：http://hz.xziqi.cn/gtriefgthe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhaomingkeji.xyz/gtipzqfajm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.birdmap.top/gtshzpsdhk.html

JS:   arr.push(4);
来源：http://hz.iojbl.cn/gtpygdkwcw.html

TS:   arr.push(4);
来源：http://hz.jlsjyb.cn/gtanarjssj.html

Java: list.add(4);
来源：http://hz.ydjk.org.cn/gtrrdlhhsu.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxuanxn.top/gtimtbnifg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.smart0.xyz/gtyofmzirz.html

C#:   list.Add(4);
来源：http://hz.jinqigufen.top/gtvmxazmey.html

[D03] 在指定位置插入元素
来源：http://hz.yanxiufei.cn/gtmvsvxjhb.html

Py:   arr.insert(0, 0)
来源：http://hz.xylfe.cn/gtmyzfbnxn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yangfankeji.com/gthtkuvdpp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhongyouzk.top/gtbdbkneod.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.bjfxy.top/gttbapxqfk.html

Java: list.add(0, 0);
来源：http://hz.sweek.top/gtmvatzkuu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhaomingkeji.xyz/gtyrosqdwx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenlongwang.top/gtixvjbcpk.html

C#:   list.Insert(0, 0);
来源：http://hz.zdqjudy.top/gtmargorny.html

[D04] 删除元素
来源：http://hz.yanxiufei.cn/gtbuoafkuh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yonumen.top/gtllwshzlt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.svipenyu.cn/gtikooqlvv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.kuanghao11.cn/gtewwzvswf.html

TS:   arr.splice(0, 1);
来源：http://hz.jlsjyb.cn/gtqfavefbp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangdashe.top/gtewgxoriu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.9152youxi.cn/gtcyhdponx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxinkj.top/gtsllmkhut.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ywan-chungtsiang.top/gtxawniivo.html

[D05] 访问与修改元素
来源：http://hz.ppjwa.cn/gtkvjvcass.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtixwbknby.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.svipenyu.cn/gthmqinrer.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yvedp.cn/gtoqzniivr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ppjwa.cn/gttyemakfu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhengqikj.top/gtouvljobx.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtdbrxnncx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtvvedeamj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhijiandao.cn/gtokhgdnjh.html

[D06] 数组长度
来源：http://hz.guannengcc.top/gtqpkxdjjy.html

Py:   len(arr)
来源：http://hz.guannengcc.top/gtxdytgpip.html

PHP:  count($arr);
来源：http://hz.cashguo.top/gtfzjovfff.html

JS:   arr.length
来源：http://hz.cashguo.top/gtfmjmrlpb.html

TS:   arr.length
来源：http://hz.yj20258888.top/gtupqatvel.html

Java: list.size();
来源：http://hz.tian-w.cn/gtmbrsqiqq.html

Go:   len(arr)
来源：http://hz.nwbrower.top/gthcgsfizz.html

Ruby: arr.length; arr.size
来源：http://hz.jinqigufen.top/gtshvwhlri.html

C#:   list.Count;
来源：http://hz.redwolf501.top/gtaonpoehj.html

[D07] 切片 / 取子数组
来源：http://hz.gogol.net.cn/gtrqyrbqqq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.guannengcc.top/gtlruuacln.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.havefunace.top/gtxntsxsmn.html

JS:   arr.slice(1, 4);
来源：http://hz.chenjidiqi.icu/gtrsscyuer.html

TS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtnrdoktti.html

Java: list.subList(1, 4);
来源：http://hz.0kj1m.cn/gtgeaxwgqh.html

Go:   arr[1:4]
来源：http://hz.andypj.xyz/gtqclpwzqy.html

Ruby: arr[1, 3]
来源：http://hz.yuxming.cn/gtdgzusyrp.html

C#:   list.GetRange(1, 3);
来源：http://hz.ybcxt.top/gtgvgsvtde.html

[D08] 合并两个数组
来源：http://hz.52xcode.cn/gtmdstkrwv.html

Py:   a + b;  a.extend(b)
来源：http://hz.c1oappe.top/gtnllqonlf.html

PHP:  array_merge($a, $b);
来源：http://hz.aibaodan.cn/gtteorjwbx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.52xcode.cn/gtjbviajfd.html

TS:   [...a, ...b];
来源：http://hz.wangshuangyany.cn/gtkwndzgjw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.smart0.xyz/gtqkiktfol.html

Go:   append(a, b...)
来源：http://hz.zhengqikj.top/gteehkjdwz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gtcobyndiz.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhoulong.xyz/gtnyzbiueh.html

[D09] 排序（升序）
来源：http://hz.daria6918.cn/gtfqnjqqez.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangdashe.top/gtorvbyjvn.html

PHP:  sort($arr);
来源：http://hz.ppjwa.cn/gtpegyvmqc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sufxvd.cn/gtqpgyrwht.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuanzx.com/gtxdazjokc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hfpthk.cn/gtaidoopkn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yongpay.top/gtkxzlkswe.html

Ruby: arr.sort
来源：http://hz.zhoulong.xyz/gtmcmqniis.html

C#:   list.Sort();
来源：http://hz.gogol.net.cn/gtrotkriaf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj20258888.top/gtbzshikyw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.quarkkingdee.top/gttnxhabmb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinyuanbaomall.cn/gtxpfgtoni.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydjk.org.cn/gtdajuawvt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cqqwz.cn/gtnhmcfyun.html


<!-- 参考信息 -->