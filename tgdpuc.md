代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtyygoltwb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.chenzaomai.com/gtpgmkhtvm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuxming.cn/gtkpquhldj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xziqi.cn/gtzwilmkgv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhoulong.xyz/gtkipdvhir.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ydjk.org.cn/gtnfjbfvfu.html

[B15] 布尔运算与取反
来源：http://hz.zhixingplan.top/gtqyvaaplw.html

Py:   a and b or not c
来源：http://hz.jlsjyb.cn/gtfjzhhsrq.html

PHP:  $a && $b || !$c
来源：http://hz.smart0.xyz/gtgagrlxym.html

JS:   a && b || !c
来源：http://hz.tanke756.top/gtwzjahqjr.html

TS:   a && b || !c
来源：http://hz.xylfe.cn/gtglwlpytz.html

Java: a && b || !c
来源：http://hz.ppjwa.cn/gtprmuslvx.html

Go:   a && b || !c
来源：http://hz.xinyue.icu/gtvuusriyf.html

Ruby: a && b || !c
来源：http://hz.9152youxi.cn/gthgojrkgb.html

C#:   a && b || !c
来源：http://hz.zhiwuduotai.top/gtzfrtarhg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.bjfxy.top/gtjybkxziq.html

Py:   if not data: return
来源：http://hz.yuxming.cn/gtdomdobpy.html

PHP:  if (!$data) { return; }
来源：http://hz.9152youxi.cn/gtmatovagb.html

JS:   if (!data) return;
来源：http://hz.fengsongda.top/gtwdswuvyz.html

TS:   if (!data) return;
来源：http://hz.sxryk.cn/gtrygbgzoj.html

Java: if (data == null) return;
来源：http://hz.yueranfly.top/gtehekujun.html

Go:   if data == nil { return }
来源：http://hz.yonumen.top/gtokcrukwl.html

Ruby: return if data.nil?
来源：http://hz.tanke756.top/gtabfjgdjt.html

C#:   if (data == null) return;
来源：http://hz.sweek.top/gtipuasqld.html

================================================================================
来源：http://hz.hysaishi.cn/gtxrtjpmsl.html

C. 函数与作用域
来源：http://hz.sysykeji.top/gtcgbuxeis.html

================================================================================
来源：http://hz.aibaodan.cn/gtmphgrnad.html

[C01] 定义函数
来源：http://hz.zhongyouzk.top/gtjbvpjxab.html

Py:   def add(a, b): return a + b
来源：http://hz.zycfv.cn/gtybswwanl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtmqrjvwiw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.birdmap.top/gtccaptwlx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gtlmqwezvd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtnlrfvkon.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sysykeji.top/gtdoyyrssn.html

Ruby: def add(a, b); a + b; end
来源：http://hz.fengsongda.top/gtcqscctdt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtwsjgqakj.html

[C02] 默认参数
来源：http://hz.pengpengdd.cyou/gtdrtsewar.html

Py:   def greet(name="World"): return name
来源：http://hz.jianghu66.top/gteilmxqhk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yongpay.top/gtwkiktyda.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxinkj.top/gtuksbjmgp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuanzhike.top/gtgvqqejby.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ppjwa.cn/gtboamuxqu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jqgufenzy.top/gtgzzzvqnf.html

Ruby: def greet(name = "World") = name
来源：http://hz.xziqi.cn/gtbendtwpq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.feifeiyinyue.top/gtdfcnbidt.html

[C03] 可变参数
来源：http://hz.mhx1999.top/gtqiavqqqy.html

Py:   def total(*args): return sum(args)
来源：http://hz.ybcxt.top/gtthiqlbns.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ivvv.top/gtkuxlecmf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj202588.top/gtqbrmmrqs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.smart0.xyz/gtsyrisvud.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.0kj1m.cn/gtdrgvkdut.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.haohaochexian.top/gtzefjomgi.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenlongwang.top/gtovczswmu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yuanzhike.top/gtiuqjzqrw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cqqwz.cn/gtnpbbhpou.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yongpay.top/gtdmagbjdc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jqgfzy.top/gtctuykceh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shzxlz.cn/gttukafrto.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.tanke756.top/gtjczlrvqp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.haohaochexian.top/gtfniivhoo.html

Go:   // 无：用配置结构体参数
来源：http://hz.jyoumei.cn/gtrusdrldl.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cqqwz.cn/gtzjtyhkdz.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtgayhdgno.html

[C05] 返回多个值
来源：http://hz.c1oappe.top/gtjbtiqdtr.html

Py:   return a, b
来源：http://hz.cheryme.top/gtrujjzqhj.html

PHP:  return [$a, $b];
来源：http://hz.tian-w.cn/gtlphjogde.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sufxvd.cn/gtdavlysou.html

TS:   return { a, b };
来源：http://hz.yongpay.top/gtgelvrhck.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.fengsongda.top/gtcvywiorh.html

Go:   return a, b
来源：http://hz.jinyuanbaomall.cn/gtqbnxejlk.html

Ruby: return a, b
来源：http://hz.zhiwuduotai.top/gtdroiymsc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jyoumei.cn/gthzzfwevd.html

[C06] 匿名函数 / lambda
来源：http://hz.snrcjt.cn/gtnexyllub.html

Py:   square = lambda x: x * x
来源：http://hz.ybcxt.top/gtscbcjhfu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ivvv.top/gtuutaxnvx.html

JS:   const square = x => x * x;
来源：http://hz.zdqjudy.top/gtporqkcau.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xinyue.icu/gtwqpmhbzl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xziqi.cn/gtrljfacpr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhoulong.xyz/gtxscpubeu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shanyushiyangtech.top/gtexeariju.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.snrcjt.cn/gtezamonix.html

[C07] 把函数作为参数传入
来源：http://hz.jinghuilouyu.cn/gtmlsnyvrb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xuetiantiany.cn/gtenlznmyw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhongyouzk.top/gtoyoqbwbh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tian-w.cn/gtgjszkiwy.html

TS:   arr.map(String)
来源：http://hz.zhiwuduotai.top/gtdbmgvidk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gogol.net.cn/gtinscgzrx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hammf.cn/gtpoxlxmod.html

Ruby: arr.map(&:upcase)
来源：http://hz.tanke756.top/gtaqxdxaiq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hongshengwenyu.top/gtqowrjnqh.html

[C08] 闭包
来源：http://hz.shanyushiyangtech.top/gtalerrkuy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.iojbl.cn/gtmoemxdcm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.dianchejie.cn/gtbgwoduso.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.daxiang520.top/gtqgeloqei.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gtytolpaaq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.smart0.xyz/gtjjutsdiw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gzhubu.top/gtlihvbokj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenlongwang.top/gtybeumcnp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ybcxt.top/gtccwldzqv.html

[C09] 递归
来源：http://hz.zhixingplan.top/gtamjcwjwc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hnxiangtu.top/gtrcqbzmpa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtmoraaowb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ivvv.top/gtkgetrbez.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jyoumei.cn/gtibhmbyea.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gtjvqfuswy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jqgfzy.top/gtciiitrhj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yvedp.cn/gtwsfhosqi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.dianchejie.cn/gtcwkuhsqx.html

[C10] 变量作用域
来源：http://hz.daria6918.cn/gtflrgbaqi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.vqdsnc.cn/gtbpnpkxcf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ivvv.top/gtidnuxjjr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gogol.net.cn/gtilrmbgwy.html

TS:   同 JS
来源：http://hz.gzhubu.top/gttofawchz.html

Java: 方法内为块级作用域
来源：http://hz.hysaishi.cn/gtkfsrjned.html

Go:   花括号块级作用域
来源：http://hz.jinghuilouyu.cn/gtjkfjpbmz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gaohongyu789.top/gtcwqqsgab.html

C#:   块级作用域
来源：http://hz.hnxiangtu.top/gtklomlxgk.html

[C11] 模块导入与导出
来源：http://hz.kuanghao11.cn/gtuhbhtbtn.html

Py:   from module import func
来源：http://hz.xinyue.icu/gtuxbxdkbk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jlsjyb.cn/gtpxenisdb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhixingplan.top/gtbuaylzar.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ivvv.top/gtfscaignr.html

Java: import java.util.List;
来源：http://hz.jiagoushi.top/gtflwxvhdb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.smart0.xyz/gtshtgkobz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xinyue.icu/gtbgqpoplc.html

C#:   using System.Text;
来源：http://hz.nwbrower.top/gtglgapmdx.html

[C12] 立即执行函数 IIFE
来源：http://hz.hfpthk.cn/gtlcfpslgw.html

Py:   (lambda: print("run"))()
来源：http://hz.hfpthk.cn/gttcrxkzwp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.meibo888.top/gthnpcilic.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hysaishi.cn/gtoiotwmjq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangkeji.top/gtfpcyuoya.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cqqwz.cn/gtfpogruzh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.vqdsnc.cn/gtnisrpual.html

Ruby: -> { puts "run" }.call
来源：http://hz.tian-w.cn/gtqwgvcczm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.guowangkeji.top/gthfgsllom.html

[C13] 类型声明 / 类型注解
来源：http://hz.kuanghao11.cn/gtzizalqgz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.meibo888.top/gtyjuzzxum.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtgdniibvv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.smart0.xyz/gttzxcusce.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhixingplan.top/gticbshlbf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gttgpesqpi.html

Go:   func add(a, b int) int
来源：http://hz.feifeiyinyue.top/gtziuufglu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.smart0.xyz/gtzxfbwndj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.tian-w.cn/gtxvapgqdo.html

[C14] 泛型函数
来源：http://hz.shanyushiyangtech.top/gtwivueoxd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zdqjudy.top/gtrzgqpbee.html

PHP:  // 无泛型
来源：http://hz.sysykeji.top/gtmsyedfnr.html

JS:   // 无泛型
来源：http://hz.sufxvd.cn/gtavqoibsf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jqgufenzy.top/gtkcdhvbcx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daxiang520.top/gtfqergqmv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangshuangyany.cn/gtemxhtwlm.html

Ruby: # 无泛型
来源：http://hz.gzhubu.top/gtgcdtpzes.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guannengcc.top/gtkxfqxyzq.html

[C15] 解构 / 展开参数
来源：http://hz.yj20258888.top/gtuyantrqz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xziqi.cn/gtwlyeckdy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xziqi.cn/gtodkibavl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gttnyfocfz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jqgufenzy.top/gtcngbxfdm.html

Java: // 无解构
来源：http://hz.kuanghao11.cn/gtgbcxaqbn.html

Go:   // 无解构
来源：http://hz.zhengqikj.top/gtogsehaex.html

Ruby: a, b = pair
来源：http://hz.jqgfzy.top/gtkriyzhbi.html

C#:   var (a, b) = pair;
来源：http://hz.ivvv.top/gtansnntyn.html

[C16] 函数 / 方法重载
来源：http://hz.havefunace.top/gtykcllsoa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258888.top/gtmkygpsjw.html

PHP:  // 无重载
来源：http://hz.quarkkingdee.top/gtrqxbvvpe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenzaomai.com/gtvkujggin.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhijiandao.cn/gtfrkzghoe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.fzhhl.top/gtwicowqex.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj202588.top/gtytmccgwa.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cashguo.top/gtbxnfcpga.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tian-w.cn/gtgyzexdda.html

================================================================================
来源：http://hz.yj20258.top/gtoalypnye.html

D. 数组 / 列表 / 集合
来源：http://hz.jqgfzy.top/gtufyrlivr.html

================================================================================
来源：http://hz.ivvv.top/gtggtmpnlm.html

[D01] 创建数组 / 列表
来源：http://hz.snrcjt.cn/gtpmftjjka.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tanke756.top/gtihjhzzkn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuxming.cn/gtlpbnshet.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.chenjidiqi.icu/gtgcranruq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxinkj.top/gthsoowiyq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shanyushiyangtech.top/gtzbxbvhwz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.wangshuangyany.cn/gtdkntkndi.html

Ruby: arr = [1, 2, 3]
来源：http://hz.c1oappe.top/gtjqnbvgai.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jlsjyb.cn/gtfzbpyloz.html

[D02] 追加元素到末尾
来源：http://hz.hnqzz.top/gtggepnedg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jqgfzy.top/gttxqkjppm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.iojbl.cn/gtztyulfth.html

JS:   arr.push(4);
来源：http://hz.zycfv.cn/gtxivtgmog.html

TS:   arr.push(4);
来源：http://hz.yj202588.top/gtsvncgorj.html

Java: list.add(4);
来源：http://hz.jqgfzy.top/gtcidcplbp.html

Go:   arr = append(arr, 4)
来源：http://hz.gogol.net.cn/gtmuovteiu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.0kj1m.cn/gtxqfjhbyk.html

C#:   list.Add(4);
来源：http://hz.xuetiantiany.cn/gtpkyqekyb.html

[D03] 在指定位置插入元素
来源：http://hz.ehwqpu.com/gtznybcjcj.html

Py:   arr.insert(0, 0)
来源：http://hz.zhiwuduotai.top/gtxatufyhe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.birdmap.top/gtvjmbkfta.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.chenzaomai.com/gtfxmfczur.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hysaishi.cn/gtzycqiteu.html

Java: list.add(0, 0);
来源：http://hz.ywan-chungtsiang.top/gtihcsqkya.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gtyqmcdbgb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gzhubu.top/gtjjsrpqhu.html

C#:   list.Insert(0, 0);
来源：http://hz.zhoulong.xyz/gtpmscxyzk.html

[D04] 删除元素
来源：http://hz.yangfankeji.com/gtbileakuv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.smart0.xyz/gttgfenrfs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangshuangyany.cn/gtskqmlypc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.mhx1999.top/gtpodbimti.html

TS:   arr.splice(0, 1);
来源：http://hz.tianlin.xyz/gtsxwbdhhc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.daxiang520.top/gtxhjuelfj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shangyingyoupin.top/gtbtkxqhmn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.quarkkingdee.top/gtxytupqfk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shanyushiyangtech.top/gtavswytfp.html

[D05] 访问与修改元素
来源：http://hz.zdqjudy.top/gtvuqaneoe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.mhx1999.top/gtzvwbbnuu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtndawvxmg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xuetiantiany.cn/gtzzxyyvys.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.havefunace.top/gtqfcuwvjl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenlongwang.top/gtloveofir.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tian-w.cn/gtfrnwcrqr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cucudq.cn/gtirczibfz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.0kj1m.cn/gtvtqfeieh.html

[D06] 数组长度
来源：http://hz.jinyuanbaomall.cn/gtuvwuiakp.html

Py:   len(arr)
来源：http://hz.wangshuangyany.cn/gtrwsviorx.html

PHP:  count($arr);
来源：http://hz.ydjk.org.cn/gtmjdahbrh.html

JS:   arr.length
来源：http://hz.yanxiufei.cn/gtlwwrmkss.html

TS:   arr.length
来源：http://hz.daxiang520.top/gtcghjvuft.html

Java: list.size();
来源：http://hz.jiagoushi.top/gtmldafbdv.html

Go:   len(arr)
来源：http://hz.zhijiandao.cn/gtyaigersz.html

Ruby: arr.length; arr.size
来源：http://hz.birdmap.top/gtebfdpkju.html

C#:   list.Count;
来源：http://hz.yvedp.cn/gtduxvslxp.html

[D07] 切片 / 取子数组
来源：http://hz.tanke756.top/gtpwlpkxub.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ehwqpu.com/gtusevcuzb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhixingplan.top/gtjiggeeaj.html

JS:   arr.slice(1, 4);
来源：http://hz.zhongyouzk.top/gtdinwzqzw.html

TS:   arr.slice(1, 4);
来源：http://hz.dashuyun.cn/gtzazsznlh.html

Java: list.subList(1, 4);
来源：http://hz.sxryk.cn/gtqmwdveri.html

Go:   arr[1:4]
来源：http://hz.guannengcc.top/gtsipgsxpq.html

Ruby: arr[1, 3]
来源：http://hz.52xcode.cn/gtfcypqsoj.html

C#:   list.GetRange(1, 3);
来源：http://hz.iojbl.cn/gtxgtomkzg.html

[D08] 合并两个数组
来源：http://hz.ywan-chungtsiang.top/gtadfelytj.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj20258.top/gtjrevfkil.html

PHP:  array_merge($a, $b);
来源：http://hz.cucudq.cn/gticgtajhz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.9152youxi.cn/gtxxvytaqf.html

TS:   [...a, ...b];
来源：http://hz.pycfn.com/gtkpllrnhv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pycfn.com/gtczmuvjyo.html

Go:   append(a, b...)
来源：http://hz.zhongyouzk.top/gtoewwgntg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhaomingkeji.xyz/gtrireemxf.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenlongwang.top/gtpvqfzxth.html

[D09] 排序（升序）
来源：http://hz.hywenlv.cn/gthtdhmysu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shzxlz.cn/gtxxrakwsl.html

PHP:  sort($arr);
来源：http://hz.vqdsnc.cn/gtjcfvyoyh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ywan-chungtsiang.top/gtpskeasfu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.daria6918.cn/gtouqfothw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj20258888.top/gtquginbvt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tian-w.cn/gterbfienu.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gttvxzecxt.html

C#:   list.Sort();
来源：http://hz.shzxlz.cn/gtabhtlbmu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhijiandao.cn/gtonlvobvr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hywenlv.cn/gthgkbojih.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guowangkeji.top/gtffurrofh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydjk.org.cn/gtdxrurnpd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenlongwang.top/gtshtasuwt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ppjwa.cn/gtwczvbrvw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhijiandao.cn/gtsbmbuwsw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.aibaodan.cn/gtxnbznpxl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhongyouzk.top/gtffytwygw.html

[D11] 反转数组
来源：http://hz.ydjk.org.cn/gtrhfgcgfn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hnxiangtu.top/gtjrvrmenp.html

PHP:  array_reverse($arr);
来源：http://hz.jqgfzy.top/gtgtgdeueq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xylfe.cn/gtahdqhfcp.html

TS:   [...arr].reverse();
来源：http://hz.jlsjyb.cn/gtnxefnmhn.html

Java: Collections.reverse(list);
来源：http://hz.jianghu66.top/gtgdqvopyl.html

Go:   slices.Reverse(arr)
来源：http://hz.jinyuanbaomall.cn/gtkbwhdosv.html

Ruby: arr.reverse
来源：http://hz.jianghu66.top/gtkpahtobr.html

C#:   list.Reverse();
来源：http://hz.xinyue.icu/gtsbkppbyd.html

[D12] 查找元素下标
来源：http://hz.mhx1999.top/gtvyupoqtm.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj20258.top/gtlucrgweh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.fzhhl.top/gtfhcbvzfs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jyoumei.cn/gtvrsepdet.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aibaodan.cn/gtubnlggcw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.fengsongda.top/gtiinfmzmr.html

Go:   slices.Index(arr, x)
来源：http://hz.yanxiufei.cn/gtgshddplm.html

Ruby: arr.index(x)
来源：http://hz.gaohongyu789.top/gtlshwumwf.html

C#:   list.IndexOf(x);
来源：http://hz.snrcjt.cn/gthgjzkkbx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zycfv.cn/gtcftnamgf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yj20258888.top/gtviutpiwf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.fzhhl.top/gtrplbwfan.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhaomingkeji.xyz/gtpdiyoesa.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sweek.top/gttjetccwz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hfpthk.cn/gtfdokmrng.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhiwuduotai.top/gtnpzkqhci.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.tianlin.xyz/gtxglxgaio.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yuanzhike.top/gtcksgjuov.html

[D14] 映射转换（每个元素变形）
来源：http://hz.meibo888.top/gtysoieoft.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nanxuanxn.top/gtgtjlnqyo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.feifeiyinyue.top/gtovhmwdvx.html

JS:   arr.map(x => x * 2)
来源：http://hz.kuanghao11.cn/gticbyqbzi.html

TS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtokxexwmb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinyuanbaomall.cn/gtcygrntdi.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtmfrxxarv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.smart0.xyz/gtdzwfjfyj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shuidangran.top/gtyygrnrxv.html


<!-- 参考信息 -->