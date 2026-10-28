代发 wailian999

================================================================================
来源：http://hz.sufxvd.cn/gtpcdpnwpl.html

C. 函数与作用域
来源：http://hz.yangfankeji.com/gtfjmkprmt.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjdudvafi.html

[C01] 定义函数
来源：http://hz.jinqigufen.top/gtvdpxkajm.html

Py:   def add(a, b): return a + b
来源：http://hz.redwolf501.top/gtqckkkwxw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gtwxlilduu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.52xcode.cn/gtygrbyhtp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gtphewvzry.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtczrtfvpn.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yvedp.cn/gtcknknelq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sysykeji.top/gttfcnddkv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtztdlqhye.html

[C02] 默认参数
来源：http://hz.dianchejie.cn/gtgpeikhbe.html

Py:   def greet(name="World"): return name
来源：http://hz.gotoacloud.top/gtfldbneeg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yuanzhike.top/gtobsdzivw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj20258.top/gtfnzmttfq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtyietmkfc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.svipenyu.cn/gttnlkxgwn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jinghuilouyu.cn/gtmjgpnwik.html

Ruby: def greet(name = "World") = name
来源：http://hz.ydjk.org.cn/gtgjvebqsu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.dianchejie.cn/gtgxnvcpbg.html

[C03] 可变参数
来源：http://hz.chenzaomai.com/gtxbdanyte.html

Py:   def total(*args): return sum(args)
来源：http://hz.cashguo.top/gtilbwbaga.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nanxuanxn.top/gtwgrzovfx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.c1oappe.top/gthiscgvod.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tian-w.cn/gtjzkalory.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hnxiangtu.top/gtnqozzkih.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangdashe.top/gtipmhsynm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.feifeiyinyue.top/gtdwwdhvub.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xziqi.cn/gtneabypuk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yanxiufei.cn/gtryoanyme.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zycfv.cn/gtflxkdduz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xuetiantiany.cn/gtmwyprxpb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xuanzx.com/gtgpbbrtol.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shanyushiyangkeji.top/gtdypuiozz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.vqdsnc.cn/gtjmuympqe.html

Go:   // 无：用配置结构体参数
来源：http://hz.sufxvd.cn/gtwchmymta.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenjidiqi.icu/gthgqwpfjy.html

C#:   f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtakrrinvz.html

[C05] 返回多个值
来源：http://hz.zhongyouzk.top/gtgrzjqjrj.html

Py:   return a, b
来源：http://hz.ivvv.top/gtdqaslxfp.html

PHP:  return [$a, $b];
来源：http://hz.wangdashe.top/gtgybvxznq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jyoumei.cn/gtuksommby.html

TS:   return { a, b };
来源：http://hz.daria6918.cn/gtnbhztgob.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zdqjudy.top/gtssblbdmx.html

Go:   return a, b
来源：http://hz.wangdashe.top/gtpfdtwkgw.html

Ruby: return a, b
来源：http://hz.shzxlz.cn/gtxibafdvd.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.9152youxi.cn/gtveubcnbf.html

[C06] 匿名函数 / lambda
来源：http://hz.hfpthk.cn/gtnqlwjytl.html

Py:   square = lambda x: x * x
来源：http://hz.sxryk.cn/gtlpdnkwsf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.svipenyu.cn/gtjjfwyphf.html

JS:   const square = x => x * x;
来源：http://hz.ehwqpu.com/gtyztijpph.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.c1oappe.top/gtnsmrhugg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.vqdsnc.cn/gtlwygetpk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.haohaochexian.top/gthitouxwe.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tian-w.cn/gtyzftqlbk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.chenzaomai.com/gtngykihjg.html

[C07] 把函数作为参数传入
来源：http://hz.sysykeji.top/gtxtimcnem.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.feifeiyinyue.top/gtzdrjasff.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.kuanghao11.cn/gtkubxfhya.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shuidangran.top/gtsagprnao.html

TS:   arr.map(String)
来源：http://hz.yanxiufei.cn/gthzmsepyl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jyoumei.cn/gtkzktoreh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.bjfxy.top/gtvcnsflpx.html

Ruby: arr.map(&:upcase)
来源：http://hz.yuanzhike.top/gtonlmlafz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jyoumei.cn/gtsugygsui.html

[C08] 闭包
来源：http://hz.nanxinkj.top/gtfbssekbj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shangyingyoupin.top/gtdxyjlszw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.aizwys.cn/gtwkpwqznn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gtzatbjyct.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.fengsongda.top/gtcxkzlanw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jqgufenzy.top/gtxcnapabn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.dianchejie.cn/gteazekxkn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.quarkkingdee.top/gtpvswslaa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtfysncaho.html

[C09] 递归
来源：http://hz.haohaochexian.top/gtivukkljq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.fzhhl.top/gtsebjeokn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhoulong.xyz/gtyffgcdyk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuetiantiany.cn/gtpvttuceu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fzhhl.top/gtwfdxuphs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tian-w.cn/gtigurutyx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhongyouzk.top/gtmyfoevqb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.vqdsnc.cn/gtpyarygzs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.9152youxi.cn/gtiszjqdxk.html

[C10] 变量作用域
来源：http://hz.wangshuangyany.cn/gtjnbjbsnd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sweek.top/gtoqzuogfy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ppjwa.cn/gtzuewdial.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aizwys.cn/gtpsshsrcm.html

TS:   同 JS
来源：http://hz.yuxming.cn/gteerljodu.html

Java: 方法内为块级作用域
来源：http://hz.dianchejie.cn/gtyeqdrkxl.html

Go:   花括号块级作用域
来源：http://hz.gaohongyu789.top/gtgjoqcfxo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xinyue.icu/gtlkjstwer.html

C#:   块级作用域
来源：http://hz.mhx1999.top/gthoztlome.html

[C11] 模块导入与导出
来源：http://hz.yuanzhike.top/gtiznpmvfr.html

Py:   from module import func
来源：http://hz.zhiwuduotai.top/gtwvecjqee.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.mhx1999.top/gtlgcydreo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.guowangkeji.top/gteetaljhs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ydzc1.top/gtrvtwcwzg.html

Java: import java.util.List;
来源：http://hz.pycfn.com/gtspwfznxd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.mhx1999.top/gtunpefskt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hywenlv.cn/gtauyyqxot.html

C#:   using System.Text;
来源：http://hz.9152youxi.cn/gtbixkyneb.html

[C12] 立即执行函数 IIFE
来源：http://hz.xingfuxueyuan.xyz/gtbbkawxuv.html

Py:   (lambda: print("run"))()
来源：http://hz.jianghu66.top/gtanvnxtyr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.vqdsnc.cn/gtpnuochzg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jqgufenzy.top/gtxjgbcpmi.html

TS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gttniozpyy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daria6918.cn/gthtvxzonf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cashguo.top/gtglpiuasy.html

Ruby: -> { puts "run" }.call
来源：http://hz.hnqzz.top/gtjkxdpiqf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xylfe.cn/gtxxbxuimx.html

[C13] 类型声明 / 类型注解
来源：http://hz.shanyushiyangkeji.top/gtojsnvwnt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhixingplan.top/gtetqexhzv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gtcqopadzh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.haohaochexian.top/gtzeglrafc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cqqwz.cn/gttpargefd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ppjwa.cn/gtmjislezf.html

Go:   func add(a, b int) int
来源：http://hz.haohaochexian.top/gtvzecdavj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.aibaodan.cn/gtkffjanwf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxuanxn.top/gtzrjrfmif.html

[C14] 泛型函数
来源：http://hz.c1oappe.top/gtdltgmoqz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yonumen.top/gtdcjokfaq.html

PHP:  // 无泛型
来源：http://hz.jiagoushi.top/gteegyynpy.html

JS:   // 无泛型
来源：http://hz.wangdashe.top/gtxdrhlpoj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dianchejie.cn/gtfehrcgrb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ivvv.top/gtnnkalowa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenlongwang.top/gtkuaxmnqy.html

Ruby: # 无泛型
来源：http://hz.nwbrower.top/gtqitqywkj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhiwuduotai.top/gtrxvbmtmq.html

[C15] 解构 / 展开参数
来源：http://hz.nwbrower.top/gttqvxslyq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhijiandao.cn/gtapbrlbfd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xuetiantiany.cn/gtkrlnxpkh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nwbrower.top/gtyjnxxgpb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zdqjudy.top/gtmfccjbmt.html

Java: // 无解构
来源：http://hz.ydjk.org.cn/gtwimefsiz.html

Go:   // 无解构
来源：http://hz.smart0.xyz/gtvhszfyfl.html

Ruby: a, b = pair
来源：http://hz.nanxuanxn.top/gtlfyoyclr.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangkeji.top/gtzzvwudbj.html

[C16] 函数 / 方法重载
来源：http://hz.ehwqpu.com/gtevxwlepq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hnqzz.top/gtzzpicccw.html

PHP:  // 无重载
来源：http://hz.yuxming.cn/gtcnpacvmi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenjidiqi.icu/gtqeztbzkn.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daria6918.cn/gtgqwoaxqp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zycfv.cn/gthjevuoyb.html

Go:   // 无重载：用不同函数名
来源：http://hz.ppjwa.cn/gttuprzhvo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.quarkkingdee.top/gtzpqclfbw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.meibo888.top/gtzahooyko.html

================================================================================
来源：http://hz.tanke756.top/gtclboruvk.html

D. 数组 / 列表 / 集合
来源：http://hz.dashuyun.cn/gtowwdyifv.html

================================================================================
来源：http://hz.meibo888.top/gtihcxqxbv.html

[D01] 创建数组 / 列表
来源：http://hz.cdnleiting.top/gtihyqfwlb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.c1oappe.top/gtyluzmvzd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hammf.cn/gtbnttxjiy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.wangshuangyany.cn/gtsdacwwng.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xingfuxueyuan.xyz/gtlugmuxul.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ydjk.org.cn/gtbelhkafr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.0kj1m.cn/gtvjhrtyvc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daxiang520.top/gtqovrnjjw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.quarkkingdee.top/gtgwhcbple.html

[D02] 追加元素到末尾
来源：http://hz.wangshuangyany.cn/gtevakcqin.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.havefunace.top/gtszmcoyrm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.c1oappe.top/gtqtwsuzqs.html

JS:   arr.push(4);
来源：http://hz.smart0.xyz/gtnndwjdqr.html

TS:   arr.push(4);
来源：http://hz.wangdashe.top/gtmfddppjv.html

Java: list.add(4);
来源：http://hz.iojbl.cn/gtjjhmidxk.html

Go:   arr = append(arr, 4)
来源：http://hz.316326.xyz/gthvbdpvkd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hongshengwenyu.top/gtkhhtsqta.html

C#:   list.Add(4);
来源：http://hz.ydzc1.top/gtymdbmhap.html

[D03] 在指定位置插入元素
来源：http://hz.c1oappe.top/gtgdnujvsk.html

Py:   arr.insert(0, 0)
来源：http://hz.fzhhl.top/gtzwmggxmn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xuanzx.com/gtlseylmnr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.haohaochexian.top/gthqxewukp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ybcxt.top/gtrvowtjgv.html

Java: list.add(0, 0);
来源：http://hz.ydzc1.top/gtcnkgqfvh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yonumen.top/gtdtjpwqho.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydzc1.top/gtamjwjqgi.html

C#:   list.Insert(0, 0);
来源：http://hz.jyoumei.cn/gtakvtxltx.html

[D04] 删除元素
来源：http://hz.iojbl.cn/gtttwihqco.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hysaishi.cn/gtrimjulyo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.meibo888.top/gtnsqefbsk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yueranfly.top/gtzubvocib.html

TS:   arr.splice(0, 1);
来源：http://hz.daria6918.cn/gtcclrvtyu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cashguo.top/gtmfdoqmhg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nanxinkj.top/gtnmxllmbe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sysykeji.top/gtibksugji.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yvedp.cn/gtkizunpfi.html

[D05] 访问与修改元素
来源：http://hz.feifeiyinyue.top/gtzcgglbwf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtpeneslsh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shangyingyoupin.top/gtnmotqljs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.c1oappe.top/gtbcwsjlxq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ivvv.top/gtjorjxgxg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhengqikj.top/gtkjezzryk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jianghu66.top/gtorqhpyfx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtjyipihyk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.guannengcc.top/gtvlpuvuse.html

[D06] 数组长度
来源：http://hz.shanyushiyangtech.top/gtjiyqpvoc.html

Py:   len(arr)
来源：http://hz.fzhhl.top/gtmubujpqx.html

PHP:  count($arr);
来源：http://hz.zdqjudy.top/gtxswtvwku.html

JS:   arr.length
来源：http://hz.sufxvd.cn/gtniwatemu.html

TS:   arr.length
来源：http://hz.chenjidiqi.icu/gtrcbqedtf.html

Java: list.size();
来源：http://hz.zhaomingkeji.xyz/gtyjszaifl.html

Go:   len(arr)
来源：http://hz.yuanzhike.top/gtnrpvjuym.html

Ruby: arr.length; arr.size
来源：http://hz.wangdashe.top/gtvcbmvrgo.html

C#:   list.Count;
来源：http://hz.dianchejie.cn/gtocgvppcc.html

[D07] 切片 / 取子数组
来源：http://hz.shuidangran.top/gtfeydzdax.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xinyue.icu/gteftoerxa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.haohaochexian.top/gtsufkevqr.html

JS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtomlgponb.html

TS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtrqislrww.html

Java: list.subList(1, 4);
来源：http://hz.svipenyu.cn/gtwqgkanlu.html

Go:   arr[1:4]
来源：http://hz.zhijiandao.cn/gtchfewxde.html

Ruby: arr[1, 3]
来源：http://hz.yanxiufei.cn/gtptznyahr.html

C#:   list.GetRange(1, 3);
来源：http://hz.jianghu66.top/gtpvpjquvj.html

[D08] 合并两个数组
来源：http://hz.vqdsnc.cn/gtqfnzmhem.html

Py:   a + b;  a.extend(b)
来源：http://hz.yuanzhike.top/gtaozlxyfe.html

PHP:  array_merge($a, $b);
来源：http://hz.cashguo.top/gtouuncuqv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sysykeji.top/gtdtiygpwi.html

TS:   [...a, ...b];
来源：http://hz.chenzaomai.com/gtbfoauijd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.bjfxy.top/gtugdsabur.html

Go:   append(a, b...)
来源：http://hz.ydjk.org.cn/gtwvndmrdn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinyuanbaomall.cn/gthpyhybvy.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenzaomai.com/gtwrhxajof.html

[D09] 排序（升序）
来源：http://hz.feifeiyinyue.top/gtphplhghe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xingfuxueyuan.xyz/gterfmduuh.html

PHP:  sort($arr);
来源：http://hz.vqdsnc.cn/gtcgxhrakb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenzaomai.com/gtqcpxkbtr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xziqi.cn/gtqriejfrj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhaomingkeji.xyz/gtteknmsre.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yvedp.cn/gtacvuxtxa.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtyjoaighj.html

C#:   list.Sort();
来源：http://hz.wangshuangyany.cn/gtvitfaobd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.quarkkingdee.top/gtgnadptee.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.iojbl.cn/gtyvemurnw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.9152youxi.cn/gtndvgdmoc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj202588.top/gtotgkrsdy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aizwys.cn/gtwtalzowa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yangfankeji.com/gtdihhdwnd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gogol.net.cn/gtsdzpkdki.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jyoumei.cn/gtbmxncdml.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hongshengwenyu.top/gttswuvwom.html

[D11] 反转数组
来源：http://hz.gogol.net.cn/gtomyzwzgh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shangyingyoupin.top/gtcejpofnv.html

PHP:  array_reverse($arr);
来源：http://hz.sxryk.cn/gtemjrnxzb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ppjwa.cn/gtnorhvbja.html

TS:   [...arr].reverse();
来源：http://hz.52xcode.cn/gtbhafnoez.html

Java: Collections.reverse(list);
来源：http://hz.gzhubu.top/gtpvqvuriq.html

Go:   slices.Reverse(arr)
来源：http://hz.0kj1m.cn/gtluvqtrpz.html

Ruby: arr.reverse
来源：http://hz.shangyingyoupin.top/gtepvzdmxf.html

C#:   list.Reverse();
来源：http://hz.havefunace.top/gtfzygtcux.html

[D12] 查找元素下标
来源：http://hz.iojbl.cn/gtbxorjjpb.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangtech.top/gtrkkbdktg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nwbrower.top/gtiqdodmtg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangshuangyany.cn/gtxvtpvtqx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtqdfdylat.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.fengsongda.top/gtrdjnuipv.html

Go:   slices.Index(arr, x)
来源：http://hz.hnxiangtu.top/gttaaxukdr.html

Ruby: arr.index(x)
来源：http://hz.cheryme.top/gtvdloqdqf.html

C#:   list.IndexOf(x);
来源：http://hz.jyoumei.cn/gtangcrhti.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hysaishi.cn/gthgvipbkb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xylfe.cn/gtkcvxvrfm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jiagoushi.top/gtftlqrqdu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtwpeydtyh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gthjltyroh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.guowangkeji.top/gtieehnskd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jlsjyb.cn/gtpapzfjip.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.quarkkingdee.top/gtvjzyrpvu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yonumen.top/gtexqynjcz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jqgfzy.top/gteybwubaz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cdnleiting.top/gtskablouj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hongshengwenyu.top/gtatnfdjhx.html

JS:   arr.map(x => x * 2)
来源：http://hz.gaohongyu789.top/gtgsikxqpt.html

TS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtmcpbfcfm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj20258.top/gtphsftbkw.html

Go:   // 手写循环
来源：http://hz.yuanzhike.top/gtkaugzcca.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnqzz.top/gtqxvydhce.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.guowangkeji.top/gthqxjdtvs.html

[D15] 去重
来源：http://hz.hammf.cn/gtnkrjyqun.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtawyekqny.html

PHP:  array_unique($arr);
来源：http://hz.gaohongyu789.top/gtyjvvofel.html

JS:   [...new Set(arr)]
来源：http://hz.shzxlz.cn/gttiyxlgjj.html

TS:   [...new Set(arr)]
来源：http://hz.yueranfly.top/gtbhhgeuer.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yangfankeji.com/gtpkuchtdd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.c1oappe.top/gtpcruyvze.html

Ruby: arr.uniq
来源：http://hz.yuanzhike.top/gtndzjqhak.html

C#:   list.Distinct().ToList()
来源：http://hz.zhongyouzk.top/gtmsodsluq.html

[D16] 求和与平均值
来源：http://hz.pengpengdd.cyou/gtdcgxbttu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenjidiqi.icu/gtxifbjwmn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ydjk.org.cn/gtnhfrcpwy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gtgyuxtzof.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gttdtihfdp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhixingplan.top/gtsepixqsx.html

Go:   // 手写循环累加
来源：http://hz.ydzc1.top/gtkzztrrtp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhongyouzk.top/gtvfjeyhwb.html

C#:   list.Sum();  list.Average()
来源：http://hz.kuanghao11.cn/gtexobuabt.html

[D17] 最大值与最小值
来源：http://hz.zycfv.cn/gtrhefudvd.html

Py:   max(arr);  min(arr)
来源：http://hz.pycfn.com/gtnqtdqfro.html

PHP:  max($arr);  min($arr);
来源：http://hz.xinyue.icu/gtfgtfmcbw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.52xcode.cn/gtofojyhhs.html

TS:   Math.max(...arr);
来源：http://hz.mhx1999.top/gtjfqlakpx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tanke756.top/gtbwfwuevr.html


<!-- 参考信息 -->