代发 wailian999

[B13] 判断是否为数字
来源：http://hz.zhongyouzk.top/gthuzwnshh.html

Py:   isinstance(x, (int, float))
来源：http://hz.cucudq.cn/gtprzdwqns.html

PHP:  is_numeric($x)
来源：http://hz.hammf.cn/gthhywvxam.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jiagoushi.top/gtcroovrup.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hongshengwenyu.top/gtsouhwlph.html

Java: x instanceof Number
来源：http://hz.sweek.top/gtneqvtctv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yonumen.top/gtvfvvigdh.html

Ruby: x.is_a?(Numeric)
来源：http://hz.smart0.xyz/gtekmskekh.html

C#:   x is int or double or decimal
来源：http://hz.ydzc1.top/gtzbdaiikr.html

[B14] 判断值是否在集合内
来源：http://hz.jinqigufen.top/gtwbhtbvgb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gzhubu.top/gtoxaemwxr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.andypj.xyz/gtwfvzfqif.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zycfv.cn/gtuarydopt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jqgfzy.top/gthslllbqi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sweek.top/gtnfrevoxn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gzhubu.top/gtbznwrsrn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.tianlin.xyz/gthuooyywq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tanke756.top/gtmrfbsnuz.html

[B15] 布尔运算与取反
来源：http://hz.sxryk.cn/gtvzlfpzxn.html

Py:   a and b or not c
来源：http://hz.zhaomingkeji.xyz/gtmsyhiztn.html

PHP:  $a && $b || !$c
来源：http://hz.ybcxt.top/gtxicwswlo.html

JS:   a && b || !c
来源：http://hz.jianghu66.top/gtddiofuro.html

TS:   a && b || !c
来源：http://hz.yvedp.cn/gtcufgrrza.html

Java: a && b || !c
来源：http://hz.chenjidiqi.icu/gtuaqnoovi.html

Go:   a && b || !c
来源：http://hz.nanxuanxn.top/gtwyzviigx.html

Ruby: a && b || !c
来源：http://hz.xinyue.icu/gtjomppmyb.html

C#:   a && b || !c
来源：http://hz.316326.xyz/gtzerpbazl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.quarkkingdee.top/gtsygkxpep.html

Py:   if not data: return
来源：http://hz.c1oappe.top/gtjehqdjgl.html

PHP:  if (!$data) { return; }
来源：http://hz.zhixingplan.top/gtsrewuyyu.html

JS:   if (!data) return;
来源：http://hz.hywenlv.cn/gtwbekdhfk.html

TS:   if (!data) return;
来源：http://hz.9152youxi.cn/gttzpudvob.html

Java: if (data == null) return;
来源：http://hz.cqqwz.cn/gtqwyzffti.html

Go:   if data == nil { return }
来源：http://hz.jinqigfzy.top/gtcrwkmxoh.html

Ruby: return if data.nil?
来源：http://hz.cdnleiting.top/gtxlgwwbmh.html

C#:   if (data == null) return;
来源：http://hz.9152youxi.cn/gtyuygxnuj.html

================================================================================
来源：http://hz.hnxiangtu.top/gtmbrjqyvv.html

C. 函数与作用域
来源：http://hz.zhixingplan.top/gtydcmqtzm.html

================================================================================
来源：http://hz.0kj1m.cn/gthgvnxrzq.html

[C01] 定义函数
来源：http://hz.zhoulong.xyz/gtejeuffgk.html

Py:   def add(a, b): return a + b
来源：http://hz.xziqi.cn/gtkebumxfc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangdashe.top/gtmslizlfx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtvdwfqbbx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtlxyfrbln.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtqegkmvzl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxuanxn.top/gtftjhlzdm.html

Ruby: def add(a, b); a + b; end
来源：http://hz.fzhhl.top/gtonbteqnl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.guannengcc.top/gthtaxklhn.html

[C02] 默认参数
来源：http://hz.jinqigfzy.top/gtjjemxoef.html

Py:   def greet(name="World"): return name
来源：http://hz.zhaomingkeji.xyz/gtewyipjmu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zycfv.cn/gtqorsdbtf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.sweek.top/gtotpneoiq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.feifeiyinyue.top/gtnqvcvwbv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yueranfly.top/gtfubnbqji.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.fengsongda.top/gtvgwnnlne.html

Ruby: def greet(name = "World") = name
来源：http://hz.ehwqpu.com/gtjzswdjkh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ppjwa.cn/gttsuqnxal.html

[C03] 可变参数
来源：http://hz.jinyuanbaomall.cn/gtmlslgofc.html

Py:   def total(*args): return sum(args)
来源：http://hz.smart0.xyz/gtrlwtlxuu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yuanzhike.top/gtxnzgqpne.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gtcflnfjxh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtichqgtyz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jiagoushi.top/gtbbqqfevr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.svipenyu.cn/gtvezfeled.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.andypj.xyz/gtovlaawqr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.tianlin.xyz/gtggralrad.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jianghu66.top/gtyfenpwke.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sweek.top/gtrmoulyot.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sweek.top/gtazzlazkg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.fzhhl.top/gtekscrufe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.nanxuanxn.top/gtkeinfncc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shzxlz.cn/gtlbrudfoj.html

Go:   // 无：用配置结构体参数
来源：http://hz.jqgufenzy.top/gthaqrbxnq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hongshengwenyu.top/gtuosmiybt.html

C#:   f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gthrxosyln.html

[C05] 返回多个值
来源：http://hz.zhaomingkeji.xyz/gtjsngtals.html

Py:   return a, b
来源：http://hz.gzhubu.top/gtmkxpqgpw.html

PHP:  return [$a, $b];
来源：http://hz.jinqigfzy.top/gtlywpauqv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhijiandao.cn/gtgbuvbvht.html

TS:   return { a, b };
来源：http://hz.yj20258.top/gtjushjrzd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.iojbl.cn/gtlfvwjple.html

Go:   return a, b
来源：http://hz.hnqzz.top/gtpyayzcmp.html

Ruby: return a, b
来源：http://hz.snrcjt.cn/gtckzpphed.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dashuyun.cn/gtdluigulv.html

[C06] 匿名函数 / lambda
来源：http://hz.xuanzx.com/gtixmlxwos.html

Py:   square = lambda x: x * x
来源：http://hz.havefunace.top/gtbazklcax.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.c1oappe.top/gtbivmsaec.html

JS:   const square = x => x * x;
来源：http://hz.wangshuangyany.cn/gtaxqjogpy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.haohaochexian.top/gtxaaswwwp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ehwqpu.com/gtidjxqibt.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gogol.net.cn/gttfqyvhka.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yj202588.top/gtrbkqzmsp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shangyingyoupin.top/gtpcdpyjwn.html

[C07] 把函数作为参数传入
来源：http://hz.guannengcc.top/gtnmuykajb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dashuyun.cn/gtrlimhsho.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ydjk.org.cn/gtyvmloxyc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xingfuxueyuan.xyz/gtoyvdtgbq.html

TS:   arr.map(String)
来源：http://hz.zhoulong.xyz/gtlwqtqvfh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.c1oappe.top/gtcgrvkyat.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tanke756.top/gtyttpwtca.html

Ruby: arr.map(&:upcase)
来源：http://hz.xuanzx.com/gtvguzvnks.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yongpay.top/gtlgfeitue.html

[C08] 闭包
来源：http://hz.aizwys.cn/gtfliaqauf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhengqikj.top/gtbkrnbrtn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ydjk.org.cn/gtqaldhota.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtmttmachk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jiagoushi.top/gtmzrkiqjg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.iojbl.cn/gtjzsquyrz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.havefunace.top/gtmpsdzkpl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hammf.cn/gtyxdjiamd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.iojbl.cn/gtvljvyrni.html

[C09] 递归
来源：http://hz.snrcjt.cn/gtpabyyhko.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhixingplan.top/gtoffnmkiv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sxryk.cn/gtsdmnjtrk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zdqjudy.top/gtymotxurn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gtyhasjrfy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuxming.cn/gtstevpkwr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.meibo888.top/gtbvwvqhdo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtlivqiuts.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.smart0.xyz/gtnwlqeesk.html

[C10] 变量作用域
来源：http://hz.hfpthk.cn/gtmptkrmho.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jiagoushi.top/gtnxeggspq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sysykeji.top/gtqdldaojw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gogol.net.cn/gtmrntmsvw.html

TS:   同 JS
来源：http://hz.andypj.xyz/gtqirskcae.html

Java: 方法内为块级作用域
来源：http://hz.xylfe.cn/gtldzobecz.html

Go:   花括号块级作用域
来源：http://hz.nanxuanxn.top/gtljgakyjn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nwbrower.top/gtakytofcm.html

C#:   块级作用域
来源：http://hz.xuanzx.com/gtyempprot.html

[C11] 模块导入与导出
来源：http://hz.ywan-chungtsiang.top/gthtzqjnwx.html

Py:   from module import func
来源：http://hz.smart0.xyz/gtsakycgwf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigfzy.top/gthomhnrau.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yvedp.cn/gtrzbllnly.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cqqwz.cn/gtamdvnivp.html

Java: import java.util.List;
来源：http://hz.jqgufenzy.top/gtkdsjtigo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.guannengcc.top/gthkgiiftv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nanxuanxn.top/gtixqzejug.html

C#:   using System.Text;
来源：http://hz.quarkkingdee.top/gtkftribyk.html

[C12] 立即执行函数 IIFE
来源：http://hz.cqqwz.cn/gtkkwjnnit.html

Py:   (lambda: print("run"))()
来源：http://hz.yuanzhike.top/gtbodtbmjf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ywan-chungtsiang.top/gtlicsxfqb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtbeaxbott.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhijiandao.cn/gtdcuxrwid.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hnqzz.top/gtriufkvee.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenjidiqi.icu/gtuqwoeppe.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinqigufen.top/gturtbrtbk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.snrcjt.cn/gtcajgdzvq.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuetiantiany.cn/gtuqwlcqga.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jlsjyb.cn/gtsheijdoe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gthkvvtact.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.haohaochexian.top/gtbdafhfgg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shzxlz.cn/gtbexirrsz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtteyotbxg.html

Go:   func add(a, b int) int
来源：http://hz.yanxiufei.cn/gtbcbujaxm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.feifeiyinyue.top/gtdwkhbtlk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.iojbl.cn/gtavdafahg.html

[C14] 泛型函数
来源：http://hz.nanxuanxn.top/gtikksxldk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ppjwa.cn/gtzpstqmoz.html

PHP:  // 无泛型
来源：http://hz.yj202588.top/gtuewtlslf.html

JS:   // 无泛型
来源：http://hz.hfpthk.cn/gtrljpiemz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yonumen.top/gthaswicwt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guowangkeji.top/gtnvffxajb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.mhx1999.top/gtgaxssmid.html

Ruby: # 无泛型
来源：http://hz.daxiang520.top/gtjsiohfld.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aibaodan.cn/gthelqjtzz.html

[C15] 解构 / 展开参数
来源：http://hz.jianghu66.top/gtnxsqqpam.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.guannengcc.top/gtpxiinxvv.html

PHP:  [$a, $b] = $pair;
来源：http://hz.nwbrower.top/gtzrdxhafm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shanyushiyangtech.top/gtjwfrwjcz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinghuilouyu.cn/gteybbdzny.html

Java: // 无解构
来源：http://hz.xinyue.icu/gtwyrrpzku.html

Go:   // 无解构
来源：http://hz.xuetiantiany.cn/gtwvspcduq.html

Ruby: a, b = pair
来源：http://hz.cashguo.top/gtasdwwwrp.html

C#:   var (a, b) = pair;
来源：http://hz.xinyue.icu/gtahcwpffv.html

[C16] 函数 / 方法重载
来源：http://hz.havefunace.top/gtixrvhlxu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yuxming.cn/gtssdsqotz.html

PHP:  // 无重载
来源：http://hz.jqgfzy.top/gtkhjfiiji.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dashuyun.cn/gthfwmgowc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ybcxt.top/gtsffbaxkd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.snrcjt.cn/gtcxdiwabr.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgufenzy.top/gtzqjevuti.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhixingplan.top/gtdciswich.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gaohongyu789.top/gtuonapsif.html

================================================================================
来源：http://hz.redwolf501.top/gteytigyvl.html

D. 数组 / 列表 / 集合
来源：http://hz.jiagoushi.top/gtzvyfctkn.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxocodbkt.html

[D01] 创建数组 / 列表
来源：http://hz.xziqi.cn/gtvnpkggzp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cucudq.cn/gtajmklfem.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yongpay.top/gtzarjncdk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hongshengwenyu.top/gtltobahrj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gzhubu.top/gtfzazxrmo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cqqwz.cn/gtvppjxfhf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gaohongyu789.top/gtsuufhfkt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.guannengcc.top/gtbzygrkbs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhengqikj.top/gthbyjlpvf.html

[D02] 追加元素到末尾
来源：http://hz.gzhubu.top/gtboauxltu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zdqjudy.top/gtyjfhmlkl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jianghu66.top/gtbidjomde.html

JS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtzoyovuex.html

TS:   arr.push(4);
来源：http://hz.hammf.cn/gtumoizdib.html

Java: list.add(4);
来源：http://hz.pycfn.com/gtopfexzym.html

Go:   arr = append(arr, 4)
来源：http://hz.dianchejie.cn/gtguxajdpd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinqigufen.top/gtzrdkmazx.html

C#:   list.Add(4);
来源：http://hz.shzxlz.cn/gtkhetdaxh.html

[D03] 在指定位置插入元素
来源：http://hz.jinyuanbaomall.cn/gtdkmpnnmp.html

Py:   arr.insert(0, 0)
来源：http://hz.birdmap.top/gtdhcrivck.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nanxinkj.top/gtlqjpumla.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sweek.top/gtvamyuuuj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gotoacloud.top/gtoytfilcz.html

Java: list.add(0, 0);
来源：http://hz.jyoumei.cn/gtcgewdtud.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.0kj1m.cn/gtxgxreeod.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydzc1.top/gtvcpbzwlf.html

C#:   list.Insert(0, 0);
来源：http://hz.fengsongda.top/gtjxdrpdvi.html

[D04] 删除元素
来源：http://hz.iojbl.cn/gtiplqnche.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cashguo.top/gtfzwwbzqt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shanyushiyangtech.top/gtkrmtxwbv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.haohaochexian.top/gtymctdnfb.html

TS:   arr.splice(0, 1);
来源：http://hz.gaohongyu789.top/gtdotrpcia.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinqigfzy.top/gtgfncndcm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.andypj.xyz/gtrxcalgmr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sxryk.cn/gtlsqnezee.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenjidiqi.icu/gtqxngfeos.html

[D05] 访问与修改元素
来源：http://hz.snrcjt.cn/gtbteqiskj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtwxiftsyf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258888.top/gtcukjxrqz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.daxiang520.top/gtyteqwroo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yangfankeji.com/gtpaakkqon.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tianlin.xyz/gttqfizvpz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtgojjhxib.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtpnwxkiso.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.daxiang520.top/gturrdyaqf.html

[D06] 数组长度
来源：http://hz.hywenlv.cn/gttcwcqpum.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gtpatdnnbh.html

PHP:  count($arr);
来源：http://hz.jianghu66.top/gteqqvilbv.html

JS:   arr.length
来源：http://hz.nwbrower.top/gtovcactwy.html

TS:   arr.length
来源：http://hz.yj202588.top/gtoacfnuuu.html

Java: list.size();
来源：http://hz.zhaomingkeji.xyz/gthovgocnk.html

Go:   len(arr)
来源：http://hz.chenjidiqi.icu/gtlmrcxeow.html

Ruby: arr.length; arr.size
来源：http://hz.tianlin.xyz/gtiycyheqx.html

C#:   list.Count;
来源：http://hz.hfpthk.cn/gtvqcqewcn.html

[D07] 切片 / 取子数组
来源：http://hz.dianchejie.cn/gtsbjilrhl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.316326.xyz/gtpacfdxqk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.pycfn.com/gtuyorwket.html

JS:   arr.slice(1, 4);
来源：http://hz.hammf.cn/gtsynkxvmi.html

TS:   arr.slice(1, 4);
来源：http://hz.yuxming.cn/gtqtwridnn.html

Java: list.subList(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtwohwlxml.html

Go:   arr[1:4]
来源：http://hz.yuanzhike.top/gtodsxjtfp.html

Ruby: arr[1, 3]
来源：http://hz.shangyingyoupin.top/gtavxwvtra.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangtech.top/gtykwzjdur.html

[D08] 合并两个数组
来源：http://hz.xinyue.icu/gtgjonzvre.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinyuanbaomall.cn/gtsscarrhb.html

PHP:  array_merge($a, $b);
来源：http://hz.ywan-chungtsiang.top/gtcfhjzclp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.wangdashe.top/gtvxxkcbxc.html

TS:   [...a, ...b];
来源：http://hz.jlsjyb.cn/gtwulqaqvd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yangfankeji.com/gtcucntymx.html

Go:   append(a, b...)
来源：http://hz.zycfv.cn/gtqwuntbsa.html

Ruby: a + b;  a.concat(b)
来源：http://hz.svipenyu.cn/gtaaoeuiqy.html

C#:   a.Concat(b).ToList()
来源：http://hz.wangdashe.top/gtnseqqtzf.html

[D09] 排序（升序）
来源：http://hz.wangdashe.top/gtzyyyywaa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.mhx1999.top/gtonybqcrp.html

PHP:  sort($arr);
来源：http://hz.zhengqikj.top/gtgknsytrf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.snrcjt.cn/gtecdkjvmn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhijiandao.cn/gtakiotdnz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zycfv.cn/gtqlcsdnhe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.quarkkingdee.top/gtbbgywhsv.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtaohrcvjz.html

C#:   list.Sort();
来源：http://hz.wangshuangyany.cn/gtwzjrwkpw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yvedp.cn/gtpvofnolb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhiwuduotai.top/gtvenciwkr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tanke756.top/gttcbtpkji.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yongpay.top/gtpudqdftd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sysykeji.top/gtvsixyajt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xuetiantiany.cn/gthgwhvdpb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhengqikj.top/gtvsjaswsi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nwbrower.top/gthbqobtfg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ydjk.org.cn/gtgmymijme.html

[D11] 反转数组
来源：http://hz.gaohongyu789.top/gtrzoybgrg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.0kj1m.cn/gthjcpjysy.html

PHP:  array_reverse($arr);
来源：http://hz.mhx1999.top/gtbdcnuugx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuanzx.com/gtechuymdt.html

TS:   [...arr].reverse();
来源：http://hz.yj202588.top/gtnxgdlrok.html

Java: Collections.reverse(list);
来源：http://hz.hnxiangtu.top/gtkdwphxfk.html

Go:   slices.Reverse(arr)
来源：http://hz.shanyushiyangkeji.top/gtfvmixken.html

Ruby: arr.reverse
来源：http://hz.ydjk.org.cn/gtkcldqwrm.html

C#:   list.Reverse();
来源：http://hz.zhiwuduotai.top/gtwqfxpfkx.html

[D12] 查找元素下标
来源：http://hz.gaohongyu789.top/gtozromiyp.html

Py:   arr.index(x);  x in arr
来源：http://hz.gogol.net.cn/gtgqfnqvsh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jiagoushi.top/gtukybgdtv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gtbobnethl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gogol.net.cn/gtsbqzqxlz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shzxlz.cn/gtzhslikjq.html

Go:   slices.Index(arr, x)
来源：http://hz.shuidangran.top/gtraupdpqn.html

Ruby: arr.index(x)
来源：http://hz.yj20258.top/gtcbjvmiuy.html

C#:   list.IndexOf(x);
来源：http://hz.52xcode.cn/gtdguepxxq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gotoacloud.top/gtlnvyvejn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.fengsongda.top/gtcfmzixny.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yvedp.cn/gtcbawypqi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtpsexjxcw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gtwyxnktrn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.pengpengdd.cyou/gtyotqemnv.html


<!-- 参考信息 -->