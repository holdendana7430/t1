代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gtwftgfnsv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhaomingkeji.xyz/gtlxettfvz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.aizwys.cn/gtdsnxbkqo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tanke756.top/gtroawwquk.html

[B13] 判断是否为数字
来源：http://hz.zhengqikj.top/gthuodlftc.html

Py:   isinstance(x, (int, float))
来源：http://hz.cashguo.top/gttldqenrv.html

PHP:  is_numeric($x)
来源：http://hz.zhoulong.xyz/gtchcaxrxc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cqqwz.cn/gtwnoprrzo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gtyaruteus.html

Java: x instanceof Number
来源：http://hz.dashuyun.cn/gtmjjyqefn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.gogol.net.cn/gtramtcqwn.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yuxming.cn/gtuixkylvm.html

C#:   x is int or double or decimal
来源：http://hz.ywan-chungtsiang.top/gtvdndkvfv.html

[B14] 判断值是否在集合内
来源：http://hz.316326.xyz/gtqjfoglha.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hysaishi.cn/gtmicommsu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sweek.top/gtfupmcycv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xuetiantiany.cn/gtyznzeisg.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.tian-w.cn/gtnsumgihw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zycfv.cn/gtazurrydu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jlsjyb.cn/gtvovgdvjo.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hnqzz.top/gtxtcubgjr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.shuidangran.top/gtrbaczjjy.html

[B15] 布尔运算与取反
来源：http://hz.nanxinkj.top/gtdepqwvbu.html

Py:   a and b or not c
来源：http://hz.zhoulong.xyz/gtsaulpspb.html

PHP:  $a && $b || !$c
来源：http://hz.shangyingyoupin.top/gtllmijmqq.html

JS:   a && b || !c
来源：http://hz.cheryme.top/gttwmifkqb.html

TS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gthfanjkdr.html

Java: a && b || !c
来源：http://hz.sufxvd.cn/gtippppsey.html

Go:   a && b || !c
来源：http://hz.guannengcc.top/gtwlchbbbz.html

Ruby: a && b || !c
来源：http://hz.daxiang520.top/gtpmuvhpco.html

C#:   a && b || !c
来源：http://hz.jinqigfzy.top/gtihntmolz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jqgufenzy.top/gtdfnjlbcr.html

Py:   if not data: return
来源：http://hz.sxryk.cn/gtbifxthfk.html

PHP:  if (!$data) { return; }
来源：http://hz.gotoacloud.top/gtwjwjfizq.html

JS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtiobabfzu.html

TS:   if (!data) return;
来源：http://hz.zhoulong.xyz/gtsnsnmlfm.html

Java: if (data == null) return;
来源：http://hz.jqgfzy.top/gtkcmqakgx.html

Go:   if data == nil { return }
来源：http://hz.daxiang520.top/gthldxlhdl.html

Ruby: return if data.nil?
来源：http://hz.cqqwz.cn/gtxnwecnod.html

C#:   if (data == null) return;
来源：http://hz.jinghuilouyu.cn/gtrldkfdta.html

================================================================================
来源：http://hz.jianghu66.top/gtexjitpex.html

C. 函数与作用域
来源：http://hz.jinyuanbaomall.cn/gthgotjqhh.html

================================================================================
来源：http://hz.gotoacloud.top/gtzmcfekxk.html

[C01] 定义函数
来源：http://hz.shanyushiyangtech.top/gtsnuvirgj.html

Py:   def add(a, b): return a + b
来源：http://hz.yangfankeji.com/gtkywvcqfd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtqfxzabyw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xuanzx.com/gtgtotihjy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.9152youxi.cn/gtnaquovss.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tianlin.xyz/gtstanmcae.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhixingplan.top/gtilpurfnf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hysaishi.cn/gtyufyassa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtkpufqycb.html

[C02] 默认参数
来源：http://hz.yueranfly.top/gtaupuhfzu.html

Py:   def greet(name="World"): return name
来源：http://hz.zhijiandao.cn/gtgmxurqqf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fengsongda.top/gtdavbhlli.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gttlifosfk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.dashuyun.cn/gtdprgiupg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nanxuanxn.top/gtxcltcxmo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.wangdashe.top/gtulloqfnx.html

Ruby: def greet(name = "World") = name
来源：http://hz.sufxvd.cn/gtgzcpnpqh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jlsjyb.cn/gthgtymfdz.html

[C03] 可变参数
来源：http://hz.ywan-chungtsiang.top/gtdqllbgxd.html

Py:   def total(*args): return sum(args)
来源：http://hz.yueranfly.top/gtlmqsygcv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.gogol.net.cn/gtlmfxfwxj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinghuilouyu.cn/gtduvvrvku.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtperulift.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hongshengwenyu.top/gtgotvihrw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhongyouzk.top/gtscpmzyps.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydzc1.top/gtthsrgbnz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yonumen.top/gtkozdxvnz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sufxvd.cn/gtgxfnzjty.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hnxiangtu.top/gtjeaeywyg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhaomingkeji.xyz/gtyvxnhycs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gtxrgibndv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yuanzhike.top/gtvgxxgyyi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jqgufenzy.top/gtqdlhhski.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj20258.top/gtzypeqplr.html

Ruby: f(a: 1, b: 2)
来源：http://hz.snrcjt.cn/gtmkekvmjd.html

C#:   f(a: 1, b: 2)
来源：http://hz.kuanghao11.cn/gtjahzzkfd.html

[C05] 返回多个值
来源：http://hz.daria6918.cn/gtyrlcdabz.html

Py:   return a, b
来源：http://hz.jinqigufen.top/gtycsvwuqq.html

PHP:  return [$a, $b];
来源：http://hz.wangdashe.top/gtmyrensnu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cdnleiting.top/gtsnohcrmk.html

TS:   return { a, b };
来源：http://hz.meibo888.top/gtdtizyjyf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.mhx1999.top/gtyknjusco.html

Go:   return a, b
来源：http://hz.zhijiandao.cn/gtoormhucs.html

Ruby: return a, b
来源：http://hz.hongshengwenyu.top/gtikgrbfuw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydjk.org.cn/gttnpcrufe.html

[C06] 匿名函数 / lambda
来源：http://hz.feifeiyinyue.top/gtubnruniq.html

Py:   square = lambda x: x * x
来源：http://hz.tian-w.cn/gtioeonxwv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.haohaochexian.top/gtswofmeyn.html

JS:   const square = x => x * x;
来源：http://hz.zhengqikj.top/gtgrmpczlm.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yj202588.top/gtnfveymur.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ywan-chungtsiang.top/gtodudmqvo.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xuetiantiany.cn/gteapppvai.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jqgufenzy.top/gtyzbcmcow.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ydzc1.top/gtdaefoptw.html

[C07] 把函数作为参数传入
来源：http://hz.gaohongyu789.top/gtofmbrqkc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shanyushiyangtech.top/gtlwehasli.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj202588.top/gtbiectxqa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinghuilouyu.cn/gtqvmtzkhq.html

TS:   arr.map(String)
来源：http://hz.yvedp.cn/gtlejakelf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xziqi.cn/gtpnnqrfpj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhongyouzk.top/gtyexdbiel.html

Ruby: arr.map(&:upcase)
来源：http://hz.ywan-chungtsiang.top/gtwlaornet.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.dianchejie.cn/gtnyfikuof.html

[C08] 闭包
来源：http://hz.chenjidiqi.icu/gtnibvkdzw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangtech.top/gtgceszgxy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jqgfzy.top/gtwxuqeeoi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gtxslvdytj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.redwolf501.top/gtkhclswgz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hnqzz.top/gtzfmihtld.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shzxlz.cn/gtjgyvxcjc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pycfn.com/gtooclmohc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtnwnxidet.html

[C09] 递归
来源：http://hz.iojbl.cn/gtroutbvfy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ydzc1.top/gtswbocvmh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shuidangran.top/gtttyzlrtn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gternixamy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinghuilouyu.cn/gtrmrxlruz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhiwuduotai.top/gtgcogzmyq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zycfv.cn/gtlecoblej.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ydzc1.top/gtgrzidptg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yangfankeji.com/gtjrdxrqik.html

[C10] 变量作用域
来源：http://hz.gaohongyu789.top/gtooqmtywa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cucudq.cn/gtrcctuxvi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tian-w.cn/gtlmdelosu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hongshengwenyu.top/gtybxbllip.html

TS:   同 JS
来源：http://hz.jlsjyb.cn/gtbpqmmerb.html

Java: 方法内为块级作用域
来源：http://hz.gogol.net.cn/gtosufvrhj.html

Go:   花括号块级作用域
来源：http://hz.mhx1999.top/gtbarhfkii.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jiagoushi.top/gtpgyhpivu.html

C#:   块级作用域
来源：http://hz.chenzaomai.com/gtqkrmirnn.html

[C11] 模块导入与导出
来源：http://hz.52xcode.cn/gtvpjxthdm.html

Py:   from module import func
来源：http://hz.yj20258.top/gtoxbcfxdg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.snrcjt.cn/gtansxgntb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dianchejie.cn/gtnxbwrisl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.havefunace.top/gtjqmqgerw.html

Java: import java.util.List;
来源：http://hz.hywenlv.cn/gtsregakoc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhixingplan.top/gtpsrvptux.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.gaohongyu789.top/gtzundjcgk.html

C#:   using System.Text;
来源：http://hz.hywenlv.cn/gtpcwzqerc.html

[C12] 立即执行函数 IIFE
来源：http://hz.snrcjt.cn/gtthuromdq.html

Py:   (lambda: print("run"))()
来源：http://hz.jiagoushi.top/gtdkpuvgnu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj20258888.top/gtymuzswvu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.chenlongwang.top/gtokvyoryy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.daria6918.cn/gtqcesllyv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.dashuyun.cn/gtqgogjskj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hfpthk.cn/gtmdrsmpjm.html

Ruby: -> { puts "run" }.call
来源：http://hz.zdqjudy.top/gthaczymqr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.dashuyun.cn/gtzfpcfjbt.html

[C13] 类型声明 / 类型注解
来源：http://hz.chenlongwang.top/gtltiveitr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jyoumei.cn/gtnataxrey.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtctcefwib.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinyuanbaomall.cn/gtidkpgnti.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gtctyslcph.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gtjiferbsy.html

Go:   func add(a, b int) int
来源：http://hz.wangdashe.top/gteywasvex.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuxming.cn/gtkkamunah.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.tian-w.cn/gtikievvdk.html

[C14] 泛型函数
来源：http://hz.shuidangran.top/gthjeamihp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.0kj1m.cn/gtkunjvzxx.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangkeji.top/gtoggsmnad.html

JS:   // 无泛型
来源：http://hz.52xcode.cn/gtglxwpphf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sxryk.cn/gtqhvipyhu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.birdmap.top/gtrtjjlieg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jiagoushi.top/gtshrlxxby.html

Ruby: # 无泛型
来源：http://hz.fzhhl.top/gtbhkmxptc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuanzx.com/gtpjoiwsty.html

[C15] 解构 / 展开参数
来源：http://hz.yj20258888.top/gtpbopqgxv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhaomingkeji.xyz/gtxkrebcmg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xuanzx.com/gthmcmocec.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jiagoushi.top/gtfhksvltj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhaomingkeji.xyz/gtqyrichjj.html

Java: // 无解构
来源：http://hz.zdqjudy.top/gtwcbrodtm.html

Go:   // 无解构
来源：http://hz.shzxlz.cn/gtvdkpbjky.html

Ruby: a, b = pair
来源：http://hz.316326.xyz/gtvdapunqn.html

C#:   var (a, b) = pair;
来源：http://hz.jqgufenzy.top/gtrpblcubd.html

[C16] 函数 / 方法重载
来源：http://hz.jyoumei.cn/gtqymgqbsj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.daria6918.cn/gtlchgmixr.html

PHP:  // 无重载
来源：http://hz.shanyushiyangtech.top/gtqhohrgbw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigufen.top/gtbsvbewfm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cqqwz.cn/gtlrhxwqzm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yueranfly.top/gtzfvcnsbn.html

Go:   // 无重载：用不同函数名
来源：http://hz.nwbrower.top/gtzjriqdrn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.fzhhl.top/gtndjagbee.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.fengsongda.top/gtyzlsoaky.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtkgwhdcex.html

D. 数组 / 列表 / 集合
来源：http://hz.xuanzx.com/gtqzogbfpc.html

================================================================================
来源：http://hz.9152youxi.cn/gtdnepnhkk.html

[D01] 创建数组 / 列表
来源：http://hz.haohaochexian.top/gtbpavqnmp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ehwqpu.com/gtkitzsmbm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sxryk.cn/gtxbevpomm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.wangdashe.top/gtzzuuhlic.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuetiantiany.cn/gtbtkuekqq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj202588.top/gtzrhtmdno.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gaohongyu789.top/gtumviscyx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daxiang520.top/gtwosmvmps.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ybcxt.top/gtmxmmjfaz.html

[D02] 追加元素到末尾
来源：http://hz.nanxuanxn.top/gtyilaaojb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nanxuanxn.top/gttwthyyxh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhijiandao.cn/gtovedjmgh.html

JS:   arr.push(4);
来源：http://hz.cashguo.top/gtmpmbhrrj.html

TS:   arr.push(4);
来源：http://hz.xylfe.cn/gtdeugczgs.html

Java: list.add(4);
来源：http://hz.shuidangran.top/gtrsvmlwwa.html

Go:   arr = append(arr, 4)
来源：http://hz.tianlin.xyz/gtsvinngyo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuanzhike.top/gtapsuwrlw.html

C#:   list.Add(4);
来源：http://hz.jinyuanbaomall.cn/gtqlhzkdvd.html

[D03] 在指定位置插入元素
来源：http://hz.316326.xyz/gtpdzxuqhq.html

Py:   arr.insert(0, 0)
来源：http://hz.bjfxy.top/gtifgrjztr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.dashuyun.cn/gtjpllkrwz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gogol.net.cn/gtritnrtbt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jyoumei.cn/gtewyolzfh.html

Java: list.add(0, 0);
来源：http://hz.dianchejie.cn/gtqfsfksbo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.mhx1999.top/gteblvmgjh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yanxiufei.cn/gtvnbxgnlt.html

C#:   list.Insert(0, 0);
来源：http://hz.sweek.top/gtpjznhokp.html

[D04] 删除元素
来源：http://hz.guowangkeji.top/gtndhfvjjm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fengsongda.top/gthxdhdpqd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xingfuxueyuan.xyz/gtyvtxanji.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhijiandao.cn/gtsnpfrcwj.html

TS:   arr.splice(0, 1);
来源：http://hz.shangyingyoupin.top/gtdmggxeit.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.feifeiyinyue.top/gtqogrkzvg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cqqwz.cn/gtuntrvdej.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jlsjyb.cn/gtniebjgbe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.snrcjt.cn/gtlfzoqccd.html

[D05] 访问与修改元素
来源：http://hz.chenlongwang.top/gtfwaoubxh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtrfejjjxc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gogol.net.cn/gtaiiacapg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtazsmvwsm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhengqikj.top/gtqxobvcha.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jiagoushi.top/gtmvxkayay.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtdkcmewvj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtpkunzuix.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sufxvd.cn/gtawciqqqh.html

[D06] 数组长度
来源：http://hz.ehwqpu.com/gtgnselqzz.html

Py:   len(arr)
来源：http://hz.ppjwa.cn/gtlkbimoga.html

PHP:  count($arr);
来源：http://hz.snrcjt.cn/gtglentpox.html

JS:   arr.length
来源：http://hz.zhongyouzk.top/gtobjcdjsb.html

TS:   arr.length
来源：http://hz.shanyushiyangkeji.top/gtkbeuaexk.html

Java: list.size();
来源：http://hz.yj20258888.top/gtnndfqzpy.html

Go:   len(arr)
来源：http://hz.zhijiandao.cn/gtodlvibet.html

Ruby: arr.length; arr.size
来源：http://hz.daxiang520.top/gtqrngbcfc.html

C#:   list.Count;
来源：http://hz.aibaodan.cn/gtxcuxqpbz.html

[D07] 切片 / 取子数组
来源：http://hz.xingfuxueyuan.xyz/gtcvsgifbn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.dianchejie.cn/gtyvsdlojd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yongpay.top/gtataifmcz.html

JS:   arr.slice(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtfkdxznvh.html

TS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtflozicrw.html

Java: list.subList(1, 4);
来源：http://hz.xuetiantiany.cn/gtxruozwtf.html

Go:   arr[1:4]
来源：http://hz.sweek.top/gtlkgsnzmb.html

Ruby: arr[1, 3]
来源：http://hz.jiagoushi.top/gtgqzbkenh.html

C#:   list.GetRange(1, 3);
来源：http://hz.xingfuxueyuan.xyz/gtovgpanhw.html

[D08] 合并两个数组
来源：http://hz.jinghuilouyu.cn/gtknjkgwiv.html

Py:   a + b;  a.extend(b)
来源：http://hz.jlsjyb.cn/gtftucqtln.html

PHP:  array_merge($a, $b);
来源：http://hz.yuxming.cn/gtoehbivwb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ybcxt.top/gtuwzzfsgj.html

TS:   [...a, ...b];
来源：http://hz.ybcxt.top/gttpozyddt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydjk.org.cn/gtgmxybzie.html

Go:   append(a, b...)
来源：http://hz.ehwqpu.com/gtngogqfcu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ehwqpu.com/gtbdruginh.html

C#:   a.Concat(b).ToList()
来源：http://hz.yuxming.cn/gtmszzhnbm.html

[D09] 排序（升序）
来源：http://hz.dianchejie.cn/gtrecqbytt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gtyjkpqddr.html

PHP:  sort($arr);
来源：http://hz.nanxinkj.top/gtudjeycqr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aizwys.cn/gtmjbeybhv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.nwbrower.top/gtuivzwlbi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj202588.top/gtyplijiir.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangtech.top/gtkkbwwqth.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtgrfbswfd.html

C#:   list.Sort();
来源：http://hz.jinyuanbaomall.cn/gtwxsyjtot.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangshuangyany.cn/gtnoszmlio.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangdashe.top/gtcwadcmdr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hfpthk.cn/gtdxfjtoqs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.c1oappe.top/gtqvbiqjdr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gtjfjvcjcu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.quarkkingdee.top/gtfyyivvcf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gaohongyu789.top/gtpcitluam.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.guannengcc.top/gtnbqwwhcc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shanyushiyangtech.top/gtdmffreun.html

[D11] 反转数组
来源：http://hz.zhongyouzk.top/gttbcuhwid.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yongpay.top/gtodtdxxpu.html

PHP:  array_reverse($arr);
来源：http://hz.shangyingyoupin.top/gtgvcfxqea.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sysykeji.top/gtnnonciyw.html

TS:   [...arr].reverse();
来源：http://hz.iojbl.cn/gtowbtbefa.html

Java: Collections.reverse(list);
来源：http://hz.gotoacloud.top/gtvonzbfcc.html

Go:   slices.Reverse(arr)
来源：http://hz.haohaochexian.top/gtmywargca.html

Ruby: arr.reverse
来源：http://hz.c1oappe.top/gtqczjnrxi.html

C#:   list.Reverse();
来源：http://hz.cheryme.top/gtpwjnnrhs.html

[D12] 查找元素下标
来源：http://hz.dianchejie.cn/gtrrackeer.html

Py:   arr.index(x);  x in arr
来源：http://hz.xuanzx.com/gtzsxjnjso.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.mhx1999.top/gtuvsppunf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gtcacstnxa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ehwqpu.com/gtzkvakuno.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ehwqpu.com/gtnuxjnabj.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtbzjhgaqq.html

Ruby: arr.index(x)
来源：http://hz.tian-w.cn/gtsmtnerpf.html

C#:   list.IndexOf(x);
来源：http://hz.yonumen.top/gtnnvqcndu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sweek.top/gtehfalxkc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cdnleiting.top/gtpxttjwni.html


<!-- 参考信息 -->