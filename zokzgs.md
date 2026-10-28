代发 wailian999

Py:   if not data: return
来源：http://hz.tianlin.xyz/gthnyukmvd.html

PHP:  if (!$data) { return; }
来源：http://hz.sxryk.cn/gtaorooqdh.html

JS:   if (!data) return;
来源：http://hz.cdnleiting.top/gttiqzxpfk.html

TS:   if (!data) return;
来源：http://hz.cdnleiting.top/gtlrlmnjuy.html

Java: if (data == null) return;
来源：http://hz.zhixingplan.top/gtwnajbjxl.html

Go:   if data == nil { return }
来源：http://hz.yj20258888.top/gtgsjfgyri.html

Ruby: return if data.nil?
来源：http://hz.yvedp.cn/gtdhdisigt.html

C#:   if (data == null) return;
来源：http://hz.cucudq.cn/gtupgokuxx.html

================================================================================
来源：http://hz.tian-w.cn/gtcekvcthm.html

C. 函数与作用域
来源：http://hz.zhijiandao.cn/gtpombkmyj.html

================================================================================
来源：http://hz.ydjk.org.cn/gtjsrzekby.html

[C01] 定义函数
来源：http://hz.dashuyun.cn/gtpupkxrvt.html

Py:   def add(a, b): return a + b
来源：http://hz.fzhhl.top/gtkgijxjzz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gtelwyfqjj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ybcxt.top/gtjkehpaxp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtepvztwzc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.mhx1999.top/gtmcysgdmu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhaomingkeji.xyz/gthfkehxep.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yuanzhike.top/gtowbgnlqq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gtfnckuput.html

[C02] 默认参数
来源：http://hz.yonumen.top/gtjzwtggho.html

Py:   def greet(name="World"): return name
来源：http://hz.gaohongyu789.top/gtbfrefnjd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ywan-chungtsiang.top/gtqiwgwycl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zdqjudy.top/gtvvtzirwp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jianghu66.top/gtxbdxwoyl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinghuilouyu.cn/gtgtdnpvbr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hfpthk.cn/gtjdrqzlvl.html

Ruby: def greet(name = "World") = name
来源：http://hz.shuidangran.top/gtultpjbop.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj20258.top/gtiydehtep.html

[C03] 可变参数
来源：http://hz.c1oappe.top/gteikhmopw.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinqigfzy.top/gtluokcuom.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nanxinkj.top/gtzyvqgzyj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxuanxn.top/gtuxclzsns.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258.top/gtuvekzhuh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gaohongyu789.top/gtogvhyhid.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nanxinkj.top/gtyoubgvfs.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tianlin.xyz/gtnumvfjtz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hammf.cn/gtvpktxbbn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.316326.xyz/gtpaqcwhxs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj20258.top/gtbfjczmkm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhaomingkeji.xyz/gtcmhjxnyx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hysaishi.cn/gtsqprpedg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yonumen.top/gtznnebuqi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.bjfxy.top/gtknihnkng.html

Go:   // 无：用配置结构体参数
来源：http://hz.andypj.xyz/gthgeyhgor.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jyoumei.cn/gtwobhvbwr.html

C#:   f(a: 1, b: 2)
来源：http://hz.yangfankeji.com/gtouglotyw.html

[C05] 返回多个值
来源：http://hz.9152youxi.cn/gtqwozopoo.html

Py:   return a, b
来源：http://hz.wangdashe.top/gttehndtbd.html

PHP:  return [$a, $b];
来源：http://hz.jqgufenzy.top/gtsbiqcqcm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sufxvd.cn/gtytiimvqc.html

TS:   return { a, b };
来源：http://hz.gogol.net.cn/gtmilyypwa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cqqwz.cn/gtfxnhvvqn.html

Go:   return a, b
来源：http://hz.xinyue.icu/gtpvkeikve.html

Ruby: return a, b
来源：http://hz.iojbl.cn/gtkiscyawc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gtxclubyax.html

[C06] 匿名函数 / lambda
来源：http://hz.jqgufenzy.top/gtuksoaboq.html

Py:   square = lambda x: x * x
来源：http://hz.yueranfly.top/gthehmofjm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.0kj1m.cn/gtbmkvdeou.html

JS:   const square = x => x * x;
来源：http://hz.yuanzhike.top/gtokretbjo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.fzhhl.top/gthyvploje.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yongpay.top/gthjtermqm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.meibo888.top/gtwhqozrhf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.316326.xyz/gthjeihylq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tanke756.top/gtejgpwidv.html

[C07] 把函数作为参数传入
来源：http://hz.hammf.cn/gteigemplc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhiwuduotai.top/gtvyuhbqrr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ydzc1.top/gtmrgrvoki.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nanxuanxn.top/gtagogijoc.html

TS:   arr.map(String)
来源：http://hz.pengpengdd.cyou/gtwnddxrbt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tanke756.top/gtqoyvgjlc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.haohaochexian.top/gtvludvufo.html

Ruby: arr.map(&:upcase)
来源：http://hz.cdnleiting.top/gttrevgrey.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinqigfzy.top/gtthsvxmoi.html

[C08] 闭包
来源：http://hz.hnqzz.top/gthphbedps.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.fzhhl.top/gtnjooxtpg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.pycfn.com/gtxrrlecri.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtonqhyshq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gtimtyxgsp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ivvv.top/gtcvnbymjp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.quarkkingdee.top/gtpryrbygb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shangyingyoupin.top/gtmeuwltdy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gtyahhjjxc.html

[C09] 递归
来源：http://hz.zhixingplan.top/gtakemjgam.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.bjfxy.top/gthevvjcnb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenlongwang.top/gtclwtqpce.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258.top/gtalqzthqj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yvedp.cn/gtvvakrgte.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zdqjudy.top/gtxaemogci.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yanxiufei.cn/gttoigekyb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cqqwz.cn/gtkivxsehy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yuxming.cn/gtzrvbqqyv.html

[C10] 变量作用域
来源：http://hz.zycfv.cn/gthyxuxcox.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aibaodan.cn/gtiouncpco.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ybcxt.top/gtnugigrsp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yongpay.top/gtedxdzioo.html

TS:   同 JS
来源：http://hz.yonumen.top/gtxtkwmqnq.html

Java: 方法内为块级作用域
来源：http://hz.zhixingplan.top/gtqqvpplgx.html

Go:   花括号块级作用域
来源：http://hz.zhoulong.xyz/gtvkmmsjfs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tanke756.top/gtmrdfbxjb.html

C#:   块级作用域
来源：http://hz.haohaochexian.top/gtizzygqsl.html

[C11] 模块导入与导出
来源：http://hz.xuetiantiany.cn/gtmxssxfuv.html

Py:   from module import func
来源：http://hz.0kj1m.cn/gtjocqdtfs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shzxlz.cn/gtactalzsz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tian-w.cn/gtbzaugdjl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.mhx1999.top/gtgptdaylc.html

Java: import java.util.List;
来源：http://hz.meibo888.top/gtctbdvbol.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.chenlongwang.top/gtaoqkewwb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fengsongda.top/gtmvwvmdst.html

C#:   using System.Text;
来源：http://hz.yangfankeji.com/gtlbeztcco.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhixingplan.top/gtlnidjkwf.html

Py:   (lambda: print("run"))()
来源：http://hz.gzhubu.top/gtbmtutlei.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pengpengdd.cyou/gtyeqamtnn.html

JS:   (() => { console.log("run"); })();
来源：http://hz.quarkkingdee.top/gtujqrslxw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nwbrower.top/gttqiwlfkw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj202588.top/gtolmxrkfg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ehwqpu.com/gtnomspqts.html

Ruby: -> { puts "run" }.call
来源：http://hz.hammf.cn/gtkzazdzkk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xziqi.cn/gtnhwlkbkt.html

[C13] 类型声明 / 类型注解
来源：http://hz.xuetiantiany.cn/gtjqvajxlf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinghuilouyu.cn/gtbbczsevk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnxiangtu.top/gtbwhsmmkx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shuidangran.top/gtaackyxpr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtuzdcwysn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtpiskendv.html

Go:   func add(a, b int) int
来源：http://hz.yvedp.cn/gtcddmnucf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yonumen.top/gtlcxlqztj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cdnleiting.top/gteaktyvmt.html

[C14] 泛型函数
来源：http://hz.zhoulong.xyz/gtebqjgnfb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jiagoushi.top/gtcebfkexu.html

PHP:  // 无泛型
来源：http://hz.jianghu66.top/gtiogwmqxe.html

JS:   // 无泛型
来源：http://hz.cqqwz.cn/gtdawnvdxq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jqgfzy.top/gtggzsspnx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cheryme.top/gtjvwtltrj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.kuanghao11.cn/gtlrfzzggb.html

Ruby: # 无泛型
来源：http://hz.hywenlv.cn/gtlrzbnqlo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.vqdsnc.cn/gtautzojfd.html

[C15] 解构 / 展开参数
来源：http://hz.52xcode.cn/gtrqqovqjm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigfzy.top/gtdkjnespg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aizwys.cn/gtysvqgezh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gtwrxpkxzo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.feifeiyinyue.top/gtkuhljtod.html

Java: // 无解构
来源：http://hz.xuanzx.com/gtedoqjxdl.html

Go:   // 无解构
来源：http://hz.gogol.net.cn/gtlhgynvzk.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtqdkhmixv.html

C#:   var (a, b) = pair;
来源：http://hz.yj20258.top/gtwcuixyek.html

[C16] 函数 / 方法重载
来源：http://hz.fzhhl.top/gtkxjsbdrp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.pengpengdd.cyou/gtjbkszejv.html

PHP:  // 无重载
来源：http://hz.bjfxy.top/gtyoqdyzhc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tian-w.cn/gtpugmpwqs.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhaomingkeji.xyz/gtzjmeccjy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gotoacloud.top/gtovphtfrn.html

Go:   // 无重载：用不同函数名
来源：http://hz.snrcjt.cn/gtqzkxakmi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.haohaochexian.top/gtkgklbsal.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cashguo.top/gtdgfrmihk.html

================================================================================
来源：http://hz.jlsjyb.cn/gtlrgnzick.html

D. 数组 / 列表 / 集合
来源：http://hz.ppjwa.cn/gtkwybjkok.html

================================================================================
来源：http://hz.hfpthk.cn/gttwumdniv.html

[D01] 创建数组 / 列表
来源：http://hz.gogol.net.cn/gtbywwxyxe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.mhx1999.top/gtjdmrodaa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yongpay.top/gtqpbovntw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.snrcjt.cn/gtrbnbdouq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yangfankeji.com/gtbrzsnsqe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.9152youxi.cn/gtnzixexvs.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhijiandao.cn/gtlqpiffbp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nwbrower.top/gtxbagkpie.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yonumen.top/gtluyddypv.html

[D02] 追加元素到末尾
来源：http://hz.316326.xyz/gtepsdvivm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xziqi.cn/gtkilrejdt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nanxinkj.top/gtohkhcmzy.html

JS:   arr.push(4);
来源：http://hz.c1oappe.top/gtjbthmwrl.html

TS:   arr.push(4);
来源：http://hz.jqgfzy.top/gtrvesczki.html

Java: list.add(4);
来源：http://hz.cdnleiting.top/gtrwenfauf.html

Go:   arr = append(arr, 4)
来源：http://hz.daria6918.cn/gtdmxiorhd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gotoacloud.top/gtjuslncjy.html

C#:   list.Add(4);
来源：http://hz.xingfuxueyuan.xyz/gtrscapbvs.html

[D03] 在指定位置插入元素
来源：http://hz.daria6918.cn/gtidxklqcz.html

Py:   arr.insert(0, 0)
来源：http://hz.cheryme.top/gtbnetzahs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xuanzx.com/gtrvslyloe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hywenlv.cn/gtkgngmlcl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ehwqpu.com/gtlxwwsbsa.html

Java: list.add(0, 0);
来源：http://hz.cqqwz.cn/gtptfjhoat.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yangfankeji.com/gtaystyxij.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yueranfly.top/gtmhrtyeye.html

C#:   list.Insert(0, 0);
来源：http://hz.cdnleiting.top/gtuardrnej.html

[D04] 删除元素
来源：http://hz.ydzc1.top/gtweqiixya.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.52xcode.cn/gtugvbznte.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.redwolf501.top/gtwccfnqlt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenjidiqi.icu/gttmalhucw.html

TS:   arr.splice(0, 1);
来源：http://hz.shanyushiyangtech.top/gtqrlcpxur.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pengpengdd.cyou/gthgrkaufy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj20258888.top/gtycgcjhdh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhongyouzk.top/gtxikhxbpm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ywan-chungtsiang.top/gtityawrbz.html

[D05] 访问与修改元素
来源：http://hz.nanxuanxn.top/gtbsqlxweh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shangyingyoupin.top/gtoefzfwpc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daxiang520.top/gtxgqngwgr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hnxiangtu.top/gtlcyjljxe.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.aibaodan.cn/gtxqjiyeik.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhaomingkeji.xyz/gtkkywosbs.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jianghu66.top/gtjliyabaz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.smart0.xyz/gtggbtyccv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.tanke756.top/gtbkjiulzf.html

[D06] 数组长度
来源：http://hz.fengsongda.top/gtqhuucedv.html

Py:   len(arr)
来源：http://hz.nwbrower.top/gtkuekwwgs.html

PHP:  count($arr);
来源：http://hz.havefunace.top/gtthfpyasq.html

JS:   arr.length
来源：http://hz.c1oappe.top/gtosfybuzq.html

TS:   arr.length
来源：http://hz.daria6918.cn/gtiojoklfo.html

Java: list.size();
来源：http://hz.wangshuangyany.cn/gtwhirhmbh.html

Go:   len(arr)
来源：http://hz.svipenyu.cn/gtnxgwqfdd.html

Ruby: arr.length; arr.size
来源：http://hz.jinyuanbaomall.cn/gthyscsjxd.html

C#:   list.Count;
来源：http://hz.zhiwuduotai.top/gtpunppuzp.html

[D07] 切片 / 取子数组
来源：http://hz.chenjidiqi.icu/gtxnulxqle.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.andypj.xyz/gtzrbuadpr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gzhubu.top/gtrxdzrnwb.html

JS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gthauioaqy.html

TS:   arr.slice(1, 4);
来源：http://hz.pycfn.com/gtvjoxhpga.html

Java: list.subList(1, 4);
来源：http://hz.gogol.net.cn/gtvfzakxig.html

Go:   arr[1:4]
来源：http://hz.jinqigufen.top/gtqxnwyacr.html

Ruby: arr[1, 3]
来源：http://hz.zhongyouzk.top/gtgbpignvc.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangtech.top/gtivcyoeau.html

[D08] 合并两个数组
来源：http://hz.bjfxy.top/gtoxnxvpkv.html

Py:   a + b;  a.extend(b)
来源：http://hz.shanyushiyangtech.top/gtekhbzuwr.html

PHP:  array_merge($a, $b);
来源：http://hz.jqgfzy.top/gtnyvwvswq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenzaomai.com/gtdwlrkcex.html

TS:   [...a, ...b];
来源：http://hz.jlsjyb.cn/gtpvfuflmm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.9152youxi.cn/gtrjaqupab.html

Go:   append(a, b...)
来源：http://hz.dianchejie.cn/gtjatxihkc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yanxiufei.cn/gtkezistyd.html

C#:   a.Concat(b).ToList()
来源：http://hz.9152youxi.cn/gtlrkfukpk.html

[D09] 排序（升序）
来源：http://hz.yj202588.top/gtwelgqjva.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtzdfvhmow.html

PHP:  sort($arr);
来源：http://hz.cucudq.cn/gtxljujyft.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj20258.top/gtzqmyjqsl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hnqzz.top/gtdadzrwau.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhiwuduotai.top/gtivspubqh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nwbrower.top/gtjouymxqd.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtqbyzjzzv.html

C#:   list.Sort();
来源：http://hz.zhixingplan.top/gtqwudfhcc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.0kj1m.cn/gtphrdwycd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.daxiang520.top/gtxlnyngvv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhaomingkeji.xyz/gtxtofdfze.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.smart0.xyz/gtfteylqxf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.kuanghao11.cn/gtwopmjdqm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ydjk.org.cn/gtazmezqrj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ybcxt.top/gtqeqyrnzj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhongyouzk.top/gtcyezahye.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cheryme.top/gtzbbbpygb.html

[D11] 反转数组
来源：http://hz.52xcode.cn/gtznbfrbhf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangtech.top/gtbgcrdyam.html

PHP:  array_reverse($arr);
来源：http://hz.kuanghao11.cn/gtuopkmtln.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258888.top/gtbjjxexea.html

TS:   [...arr].reverse();
来源：http://hz.wangdashe.top/gtnjrfyloj.html

Java: Collections.reverse(list);
来源：http://hz.dashuyun.cn/gtfnnibduw.html

Go:   slices.Reverse(arr)
来源：http://hz.cashguo.top/gtnhrsetkt.html

Ruby: arr.reverse
来源：http://hz.pycfn.com/gtodgiviwj.html

C#:   list.Reverse();
来源：http://hz.jlsjyb.cn/gtkranhuxe.html

[D12] 查找元素下标
来源：http://hz.yongpay.top/gtgaphyfkv.html

Py:   arr.index(x);  x in arr
来源：http://hz.cqqwz.cn/gttdbfhguv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sufxvd.cn/gtlqhowoxp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtkudgmpwn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenlongwang.top/gthwjwzikv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yongpay.top/gttmljamhi.html

Go:   slices.Index(arr, x)
来源：http://hz.cdnleiting.top/gthitysull.html

Ruby: arr.index(x)
来源：http://hz.gogol.net.cn/gtpxltuswv.html

C#:   list.IndexOf(x);
来源：http://hz.9152youxi.cn/gtomnfzdep.html

[D13] 过滤（保留满足条件的）
来源：http://hz.dashuyun.cn/gtckyfgcfh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ydzc1.top/gtqzjjqqlp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yanxiufei.cn/gtvaeezzqq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenlongwang.top/gtmpqpimlc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtjlgwpjcj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.daria6918.cn/gtsmqlcema.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cdnleiting.top/gtglaoxamw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.316326.xyz/gtsxidnbjd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hnqzz.top/gtiegaouwu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shzxlz.cn/gtidawqfnf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aizwys.cn/gtiualfkvu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cheryme.top/gtazzsgheq.html

JS:   arr.map(x => x * 2)
来源：http://hz.9152youxi.cn/gtpeypkgwm.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj20258888.top/gtdycpsfgj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.dianchejie.cn/gtkjddvjzl.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtaydgvnoe.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinqigfzy.top/gtopvrqvjr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cdnleiting.top/gtofuvtelr.html

[D15] 去重
来源：http://hz.daria6918.cn/gttaqfwmmr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gtuidbsqsl.html

PHP:  array_unique($arr);
来源：http://hz.chenzaomai.com/gteydmuvce.html

JS:   [...new Set(arr)]
来源：http://hz.birdmap.top/gtumslwins.html

TS:   [...new Set(arr)]
来源：http://hz.birdmap.top/gtqwptvtre.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yanxiufei.cn/gtwxxbohmo.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinyuanbaomall.cn/gtezwaxkdd.html

Ruby: arr.uniq
来源：http://hz.hammf.cn/gtxgjtwdlq.html

C#:   list.Distinct().ToList()
来源：http://hz.kuanghao11.cn/gtswudiewk.html

[D16] 求和与平均值
来源：http://hz.haohaochexian.top/gtyocpxoba.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aibaodan.cn/gtwjpvasec.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.316326.xyz/gtyvvzousj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.kuanghao11.cn/gtoyziraqf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gtecrapxlg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.0kj1m.cn/gtigerqxeq.html

Go:   // 手写循环累加
来源：http://hz.yongpay.top/gtzpzldqba.html


<!-- 参考信息 -->