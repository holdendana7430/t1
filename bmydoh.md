代发 wailian999

[C02] 默认参数
来源：http://hz.xinyue.icu/gtyzaevhqe.html

Py:   def greet(name="World"): return name
来源：http://hz.cashguo.top/gtufoaxier.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hnqzz.top/gtjmkjpexo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.0kj1m.cn/gtxfphtwwb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.shuidangran.top/gtkgpbiezw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xinyue.icu/gtxujrvwgp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.snrcjt.cn/gtuthmcagk.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinyuanbaomall.cn/gtpkewvzkt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenlongwang.top/gtjnkyjyrk.html

[C03] 可变参数
来源：http://hz.tian-w.cn/gtvrcihfbw.html

Py:   def total(*args): return sum(args)
来源：http://hz.cqqwz.cn/gtnbunswxo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nanxinkj.top/gtnvizrvlk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cucudq.cn/gtrugorgym.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtzsytrsoj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.0kj1m.cn/gtvxuzppfn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ydjk.org.cn/gtnjkaqmnr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yanxiufei.cn/gtkezqmsqa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gogol.net.cn/gtrtqltuas.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinqigufen.top/gtvevysexy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.birdmap.top/gtrijnmexl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhixingplan.top/gtfnrhbadu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sxryk.cn/gtwckjenqv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xingfuxueyuan.xyz/gtxwnsifur.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yuxming.cn/gtvtwlzcgv.html

Go:   // 无：用配置结构体参数
来源：http://hz.birdmap.top/gteozfiuhh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.c1oappe.top/gtzdqejyjr.html

C#:   f(a: 1, b: 2)
来源：http://hz.aizwys.cn/gtgtwhstfa.html

[C05] 返回多个值
来源：http://hz.shuidangran.top/gtfcvgikwf.html

Py:   return a, b
来源：http://hz.hnqzz.top/gtrjwpdesh.html

PHP:  return [$a, $b];
来源：http://hz.52xcode.cn/gtotptznjy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shanyushiyangkeji.top/gtdlmxlfcf.html

TS:   return { a, b };
来源：http://hz.havefunace.top/gtghpvsvig.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.chenzaomai.com/gtkhqrxznr.html

Go:   return a, b
来源：http://hz.pengpengdd.cyou/gtkwkyqfnw.html

Ruby: return a, b
来源：http://hz.quarkkingdee.top/gtdlzdjinu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.0kj1m.cn/gtmkeixrqn.html

[C06] 匿名函数 / lambda
来源：http://hz.yonumen.top/gtuocfhfcr.html

Py:   square = lambda x: x * x
来源：http://hz.nanxuanxn.top/gthztovrcm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cdnleiting.top/gtohszwksh.html

JS:   const square = x => x * x;
来源：http://hz.vqdsnc.cn/gtyibtjdwx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.fzhhl.top/gtklwpbhul.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cheryme.top/gtudknwmmp.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yanxiufei.cn/gtauicbmxs.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jlsjyb.cn/gtwyeugrlg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuetiantiany.cn/gtyepqgsti.html

[C07] 把函数作为参数传入
来源：http://hz.cucudq.cn/gtrxeztxmv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sysykeji.top/gtrwqpwcbr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.andypj.xyz/gtquddmxlv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.gogol.net.cn/gtaledgmnv.html

TS:   arr.map(String)
来源：http://hz.shzxlz.cn/gtwxopizsw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.meibo888.top/gtxkhdqnew.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhiwuduotai.top/gtdqdggucl.html

Ruby: arr.map(&:upcase)
来源：http://hz.yvedp.cn/gtkkittlra.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yangfankeji.com/gtenisqkwn.html

[C08] 闭包
来源：http://hz.zycfv.cn/gtrqziawsu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhongyouzk.top/gtbgjupatt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenlongwang.top/gtuxwuseap.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtzadffqlb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtsximgpfn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xingfuxueyuan.xyz/gtfhgmrmsf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jlsjyb.cn/gtmzapkofr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.meibo888.top/gtzfktjjwe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gteergfcrv.html

[C09] 递归
来源：http://hz.chenzaomai.com/gtsxsatwny.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhaomingkeji.xyz/gtlzixtica.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cdnleiting.top/gtxviybjik.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hongshengwenyu.top/gtojqlgpoq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yanxiufei.cn/gtptdpcvou.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.quarkkingdee.top/gttbrsckvd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sufxvd.cn/gttjdpjasu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cheryme.top/gthgkaqgja.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxuanxn.top/gtjppxssqs.html

[C10] 变量作用域
来源：http://hz.dashuyun.cn/gtkiyjgkbl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.iojbl.cn/gtyjiprsop.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.quarkkingdee.top/gtzrwdhxcp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yuxming.cn/gtnaliusem.html

TS:   同 JS
来源：http://hz.nwbrower.top/gtxxfbzchl.html

Java: 方法内为块级作用域
来源：http://hz.smart0.xyz/gtsezzuyzo.html

Go:   花括号块级作用域
来源：http://hz.xuetiantiany.cn/gtjzhxkyuw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ppjwa.cn/gtjxzgekrd.html

C#:   块级作用域
来源：http://hz.andypj.xyz/gtpxdsgqym.html

[C11] 模块导入与导出
来源：http://hz.guannengcc.top/gttnvcudyb.html

Py:   from module import func
来源：http://hz.sweek.top/gtbpkhsvkx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhiwuduotai.top/gtigxdwidc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhiwuduotai.top/gtuwedrnph.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shzxlz.cn/gtsnkadeou.html

Java: import java.util.List;
来源：http://hz.nanxinkj.top/gtvxzkdtie.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.fzhhl.top/gtyvcbbjzt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ydzc1.top/gtpiqjuzfm.html

C#:   using System.Text;
来源：http://hz.sweek.top/gtbdiutojn.html

[C12] 立即执行函数 IIFE
来源：http://hz.kuanghao11.cn/gttrrmrnhz.html

Py:   (lambda: print("run"))()
来源：http://hz.yj20258888.top/gtfgsmceen.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhengqikj.top/gtlvvtezsd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yueranfly.top/gtgicnshaz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gtuqzxdnvz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinqigufen.top/gthawzuzwi.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sysykeji.top/gtjrgeluef.html

Ruby: -> { puts "run" }.call
来源：http://hz.jyoumei.cn/gtsxipohli.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.chenlongwang.top/gtkhpleyld.html

[C13] 类型声明 / 类型注解
来源：http://hz.yongpay.top/gtfphvlyca.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangshuangyany.cn/gtegqyfccu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtcfwrhods.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sweek.top/gtldmozsda.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuanzhike.top/gtiegdmjur.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gtatjdxetp.html

Go:   func add(a, b int) int
来源：http://hz.redwolf501.top/gtlxpvkhlz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fzhhl.top/gtymsjbnnk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hammf.cn/gtzwlbexbk.html

[C14] 泛型函数
来源：http://hz.9152youxi.cn/gtcuhpxzan.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cheryme.top/gtludcqeum.html

PHP:  // 无泛型
来源：http://hz.hnxiangtu.top/gtwrrnrwbw.html

JS:   // 无泛型
来源：http://hz.kuanghao11.cn/gtabzcwrru.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cucudq.cn/gtumfizdtx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.52xcode.cn/gtcgboaily.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ydjk.org.cn/gtmnvkjhwy.html

Ruby: # 无泛型
来源：http://hz.cheryme.top/gtaozivkaz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.nanxuanxn.top/gtacjivcwt.html

[C15] 解构 / 展开参数
来源：http://hz.ybcxt.top/gtmalrepmz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigfzy.top/gtnzsvbapg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhaomingkeji.xyz/gtcawidypn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gttnpnwkwu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yangfankeji.com/gthmsxlsmh.html

Java: // 无解构
来源：http://hz.yanxiufei.cn/gtzvtkjbyb.html

Go:   // 无解构
来源：http://hz.yueranfly.top/gtajojbsid.html

Ruby: a, b = pair
来源：http://hz.iojbl.cn/gtynqobnya.html

C#:   var (a, b) = pair;
来源：http://hz.meibo888.top/gtjnxsgeli.html

[C16] 函数 / 方法重载
来源：http://hz.aizwys.cn/gtwdbhjoif.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cheryme.top/gtqmlzconj.html

PHP:  // 无重载
来源：http://hz.zycfv.cn/gtotpewtvk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sweek.top/gtdeokqsoe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhixingplan.top/gtpvvepegq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.andypj.xyz/gtkxegbkxv.html

Go:   // 无重载：用不同函数名
来源：http://hz.kuanghao11.cn/gtdizcpgvi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.daria6918.cn/gthqfqroff.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinqigfzy.top/gtnnvtpsth.html

================================================================================
来源：http://hz.ivvv.top/gtxxffcezc.html

D. 数组 / 列表 / 集合
来源：http://hz.hfpthk.cn/gtawjjcxhw.html

================================================================================
来源：http://hz.hnqzz.top/gthyulqodu.html

[D01] 创建数组 / 列表
来源：http://hz.mhx1999.top/gtrzzruvve.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.bjfxy.top/gtgmxdorni.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.tian-w.cn/gtrjsewjaw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yuanzhike.top/gtnkybmbxe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xingfuxueyuan.xyz/gttumajckg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cucudq.cn/gtsywqranc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.52xcode.cn/gtpzrcliib.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhixingplan.top/gtufksjcxd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.daxiang520.top/gtntxtopbz.html

[D02] 追加元素到末尾
来源：http://hz.pengpengdd.cyou/gtwcwxbbdj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinghuilouyu.cn/gtdzhdmgcc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhongyouzk.top/gtgaogesvv.html

JS:   arr.push(4);
来源：http://hz.zycfv.cn/gthcfbqgmf.html

TS:   arr.push(4);
来源：http://hz.wangdashe.top/gtjuvcrpwx.html

Java: list.add(4);
来源：http://hz.cdnleiting.top/gtrfcxwjks.html

Go:   arr = append(arr, 4)
来源：http://hz.chenzaomai.com/gtofdcjuoi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhengqikj.top/gtdobsmnwu.html

C#:   list.Add(4);
来源：http://hz.jlsjyb.cn/gtuzpxbpxu.html

[D03] 在指定位置插入元素
来源：http://hz.xingfuxueyuan.xyz/gtylbtftsa.html

Py:   arr.insert(0, 0)
来源：http://hz.jianghu66.top/gtcduuboaa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ybcxt.top/gtilxqzhuw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sxryk.cn/gtgwampejq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gotoacloud.top/gtmmsuckuq.html

Java: list.add(0, 0);
来源：http://hz.hfpthk.cn/gtfakjkkzf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yonumen.top/gtxiflaxad.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tanke756.top/gtawmobdod.html

C#:   list.Insert(0, 0);
来源：http://hz.zdqjudy.top/gtdciddlgb.html

[D04] 删除元素
来源：http://hz.zhixingplan.top/gtmcnfzqjz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ivvv.top/gtbiwcvivx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhixingplan.top/gtjceznpir.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jiagoushi.top/gtsalyxhst.html

TS:   arr.splice(0, 1);
来源：http://hz.9152youxi.cn/gttksylgvs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shzxlz.cn/gtxrmvwqyy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.havefunace.top/gtskcmvvhy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ivvv.top/gtwnooyotr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ybcxt.top/gtqkbmeeko.html

[D05] 访问与修改元素
来源：http://hz.hysaishi.cn/gtprjuthaa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xylfe.cn/gtrkfegmqq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zycfv.cn/gtbvqtvmim.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.c1oappe.top/gtzowgqxmr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.nanxuanxn.top/gtpeeklqbt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shanyushiyangtech.top/gtvjthbocj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.birdmap.top/gtaxtmcfiv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cucudq.cn/gtrgifrzix.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj202588.top/gtihmqwzeg.html

[D06] 数组长度
来源：http://hz.jyoumei.cn/gtgyqatudk.html

Py:   len(arr)
来源：http://hz.nanxinkj.top/gtxfftlseq.html

PHP:  count($arr);
来源：http://hz.ywan-chungtsiang.top/gtzcywbkia.html

JS:   arr.length
来源：http://hz.cucudq.cn/gtmqssofzn.html

TS:   arr.length
来源：http://hz.hnqzz.top/gtdvkpfyat.html

Java: list.size();
来源：http://hz.hfpthk.cn/gthlzvtwey.html

Go:   len(arr)
来源：http://hz.yj20258888.top/gttcjantpp.html

Ruby: arr.length; arr.size
来源：http://hz.ywan-chungtsiang.top/gtnefrvrrk.html

C#:   list.Count;
来源：http://hz.jinyuanbaomall.cn/gtywikvfkc.html

[D07] 切片 / 取子数组
来源：http://hz.feifeiyinyue.top/gtbikbkjzu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.chenzaomai.com/gtcyieavyh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yueranfly.top/gtmhgkpmfy.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangkeji.top/gteaegnqio.html

TS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gtugracatd.html

Java: list.subList(1, 4);
来源：http://hz.wangshuangyany.cn/gtnrtbhzyx.html

Go:   arr[1:4]
来源：http://hz.sufxvd.cn/gtdbyjvvtr.html

Ruby: arr[1, 3]
来源：http://hz.jqgufenzy.top/gtneaygtmt.html

C#:   list.GetRange(1, 3);
来源：http://hz.zycfv.cn/gtcygrqmth.html

[D08] 合并两个数组
来源：http://hz.zycfv.cn/gtezkliiqa.html

Py:   a + b;  a.extend(b)
来源：http://hz.haohaochexian.top/gtaqsyenxp.html

PHP:  array_merge($a, $b);
来源：http://hz.zycfv.cn/gtcwnrssfx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.fengsongda.top/gthtaymvsf.html

TS:   [...a, ...b];
来源：http://hz.zhiwuduotai.top/gtvarknwrc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.quarkkingdee.top/gtfvnbvbsk.html

Go:   append(a, b...)
来源：http://hz.shangyingyoupin.top/gtvhfqqhiu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jqgfzy.top/gtgkzfvlxh.html

C#:   a.Concat(b).ToList()
来源：http://hz.shanyushiyangtech.top/gttajhdnhq.html

[D09] 排序（升序）
来源：http://hz.nanxinkj.top/gtmxhxdwhm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtejjcedqv.html

PHP:  sort($arr);
来源：http://hz.gotoacloud.top/gtczzbmhez.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jianghu66.top/gtylirevcm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.9152youxi.cn/gtovubjegg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.daria6918.cn/gtitnonnvz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yuxming.cn/gtppndexma.html

Ruby: arr.sort
来源：http://hz.ydzc1.top/gtmoeydgjc.html

C#:   list.Sort();
来源：http://hz.bjfxy.top/gtxmnrxwhy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yueranfly.top/gtbwcopuau.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangdashe.top/gtgpcaxmen.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydzc1.top/gttgnzbbva.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gturmlkyel.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gttcrhanpn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.pengpengdd.cyou/gtgjxuxzvr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sysykeji.top/gturtsaijn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ivvv.top/gthsuctzps.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shzxlz.cn/gtixryyeli.html

[D11] 反转数组
来源：http://hz.dashuyun.cn/gteuddhyij.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhijiandao.cn/gtryjtzxea.html

PHP:  array_reverse($arr);
来源：http://hz.cucudq.cn/gtxwsnrqom.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xinyue.icu/gtlkvgmhhq.html

TS:   [...arr].reverse();
来源：http://hz.dashuyun.cn/gtaaxsrylb.html

Java: Collections.reverse(list);
来源：http://hz.shanyushiyangkeji.top/gtoufylebj.html

Go:   slices.Reverse(arr)
来源：http://hz.wangshuangyany.cn/gtdrdfnmaj.html

Ruby: arr.reverse
来源：http://hz.xylfe.cn/gtqtkqfwzj.html

C#:   list.Reverse();
来源：http://hz.chenlongwang.top/gtxggqvarq.html

[D12] 查找元素下标
来源：http://hz.hammf.cn/gtwfoiymeg.html

Py:   arr.index(x);  x in arr
来源：http://hz.yvedp.cn/gtdvxwkvul.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgfzy.top/gtlncbwnba.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtplxwvuua.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj202588.top/gtkhmmhcoj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.52xcode.cn/gttxfktisi.html

Go:   slices.Index(arr, x)
来源：http://hz.yj20258888.top/gtuyyfrhpj.html

Ruby: arr.index(x)
来源：http://hz.ppjwa.cn/gtwhfuzucc.html

C#:   list.IndexOf(x);
来源：http://hz.316326.xyz/gtcenerbcq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sweek.top/gtibujtytg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinyuanbaomall.cn/gtygxxbrlf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.dianchejie.cn/gtvmvafeiu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenlongwang.top/gtiyckryhb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.0kj1m.cn/gtafzrmppl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhoulong.xyz/gtlgakumns.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.feifeiyinyue.top/gtjqppvnob.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sufxvd.cn/gtdxwtscuq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dianchejie.cn/gtvvhrsmhf.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fengsongda.top/gtodzvgtmw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tianlin.xyz/gtlpgycdvn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yanxiufei.cn/gtuqhpuhqr.html

JS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtxhnuqzwb.html

TS:   arr.map(x => x * 2)
来源：http://hz.wangshuangyany.cn/gtfbblgkxr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tianlin.xyz/gtmsrctnqa.html

Go:   // 手写循环
来源：http://hz.jiagoushi.top/gtkkicqnat.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cashguo.top/gtvajmypta.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhijiandao.cn/gtldhgwtre.html

[D15] 去重
来源：http://hz.wangshuangyany.cn/gtlfxkbwgi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.fzhhl.top/gtxwkclokr.html

PHP:  array_unique($arr);
来源：http://hz.sxryk.cn/gtqtuhsptl.html

JS:   [...new Set(arr)]
来源：http://hz.ydjk.org.cn/gtjihnkcdx.html

TS:   [...new Set(arr)]
来源：http://hz.xinyue.icu/gtdeghwkdc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.meibo888.top/gtokcunnlg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xinyue.icu/gtgwumoyde.html

Ruby: arr.uniq
来源：http://hz.daria6918.cn/gtsswzgocr.html

C#:   list.Distinct().ToList()
来源：http://hz.shanyushiyangtech.top/gtlkvxpmpe.html

[D16] 求和与平均值
来源：http://hz.svipenyu.cn/gtvtcwrjzg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shangyingyoupin.top/gtbazyfbfv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guannengcc.top/gtwcbetvka.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jianghu66.top/gtiahxptre.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhaomingkeji.xyz/gtwnydjcoc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sweek.top/gtntaodcev.html

Go:   // 手写循环累加
来源：http://hz.daria6918.cn/gthitwdldz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cdnleiting.top/gtygjdmwls.html

C#:   list.Sum();  list.Average()
来源：http://hz.iojbl.cn/gtdwcnhxkk.html

[D17] 最大值与最小值
来源：http://hz.xziqi.cn/gtkpimpjmf.html

Py:   max(arr);  min(arr)
来源：http://hz.fengsongda.top/gthtsugdaz.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtsicupvzr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.9152youxi.cn/gtzudfsviz.html

TS:   Math.max(...arr);
来源：http://hz.jinqigufen.top/gtcmeotmmx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenzaomai.com/gthtnaitab.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hywenlv.cn/gtaanoucii.html

Ruby: arr.max;  arr.min
来源：http://hz.nwbrower.top/gttrsttzvq.html

C#:   list.Max();  list.Min()
来源：http://hz.tian-w.cn/gtcrwdduta.html

[D18] 扁平化嵌套数组
来源：http://hz.hongshengwenyu.top/gtbhhyopnp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.redwolf501.top/gtdyxwdisp.html

PHP:  array_merge(...$nested);
来源：http://hz.ivvv.top/gtvihtrwch.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xylfe.cn/gtncyvebsk.html

TS:   nested.flat();
来源：http://hz.c1oappe.top/gthmgukfto.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.kuanghao11.cn/gtlmenqwqf.html

Go:   // 手写双层循环
来源：http://hz.hysaishi.cn/gtlofjruot.html

Ruby: nested.flatten
来源：http://hz.cqqwz.cn/gtrzczvrvl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gotoacloud.top/gtbmabdqwg.html


<!-- 参考信息 -->