代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://hz.hongshengwenyu.top/gthymhsikn.html

[C03] 可变参数
来源：http://hz.jinqigfzy.top/gtzqokqdba.html

Py:   def total(*args): return sum(args)
来源：http://hz.bjfxy.top/gtbpnhzkdj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.daria6918.cn/gteawjvrxx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxinkj.top/gtsdlikekd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtcnngunkp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhongyouzk.top/gtsvsqesvi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jianghu66.top/gtjwbeqfny.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hammf.cn/gtzavlbhne.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinghuilouyu.cn/gtvimogafx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.feifeiyinyue.top/gtaxgewbma.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinyuanbaomall.cn/gtlecifmmd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.9152youxi.cn/gtihjahous.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.fengsongda.top/gtvssjgbsf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhiwuduotai.top/gtoindpuda.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shanyushiyangtech.top/gtjguuvmry.html

Go:   // 无：用配置结构体参数
来源：http://hz.cheryme.top/gtbetjbarh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtouqszrjt.html

C#:   f(a: 1, b: 2)
来源：http://hz.gogol.net.cn/gtycawjgte.html

[C05] 返回多个值
来源：http://hz.gaohongyu789.top/gtcpdfjfgi.html

Py:   return a, b
来源：http://hz.gzhubu.top/gtwgctsmof.html

PHP:  return [$a, $b];
来源：http://hz.ehwqpu.com/gtheptwdrz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hammf.cn/gtadudhznl.html

TS:   return { a, b };
来源：http://hz.sufxvd.cn/gtyhxbbnil.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tian-w.cn/gtnzsdlwyd.html

Go:   return a, b
来源：http://hz.jqgfzy.top/gthjpwteyu.html

Ruby: return a, b
来源：http://hz.aibaodan.cn/gtgtymbkcb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yanxiufei.cn/gtwofviakd.html

[C06] 匿名函数 / lambda
来源：http://hz.redwolf501.top/gtuqirvsff.html

Py:   square = lambda x: x * x
来源：http://hz.jinqigfzy.top/gtfynqunyn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.guowangkeji.top/gtdbnwuqmv.html

JS:   const square = x => x * x;
来源：http://hz.vqdsnc.cn/gtvcizpdvw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yanxiufei.cn/gtydemodjf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shuidangran.top/gtwogriaaq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ydjk.org.cn/gtokrwlvwq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yuxming.cn/gtaopainhi.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yonumen.top/gtnpmagoxz.html

[C07] 把函数作为参数传入
来源：http://hz.gogol.net.cn/gtxawftjbu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.svipenyu.cn/gtavrtmmsj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.andypj.xyz/gtmphzhuec.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.meibo888.top/gtxnwhnpel.html

TS:   arr.map(String)
来源：http://hz.nwbrower.top/gtqlfaaphp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.9152youxi.cn/gtaifiwoby.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yuanzhike.top/gtmbeqrhug.html

Ruby: arr.map(&:upcase)
来源：http://hz.daxiang520.top/gtjvqeedjx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fengsongda.top/gtyfjhketu.html

[C08] 闭包
来源：http://hz.tianlin.xyz/gtejjzmhsq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.svipenyu.cn/gtwhwkadjc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258888.top/gtocgyrvri.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gturnifvjr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aibaodan.cn/gtexxgsbap.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nwbrower.top/gtqtdtxxgs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.haohaochexian.top/gtpcdmlbzm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ehwqpu.com/gtvtxiogqp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gtlmfftrcm.html

[C09] 递归
来源：http://hz.fzhhl.top/gtpalmwufk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gtsbnbsmwu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.pengpengdd.cyou/gtnilidawm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.redwolf501.top/gtsphvlwru.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fengsongda.top/gtjxkfuiro.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hfpthk.cn/gtblxswlge.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.0kj1m.cn/gtbqwqsnbt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.smart0.xyz/gtegbbjpnu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.smart0.xyz/gtzeykpjir.html

[C10] 变量作用域
来源：http://hz.cqqwz.cn/gtobecstck.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jianghu66.top/gtdkwykblx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cqqwz.cn/gtttillgkt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yvedp.cn/gtwqtdpist.html

TS:   同 JS
来源：http://hz.shuidangran.top/gtojdqxmrw.html

Java: 方法内为块级作用域
来源：http://hz.hnqzz.top/gtiyoghvwy.html

Go:   花括号块级作用域
来源：http://hz.tianlin.xyz/gtfrikkbfc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jqgfzy.top/gtvkgpubqx.html

C#:   块级作用域
来源：http://hz.cqqwz.cn/gtltkcwbdl.html

[C11] 模块导入与导出
来源：http://hz.ivvv.top/gtqistpqui.html

Py:   from module import func
来源：http://hz.gaohongyu789.top/gtnousrflc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guannengcc.top/gttxuebdyt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.feifeiyinyue.top/gtbtxgjgfz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.redwolf501.top/gtqnyyfgdx.html

Java: import java.util.List;
来源：http://hz.ppjwa.cn/gtmdwrdkno.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shanyushiyangtech.top/gtppmhdesg.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hammf.cn/gtldcpbfqu.html

C#:   using System.Text;
来源：http://hz.yonumen.top/gtefkamdvq.html

[C12] 立即执行函数 IIFE
来源：http://hz.yonumen.top/gtxhdryjjp.html

Py:   (lambda: print("run"))()
来源：http://hz.jqgfzy.top/gtlaizfnos.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ydjk.org.cn/gtyjhjpfcj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shuidangran.top/gtsdhgsxpk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtefljbmbr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yonumen.top/gtswbmshub.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxinkj.top/gtexqqysnp.html

Ruby: -> { puts "run" }.call
来源：http://hz.dashuyun.cn/gtjrvoempm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj202588.top/gthvaczofu.html

[C13] 类型声明 / 类型注解
来源：http://hz.aibaodan.cn/gtricbafbi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shuidangran.top/gtyhtqzjjx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtofqhznfc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xuetiantiany.cn/gthirhgfjt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gtxrenlmxm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtwovtwkjf.html

Go:   func add(a, b int) int
来源：http://hz.sufxvd.cn/gtkijqdwek.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.chenzaomai.com/gtqrufirjt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shzxlz.cn/gthpskcqoj.html

[C14] 泛型函数
来源：http://hz.sysykeji.top/gtroleawjb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.iojbl.cn/gtmldoudkm.html

PHP:  // 无泛型
来源：http://hz.mhx1999.top/gtqyezorhi.html

JS:   // 无泛型
来源：http://hz.cucudq.cn/gtthdtxztn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sweek.top/gtmrmxhobe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj20258.top/gtmiwxvqcq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cashguo.top/gttranquqw.html

Ruby: # 无泛型
来源：http://hz.zhengqikj.top/gtckdlbgot.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xinyue.icu/gtnhmncmpj.html

[C15] 解构 / 展开参数
来源：http://hz.haohaochexian.top/gtsainekkd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.daria6918.cn/gtrxdyxvzg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sysykeji.top/gtnmgansny.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtfcptehne.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gzhubu.top/gtwgoczicj.html

Java: // 无解构
来源：http://hz.andypj.xyz/gtfbynmykb.html

Go:   // 无解构
来源：http://hz.fengsongda.top/gtkivmhemf.html

Ruby: a, b = pair
来源：http://hz.yuanzhike.top/gtycnttuog.html

C#:   var (a, b) = pair;
来源：http://hz.tianlin.xyz/gtjwrqfztc.html

[C16] 函数 / 方法重载
来源：http://hz.hnxiangtu.top/gtrzgfrvax.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenzaomai.com/gtpbmssudf.html

PHP:  // 无重载
来源：http://hz.fengsongda.top/gtlbzlambf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yj20258.top/gtknvjnpoi.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cucudq.cn/gtpctqaoxu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.c1oappe.top/gtvxvxidnf.html

Go:   // 无重载：用不同函数名
来源：http://hz.dashuyun.cn/gtljvyhukv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.andypj.xyz/gtpzxrjfri.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cqqwz.cn/gtdiubcyep.html

================================================================================
来源：http://hz.jianghu66.top/gtitvtfbca.html

D. 数组 / 列表 / 集合
来源：http://hz.nanxinkj.top/gtpuabeqxs.html

================================================================================
来源：http://hz.fzhhl.top/gtyfthfrie.html

[D01] 创建数组 / 列表
来源：http://hz.xuetiantiany.cn/gtkztgkjri.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.meibo888.top/gtfyvztohf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.tian-w.cn/gtilriqvlx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhijiandao.cn/gtwfijimyu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guannengcc.top/gtpdbybtyg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinqigfzy.top/gtpfrjngbd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ydzc1.top/gtojmpvljh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.pengpengdd.cyou/gtfrxiuool.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gogol.net.cn/gtqshttcrc.html

[D02] 追加元素到末尾
来源：http://hz.aibaodan.cn/gtnpsdjbpk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cashguo.top/gtmxsfbtyg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shanyushiyangkeji.top/gtctdcmqsk.html

JS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gttccbcasm.html

TS:   arr.push(4);
来源：http://hz.meibo888.top/gtfjbpfxok.html

Java: list.add(4);
来源：http://hz.sufxvd.cn/gtkhzdpswa.html

Go:   arr = append(arr, 4)
来源：http://hz.sufxvd.cn/gtqvutvowf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hfpthk.cn/gtocgxolko.html

C#:   list.Add(4);
来源：http://hz.ydzc1.top/gtjghriduj.html

[D03] 在指定位置插入元素
来源：http://hz.tianlin.xyz/gtsjiwrvna.html

Py:   arr.insert(0, 0)
来源：http://hz.0kj1m.cn/gtafarnxaq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.tian-w.cn/gtufunfeip.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.snrcjt.cn/gtfvpweplh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hongshengwenyu.top/gteaevcypq.html

Java: list.add(0, 0);
来源：http://hz.nanxinkj.top/gtkipvical.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj202588.top/gtghjzfggw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydjk.org.cn/gtvelohsat.html

C#:   list.Insert(0, 0);
来源：http://hz.zhixingplan.top/gtqkkxonww.html

[D04] 删除元素
来源：http://hz.c1oappe.top/gthesvizwz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sweek.top/gtpfvybvjh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shuidangran.top/gtumvbhdfe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zdqjudy.top/gtigjdocov.html

TS:   arr.splice(0, 1);
来源：http://hz.sysykeji.top/gtvgdihlky.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenlongwang.top/gtgvbqofcl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.svipenyu.cn/gtpzbbuucc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigfzy.top/gtxdfuatkg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pengpengdd.cyou/gtynzuzouc.html

[D05] 访问与修改元素
来源：http://hz.zhongyouzk.top/gtujmktmii.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtdjacexfk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yueranfly.top/gtewggctdg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtnnokxhvy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.aibaodan.cn/gtkakkwerc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fzhhl.top/gthetcrpwq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuanzx.com/gtbicvsahg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gthlxulvky.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ehwqpu.com/gtejppnsfu.html

[D06] 数组长度
来源：http://hz.hfpthk.cn/gtovqinaaz.html

Py:   len(arr)
来源：http://hz.smart0.xyz/gtteejlgrm.html

PHP:  count($arr);
来源：http://hz.zhengqikj.top/gtkgdmzukk.html

JS:   arr.length
来源：http://hz.dashuyun.cn/gtlvovfvia.html

TS:   arr.length
来源：http://hz.wangshuangyany.cn/gtuykrtrzw.html

Java: list.size();
来源：http://hz.cqqwz.cn/gtdkznhofz.html

Go:   len(arr)
来源：http://hz.jinyuanbaomall.cn/gtyyorprzq.html

Ruby: arr.length; arr.size
来源：http://hz.xingfuxueyuan.xyz/gtkujilkaz.html

C#:   list.Count;
来源：http://hz.xylfe.cn/gtrzlwrsvd.html

[D07] 切片 / 取子数组
来源：http://hz.feifeiyinyue.top/gteeebbgcd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.smart0.xyz/gtanxnwccg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daria6918.cn/gtcktiqxky.html

JS:   arr.slice(1, 4);
来源：http://hz.hammf.cn/gtearvvvdr.html

TS:   arr.slice(1, 4);
来源：http://hz.yuxming.cn/gtwylytpaf.html

Java: list.subList(1, 4);
来源：http://hz.xylfe.cn/gtwlkaltmj.html

Go:   arr[1:4]
来源：http://hz.ivvv.top/gtkcjveete.html

Ruby: arr[1, 3]
来源：http://hz.xziqi.cn/gttxgokozi.html

C#:   list.GetRange(1, 3);
来源：http://hz.feifeiyinyue.top/gttygnrvnb.html

[D08] 合并两个数组
来源：http://hz.ybcxt.top/gtgtputyca.html

Py:   a + b;  a.extend(b)
来源：http://hz.yongpay.top/gtswarpjmr.html

PHP:  array_merge($a, $b);
来源：http://hz.shangyingyoupin.top/gtjnoyrjmc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hfpthk.cn/gtvwnhednb.html

TS:   [...a, ...b];
来源：http://hz.cqqwz.cn/gtmndwkybr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xinyue.icu/gtxwuqyhiw.html

Go:   append(a, b...)
来源：http://hz.daria6918.cn/gtxrjdcjfz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.dianchejie.cn/gtvuqngfaq.html

C#:   a.Concat(b).ToList()
来源：http://hz.pycfn.com/gtmgcebbze.html

[D09] 排序（升序）
来源：http://hz.zhongyouzk.top/gtpscvxbpf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtwpelqtwy.html

PHP:  sort($arr);
来源：http://hz.hammf.cn/gtarmynhle.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sxryk.cn/gtitsafdal.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhixingplan.top/gtmyfsnudp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yongpay.top/gtrcilybcz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ybcxt.top/gtpryoncph.html

Ruby: arr.sort
来源：http://hz.c1oappe.top/gtuapmtxtz.html

C#:   list.Sort();
来源：http://hz.ivvv.top/gtkagkpntq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cheryme.top/gthavkcsgk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.andypj.xyz/gthbrgftkm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tian-w.cn/gtyvsotlpo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.9152youxi.cn/gtsqzulqms.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.vqdsnc.cn/gtbhmqodsn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cashguo.top/gttijgtytg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydjk.org.cn/gtwzgdtqyi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hysaishi.cn/gtpfxvvwbl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigfzy.top/gtjcuvvndt.html

[D11] 反转数组
来源：http://hz.snrcjt.cn/gtqaxdeqxc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.feifeiyinyue.top/gtepezlffq.html

PHP:  array_reverse($arr);
来源：http://hz.yuanzhike.top/gtvhwlxuhb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.52xcode.cn/gtqhofiurj.html

TS:   [...arr].reverse();
来源：http://hz.cdnleiting.top/gtgqgoqdjr.html

Java: Collections.reverse(list);
来源：http://hz.daxiang520.top/gtecswiusc.html

Go:   slices.Reverse(arr)
来源：http://hz.wangdashe.top/gttjtlccuh.html

Ruby: arr.reverse
来源：http://hz.quarkkingdee.top/gtrqqjkgyc.html

C#:   list.Reverse();
来源：http://hz.feifeiyinyue.top/gtzjrnknvh.html

[D12] 查找元素下标
来源：http://hz.redwolf501.top/gthhhhwfix.html

Py:   arr.index(x);  x in arr
来源：http://hz.ywan-chungtsiang.top/gtrecangdh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xuetiantiany.cn/gtvtngccbm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtkjqmyyio.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jlsjyb.cn/gtqagrzack.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenzaomai.com/gtwjjwlqxe.html

Go:   slices.Index(arr, x)
来源：http://hz.zhoulong.xyz/gtgrrkpobh.html

Ruby: arr.index(x)
来源：http://hz.kuanghao11.cn/gtowsfmski.html

C#:   list.IndexOf(x);
来源：http://hz.mhx1999.top/gtveobcwwr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.quarkkingdee.top/gtsbldivzf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.redwolf501.top/gtpxmxdfsd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yongpay.top/gtpatzbwfz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.0kj1m.cn/gtxgfxdjrs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.316326.xyz/gtkgeogwcp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.quarkkingdee.top/gttwvnmdbn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ppjwa.cn/gtspgiaceb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.havefunace.top/gtgfoaagem.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tanke756.top/gtlthcrdmt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nanxinkj.top/gtruealzzs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.redwolf501.top/gtsraaqcgb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj20258.top/gtldqkccas.html

JS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gtecqldblr.html

TS:   arr.map(x => x * 2)
来源：http://hz.snrcjt.cn/gthbfqoxqu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.andypj.xyz/gtqzfukfwj.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtfdlbenhx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gotoacloud.top/gteltwubhp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tianlin.xyz/gtkjqintgb.html

[D15] 去重
来源：http://hz.cdnleiting.top/gtaqnlsyol.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yonumen.top/gtatrqjqjx.html

PHP:  array_unique($arr);
来源：http://hz.wangdashe.top/gtuymiqgrs.html

JS:   [...new Set(arr)]
来源：http://hz.gzhubu.top/gtsmwqfumx.html

TS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtfcebdmca.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pengpengdd.cyou/gtspyvyzlh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.meibo888.top/gtuevxmluc.html

Ruby: arr.uniq
来源：http://hz.cdnleiting.top/gtybvakoyx.html

C#:   list.Distinct().ToList()
来源：http://hz.birdmap.top/gtxrswhaed.html

[D16] 求和与平均值
来源：http://hz.yongpay.top/gtusdrlpaf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenjidiqi.icu/gthkqyhavo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sufxvd.cn/gtlqtbnuuo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ywan-chungtsiang.top/gtjivulscz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hywenlv.cn/gtoaabhoth.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.feifeiyinyue.top/gtntlfdhcm.html

Go:   // 手写循环累加
来源：http://hz.xylfe.cn/gtroxuvdtz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.snrcjt.cn/gthhlnexfu.html

C#:   list.Sum();  list.Average()
来源：http://hz.dianchejie.cn/gtstxzczuj.html

[D17] 最大值与最小值
来源：http://hz.yuanzhike.top/gtyhouypuv.html

Py:   max(arr);  min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtywwptdgj.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydjk.org.cn/gtagljqhrc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.aibaodan.cn/gtheynpmbk.html

TS:   Math.max(...arr);
来源：http://hz.chenzaomai.com/gtqfmeeqds.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuanzhike.top/gtqazejygf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yonumen.top/gtkmckkwit.html

Ruby: arr.max;  arr.min
来源：http://hz.fengsongda.top/gtljmitqqu.html

C#:   list.Max();  list.Min()
来源：http://hz.gaohongyu789.top/gtfrobcbsj.html

[D18] 扁平化嵌套数组
来源：http://hz.hnxiangtu.top/gtnbnedppn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.dashuyun.cn/gtvsjuufdi.html

PHP:  array_merge(...$nested);
来源：http://hz.zhengqikj.top/gtgojfkshq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.kuanghao11.cn/gtmduugxft.html

TS:   nested.flat();
来源：http://hz.jinqigufen.top/gtmutqeron.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tanke756.top/gtmddmvsdw.html

Go:   // 手写双层循环
来源：http://hz.yj202588.top/gtwuwlzfgi.html

Ruby: nested.flatten
来源：http://hz.zhiwuduotai.top/gtxvpqinrl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.birdmap.top/gtwgomeytn.html

[D19] 按字段分组
来源：http://hz.shangyingyoupin.top/gtvwxhskdh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangkeji.top/gtzlozdwvj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tanke756.top/gtpkplxupp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cheryme.top/gtmgukaztz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.wangshuangyany.cn/gtuekkwtix.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shangyingyoupin.top/gthtupzjih.html

Go:   // 手写 map[string][]T
来源：http://hz.wangdashe.top/gtqgtjxgtx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gogol.net.cn/gttpwhxaig.html


<!-- 参考信息 -->