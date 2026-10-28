代发 wailian999

Go:   a && b || !c
来源：http://hz.chenlongwang.top/gtuenjqvgo.html

Ruby: a && b || !c
来源：http://hz.zhiwuduotai.top/gtrzdyrqzj.html

C#:   a && b || !c
来源：http://hz.cucudq.cn/gtfvedkzmn.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.wangshuangyany.cn/gtelsjfgik.html

Py:   if not data: return
来源：http://hz.yuanzhike.top/gtewlxfiju.html

PHP:  if (!$data) { return; }
来源：http://hz.yonumen.top/gtmmezpruj.html

JS:   if (!data) return;
来源：http://hz.pycfn.com/gtderqpcgr.html

TS:   if (!data) return;
来源：http://hz.9152youxi.cn/gtajaflqlc.html

Java: if (data == null) return;
来源：http://hz.ivvv.top/gtfzogtqtp.html

Go:   if data == nil { return }
来源：http://hz.xinyue.icu/gtrrvyqrko.html

Ruby: return if data.nil?
来源：http://hz.xuanzx.com/gtegcejrmg.html

C#:   if (data == null) return;
来源：http://hz.xuanzx.com/gtfgyaanbp.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgutiylep.html

C. 函数与作用域
来源：http://hz.zycfv.cn/gtuyyftdax.html

================================================================================
来源：http://hz.jlsjyb.cn/gtgvjnvbsb.html

[C01] 定义函数
来源：http://hz.jqgufenzy.top/gtkqgkjsdn.html

Py:   def add(a, b): return a + b
来源：http://hz.ywan-chungtsiang.top/gtxzhjcrco.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtoasypctc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hnqzz.top/gtcpancipi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258888.top/gtvfdacltj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtvjccczcc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gaohongyu789.top/gtvaaxkyxe.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xuanzx.com/gtnmnspvgh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gtbuxkouun.html

[C02] 默认参数
来源：http://hz.haohaochexian.top/gtcztqhaiu.html

Py:   def greet(name="World"): return name
来源：http://hz.svipenyu.cn/gtepuvjgle.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sweek.top/gtcvlltqxc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtfaymyoiu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.andypj.xyz/gtyqhwavmn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.havefunace.top/gtahcseixc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ehwqpu.com/gtzgitvkma.html

Ruby: def greet(name = "World") = name
来源：http://hz.yvedp.cn/gtmwxdqwqg.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hnxiangtu.top/gtmpolhkem.html

[C03] 可变参数
来源：http://hz.wangdashe.top/gtcixsmfzk.html

Py:   def total(*args): return sum(args)
来源：http://hz.ppjwa.cn/gtrbdiejej.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.andypj.xyz/gtkowetmna.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.haohaochexian.top/gtrxjqyknf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.vqdsnc.cn/gtlcqfkhev.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinyuanbaomall.cn/gtlbkhtbwg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.bjfxy.top/gtvhegmopv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shanyushiyangtech.top/gtuhglsrgj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.c1oappe.top/gtkhwhhpuf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhongyouzk.top/gtbykrmjqz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sweek.top/gtzeqfilgu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sysykeji.top/gtldkzacba.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shuidangran.top/gtahuhanct.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yvedp.cn/gtlbhcsdpd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hywenlv.cn/gtdddntphi.html

Go:   // 无：用配置结构体参数
来源：http://hz.meibo888.top/gtioxrcyhl.html

Ruby: f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtcwyltgnl.html

C#:   f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtwxybqhxv.html

[C05] 返回多个值
来源：http://hz.haohaochexian.top/gtrysetkzx.html

Py:   return a, b
来源：http://hz.hysaishi.cn/gtffmwmvhw.html

PHP:  return [$a, $b];
来源：http://hz.zycfv.cn/gtbnsldjvd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jqgufenzy.top/gtfoejnobp.html

TS:   return { a, b };
来源：http://hz.guannengcc.top/gtnwxhiref.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.meibo888.top/gtqccsrzbd.html

Go:   return a, b
来源：http://hz.yongpay.top/gtsbkzvohj.html

Ruby: return a, b
来源：http://hz.yangfankeji.com/gtklzwkpxz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sufxvd.cn/gtygyvwwlx.html

[C06] 匿名函数 / lambda
来源：http://hz.ydjk.org.cn/gthuvdkcdv.html

Py:   square = lambda x: x * x
来源：http://hz.shangyingyoupin.top/gtbwlmswju.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tanke756.top/gtciicohub.html

JS:   const square = x => x * x;
来源：http://hz.yuanzhike.top/gtcpsytuoz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xingfuxueyuan.xyz/gthqzttppv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.dashuyun.cn/gtlxoejygy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jianghu66.top/gtvclvkcrb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hysaishi.cn/gtxcmstqgn.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.haohaochexian.top/gtkjzolemq.html

[C07] 把函数作为参数传入
来源：http://hz.iojbl.cn/gtgdqimkvh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yonumen.top/gtxrxfvmhh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tanke756.top/gtkihricym.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yonumen.top/gtavojijtj.html

TS:   arr.map(String)
来源：http://hz.yangfankeji.com/gtleeamtof.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhixingplan.top/gtzyrpwjxq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.nwbrower.top/gtefptdncl.html

Ruby: arr.map(&:upcase)
来源：http://hz.9152youxi.cn/gtxblzckjc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yangfankeji.com/gthtesjwhi.html

[C08] 闭包
来源：http://hz.vqdsnc.cn/gtwsceopvu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigfzy.top/gtgaeirtdu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xziqi.cn/gtmgcndavk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtfwgragzg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gthlhmkxed.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cashguo.top/gtznpdrtuh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.bjfxy.top/gtorjrzoug.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xingfuxueyuan.xyz/gtwnlnrfsw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtbrtzabow.html

[C09] 递归
来源：http://hz.jianghu66.top/gtfbzuqpbt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shangyingyoupin.top/gtvjnmvsfh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.guannengcc.top/gtrebwuptw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenlongwang.top/gtkuzonxfm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gtpwzuoafk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.guannengcc.top/gtuaoyiqbi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shanyushiyangkeji.top/gtoouyoamk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hfpthk.cn/gtymqejkdz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydzc1.top/gtxmrnwngw.html

[C10] 变量作用域
来源：http://hz.tianlin.xyz/gtcmfluszz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gogol.net.cn/gtgompbiaf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cdnleiting.top/gtpkaqiruf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jyoumei.cn/gtpwfdddxx.html

TS:   同 JS
来源：http://hz.ehwqpu.com/gtvhbtkgvh.html

Java: 方法内为块级作用域
来源：http://hz.52xcode.cn/gtspvvowze.html

Go:   花括号块级作用域
来源：http://hz.aizwys.cn/gtynmqmrlp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tanke756.top/gtskktmnqn.html

C#:   块级作用域
来源：http://hz.jqgufenzy.top/gtyscezhwb.html

[C11] 模块导入与导出
来源：http://hz.zhaomingkeji.xyz/gtenvyiyzs.html

Py:   from module import func
来源：http://hz.yj202588.top/gtquqgoucs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ydzc1.top/gtanqwnicu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinqigufen.top/gtxjwsckug.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj202588.top/gtpndazfiq.html

Java: import java.util.List;
来源：http://hz.haohaochexian.top/gtochagxij.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gogol.net.cn/gtcpqozejy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.snrcjt.cn/gtithetour.html

C#:   using System.Text;
来源：http://hz.mhx1999.top/gtoxinkidx.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinghuilouyu.cn/gtpwzvskpr.html

Py:   (lambda: print("run"))()
来源：http://hz.zhongyouzk.top/gtidqvquvx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxuanxn.top/gtrfsjmhxc.html

JS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gtavwdekyi.html

TS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtwkxkvnuh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ydjk.org.cn/gtpmskvryo.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jqgfzy.top/gtdelizxfq.html

Ruby: -> { puts "run" }.call
来源：http://hz.xingfuxueyuan.xyz/gtjszvcwwn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258888.top/gtuskfukfi.html

[C13] 类型声明 / 类型注解
来源：http://hz.jinghuilouyu.cn/gthfmuyaky.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.9152youxi.cn/gtfetmuktd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gtlxtqopgh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tian-w.cn/gthhwfpcnw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jianghu66.top/gtnfxloxtr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhengqikj.top/gtgzalyuij.html

Go:   func add(a, b int) int
来源：http://hz.bjfxy.top/gthoaiipio.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ehwqpu.com/gtjooyvkmo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.snrcjt.cn/gtdjqxeluk.html

[C14] 泛型函数
来源：http://hz.yvedp.cn/gtaznklpmq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tianlin.xyz/gtnlvxwxor.html

PHP:  // 无泛型
来源：http://hz.ehwqpu.com/gtvjegfosb.html

JS:   // 无泛型
来源：http://hz.jqgfzy.top/gtewgsszgr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.svipenyu.cn/gtwidobutc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangdashe.top/gtkjgezcig.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxuanxn.top/gtvzyddzkq.html

Ruby: # 无泛型
来源：http://hz.iojbl.cn/gtprojdkjc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhongyouzk.top/gtahfxaive.html

[C15] 解构 / 展开参数
来源：http://hz.jinghuilouyu.cn/gtlylyjsam.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.c1oappe.top/gtznlqqhst.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pycfn.com/gtnlrcanvb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jlsjyb.cn/gtjydnunwf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj20258888.top/gtkqgriqpc.html

Java: // 无解构
来源：http://hz.quarkkingdee.top/gtgoldhhyp.html

Go:   // 无解构
来源：http://hz.jianghu66.top/gtxtvnmvhq.html

Ruby: a, b = pair
来源：http://hz.yonumen.top/gtjauqykss.html

C#:   var (a, b) = pair;
来源：http://hz.smart0.xyz/gtkpwmkpsa.html

[C16] 函数 / 方法重载
来源：http://hz.ybcxt.top/gtofcbwpae.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cashguo.top/gtmzqbcvin.html

PHP:  // 无重载
来源：http://hz.jqgfzy.top/gtjsivzist.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.kuanghao11.cn/gtsjukyvwo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.meibo888.top/gtiwhmfpup.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.birdmap.top/gttyswxjvn.html

Go:   // 无重载：用不同函数名
来源：http://hz.hammf.cn/gtyokteakf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.snrcjt.cn/gtalnzwsqk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.pengpengdd.cyou/gttxhrkywf.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtrcnoktmp.html

D. 数组 / 列表 / 集合
来源：http://hz.hongshengwenyu.top/gtnzedwasi.html

================================================================================
来源：http://hz.redwolf501.top/gtxgnrasmp.html

[D01] 创建数组 / 列表
来源：http://hz.xingfuxueyuan.xyz/gtntsbhpaf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cdnleiting.top/gtcmtxrpzz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yongpay.top/gtasikmsgh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aizwys.cn/gtsqdedtto.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhongyouzk.top/gtbgxikwla.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhaomingkeji.xyz/gtamuzjtfg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhiwuduotai.top/gtygozatml.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangshuangyany.cn/gtofxcrhmg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hammf.cn/gtweeeadaj.html

[D02] 追加元素到末尾
来源：http://hz.redwolf501.top/gtyuhknhqv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhijiandao.cn/gtihzjqnds.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sxryk.cn/gtlqvbjlnd.html

JS:   arr.push(4);
来源：http://hz.zhongyouzk.top/gtcozqukrs.html

TS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtgxsygjxc.html

Java: list.add(4);
来源：http://hz.gotoacloud.top/gtraguspqw.html

Go:   arr = append(arr, 4)
来源：http://hz.pycfn.com/gtyvgapunt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ybcxt.top/gtqhmwdsvd.html

C#:   list.Add(4);
来源：http://hz.cdnleiting.top/gtoarlhizt.html

[D03] 在指定位置插入元素
来源：http://hz.sweek.top/gtojnvpbyp.html

Py:   arr.insert(0, 0)
来源：http://hz.zhijiandao.cn/gtjsfnzthb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.fzhhl.top/gtkaodbjjy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zycfv.cn/gtapduivjb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sxryk.cn/gtyepdosob.html

Java: list.add(0, 0);
来源：http://hz.yanxiufei.cn/gtkdtotsfa.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xuanzx.com/gtrlsshxvl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aizwys.cn/gthnkoskqe.html

C#:   list.Insert(0, 0);
来源：http://hz.9152youxi.cn/gtpkjudunw.html

[D04] 删除元素
来源：http://hz.hongshengwenyu.top/gtarlonvyx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhongyouzk.top/gtbivtwefe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xinyue.icu/gtnoyvcayi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jyoumei.cn/gtgmrgcwip.html

TS:   arr.splice(0, 1);
来源：http://hz.dashuyun.cn/gtrkmrwjqx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hongshengwenyu.top/gtybmttnpi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hongshengwenyu.top/gtwvriwnpj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.wangdashe.top/gttunwdbhq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shzxlz.cn/gtxubzvyvw.html

[D05] 访问与修改元素
来源：http://hz.xuanzx.com/gthkiwbbon.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daxiang520.top/gtlpwqbrrc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hfpthk.cn/gtjqhfwyxk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhaomingkeji.xyz/gtdponcbzd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gtwyfjvsvu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.9152youxi.cn/gtppccxmvk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.redwolf501.top/gtwhmxpjjc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtgpwlbrmr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xinyue.icu/gtebtqiqzv.html

[D06] 数组长度
来源：http://hz.sweek.top/gtzlgypuux.html

Py:   len(arr)
来源：http://hz.hfpthk.cn/gtrpnaodok.html

PHP:  count($arr);
来源：http://hz.feifeiyinyue.top/gtqnjgbbbo.html

JS:   arr.length
来源：http://hz.gaohongyu789.top/gtgutzpbty.html

TS:   arr.length
来源：http://hz.yangfankeji.com/gtezronrnj.html

Java: list.size();
来源：http://hz.yonumen.top/gtgvrvafmq.html

Go:   len(arr)
来源：http://hz.yanxiufei.cn/gtfkknrdzp.html

Ruby: arr.length; arr.size
来源：http://hz.shuidangran.top/gtmeicuuvw.html

C#:   list.Count;
来源：http://hz.jinqigufen.top/gtgaetgtii.html

[D07] 切片 / 取子数组
来源：http://hz.andypj.xyz/gtkeiprnkx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shangyingyoupin.top/gtghjqbrzs.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.vqdsnc.cn/gtjuezxasq.html

JS:   arr.slice(1, 4);
来源：http://hz.ivvv.top/gthhemlnbg.html

TS:   arr.slice(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtcklypawq.html

Java: list.subList(1, 4);
来源：http://hz.gzhubu.top/gtrqquaixk.html

Go:   arr[1:4]
来源：http://hz.9152youxi.cn/gtxuaeqjxf.html

Ruby: arr[1, 3]
来源：http://hz.c1oappe.top/gtdnbtsthw.html

C#:   list.GetRange(1, 3);
来源：http://hz.kuanghao11.cn/gtfcmgswdr.html

[D08] 合并两个数组
来源：http://hz.guowangkeji.top/gtvsaobuch.html

Py:   a + b;  a.extend(b)
来源：http://hz.daxiang520.top/gtddhkdmcp.html

PHP:  array_merge($a, $b);
来源：http://hz.ydzc1.top/gtlkpddcik.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinqigufen.top/gtgqbaknzj.html

TS:   [...a, ...b];
来源：http://hz.yj20258888.top/gtokyhmafb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhijiandao.cn/gtrcicffhv.html

Go:   append(a, b...)
来源：http://hz.gogol.net.cn/gtebmjyyzz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.svipenyu.cn/gtmqtjwerw.html

C#:   a.Concat(b).ToList()
来源：http://hz.hongshengwenyu.top/gtkbsgwnrb.html

[D09] 排序（升序）
来源：http://hz.jinqigfzy.top/gtzrflecgm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gtcoektyva.html

PHP:  sort($arr);
来源：http://hz.redwolf501.top/gtskawlxcb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ywan-chungtsiang.top/gtbvmzcbvg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuxming.cn/gtozbxlwdy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nanxinkj.top/gtzkkharit.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258.top/gtowhvdvyh.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gttruoedje.html

C#:   list.Sort();
来源：http://hz.yj20258888.top/gtdaybvglv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.haohaochexian.top/gtarvpsimn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.mhx1999.top/gticlimryo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dianchejie.cn/gtkxlbtotq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtqmjzvduc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tianlin.xyz/gtqikekleo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nanxuanxn.top/gtrizdculb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hammf.cn/gtyxezxmpp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.9152youxi.cn/gtdmvjmvyz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ydjk.org.cn/gttlhtfcuq.html

[D11] 反转数组
来源：http://hz.bjfxy.top/gtafmmllkx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.aibaodan.cn/gtmnkttvrr.html

PHP:  array_reverse($arr);
来源：http://hz.yongpay.top/gtzvhuhpiu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ehwqpu.com/gtdaopfodj.html

TS:   [...arr].reverse();
来源：http://hz.zhixingplan.top/gthcvfqous.html

Java: Collections.reverse(list);
来源：http://hz.jianghu66.top/gtfnkgpebp.html

Go:   slices.Reverse(arr)
来源：http://hz.ywan-chungtsiang.top/gtxcbvjhqw.html

Ruby: arr.reverse
来源：http://hz.aizwys.cn/gttdtooyff.html

C#:   list.Reverse();
来源：http://hz.ydzc1.top/gtpwklceyy.html

[D12] 查找元素下标
来源：http://hz.yuanzhike.top/gtzxlruohb.html

Py:   arr.index(x);  x in arr
来源：http://hz.hnqzz.top/gtkfsygxzf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuxming.cn/gtcprudjrp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gterzbzdoq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtbivhsgsv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.c1oappe.top/gtrpfpbxgv.html

Go:   slices.Index(arr, x)
来源：http://hz.jqgfzy.top/gtqxcvjfug.html

Ruby: arr.index(x)
来源：http://hz.smart0.xyz/gtxhiwbinx.html

C#:   list.IndexOf(x);
来源：http://hz.haohaochexian.top/gtfbjmgfzh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.iojbl.cn/gtyvxdxlfe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yj20258888.top/gtefjuvlzh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jianghu66.top/gtfbijayqy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj20258888.top/gtahpnuijz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtgqwbmmmz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jyoumei.cn/gtjjazdiec.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.redwolf501.top/gtumtpqhap.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.316326.xyz/gtvwwgwxrn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.pycfn.com/gtnrngfrta.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj202588.top/gttqrxfenr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hywenlv.cn/gtlwxgqbyd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hfpthk.cn/gtfbxpposi.html

JS:   arr.map(x => x * 2)
来源：http://hz.aizwys.cn/gtditjelqf.html

TS:   arr.map(x => x * 2)
来源：http://hz.redwolf501.top/gtnsgrucdn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.snrcjt.cn/gtmjixvpvh.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtrhnxtigb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.daria6918.cn/gtynayutbf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ybcxt.top/gteobbtmbn.html

[D15] 去重
来源：http://hz.zhiwuduotai.top/gtbcxiremb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.dianchejie.cn/gtjlrbzkgd.html

PHP:  array_unique($arr);
来源：http://hz.yongpay.top/gtvkqibrpm.html

JS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtrngcksww.html

TS:   [...new Set(arr)]
来源：http://hz.redwolf501.top/gtaxypuhmx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhaomingkeji.xyz/gtwpszndst.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhaomingkeji.xyz/gtqzhosdqo.html

Ruby: arr.uniq
来源：http://hz.yuanzhike.top/gtitxpztgt.html

C#:   list.Distinct().ToList()
来源：http://hz.ybcxt.top/gtsoffpxkw.html

[D16] 求和与平均值
来源：http://hz.cashguo.top/gtivifwran.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jqgufenzy.top/gtsnnzjcmx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tian-w.cn/gtsbvdovil.html


<!-- 参考信息 -->