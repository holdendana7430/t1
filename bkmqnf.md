代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cqqwz.cn/gtbpsehgpa.html

Java: x instanceof Number
来源：http://hz.xinyue.icu/gtmypkotbv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ybcxt.top/gtauxuepfd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.birdmap.top/gtxwhiwreq.html

C#:   x is int or double or decimal
来源：http://hz.cdnleiting.top/gtgfvvnqto.html

[B14] 判断值是否在集合内
来源：http://hz.yongpay.top/gtywdgtwal.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yj20258888.top/gtwpbxybgk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhengqikj.top/gtczshhckt.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ehwqpu.com/gtoyinwssi.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.iojbl.cn/gtqkaykcyd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ppjwa.cn/gtmmycfpnm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.haohaochexian.top/gtfguybxfu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jqgufenzy.top/gtiofltcgb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.wangshuangyany.cn/gtfjhnjwtn.html

[B15] 布尔运算与取反
来源：http://hz.havefunace.top/gtapuyohqg.html

Py:   a and b or not c
来源：http://hz.xingfuxueyuan.xyz/gtbaqujcgd.html

PHP:  $a && $b || !$c
来源：http://hz.jinqigfzy.top/gttniweiup.html

JS:   a && b || !c
来源：http://hz.bjfxy.top/gtbmjgyznu.html

TS:   a && b || !c
来源：http://hz.316326.xyz/gtijzbaiia.html

Java: a && b || !c
来源：http://hz.zdqjudy.top/gtzglskfdw.html

Go:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtshvtfeks.html

Ruby: a && b || !c
来源：http://hz.bjfxy.top/gtqiykuvxl.html

C#:   a && b || !c
来源：http://hz.zycfv.cn/gtcgsvqavh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.quarkkingdee.top/gtegopnpws.html

Py:   if not data: return
来源：http://hz.daxiang520.top/gtbzrmcnpi.html

PHP:  if (!$data) { return; }
来源：http://hz.xingfuxueyuan.xyz/gtfjuojspr.html

JS:   if (!data) return;
来源：http://hz.cucudq.cn/gtqwanaiis.html

TS:   if (!data) return;
来源：http://hz.yvedp.cn/gtwprldosj.html

Java: if (data == null) return;
来源：http://hz.mhx1999.top/gtlnsivqfh.html

Go:   if data == nil { return }
来源：http://hz.chenlongwang.top/gtbmpurzeb.html

Ruby: return if data.nil?
来源：http://hz.52xcode.cn/gtoslxjgpx.html

C#:   if (data == null) return;
来源：http://hz.tian-w.cn/gtnzetcyvm.html

================================================================================
来源：http://hz.birdmap.top/gtgxxirwle.html

C. 函数与作用域
来源：http://hz.xingfuxueyuan.xyz/gttaratihf.html

================================================================================
来源：http://hz.hysaishi.cn/gttjjvgiwr.html

[C01] 定义函数
来源：http://hz.yanxiufei.cn/gtngdxqgsv.html

Py:   def add(a, b): return a + b
来源：http://hz.chenzaomai.com/gtawkozqbg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtduxkyisp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtcdjkmrng.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnxiangtu.top/gtxvdcxqcj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtztpdbuqh.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.feifeiyinyue.top/gtnitqfumw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.mhx1999.top/gtjzrzpgrk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtnaagtlcy.html

[C02] 默认参数
来源：http://hz.havefunace.top/gtkqjmbbjg.html

Py:   def greet(name="World"): return name
来源：http://hz.sysykeji.top/gtslhpvamq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.vqdsnc.cn/gtjgtptkqd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenjidiqi.icu/gtrakkgfks.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtgivpbscy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.redwolf501.top/gtzkyaqyxx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.kuanghao11.cn/gtjbdcdljd.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhiwuduotai.top/gtjeopdkap.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.52xcode.cn/gtgynnaegy.html

[C03] 可变参数
来源：http://hz.shzxlz.cn/gtlcimmykq.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhengqikj.top/gtqkhgrdsz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nanxinkj.top/gtfzddeydd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daxiang520.top/gtknfkrmru.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258.top/gtsnhgzqfb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.tanke756.top/gtawyvnsoc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yanxiufei.cn/gtatxzxabr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ehwqpu.com/gtckbnoczv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ehwqpu.com/gteztqraac.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sweek.top/gtlsbtofqk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hongshengwenyu.top/gtwcsasomc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinqigufen.top/gtpnvmvibh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cdnleiting.top/gtvvhiryrl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhixingplan.top/gtsmhspvet.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinghuilouyu.cn/gtijujwqbu.html

Go:   // 无：用配置结构体参数
来源：http://hz.wangshuangyany.cn/gtsfpemuky.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sxryk.cn/gtqzdpjdyw.html

C#:   f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gthopwivmh.html

[C05] 返回多个值
来源：http://hz.shuidangran.top/gtmgqmikmu.html

Py:   return a, b
来源：http://hz.shzxlz.cn/gtlootsguk.html

PHP:  return [$a, $b];
来源：http://hz.guannengcc.top/gtphctqqpi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gzhubu.top/gtuwcofoyb.html

TS:   return { a, b };
来源：http://hz.yuanzhike.top/gttbmkusvo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xylfe.cn/gtntvhyopi.html

Go:   return a, b
来源：http://hz.zhiwuduotai.top/gtlphjnexi.html

Ruby: return a, b
来源：http://hz.xuanzx.com/gtxsyvdxxa.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhongyouzk.top/gtioogkvkt.html

[C06] 匿名函数 / lambda
来源：http://hz.daxiang520.top/gtdfecufqb.html

Py:   square = lambda x: x * x
来源：http://hz.zycfv.cn/gtbmrofgbq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shzxlz.cn/gtdzuvwdfa.html

JS:   const square = x => x * x;
来源：http://hz.jiagoushi.top/gtgqogqfwi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dianchejie.cn/gtitrgjqvg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xuetiantiany.cn/gtazibskyo.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cashguo.top/gtczhttifq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hywenlv.cn/gtzuljyyye.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtyuhmilog.html

[C07] 把函数作为参数传入
来源：http://hz.pycfn.com/gtojngdwfg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ydzc1.top/gtrrruizpg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.aizwys.cn/gtzssavwpx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dianchejie.cn/gtnfakmroh.html

TS:   arr.map(String)
来源：http://hz.ydjk.org.cn/gtkowierph.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jiagoushi.top/gthxevrhzg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangtech.top/gtqpfhrbzj.html

Ruby: arr.map(&:upcase)
来源：http://hz.yonumen.top/gtpnkwfuwb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cashguo.top/gtltrmfpjb.html

[C08] 闭包
来源：http://hz.chenlongwang.top/gtkmumppqf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.andypj.xyz/gtfpbwudbm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jianghu66.top/gtdvdkxnkp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtdnlrorza.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gtsfejagok.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yj20258888.top/gtaywbuvgi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.guowangkeji.top/gtueczczqh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.meibo888.top/gtuxzqnhtu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtodsvdxvk.html

[C09] 递归
来源：http://hz.cucudq.cn/gtzhtiwhvx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gotoacloud.top/gttctuxidx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.guowangkeji.top/gtuwzudmmp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgfzy.top/gtlaufwjit.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sysykeji.top/gtrmkbklgt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnqzz.top/gtsjolqkga.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ehwqpu.com/gtoogmkxyn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gzhubu.top/gttfdicklr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xuanzx.com/gtgvxfqmdx.html

[C10] 变量作用域
来源：http://hz.ywan-chungtsiang.top/gtdxwdrxmh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sxryk.cn/gtpkcghfnh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.dashuyun.cn/gtanlvydks.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhengqikj.top/gtwyqldtlb.html

TS:   同 JS
来源：http://hz.yvedp.cn/gtnkcjdbka.html

Java: 方法内为块级作用域
来源：http://hz.iojbl.cn/gtnoolxvlb.html

Go:   花括号块级作用域
来源：http://hz.tian-w.cn/gtqsfgmzvd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.wangdashe.top/gtbnatwkxf.html

C#:   块级作用域
来源：http://hz.smart0.xyz/gtfbedxojw.html

[C11] 模块导入与导出
来源：http://hz.yongpay.top/gtiprfuwdj.html

Py:   from module import func
来源：http://hz.9152youxi.cn/gtadybirgn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guowangkeji.top/gtmanfqzuk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.bjfxy.top/gtcxcmwpbj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shuidangran.top/gtgmfcqcth.html

Java: import java.util.List;
来源：http://hz.havefunace.top/gtjgjiyxac.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.meibo888.top/gtcvkhywks.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhongyouzk.top/gtjdipyyht.html

C#:   using System.Text;
来源：http://hz.yj20258.top/gtahmmemee.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenjidiqi.icu/gtacnmntyi.html

Py:   (lambda: print("run"))()
来源：http://hz.bjfxy.top/gtgazwbiyd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.chenzaomai.com/gtdyhkiwpq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258888.top/gttxvlvjka.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xuanzx.com/gtjruzimvw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.pengpengdd.cyou/gtkiudcvjz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenlongwang.top/gtocwfkaak.html

Ruby: -> { puts "run" }.call
来源：http://hz.sysykeji.top/gtymcbjiuf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daxiang520.top/gtqhqhgdyp.html

[C13] 类型声明 / 类型注解
来源：http://hz.guannengcc.top/gtrrxunufv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.c1oappe.top/gtkolhdrkp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtgegmiqqp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hfpthk.cn/gtjeocmhww.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtmomqqqqp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtfkwfuhyz.html

Go:   func add(a, b int) int
来源：http://hz.xuetiantiany.cn/gtiwwvlihz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.chenlongwang.top/gtjaojwime.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.fengsongda.top/gtakpohzrw.html

[C14] 泛型函数
来源：http://hz.ydzc1.top/gtuwvynndg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinqigfzy.top/gtxwewlohv.html

PHP:  // 无泛型
来源：http://hz.jinghuilouyu.cn/gtplwmisqc.html

JS:   // 无泛型
来源：http://hz.daxiang520.top/gtjijyffnw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tian-w.cn/gtwjazolhd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ppjwa.cn/gtvklvdkup.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gogol.net.cn/gttzqnfqwp.html

Ruby: # 无泛型
来源：http://hz.andypj.xyz/gtkmnwndgc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xingfuxueyuan.xyz/gtmlhgfotg.html

[C15] 解构 / 展开参数
来源：http://hz.hongshengwenyu.top/gtepplsybq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhaomingkeji.xyz/gtynzdeffe.html

PHP:  [$a, $b] = $pair;
来源：http://hz.fengsongda.top/gtlvvecjco.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.feifeiyinyue.top/gtwjwzwbyj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dashuyun.cn/gtnrulaibn.html

Java: // 无解构
来源：http://hz.316326.xyz/gtvbhorqzx.html

Go:   // 无解构
来源：http://hz.cdnleiting.top/gtfcpqptok.html

Ruby: a, b = pair
来源：http://hz.tianlin.xyz/gtzkiguenx.html

C#:   var (a, b) = pair;
来源：http://hz.guowangkeji.top/gtdzykretf.html

[C16] 函数 / 方法重载
来源：http://hz.gzhubu.top/gtfwprpkhm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cashguo.top/gtmiucszys.html

PHP:  // 无重载
来源：http://hz.hammf.cn/gtfxdjdghf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.haohaochexian.top/gtkuvokjwp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.redwolf501.top/gtnxflpabf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.havefunace.top/gtriiyxrbn.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtiyuiqble.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jlsjyb.cn/gtaqdsbcrd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cdnleiting.top/gtgjdfqrdx.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtxaupxqda.html

D. 数组 / 列表 / 集合
来源：http://hz.pycfn.com/gtkwbqjaja.html

================================================================================
来源：http://hz.zdqjudy.top/gtsutkewpw.html

[D01] 创建数组 / 列表
来源：http://hz.fzhhl.top/gtynnfuhrk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ywan-chungtsiang.top/gtfbmerhwp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shuidangran.top/gtezeovmsv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yuanzhike.top/gteyylkivn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxuanxn.top/gtckzpbwzd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.tanke756.top/gteakcysrh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shzxlz.cn/gtvewpbpjp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ybcxt.top/gtyolrrxun.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tian-w.cn/gtsbrzetsy.html

[D02] 追加元素到末尾
来源：http://hz.jlsjyb.cn/gtvnqwegdc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinqigufen.top/gtxhjlzkpi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgufenzy.top/gtuywplmdj.html

JS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtbzkhcrfy.html

TS:   arr.push(4);
来源：http://hz.daria6918.cn/gtdqwllsjy.html

Java: list.add(4);
来源：http://hz.shangyingyoupin.top/gtyqtkzyal.html

Go:   arr = append(arr, 4)
来源：http://hz.dashuyun.cn/gtwewxkjjy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nanxuanxn.top/gtowrkdotx.html

C#:   list.Add(4);
来源：http://hz.chenlongwang.top/gtivnvxaya.html

[D03] 在指定位置插入元素
来源：http://hz.wangshuangyany.cn/gtbdvvvizi.html

Py:   arr.insert(0, 0)
来源：http://hz.andypj.xyz/gtphbogsxw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.quarkkingdee.top/gtfzrzfohd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgfzy.top/gtamliypce.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.aizwys.cn/gtxgdwhaos.html

Java: list.add(0, 0);
来源：http://hz.shanyushiyangkeji.top/gtbjebmodq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yueranfly.top/gthaenzaph.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.guowangkeji.top/gtvyuvckmh.html

C#:   list.Insert(0, 0);
来源：http://hz.gzhubu.top/gtffgmhzqb.html

[D04] 删除元素
来源：http://hz.zhaomingkeji.xyz/gtznyickkq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.wangdashe.top/gtpuflssqn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xziqi.cn/gtkihapvns.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxinkj.top/gtijovnsbr.html

TS:   arr.splice(0, 1);
来源：http://hz.cdnleiting.top/gtqdmmeizk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hongshengwenyu.top/gtkyzhjjdn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cqqwz.cn/gtwntvlmrp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangkeji.top/gtyfflsqci.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.snrcjt.cn/gthpbwagra.html

[D05] 访问与修改元素
来源：http://hz.zhongyouzk.top/gtrgdrqgir.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.meibo888.top/gtjxgskphs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.snrcjt.cn/gtehhpcshe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhongyouzk.top/gtmxvfjalk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj202588.top/gtxiazimcr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jiagoushi.top/gtheqkonhe.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtgcdlxnxn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtgjyyjqmm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jlsjyb.cn/gtfnvyniti.html

[D06] 数组长度
来源：http://hz.daxiang520.top/gtdqfgjfde.html

Py:   len(arr)
来源：http://hz.ivvv.top/gtevgfqwmp.html

PHP:  count($arr);
来源：http://hz.yueranfly.top/gtcsogisgq.html

JS:   arr.length
来源：http://hz.ivvv.top/gtijupdubx.html

TS:   arr.length
来源：http://hz.feifeiyinyue.top/gtozazjjdv.html

Java: list.size();
来源：http://hz.hysaishi.cn/gtdeeaeqys.html

Go:   len(arr)
来源：http://hz.yongpay.top/gtsuicbacq.html

Ruby: arr.length; arr.size
来源：http://hz.tanke756.top/gtfclzqfmi.html

C#:   list.Count;
来源：http://hz.yueranfly.top/gtqswdwoww.html

[D07] 切片 / 取子数组
来源：http://hz.jqgufenzy.top/gtbpzgghuj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.iojbl.cn/gtipfwctjw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtlqscxwzp.html

JS:   arr.slice(1, 4);
来源：http://hz.pengpengdd.cyou/gtqwitxsho.html

TS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gtduceluda.html

Java: list.subList(1, 4);
来源：http://hz.yj202588.top/gtemmrlfgy.html

Go:   arr[1:4]
来源：http://hz.yj202588.top/gtlgvvoceb.html

Ruby: arr[1, 3]
来源：http://hz.birdmap.top/gtpanjxewj.html

C#:   list.GetRange(1, 3);
来源：http://hz.hysaishi.cn/gtwbhoosie.html

[D08] 合并两个数组
来源：http://hz.cashguo.top/gtcefnhanz.html

Py:   a + b;  a.extend(b)
来源：http://hz.pengpengdd.cyou/gtwmaekves.html

PHP:  array_merge($a, $b);
来源：http://hz.hongshengwenyu.top/gtqjujeybn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.pycfn.com/gtyjzbpgpy.html

TS:   [...a, ...b];
来源：http://hz.yuxming.cn/gtsgbapqgp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cdnleiting.top/gtecujwdau.html

Go:   append(a, b...)
来源：http://hz.zhixingplan.top/gtrmagpxpn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cucudq.cn/gtspkjcmdv.html

C#:   a.Concat(b).ToList()
来源：http://hz.cdnleiting.top/gtvywspxvl.html

[D09] 排序（升序）
来源：http://hz.hammf.cn/gtkfyfuloy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jqgfzy.top/gtlcujmjvu.html

PHP:  sort($arr);
来源：http://hz.nwbrower.top/gtkrvmqypm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aizwys.cn/gtqtieudle.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cashguo.top/gtfdxiycmf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.quarkkingdee.top/gtksfxwior.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtdomsrmae.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtfjaksary.html

C#:   list.Sort();
来源：http://hz.jinyuanbaomall.cn/gthzdqqhin.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zycfv.cn/gtyjijigru.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenlongwang.top/gtezrfejpu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yangfankeji.com/gtkwekmxcw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gthmmkrgqs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtrwyhjtsz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jyoumei.cn/gtxpktuvxl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.0kj1m.cn/gtzjtxordk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daria6918.cn/gtiuzpuylb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hfpthk.cn/gtvgokndch.html

[D11] 反转数组
来源：http://hz.guowangkeji.top/gtztnyquhx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.guowangkeji.top/gtfdnbclmy.html

PHP:  array_reverse($arr);
来源：http://hz.cashguo.top/gthsrizugu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.bjfxy.top/gtsujdhrji.html

TS:   [...arr].reverse();
来源：http://hz.shanyushiyangtech.top/gtzebgtatj.html

Java: Collections.reverse(list);
来源：http://hz.zdqjudy.top/gtyeopgpdj.html

Go:   slices.Reverse(arr)
来源：http://hz.aizwys.cn/gthjcxcmxk.html

Ruby: arr.reverse
来源：http://hz.yueranfly.top/gtmmylalmf.html

C#:   list.Reverse();
来源：http://hz.yangfankeji.com/gtknrysvhy.html

[D12] 查找元素下标
来源：http://hz.tanke756.top/gtitfsaelm.html

Py:   arr.index(x);  x in arr
来源：http://hz.gaohongyu789.top/gtrpvxvuhx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.guannengcc.top/gtlqzdgbkh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtmmnldjyl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cucudq.cn/gtmzcejhcg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxinkj.top/gtvhrkfgly.html

Go:   slices.Index(arr, x)
来源：http://hz.xylfe.cn/gtxrgnlisa.html

Ruby: arr.index(x)
来源：http://hz.jinqigufen.top/gtskpmajfw.html

C#:   list.IndexOf(x);
来源：http://hz.zhiwuduotai.top/gtdguuiexb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.meibo888.top/gtwtjrciat.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gtvejlvgph.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.dashuyun.cn/gtluwcfixc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dianchejie.cn/gtmqofcyzh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangdashe.top/gtxuxofmpw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.316326.xyz/gtdpnthffb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.birdmap.top/gtywcvzcme.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.dianchejie.cn/gtmanhbpkj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenzaomai.com/gtlbagrkci.html

[D14] 映射转换（每个元素变形）
来源：http://hz.9152youxi.cn/gtafayabui.html


<!-- 参考信息 -->