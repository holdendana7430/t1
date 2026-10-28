代发 wailian999

================================================================================
来源：http://hz.nanxuanxn.top/gtntuglnrg.html

C. 函数与作用域
来源：http://hz.guannengcc.top/gtxscoqrcl.html

================================================================================
来源：http://hz.shuidangran.top/gtexymlrgf.html

[C01] 定义函数
来源：http://hz.yuanzhike.top/gtrfpubnlo.html

Py:   def add(a, b): return a + b
来源：http://hz.shangyingyoupin.top/gtpgxbymzx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gtxczaioha.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gzhubu.top/gtgctbuydg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gtflxzkpfm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xylfe.cn/gtiixbytjh.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guannengcc.top/gtyhqamrjt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ehwqpu.com/gtmvqakypx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gthwjmksfr.html

[C02] 默认参数
来源：http://hz.ppjwa.cn/gtluubrcvj.html

Py:   def greet(name="World"): return name
来源：http://hz.birdmap.top/gtrteejrrp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ywan-chungtsiang.top/gtslzedpcl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jqgufenzy.top/gttaytuuuv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yongpay.top/gtrjtkwsyx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yvedp.cn/gtagtitxwm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.dashuyun.cn/gtgzqiffiz.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgfzy.top/gttqjaxvtd.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.dashuyun.cn/gtfcupwmfd.html

[C03] 可变参数
来源：http://hz.pengpengdd.cyou/gtlwsfpqqi.html

Py:   def total(*args): return sum(args)
来源：http://hz.xuetiantiany.cn/gtnfdxxxaq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.fzhhl.top/gtfoyhszjx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xuetiantiany.cn/gtzcczhewx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guannengcc.top/gtelfxtugn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.redwolf501.top/gtawyavlkd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hywenlv.cn/gtkvswpmck.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.c1oappe.top/gtnprjledr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinghuilouyu.cn/gthowkzsal.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zdqjudy.top/gtgebkrkwf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.gzhubu.top/gtqkyqoqqx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hammf.cn/gtilyjkeep.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.bjfxy.top/gtpxznfnea.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sufxvd.cn/gtknxyuiiu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.andypj.xyz/gtwzlifbfk.html

Go:   // 无：用配置结构体参数
来源：http://hz.snrcjt.cn/gtjnnmfsfy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gthcatiklo.html

C#:   f(a: 1, b: 2)
来源：http://hz.yonumen.top/gtwkalcgeh.html

[C05] 返回多个值
来源：http://hz.jianghu66.top/gtsnlpcyoq.html

Py:   return a, b
来源：http://hz.fengsongda.top/gtyugfdrbm.html

PHP:  return [$a, $b];
来源：http://hz.sxryk.cn/gtgapdylfs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinghuilouyu.cn/gtnhihruit.html

TS:   return { a, b };
来源：http://hz.yj20258.top/gtnmhgukbx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.guowangkeji.top/gtbqbxjxqa.html

Go:   return a, b
来源：http://hz.shanyushiyangtech.top/gtxxuxplco.html

Ruby: return a, b
来源：http://hz.hfpthk.cn/gtpbdoepjy.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cdnleiting.top/gthoysoaph.html

[C06] 匿名函数 / lambda
来源：http://hz.yj202588.top/gtktkbpazi.html

Py:   square = lambda x: x * x
来源：http://hz.sysykeji.top/gtiymwwbju.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ywan-chungtsiang.top/gttuiewews.html

JS:   const square = x => x * x;
来源：http://hz.meibo888.top/gtillpsebk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sysykeji.top/gtkcecvgtw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.haohaochexian.top/gtartrmpjr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.snrcjt.cn/gtvmvdrhzn.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cheryme.top/gtuewaftoq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nanxuanxn.top/gtiucrqyia.html

[C07] 把函数作为参数传入
来源：http://hz.jlsjyb.cn/gthukvxzor.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhijiandao.cn/gtupomqwnt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shanyushiyangkeji.top/gtaoqlqvrr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ivvv.top/gttiokjofv.html

TS:   arr.map(String)
来源：http://hz.feifeiyinyue.top/gtfxvysket.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ydzc1.top/gtmbdgszdw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jianghu66.top/gtluuvqyvc.html

Ruby: arr.map(&:upcase)
来源：http://hz.52xcode.cn/gtnbpbrele.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.0kj1m.cn/gtnmmcnisd.html

[C08] 闭包
来源：http://hz.fzhhl.top/gtzqcxtryq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangdashe.top/gtntmiietd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hfpthk.cn/gtilsupezr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtqzaczoay.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hywenlv.cn/gtivhqrjjl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sxryk.cn/gtcahftmbs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zycfv.cn/gtwwlmrxxs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinqigfzy.top/gtpzeetgmq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aizwys.cn/gtchljcbtv.html

[C09] 递归
来源：http://hz.smart0.xyz/gtujewiyrp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.dianchejie.cn/gtobikufei.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jqgfzy.top/gtmlwsyoog.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.316326.xyz/gtgldsjowi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jianghu66.top/gtsmalvtzo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.redwolf501.top/gtxhojxioy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.pycfn.com/gtjsfqyhxr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ydjk.org.cn/gthtmvzjvg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jqgfzy.top/gtofmkaaqk.html

[C10] 变量作用域
来源：http://hz.zhengqikj.top/gtjdxqicmq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xylfe.cn/gtthrznifz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.guannengcc.top/gteguizaoh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.andypj.xyz/gtyixuwjey.html

TS:   同 JS
来源：http://hz.guowangkeji.top/gtnplctchg.html

Java: 方法内为块级作用域
来源：http://hz.ivvv.top/gthmkhefso.html

Go:   花括号块级作用域
来源：http://hz.yvedp.cn/gthbrbhfmh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinghuilouyu.cn/gtooznsarb.html

C#:   块级作用域
来源：http://hz.bjfxy.top/gtxztrywtf.html

[C11] 模块导入与导出
来源：http://hz.pycfn.com/gtjmfydjnt.html

Py:   from module import func
来源：http://hz.zhongyouzk.top/gtemjdwbtb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xinyue.icu/gtxmitnpgm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dashuyun.cn/gtgtcdlewb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.aizwys.cn/gtcdzuyqpt.html

Java: import java.util.List;
来源：http://hz.yueranfly.top/gtfcjsffib.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jyoumei.cn/gtyddsjtpf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgfzy.top/gtmyczwdjf.html

C#:   using System.Text;
来源：http://hz.hywenlv.cn/gtjbdruvjj.html

[C12] 立即执行函数 IIFE
来源：http://hz.feifeiyinyue.top/gthkdlfqvf.html

Py:   (lambda: print("run"))()
来源：http://hz.pycfn.com/gtlcziqesz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yvedp.cn/gtoonorkdu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtuvgiouhg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtahcdqwqi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.52xcode.cn/gtcbiiwtjk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.smart0.xyz/gtcieeetkx.html

Ruby: -> { puts "run" }.call
来源：http://hz.gogol.net.cn/gtpgfbkrhl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hnxiangtu.top/gtryurwwfv.html

[C13] 类型声明 / 类型注解
来源：http://hz.yuxming.cn/gthqwbebhr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtdpcbjhse.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gthqyxspyn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.daria6918.cn/gtluodettm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtmckpnppd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ppjwa.cn/gtgzpipxcu.html

Go:   func add(a, b int) int
来源：http://hz.gotoacloud.top/gtiioanugt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gotoacloud.top/gtwxtjjvtc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxinkj.top/gtomuorbia.html

[C14] 泛型函数
来源：http://hz.cheryme.top/gtorzdfnod.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ybcxt.top/gtfmkvwiho.html

PHP:  // 无泛型
来源：http://hz.andypj.xyz/gtkekshhqg.html

JS:   // 无泛型
来源：http://hz.zhijiandao.cn/gtvenghmlh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hywenlv.cn/gtmgiobixq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.aizwys.cn/gtmsyrnmge.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.9152youxi.cn/gtstqiyxal.html

Ruby: # 无泛型
来源：http://hz.shangyingyoupin.top/gtefwuawms.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guannengcc.top/gtilazdkvt.html

[C15] 解构 / 展开参数
来源：http://hz.pycfn.com/gtvcysdgaw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sxryk.cn/gtmydxdtbv.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yonumen.top/gtiznvklkh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gtqhhstnrh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.kuanghao11.cn/gtvjrstyoc.html

Java: // 无解构
来源：http://hz.yongpay.top/gtvdhahwjt.html

Go:   // 无解构
来源：http://hz.meibo888.top/gtikumxtio.html

Ruby: a, b = pair
来源：http://hz.jlsjyb.cn/gtuxiwjiyh.html

C#:   var (a, b) = pair;
来源：http://hz.tian-w.cn/gtcqvpamba.html

[C16] 函数 / 方法重载
来源：http://hz.9152youxi.cn/gtiwmqfpfx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hysaishi.cn/gtnyuuirqc.html

PHP:  // 无重载
来源：http://hz.jinqigfzy.top/gtoilslfcl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.meibo888.top/gttbianjax.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ehwqpu.com/gtbsjoybva.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.0kj1m.cn/gtzlwrykzw.html

Go:   // 无重载：用不同函数名
来源：http://hz.cdnleiting.top/gtwitwracw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yvedp.cn/gtqdohcful.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xylfe.cn/gthvzqntzx.html

================================================================================
来源：http://hz.wangdashe.top/gtyrthcljr.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258888.top/gtrtmljoii.html

================================================================================
来源：http://hz.xuanzx.com/gtlninrzwv.html

[D01] 创建数组 / 列表
来源：http://hz.yongpay.top/gttygacthz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.mhx1999.top/gtddfhklzo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gotoacloud.top/gtirndxxpa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zdqjudy.top/gtraucqxxy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhaomingkeji.xyz/gtgdmaoxmj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sxryk.cn/gtgjvvykjf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ppjwa.cn/gtbhnncccw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nwbrower.top/gtlxgtokja.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jyoumei.cn/gtuugmtbrj.html

[D02] 追加元素到末尾
来源：http://hz.gzhubu.top/gtjmagplfw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jianghu66.top/gtqqkmgzlo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ywan-chungtsiang.top/gtewcbkxet.html

JS:   arr.push(4);
来源：http://hz.cashguo.top/gtspfrcalq.html

TS:   arr.push(4);
来源：http://hz.dianchejie.cn/gtozonmzhm.html

Java: list.add(4);
来源：http://hz.chenjidiqi.icu/gtebonazvx.html

Go:   arr = append(arr, 4)
来源：http://hz.zhongyouzk.top/gtzakxedwk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hfpthk.cn/gtedxyzlfe.html

C#:   list.Add(4);
来源：http://hz.jqgfzy.top/gtgypvwjjm.html

[D03] 在指定位置插入元素
来源：http://hz.cdnleiting.top/gttwtmxwbb.html

Py:   arr.insert(0, 0)
来源：http://hz.yj20258.top/gtbvqowkfn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.dianchejie.cn/gtesvvuyqn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jyoumei.cn/gteqmnejyq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cucudq.cn/gttgzfbppw.html

Java: list.add(0, 0);
来源：http://hz.iojbl.cn/gtuqsqjcds.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xinyue.icu/gtfmfujgie.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cucudq.cn/gtumwfcvwa.html

C#:   list.Insert(0, 0);
来源：http://hz.ehwqpu.com/gtwvfmtsla.html

[D04] 删除元素
来源：http://hz.xylfe.cn/gtdctllxqv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenzaomai.com/gtratopwra.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.bjfxy.top/gtgnsmsjre.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.wangshuangyany.cn/gtzwexssvs.html

TS:   arr.splice(0, 1);
来源：http://hz.sxryk.cn/gtdsjawziq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yongpay.top/gthzmdbauf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ehwqpu.com/gtzsoxifqg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sufxvd.cn/gtjljgqect.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.feifeiyinyue.top/gtbunemrbk.html

[D05] 访问与修改元素
来源：http://hz.ppjwa.cn/gtowxzlvgl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtgzzpvdwd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtnbkqvtpj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cqqwz.cn/gtzcgqlnbg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.fzhhl.top/gtqpuyiwqv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.c1oappe.top/gtnvucmycx.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gtzrdkmbxy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ivvv.top/gtyrmtmqot.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.fzhhl.top/gtthkfkfxq.html

[D06] 数组长度
来源：http://hz.yuanzhike.top/gtndaceasa.html

Py:   len(arr)
来源：http://hz.vqdsnc.cn/gtdxotqnky.html

PHP:  count($arr);
来源：http://hz.jyoumei.cn/gtduojrtut.html

JS:   arr.length
来源：http://hz.ywan-chungtsiang.top/gtwfhdwkql.html

TS:   arr.length
来源：http://hz.yueranfly.top/gtrrhftqoz.html

Java: list.size();
来源：http://hz.jyoumei.cn/gtcpsdqlps.html

Go:   len(arr)
来源：http://hz.smart0.xyz/gtvynildnf.html

Ruby: arr.length; arr.size
来源：http://hz.redwolf501.top/gtecbwyzfe.html

C#:   list.Count;
来源：http://hz.fengsongda.top/gtlllmlbaq.html

[D07] 切片 / 取子数组
来源：http://hz.ydjk.org.cn/gtsmqgumij.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cdnleiting.top/gtnvfsxxlg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhongyouzk.top/gtbgizhcwd.html

JS:   arr.slice(1, 4);
来源：http://hz.aibaodan.cn/gtoxadhkqe.html

TS:   arr.slice(1, 4);
来源：http://hz.zhiwuduotai.top/gtvepahfnm.html

Java: list.subList(1, 4);
来源：http://hz.xuetiantiany.cn/gtqqwcklme.html

Go:   arr[1:4]
来源：http://hz.redwolf501.top/gtlddotsye.html

Ruby: arr[1, 3]
来源：http://hz.sxryk.cn/gtegdtxfot.html

C#:   list.GetRange(1, 3);
来源：http://hz.jyoumei.cn/gttmxaikxq.html

[D08] 合并两个数组
来源：http://hz.svipenyu.cn/gtewlqzgaf.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenzaomai.com/gtvspscvmw.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258.top/gtmhsbiijx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.havefunace.top/gtpvqdoaqo.html

TS:   [...a, ...b];
来源：http://hz.jinghuilouyu.cn/gtrlnxucoc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yueranfly.top/gtlwqhxsvw.html

Go:   append(a, b...)
来源：http://hz.gotoacloud.top/gtnuxbvwuq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zycfv.cn/gtzgcurmtm.html

C#:   a.Concat(b).ToList()
来源：http://hz.mhx1999.top/gttwhmtaps.html

[D09] 排序（升序）
来源：http://hz.smart0.xyz/gtqolapaiv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtsyvkmzuk.html

PHP:  sort($arr);
来源：http://hz.sweek.top/gtkaarorci.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhaomingkeji.xyz/gtmrqxxuqq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pycfn.com/gtwcfxwzct.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hfpthk.cn/gtpnfgaqjy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tanke756.top/gtxfwlncpz.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtfhozayrg.html

C#:   list.Sort();
来源：http://hz.shangyingyoupin.top/gtcbardkhz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.andypj.xyz/gtcvshqltw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.daxiang520.top/gtqpqkedlr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gogol.net.cn/gtjneydsfs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.birdmap.top/gtzqqlrapz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigfzy.top/gtznjupazv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gzhubu.top/gtrylapemv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yueranfly.top/gtygzaskyk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuanzhike.top/gtufddoiwc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenzaomai.com/gtrhspeawa.html

[D11] 反转数组
来源：http://hz.chenlongwang.top/gtvpcxtmpa.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jlsjyb.cn/gtzozzyyxq.html

PHP:  array_reverse($arr);
来源：http://hz.meibo888.top/gtmtciigsd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.svipenyu.cn/gtiklfhatm.html

TS:   [...arr].reverse();
来源：http://hz.chenlongwang.top/gtkjllnrml.html

Java: Collections.reverse(list);
来源：http://hz.jinqigfzy.top/gtqpnraauy.html

Go:   slices.Reverse(arr)
来源：http://hz.c1oappe.top/gtdqepvqhj.html

Ruby: arr.reverse
来源：http://hz.ybcxt.top/gtphqrdyix.html

C#:   list.Reverse();
来源：http://hz.jianghu66.top/gtiobjlecy.html

[D12] 查找元素下标
来源：http://hz.feifeiyinyue.top/gtuqgmeruu.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhaomingkeji.xyz/gtsinhagny.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shangyingyoupin.top/gtttzzdsma.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtexzdocut.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daxiang520.top/gtzumazmql.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jiagoushi.top/gtsgxkejkr.html

Go:   slices.Index(arr, x)
来源：http://hz.zdqjudy.top/gtinwfaxcj.html

Ruby: arr.index(x)
来源：http://hz.hywenlv.cn/gtfksrprsb.html

C#:   list.IndexOf(x);
来源：http://hz.fzhhl.top/gtaqjegqxk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gzhubu.top/gtnrwpiujx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yueranfly.top/gtivkheikr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tianlin.xyz/gtrulpmzyc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sysykeji.top/gtexpqeecn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xylfe.cn/gtvgtlopvi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xuanzx.com/gtqqzsvycz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xingfuxueyuan.xyz/gthgdjcoxh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.snrcjt.cn/gtzsmhtwsu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yuanzhike.top/gtlicmxdev.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aibaodan.cn/gttcbxbzfp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj202588.top/gtvmfqbsrn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aizwys.cn/gtoyfpimff.html

JS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gtepclwqag.html

TS:   arr.map(x => x * 2)
来源：http://hz.vqdsnc.cn/gtouhigzoa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangtech.top/gtmfnweulh.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gtvrxsmcsi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.wangdashe.top/gtkcumlzsw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tanke756.top/gtqeimolws.html

[D15] 去重
来源：http://hz.jinyuanbaomall.cn/gtvecomfhz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cashguo.top/gtkyluaogj.html

PHP:  array_unique($arr);
来源：http://hz.nwbrower.top/gtiqwybhxs.html

JS:   [...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gtxypwewxf.html

TS:   [...new Set(arr)]
来源：http://hz.jianghu66.top/gtsbgqlene.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ehwqpu.com/gtsegvjwpx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hnqzz.top/gtjxzkanpq.html

Ruby: arr.uniq
来源：http://hz.zhiwuduotai.top/gtwhqxxhvx.html

C#:   list.Distinct().ToList()
来源：http://hz.sweek.top/gttvaeuqvi.html

[D16] 求和与平均值
来源：http://hz.ywan-chungtsiang.top/gtrohagngc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pengpengdd.cyou/gttxfrmlnc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cucudq.cn/gtovsnyttf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtpybotrob.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtkcpeygqt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daria6918.cn/gtdwbrzoxu.html

Go:   // 手写循环累加
来源：http://hz.cqqwz.cn/gtuwozfplo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cdnleiting.top/gtjglygjrq.html

C#:   list.Sum();  list.Average()
来源：http://hz.cucudq.cn/gtgygicula.html

[D17] 最大值与最小值
来源：http://hz.iojbl.cn/gtuwjaojak.html

Py:   max(arr);  min(arr)
来源：http://hz.xylfe.cn/gtbqaddlfk.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxuanxn.top/gtxeslkvjx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhaomingkeji.xyz/gthdyodoxx.html

TS:   Math.max(...arr);
来源：http://hz.cucudq.cn/gtlqwzjlkd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shuidangran.top/gtqhvyubou.html


<!-- 参考信息 -->