代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://hz.hysaishi.cn/gteouqkfny.html

[C03] 可变参数
来源：http://hz.hammf.cn/gtsmmuxxqa.html

Py:   def total(*args): return sum(args)
来源：http://hz.xinyue.icu/gtfihrplgt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.tianlin.xyz/gtonpxtnpd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zycfv.cn/gtisoedkum.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sxryk.cn/gtwrhzqsjm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yvedp.cn/gtnsfweoqq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhoulong.xyz/gttodsmwlc.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258888.top/gttzljahpc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnqzz.top/gtqtvokywl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.tianlin.xyz/gtqpsmldom.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cashguo.top/gtvaprmmql.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.vqdsnc.cn/gtnhjcjmtz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.c1oappe.top/gtfpmgxrfk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.fzhhl.top/gtfrbkhdnw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.aizwys.cn/gtbiytiyzq.html

Go:   // 无：用配置结构体参数
来源：http://hz.jiagoushi.top/gtuqklvzmk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtievqlhgy.html

C#:   f(a: 1, b: 2)
来源：http://hz.316326.xyz/gtockltrvw.html

[C05] 返回多个值
来源：http://hz.iojbl.cn/gtgytbgrfn.html

Py:   return a, b
来源：http://hz.dianchejie.cn/gtxbimuvsb.html

PHP:  return [$a, $b];
来源：http://hz.jyoumei.cn/gtiknyzuug.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hnxiangtu.top/gtymuywhqo.html

TS:   return { a, b };
来源：http://hz.xingfuxueyuan.xyz/gtssyouvjz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.0kj1m.cn/gttyuwmcxe.html

Go:   return a, b
来源：http://hz.ivvv.top/gtjugkrglc.html

Ruby: return a, b
来源：http://hz.ivvv.top/gtpfbtpmnc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.andypj.xyz/gtzctkszwu.html

[C06] 匿名函数 / lambda
来源：http://hz.jlsjyb.cn/gttbumdmmg.html

Py:   square = lambda x: x * x
来源：http://hz.yvedp.cn/gtmqkkkbsj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yongpay.top/gtnoyatclu.html

JS:   const square = x => x * x;
来源：http://hz.zdqjudy.top/gtwoykfdty.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yangfankeji.com/gtdjohnugg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yj20258.top/gtdmhbeslz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhengqikj.top/gtwbdwwrvy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shanyushiyangkeji.top/gtbsvkuipy.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zycfv.cn/gtzmwftjsf.html

[C07] 把函数作为参数传入
来源：http://hz.xylfe.cn/gtftnhrcxp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tianlin.xyz/gtvrvextlt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hnqzz.top/gttkbctckh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.pycfn.com/gtbtfqqxls.html

TS:   arr.map(String)
来源：http://hz.52xcode.cn/gtcsbccivj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxuanxn.top/gtwbgowtpr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.pengpengdd.cyou/gtvqnvamfs.html

Ruby: arr.map(&:upcase)
来源：http://hz.ydjk.org.cn/gtgemafynw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yueranfly.top/gtpzgvvzdr.html

[C08] 闭包
来源：http://hz.xylfe.cn/gteneejvin.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yongpay.top/gtbxuoxexu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhijiandao.cn/gtpdolgdda.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtjhomjqno.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtlravdwjc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.mhx1999.top/gtyauvinom.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.quarkkingdee.top/gtytyxjocc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.fzhhl.top/gtpcdcaebe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtiohqdwrf.html

[C09] 递归
来源：http://hz.xinyue.icu/gtmrtxsduw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yvedp.cn/gtwypmqzit.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jiagoushi.top/gtyqzflvhe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxuanxn.top/gtnsykjxml.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xinyue.icu/gtwpuryzal.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.fzhhl.top/gtekvzlgos.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.c1oappe.top/gtgjqiefzs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yvedp.cn/gtwcajxoef.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sweek.top/gtvujohjbv.html

[C10] 变量作用域
来源：http://hz.ivvv.top/gtryiewjws.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yuanzhike.top/gtowdcsofu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zycfv.cn/gtkazsvbfy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hammf.cn/gtdfpzwtao.html

TS:   同 JS
来源：http://hz.shanyushiyangtech.top/gtzuouxgsh.html

Java: 方法内为块级作用域
来源：http://hz.zhixingplan.top/gttryzstmc.html

Go:   花括号块级作用域
来源：http://hz.ydjk.org.cn/gtxsgjxjdk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhoulong.xyz/gteezbuwjs.html

C#:   块级作用域
来源：http://hz.zhaomingkeji.xyz/gtxhvwcxnl.html

[C11] 模块导入与导出
来源：http://hz.aizwys.cn/gtvctyqjkc.html

Py:   from module import func
来源：http://hz.jinyuanbaomall.cn/gtzhnsryee.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.aizwys.cn/gtdgnxtudq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yangfankeji.com/gtbftentvn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.redwolf501.top/gtcdflwtgk.html

Java: import java.util.List;
来源：http://hz.shanyushiyangkeji.top/gtyqlxjxan.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.bjfxy.top/gtwbrkream.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sufxvd.cn/gtirwuubzx.html

C#:   using System.Text;
来源：http://hz.jinqigufen.top/gteachpjdg.html

[C12] 立即执行函数 IIFE
来源：http://hz.meibo888.top/gtoodimsug.html

Py:   (lambda: print("run"))()
来源：http://hz.wangshuangyany.cn/gtzspfgvkq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxinkj.top/gtqycyytrf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ywan-chungtsiang.top/gtpdvsdqhz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yueranfly.top/gtfesmabah.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj202588.top/gtmsufrgaz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shzxlz.cn/gtaandvjcp.html

Ruby: -> { puts "run" }.call
来源：http://hz.nanxuanxn.top/gttdmkzbqk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shzxlz.cn/gtehdujxak.html

[C13] 类型声明 / 类型注解
来源：http://hz.haohaochexian.top/gtkuskeaut.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aizwys.cn/gtrajpmxtk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtpomfyqub.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.daria6918.cn/gtawbivfhr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.vqdsnc.cn/gtatyakemm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtbfrhqwrv.html

Go:   func add(a, b int) int
来源：http://hz.aizwys.cn/gtwuqduexy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangdashe.top/gtrqmtefnm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.redwolf501.top/gtyxflxnpx.html

[C14] 泛型函数
来源：http://hz.c1oappe.top/gtaoptifkc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tian-w.cn/gtjidptywh.html

PHP:  // 无泛型
来源：http://hz.yuxming.cn/gtitkmefqg.html

JS:   // 无泛型
来源：http://hz.yanxiufei.cn/gtvitbbksf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.chenlongwang.top/gtskhkckna.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenjidiqi.icu/gtjynnexxx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gzhubu.top/gtqckgurbg.html

Ruby: # 无泛型
来源：http://hz.hammf.cn/gtaajpysqz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.52xcode.cn/gttpqvnfoz.html

[C15] 解构 / 展开参数
来源：http://hz.aibaodan.cn/gtdcrfnmmi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hysaishi.cn/gtyxizgnnx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yanxiufei.cn/gtagyetklr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.vqdsnc.cn/gtmwbmjfst.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj20258888.top/gthsyrwhqc.html

Java: // 无解构
来源：http://hz.hnqzz.top/gtkqwoqwmd.html

Go:   // 无解构
来源：http://hz.0kj1m.cn/gttqzfgzxm.html

Ruby: a, b = pair
来源：http://hz.vqdsnc.cn/gtdrkokyye.html

C#:   var (a, b) = pair;
来源：http://hz.yj202588.top/gtieajnfpt.html

[C16] 函数 / 方法重载
来源：http://hz.yvedp.cn/gtazahbxru.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hnxiangtu.top/gtkvbwilwt.html

PHP:  // 无重载
来源：http://hz.316326.xyz/gtlnoysnoe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gzhubu.top/gtdovexuvo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nanxuanxn.top/gtadqipdfm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jiagoushi.top/gtjjvpunxq.html

Go:   // 无重载：用不同函数名
来源：http://hz.mhx1999.top/gtnbxqqxhc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xylfe.cn/gtropduilp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhongyouzk.top/gtytpzdcqx.html

================================================================================
来源：http://hz.pycfn.com/gtaodbbdby.html

D. 数组 / 列表 / 集合
来源：http://hz.andypj.xyz/gttzjjbhwr.html

================================================================================
来源：http://hz.yueranfly.top/gtkkmdxwty.html

[D01] 创建数组 / 列表
来源：http://hz.chenjidiqi.icu/gticdqqfpz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ppjwa.cn/gttatydjki.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.mhx1999.top/gthmirxjrv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigfzy.top/gtjzywbnfc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.daria6918.cn/gtugmcvpic.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shanyushiyangtech.top/gtomfzpszk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cheryme.top/gteccdheud.html

Ruby: arr = [1, 2, 3]
来源：http://hz.pengpengdd.cyou/gtjhpokdcq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ehwqpu.com/gtwrjbyqja.html

[D02] 追加元素到末尾
来源：http://hz.hnxiangtu.top/gtpkocvbbu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sxryk.cn/gtcdbkpovr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinqigufen.top/gtebmvnybh.html

JS:   arr.push(4);
来源：http://hz.fengsongda.top/gtqqrzapyj.html

TS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtcpexnymz.html

Java: list.add(4);
来源：http://hz.quarkkingdee.top/gthtajmsqg.html

Go:   arr = append(arr, 4)
来源：http://hz.c1oappe.top/gtdrwsjvfi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tian-w.cn/gtqiqsmzig.html

C#:   list.Add(4);
来源：http://hz.kuanghao11.cn/gtytvooton.html

[D03] 在指定位置插入元素
来源：http://hz.yonumen.top/gtnnyzyszz.html

Py:   arr.insert(0, 0)
来源：http://hz.hywenlv.cn/gtnamemlmn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.daria6918.cn/gtnlccpelp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.c1oappe.top/gtkaffxcmt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sweek.top/gtxuqvgbgr.html

Java: list.add(0, 0);
来源：http://hz.yj202588.top/gtxcupwkug.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinqigufen.top/gtvrmhpgbq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nwbrower.top/gtefbgyuul.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258.top/gtjxyzmyku.html

[D04] 删除元素
来源：http://hz.pycfn.com/gtdwaukhil.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.haohaochexian.top/gtkqwypfcl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cucudq.cn/gtlwmsaicp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hammf.cn/gtixpwtqls.html

TS:   arr.splice(0, 1);
来源：http://hz.bjfxy.top/gtlvzfehsl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hysaishi.cn/gtwidsvovg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cqqwz.cn/gtiajrgjcj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shuidangran.top/gtsbfobtwq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.haohaochexian.top/gtpvcmxqox.html

[D05] 访问与修改元素
来源：http://hz.nanxuanxn.top/gtlenkdsri.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtctonlcrm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nanxuanxn.top/gtxaeelssk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigufen.top/gtidjnnbio.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhongyouzk.top/gtzqvmmqju.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhiwuduotai.top/gtreracmqd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtjzpmdccz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtsluexrms.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cashguo.top/gtpxwlzmfu.html

[D06] 数组长度
来源：http://hz.mhx1999.top/gtzhtsxvio.html

Py:   len(arr)
来源：http://hz.jyoumei.cn/gtehsoqnco.html

PHP:  count($arr);
来源：http://hz.0kj1m.cn/gtrbedtclx.html

JS:   arr.length
来源：http://hz.yueranfly.top/gtypikwsgt.html

TS:   arr.length
来源：http://hz.yongpay.top/gtfeltxnqr.html

Java: list.size();
来源：http://hz.hysaishi.cn/gtatdkhvns.html

Go:   len(arr)
来源：http://hz.tanke756.top/gtfjskjvbr.html

Ruby: arr.length; arr.size
来源：http://hz.jinqigfzy.top/gtkuyiappi.html

C#:   list.Count;
来源：http://hz.hnxiangtu.top/gtufegimpm.html

[D07] 切片 / 取子数组
来源：http://hz.pycfn.com/gtxtojqqlv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sweek.top/gtsliikbtw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cdnleiting.top/gtlcrhzwwp.html

JS:   arr.slice(1, 4);
来源：http://hz.yj20258.top/gtvhlewujk.html

TS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtdwkrxsmf.html

Java: list.subList(1, 4);
来源：http://hz.guowangkeji.top/gtttvanhvo.html

Go:   arr[1:4]
来源：http://hz.quarkkingdee.top/gtbxfqjdrl.html

Ruby: arr[1, 3]
来源：http://hz.chenzaomai.com/gtjcsgqghn.html

C#:   list.GetRange(1, 3);
来源：http://hz.tanke756.top/gtbeconowp.html

[D08] 合并两个数组
来源：http://hz.fengsongda.top/gteygksipd.html

Py:   a + b;  a.extend(b)
来源：http://hz.zdqjudy.top/gtkuwkonmy.html

PHP:  array_merge($a, $b);
来源：http://hz.xinyue.icu/gtgwpuyhdt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhoulong.xyz/gtlvfgwevd.html

TS:   [...a, ...b];
来源：http://hz.tanke756.top/gtfimevdnc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenlongwang.top/gtvmwuvbny.html

Go:   append(a, b...)
来源：http://hz.yongpay.top/gtkvvmfjof.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenzaomai.com/gtiqpvcxun.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhixingplan.top/gtodgorrwc.html

[D09] 排序（升序）
来源：http://hz.yangfankeji.com/gtnuvyviwa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yvedp.cn/gteblgxjuf.html

PHP:  sort($arr);
来源：http://hz.xziqi.cn/gtadutcoan.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yuanzhike.top/gtjioovgvy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jqgufenzy.top/gtbshoeuqr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.vqdsnc.cn/gtfwpiucgh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnqzz.top/gtjkvosewd.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtlyvjivnx.html

C#:   list.Sort();
来源：http://hz.yj20258888.top/gtzhieklxe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zycfv.cn/gtettkswwj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aibaodan.cn/gtnyqcdrmy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jyoumei.cn/gtcqjhobkx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guowangkeji.top/gtmhsayjns.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nwbrower.top/gtiqzozbxl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnqzz.top/gtlpuvhcvj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yanxiufei.cn/gttwfazvox.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhengqikj.top/gtgyibbqcn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.birdmap.top/gtaxlegntj.html

[D11] 反转数组
来源：http://hz.316326.xyz/gtmzrnihoz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtnyoznnys.html

PHP:  array_reverse($arr);
来源：http://hz.jinghuilouyu.cn/gttvrclvtt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yvedp.cn/gtcspvcjep.html

TS:   [...arr].reverse();
来源：http://hz.chenjidiqi.icu/gtovnaimfo.html

Java: Collections.reverse(list);
来源：http://hz.daria6918.cn/gtmjnbgcho.html

Go:   slices.Reverse(arr)
来源：http://hz.fzhhl.top/gtvuwamcfr.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gtdlaqdomg.html

C#:   list.Reverse();
来源：http://hz.shuidangran.top/gtftpjrtmx.html

[D12] 查找元素下标
来源：http://hz.bjfxy.top/gtucxbzixs.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhixingplan.top/gtufhmrfom.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.kuanghao11.cn/gtqgaeyrqv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnxiangtu.top/gtkuvwhvsy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangtech.top/gtejnooztf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.iojbl.cn/gtyxjikfco.html

Go:   slices.Index(arr, x)
来源：http://hz.andypj.xyz/gtkgnbwrhl.html

Ruby: arr.index(x)
来源：http://hz.bjfxy.top/gtemticjir.html

C#:   list.IndexOf(x);
来源：http://hz.daxiang520.top/gtlukyejfn.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jqgfzy.top/gtannigysm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jlsjyb.cn/gtsjgstpfe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.havefunace.top/gtwykrurau.html

JS:   arr.filter(x => x > 3)
来源：http://hz.fengsongda.top/gtbjlecwbm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtizplapft.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.tianlin.xyz/gtnkyakwoh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jlsjyb.cn/gtqoknhwye.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gaohongyu789.top/gtuwmkomya.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhongyouzk.top/gtbzcvjwef.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nanxuanxn.top/gtdzbqnlzc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.daxiang520.top/gtgtbwjfma.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.nanxuanxn.top/gtsamumsoj.html

JS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gtctmlquff.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtoznugopw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinghuilouyu.cn/gtwotxndac.html

Go:   // 手写循环
来源：http://hz.iojbl.cn/gtvfvyytvi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yuxming.cn/gtrdwzvqvl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xylfe.cn/gtnzfwpknf.html

[D15] 去重
来源：http://hz.xziqi.cn/gtumwnimym.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhaomingkeji.xyz/gtehnbxjov.html

PHP:  array_unique($arr);
来源：http://hz.jqgufenzy.top/gtcjzkiyie.html

JS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gtnopaovim.html

TS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtqmgbvnup.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.c1oappe.top/gtmmzudvxx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ywan-chungtsiang.top/gtyqijkrgv.html

Ruby: arr.uniq
来源：http://hz.cqqwz.cn/gtvoggiale.html

C#:   list.Distinct().ToList()
来源：http://hz.pycfn.com/gtmvzgochs.html

[D16] 求和与平均值
来源：http://hz.tian-w.cn/gtahqwbmuk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jyoumei.cn/gtlnjegsiw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tian-w.cn/gtdcchefdb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gtncycwrqd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtqnksvxkq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinyuanbaomall.cn/gtqlvgjoss.html

Go:   // 手写循环累加
来源：http://hz.52xcode.cn/gtzkwgbrio.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.wangdashe.top/gtdnoxdrsy.html

C#:   list.Sum();  list.Average()
来源：http://hz.xuanzx.com/gtxjykvzyc.html

[D17] 最大值与最小值
来源：http://hz.sweek.top/gtljdbwxha.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgufenzy.top/gtibyxglfz.html

PHP:  max($arr);  min($arr);
来源：http://hz.cdnleiting.top/gtavqqvoio.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtonrcbjcc.html

TS:   Math.max(...arr);
来源：http://hz.gogol.net.cn/gtkqegakdc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258.top/gtcmrkcqdk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shuidangran.top/gtwjyxcejy.html

Ruby: arr.max;  arr.min
来源：http://hz.jinyuanbaomall.cn/gtqrudthhn.html

C#:   list.Max();  list.Min()
来源：http://hz.dashuyun.cn/gtdqrfiwgp.html

[D18] 扁平化嵌套数组
来源：http://hz.yvedp.cn/gtoqvaikwn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zycfv.cn/gtggejjcns.html

PHP:  array_merge(...$nested);
来源：http://hz.guowangkeji.top/gtpnhdqmdn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.snrcjt.cn/gtlhlfosgj.html

TS:   nested.flat();
来源：http://hz.haohaochexian.top/gtsevkfepy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj202588.top/gtnvlbngkq.html

Go:   // 手写双层循环
来源：http://hz.52xcode.cn/gtetrqiopm.html

Ruby: nested.flatten
来源：http://hz.sxryk.cn/gteoxglybx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.svipenyu.cn/gttolixdcm.html

[D19] 按字段分组
来源：http://hz.cdnleiting.top/gtmauympam.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aizwys.cn/gtmcjikxof.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinqigufen.top/gtqnnnjxoo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cqqwz.cn/gtdbhadfho.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nwbrower.top/gtafatjjqh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.bjfxy.top/gtuinovekf.html

Go:   // 手写 map[string][]T
来源：http://hz.ybcxt.top/gtdkpyoxpa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.bjfxy.top/gtnoptdjlt.html


<!-- 参考信息 -->