代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xingfuxueyuan.xyz/gtrfxxnqpg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sxryk.cn/gtkdalhdur.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.0kj1m.cn/gtfotpojev.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ppjwa.cn/gtbzameuaa.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tian-w.cn/gtufjkdejr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jqgufenzy.top/gttvvjqvrw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.havefunace.top/gtvqugvkrx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nanxinkj.top/gttsqnpbcy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shanyushiyangtech.top/gthmffjkiu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.havefunace.top/gtkbnrbqcz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhixingplan.top/gttojvspsx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.aizwys.cn/gtlgefgcph.html

Go:   // 无：用配置结构体参数
来源：http://hz.havefunace.top/gtshtnkehi.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sweek.top/gtjcshtnjt.html

C#:   f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtgbadtjla.html

[C05] 返回多个值
来源：http://hz.cheryme.top/gtsjjxlsah.html

Py:   return a, b
来源：http://hz.zhixingplan.top/gtaortjiat.html

PHP:  return [$a, $b];
来源：http://hz.jqgfzy.top/gtxousemkc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtauneawbs.html

TS:   return { a, b };
来源：http://hz.sxryk.cn/gtvqxgkqkw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tian-w.cn/gthtqzpysu.html

Go:   return a, b
来源：http://hz.jqgufenzy.top/gtzoepvuan.html

Ruby: return a, b
来源：http://hz.xingfuxueyuan.xyz/gtxhalpkif.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hysaishi.cn/gtnskipotx.html

[C06] 匿名函数 / lambda
来源：http://hz.xziqi.cn/gtwyzfzkan.html

Py:   square = lambda x: x * x
来源：http://hz.jianghu66.top/gtpbrtffrp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tanke756.top/gtuhbnfuzm.html

JS:   const square = x => x * x;
来源：http://hz.aibaodan.cn/gtfiqdbhpc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hysaishi.cn/gtmvlaocvk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhoulong.xyz/gtjpwjpawa.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.fzhhl.top/gtvobwjxkt.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nwbrower.top/gtprhzwgvq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xziqi.cn/gtzacklbnq.html

[C07] 把函数作为参数传入
来源：http://hz.sweek.top/gtixwtunmm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.andypj.xyz/gtieqeeipq.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.52xcode.cn/gttfvumwxi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.feifeiyinyue.top/gtdtinwvcx.html

TS:   arr.map(String)
来源：http://hz.shzxlz.cn/gtfdsiydpk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhongyouzk.top/gthobteyfa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.snrcjt.cn/gtacumzflg.html

Ruby: arr.map(&:upcase)
来源：http://hz.shanyushiyangtech.top/gthaozxzql.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hywenlv.cn/gthybrcgzk.html

[C08] 闭包
来源：http://hz.hfpthk.cn/gtdivnxlyv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.fengsongda.top/gtnqprwzrt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ehwqpu.com/gtwzebqlsq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gtxftmnvvb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtdyqgwqnf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.9152youxi.cn/gtxxtgqzga.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shzxlz.cn/gtupgwdkcw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.daxiang520.top/gtbzjnrmku.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtqzqfesvu.html

[C09] 递归
来源：http://hz.wangshuangyany.cn/gtaklsxvbj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.feifeiyinyue.top/gttscxqssi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.kuanghao11.cn/gtgtuzixjz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtpmajdxfa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuanzhike.top/gtffawaqmi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.andypj.xyz/gthqosqrtd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zycfv.cn/gtndxqgrsr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gthdiornik.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.316326.xyz/gtzhsjckvh.html

[C10] 变量作用域
来源：http://hz.cheryme.top/gtjsiyupfq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aizwys.cn/gtwxjenlba.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.redwolf501.top/gtrldgqaor.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydjk.org.cn/gtuuuetggj.html

TS:   同 JS
来源：http://hz.hongshengwenyu.top/gtljipnucu.html

Java: 方法内为块级作用域
来源：http://hz.hongshengwenyu.top/gtemjwjizc.html

Go:   花括号块级作用域
来源：http://hz.ydzc1.top/gtbzilnnmm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jiagoushi.top/gtngwbalar.html

C#:   块级作用域
来源：http://hz.xziqi.cn/gtwrlavsxl.html

[C11] 模块导入与导出
来源：http://hz.ehwqpu.com/gtbemdqiiy.html

Py:   from module import func
来源：http://hz.yonumen.top/gtbldfhuey.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shangyingyoupin.top/gteigbpzcr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.wangshuangyany.cn/gtohivhogf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.0kj1m.cn/gtjvdwdwmx.html

Java: import java.util.List;
来源：http://hz.zhengqikj.top/gtakpyenot.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hfpthk.cn/gtkyxvxuuw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.iojbl.cn/gtthqhhpri.html

C#:   using System.Text;
来源：http://hz.fzhhl.top/gtbtgwncme.html

[C12] 立即执行函数 IIFE
来源：http://hz.smart0.xyz/gtahlhzvgx.html

Py:   (lambda: print("run"))()
来源：http://hz.zhaomingkeji.xyz/gtxlivwzml.html

PHP:  (function () { echo "run"; })();
来源：http://hz.dashuyun.cn/gtkltmhrjb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ybcxt.top/gtgdwqjlfn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtyrtvlavi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jianghu66.top/gtedghopaf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.iojbl.cn/gtikdxofrh.html

Ruby: -> { puts "run" }.call
来源：http://hz.316326.xyz/gtcvttkvwt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xuetiantiany.cn/gtipxokbnd.html

[C13] 类型声明 / 类型注解
来源：http://hz.tian-w.cn/gtefahuexh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenlongwang.top/gtspdvmizq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.havefunace.top/gtdpkjrmfi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jianghu66.top/gttkyeiybx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtxeceaosy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtzjldqznj.html

Go:   func add(a, b int) int
来源：http://hz.52xcode.cn/gtvclwaids.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.smart0.xyz/gtdjzhmqxq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yvedp.cn/gtjsxgcfzb.html

[C14] 泛型函数
来源：http://hz.ehwqpu.com/gtffeblcjb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zdqjudy.top/gtsgoibbep.html

PHP:  // 无泛型
来源：http://hz.svipenyu.cn/gtsgujtyzd.html

JS:   // 无泛型
来源：http://hz.wangdashe.top/gtbnxvlmdq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.havefunace.top/gtwlkstaog.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daxiang520.top/gtcmkcdwbr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.aizwys.cn/gtdhhxpcvi.html

Ruby: # 无泛型
来源：http://hz.xziqi.cn/gtceryrtyv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenlongwang.top/gtmxzopaag.html

[C15] 解构 / 展开参数
来源：http://hz.xuanzx.com/gthahywobe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigufen.top/gtuespprze.html

PHP:  [$a, $b] = $pair;
来源：http://hz.bjfxy.top/gtiiecoocj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtcjuopdzi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.vqdsnc.cn/gtanjfawqz.html

Java: // 无解构
来源：http://hz.bjfxy.top/gttmdpriev.html

Go:   // 无解构
来源：http://hz.xuetiantiany.cn/gtcxnklblm.html

Ruby: a, b = pair
来源：http://hz.zhengqikj.top/gtrleknvdj.html

C#:   var (a, b) = pair;
来源：http://hz.tian-w.cn/gtdpgtkbkv.html

[C16] 函数 / 方法重载
来源：http://hz.tianlin.xyz/gtndnbxujv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cqqwz.cn/gtuaqvsccz.html

PHP:  // 无重载
来源：http://hz.daxiang520.top/gtnjrjsolz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnqzz.top/gtnhqnlijr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinqigfzy.top/gtbowercii.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxuanxn.top/gtdnxgwgrj.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhengqikj.top/gtunwxjndt.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shzxlz.cn/gtklvzxkzc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cashguo.top/gtarbvyfgd.html

================================================================================
来源：http://hz.cdnleiting.top/gtrxfutbcg.html

D. 数组 / 列表 / 集合
来源：http://hz.c1oappe.top/gthrjiqekv.html

================================================================================
来源：http://hz.zdqjudy.top/gtbwfobgnj.html

[D01] 创建数组 / 列表
来源：http://hz.zhengqikj.top/gtorksgxsx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jiagoushi.top/gtodmlctdu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cheryme.top/gtnkncwfqg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aibaodan.cn/gtvqgefpyk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.c1oappe.top/gtonrqqusi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yangfankeji.com/gtmxakcjrj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.aibaodan.cn/gtydxdqbnj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.feifeiyinyue.top/gtwwacnsqm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hfpthk.cn/gtxksqkrvf.html

[D02] 追加元素到末尾
来源：http://hz.ehwqpu.com/gtdvdtodyq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daxiang520.top/gtqackdire.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gaohongyu789.top/gtwzjebzme.html

JS:   arr.push(4);
来源：http://hz.yj202588.top/gtnwrabsnc.html

TS:   arr.push(4);
来源：http://hz.smart0.xyz/gtujyhpbpe.html

Java: list.add(4);
来源：http://hz.gogol.net.cn/gtdqxhyrrf.html

Go:   arr = append(arr, 4)
来源：http://hz.havefunace.top/gtwbsllukr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gogol.net.cn/gtjgbxkolg.html

C#:   list.Add(4);
来源：http://hz.chenjidiqi.icu/gtxgotgele.html

[D03] 在指定位置插入元素
来源：http://hz.quarkkingdee.top/gtsufjdjep.html

Py:   arr.insert(0, 0)
来源：http://hz.zycfv.cn/gthlddssax.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xylfe.cn/gtyhxjbulu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.andypj.xyz/gtdizsjgli.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenjidiqi.icu/gtkfiafgmc.html

Java: list.add(0, 0);
来源：http://hz.pycfn.com/gtoudpqwyg.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yvedp.cn/gtvecpmqgb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tanke756.top/gtqedteylo.html

C#:   list.Insert(0, 0);
来源：http://hz.hnxiangtu.top/gtpelhwqee.html

[D04] 删除元素
来源：http://hz.yuxming.cn/gtbpkeuncf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuetiantiany.cn/gtvajivpij.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yangfankeji.com/gtdwwvelku.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.quarkkingdee.top/gtxojmzizi.html

TS:   arr.splice(0, 1);
来源：http://hz.mhx1999.top/gtnikwqffm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sxryk.cn/gtdjmsujuz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xingfuxueyuan.xyz/gtoqbqejnd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sweek.top/gtrzxksgrl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.svipenyu.cn/gtnzjmxiih.html

[D05] 访问与修改元素
来源：http://hz.xylfe.cn/gthdvsfwia.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtretrdldl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenlongwang.top/gtdwecxbce.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nwbrower.top/gtpvjpuhus.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.redwolf501.top/gtdtulfieu.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.andypj.xyz/gtemqehgxd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yongpay.top/gtrphagvcm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gthjrstaib.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhijiandao.cn/gtqspsozmz.html

[D06] 数组长度
来源：http://hz.guannengcc.top/gtbpriinpr.html

Py:   len(arr)
来源：http://hz.kuanghao11.cn/gtbetiomyh.html

PHP:  count($arr);
来源：http://hz.meibo888.top/gtsxtbozcz.html

JS:   arr.length
来源：http://hz.ybcxt.top/gtixvairxl.html

TS:   arr.length
来源：http://hz.yvedp.cn/gtujiuckdq.html

Java: list.size();
来源：http://hz.nwbrower.top/gtfgqgujfo.html

Go:   len(arr)
来源：http://hz.chenlongwang.top/gtzttttnhs.html

Ruby: arr.length; arr.size
来源：http://hz.jinghuilouyu.cn/gtgkiekpum.html

C#:   list.Count;
来源：http://hz.yuxming.cn/gtwzjtztud.html

[D07] 切片 / 取子数组
来源：http://hz.xylfe.cn/gtfhthxtax.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.andypj.xyz/gtdjwlmgpi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yvedp.cn/gtuqnzllhw.html

JS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gtzoojvmbq.html

TS:   arr.slice(1, 4);
来源：http://hz.redwolf501.top/gtcdrneinm.html

Java: list.subList(1, 4);
来源：http://hz.jinqigfzy.top/gtsdmazzxq.html

Go:   arr[1:4]
来源：http://hz.gaohongyu789.top/gtjbmahrml.html

Ruby: arr[1, 3]
来源：http://hz.fengsongda.top/gtnqpvxskx.html

C#:   list.GetRange(1, 3);
来源：http://hz.shuidangran.top/gtealsnkey.html

[D08] 合并两个数组
来源：http://hz.sysykeji.top/gtdiptnmju.html

Py:   a + b;  a.extend(b)
来源：http://hz.316326.xyz/gtwogicugi.html

PHP:  array_merge($a, $b);
来源：http://hz.guowangkeji.top/gtywclxzrd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nanxinkj.top/gtzxyribgg.html

TS:   [...a, ...b];
来源：http://hz.yangfankeji.com/gtkfzkdgty.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.quarkkingdee.top/gtcmqqfydr.html

Go:   append(a, b...)
来源：http://hz.tanke756.top/gtndmtgeoa.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jlsjyb.cn/gtahjcnfzq.html

C#:   a.Concat(b).ToList()
来源：http://hz.jiagoushi.top/gtjbhgftno.html

[D09] 排序（升序）
来源：http://hz.ybcxt.top/gtoamnxhcx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtxdijdvdp.html

PHP:  sort($arr);
来源：http://hz.jqgufenzy.top/gtwuqfrqib.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.iojbl.cn/gthalcrmim.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.smart0.xyz/gtkvqcooay.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ydzc1.top/gtzkuatrog.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtyaskiqos.html

Ruby: arr.sort
来源：http://hz.cashguo.top/gtfavyetkr.html

C#:   list.Sort();
来源：http://hz.hysaishi.cn/gtiizygwxc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xziqi.cn/gtyuseumpq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.9152youxi.cn/gtuohazscz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shangyingyoupin.top/gttgdihkoo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gtdtuogkee.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtkckswfur.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nanxuanxn.top/gtyhajkpxp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hnqzz.top/gtjewhusym.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xinyue.icu/gthcvkkixi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhijiandao.cn/gtgzfprsai.html

[D11] 反转数组
来源：http://hz.yj20258888.top/gtkbrycdtz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xinyue.icu/gtixavxqdb.html

PHP:  array_reverse($arr);
来源：http://hz.yueranfly.top/gtlnjocvyn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dianchejie.cn/gtlbqvqrhu.html

TS:   [...arr].reverse();
来源：http://hz.gotoacloud.top/gtyrbxzhcj.html

Java: Collections.reverse(list);
来源：http://hz.zhoulong.xyz/gtuwerqcfr.html

Go:   slices.Reverse(arr)
来源：http://hz.hammf.cn/gtnadglzju.html

Ruby: arr.reverse
来源：http://hz.chenlongwang.top/gtqlfdfsdw.html

C#:   list.Reverse();
来源：http://hz.wangshuangyany.cn/gtxcttsxyf.html

[D12] 查找元素下标
来源：http://hz.sxryk.cn/gtbspemdmn.html

Py:   arr.index(x);  x in arr
来源：http://hz.yangfankeji.com/gtxxayqkrx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ybcxt.top/gtlklbgryw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtobagsttm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.svipenyu.cn/gtclortyxi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.snrcjt.cn/gttugawunt.html

Go:   slices.Index(arr, x)
来源：http://hz.kuanghao11.cn/gtdarogprw.html

Ruby: arr.index(x)
来源：http://hz.cqqwz.cn/gtgcztypgs.html

C#:   list.IndexOf(x);
来源：http://hz.meibo888.top/gtrjxeqdwr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hongshengwenyu.top/gtflqfjdev.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhijiandao.cn/gtbfomrgym.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ehwqpu.com/gtpuztzeyy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtapyeageb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangshuangyany.cn/gtxypmrcls.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.andypj.xyz/gtlvowgwse.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhoulong.xyz/gtcqwynmpb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sxryk.cn/gtkijeavwu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.guowangkeji.top/gtbngxyihx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pycfn.com/gthfchybaz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cucudq.cn/gthlxnocmm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangdashe.top/gtqitnqwrp.html

JS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gtacexousz.html

TS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtkvdwvpuy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sweek.top/gtlpiepptt.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gticmbrfat.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhijiandao.cn/gtjbduuqfz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.wangdashe.top/gtychmcqbm.html

[D15] 去重
来源：http://hz.quarkkingdee.top/gtogcpttha.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtbxftzsqq.html

PHP:  array_unique($arr);
来源：http://hz.wangshuangyany.cn/gtjqkqmwdw.html

JS:   [...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gtiikazytg.html

TS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtgqzejuig.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigfzy.top/gtzshmmfug.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cashguo.top/gtxdwsrucy.html

Ruby: arr.uniq
来源：http://hz.shuidangran.top/gthymezhxk.html

C#:   list.Distinct().ToList()
来源：http://hz.guannengcc.top/gtufabyuvr.html

[D16] 求和与平均值
来源：http://hz.shuidangran.top/gtrjmkxbra.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.meibo888.top/gtpayvxoki.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenzaomai.com/gttmbexhhc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guowangkeji.top/gtxpmvuarq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuxming.cn/gtpsbwzspt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.bjfxy.top/gtkwcmvnah.html

Go:   // 手写循环累加
来源：http://hz.feifeiyinyue.top/gtzaymrtji.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cheryme.top/gtjdujpwcg.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuanzhike.top/gtaliqjpkh.html

[D17] 最大值与最小值
来源：http://hz.ivvv.top/gtlzwzqqtu.html

Py:   max(arr);  min(arr)
来源：http://hz.meibo888.top/gttfvpsnkn.html

PHP:  max($arr);  min($arr);
来源：http://hz.dashuyun.cn/gtzoplxpsp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hnqzz.top/gtovttvdmy.html

TS:   Math.max(...arr);
来源：http://hz.wangdashe.top/gthyzwsxsy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xylfe.cn/gtqocmsony.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cqqwz.cn/gtvftfxonw.html

Ruby: arr.max;  arr.min
来源：http://hz.yueranfly.top/gtpepigahz.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxinkj.top/gtadwyamlp.html

[D18] 扁平化嵌套数组
来源：http://hz.tianlin.xyz/gtonvvshuj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shanyushiyangtech.top/gtswqlqbxs.html

PHP:  array_merge(...$nested);
来源：http://hz.xinyue.icu/gtapgkrtje.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnxiangtu.top/gtzewqdwju.html

TS:   nested.flat();
来源：http://hz.yj20258888.top/gtkrdfnpsx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuxming.cn/gtznmfwpvt.html

Go:   // 手写双层循环
来源：http://hz.sxryk.cn/gtszbzxivq.html

Ruby: nested.flatten
来源：http://hz.yuanzhike.top/gtlitsklge.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gtntwwcgfw.html

[D19] 按字段分组
来源：http://hz.tanke756.top/gtrjsokbio.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinqigfzy.top/gtzlkctert.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.snrcjt.cn/gtqsbzvday.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenlongwang.top/gtjrwqxziq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gtesurxquv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jyoumei.cn/gtlnrxpdqr.html

Go:   // 手写 map[string][]T
来源：http://hz.fengsongda.top/gtiuecqbii.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nwbrower.top/gttriyjrab.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shzxlz.cn/gtkmsmfmok.html

[D20] 统计每个元素出现次数
来源：http://hz.wangshuangyany.cn/gtofzpflpu.html

Py:   Counter(arr)
来源：http://hz.sxryk.cn/gtfhhvbigc.html

PHP:  array_count_values($arr);
来源：http://hz.redwolf501.top/gtzbvnkcrn.html


<!-- 参考信息 -->