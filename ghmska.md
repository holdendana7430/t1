代发 wailian999

================================================================================
来源：http://hz.fzhhl.top/gtcgavofsb.html

C. 函数与作用域
来源：http://hz.hnqzz.top/gtfuacwuha.html

================================================================================
来源：http://hz.yanxiufei.cn/gtvvcwytzr.html

[C01] 定义函数
来源：http://hz.quarkkingdee.top/gtpfixafwp.html

Py:   def add(a, b): return a + b
来源：http://hz.cheryme.top/gtgayttwzw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtccqjxhyr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.fengsongda.top/gtbtnmarad.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xylfe.cn/gthvwjolit.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtchkgfmmw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.0kj1m.cn/gtjusockxr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jqgfzy.top/gtnhdqywrv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtycbxwwke.html

[C02] 默认参数
来源：http://hz.hnxiangtu.top/gtgnldiuyc.html

Py:   def greet(name="World"): return name
来源：http://hz.yangfankeji.com/gtmsdxdudl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhixingplan.top/gtqmsrarba.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxinkj.top/gtbzrucaqv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.birdmap.top/gtnpibeizt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.daria6918.cn/gtmdweuvny.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gogol.net.cn/gtyurbsvgo.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhixingplan.top/gtwalcvayp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ybcxt.top/gtstmupthd.html

[C03] 可变参数
来源：http://hz.jqgufenzy.top/gtalgleihi.html

Py:   def total(*args): return sum(args)
来源：http://hz.quarkkingdee.top/gtnzmrrszm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sweek.top/gtybearpol.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenjidiqi.icu/gtqxxwlldz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtlzflxvlg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xingfuxueyuan.xyz/gtvpfkqmau.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhongyouzk.top/gtqtcklxee.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.andypj.xyz/gtivikzglt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.redwolf501.top/gtxpravwmn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hammf.cn/gtxqgbaaye.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinyuanbaomall.cn/gtbteotsld.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.nwbrower.top/gtysssvvkn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.smart0.xyz/gtauhmqffd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.vqdsnc.cn/gtdjhjepex.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.svipenyu.cn/gtqyxmwaxz.html

Go:   // 无：用配置结构体参数
来源：http://hz.hnqzz.top/gtkametyiw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhongyouzk.top/gtzunnsqoy.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtrtbodwsg.html

[C05] 返回多个值
来源：http://hz.0kj1m.cn/gtnztcgtyj.html

Py:   return a, b
来源：http://hz.cdnleiting.top/gtzimqxoxr.html

PHP:  return [$a, $b];
来源：http://hz.iojbl.cn/gtfsufgaix.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jiagoushi.top/gtxtbvwdaz.html

TS:   return { a, b };
来源：http://hz.dashuyun.cn/gtqulbtfgg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.wangshuangyany.cn/gtwgfvxxru.html

Go:   return a, b
来源：http://hz.cdnleiting.top/gttpdsfzrq.html

Ruby: return a, b
来源：http://hz.yvedp.cn/gtjenkmkrs.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinqigufen.top/gtvkvwfhlb.html

[C06] 匿名函数 / lambda
来源：http://hz.daria6918.cn/gtkjaesxpt.html

Py:   square = lambda x: x * x
来源：http://hz.zhaomingkeji.xyz/gtuuqwmbft.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.daria6918.cn/gtimjtkzax.html

JS:   const square = x => x * x;
来源：http://hz.ppjwa.cn/gtstgoyfei.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.nanxuanxn.top/gtlbqnuavd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hysaishi.cn/gtvdcdiewy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinqigufen.top/gtzdqdauej.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jiagoushi.top/gtrdweecem.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.haohaochexian.top/gtqokllypn.html

[C07] 把函数作为参数传入
来源：http://hz.pycfn.com/gtxlvfmbva.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gaohongyu789.top/gtnlfnrimz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cucudq.cn/gtfaztjwqq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hnqzz.top/gtdsxphpni.html

TS:   arr.map(String)
来源：http://hz.shuidangran.top/gtyyopmffm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.guowangkeji.top/gtynammyib.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.316326.xyz/gtdqobgmnm.html

Ruby: arr.map(&:upcase)
来源：http://hz.xuetiantiany.cn/gtracmeupn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gzhubu.top/gturrwdvez.html

[C08] 闭包
来源：http://hz.sufxvd.cn/gtljohormd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.chenjidiqi.icu/gtgfmheqlr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yuxming.cn/gtrmaeomte.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gthvsqyhca.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sufxvd.cn/gtoaueltmb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hnxiangtu.top/gtiomyhrxj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jiagoushi.top/gtrgbjgfzi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinghuilouyu.cn/gtaoljxdpl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtfmacuxwu.html

[C09] 递归
来源：http://hz.kuanghao11.cn/gtiuzxqvgg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.0kj1m.cn/gtnaweupqe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenzaomai.com/gtphdintzd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hammf.cn/gtgylgvnmc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigufen.top/gtobbrfsvg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenlongwang.top/gtyysrldpm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhongyouzk.top/gtnrlkahpk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.bjfxy.top/gtroulnvgj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.pycfn.com/gtzyhvoooa.html

[C10] 变量作用域
来源：http://hz.nwbrower.top/gtlwlgtvyf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydzc1.top/gtvayoihkr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangdashe.top/gtfotimcvs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangshuangyany.cn/gtcmwrlgaf.html

TS:   同 JS
来源：http://hz.iojbl.cn/gtrftjyiup.html

Java: 方法内为块级作用域
来源：http://hz.yj20258.top/gtwkctzxmq.html

Go:   花括号块级作用域
来源：http://hz.guannengcc.top/gtaoqalffu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.52xcode.cn/gtxsjvbibm.html

C#:   块级作用域
来源：http://hz.xziqi.cn/gtyhxudzix.html

[C11] 模块导入与导出
来源：http://hz.meibo888.top/gtfwbqdxbv.html

Py:   from module import func
来源：http://hz.zhixingplan.top/gtvflxbtvn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhixingplan.top/gtumesheni.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.feifeiyinyue.top/gtovhqlpgf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.316326.xyz/gtjhuicfle.html

Java: import java.util.List;
来源：http://hz.0kj1m.cn/gtvofbamby.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sufxvd.cn/gtxoxkqpis.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zycfv.cn/gtqxplgfrk.html

C#:   using System.Text;
来源：http://hz.hnxiangtu.top/gtjtatxnwt.html

[C12] 立即执行函数 IIFE
来源：http://hz.bjfxy.top/gtwntclpnf.html

Py:   (lambda: print("run"))()
来源：http://hz.pycfn.com/gtrynecsxe.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hammf.cn/gtzppidxgu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gtvvmisiea.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gtslhbnrwi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.snrcjt.cn/gttlllurtc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sweek.top/gtcffplbmn.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinghuilouyu.cn/gtljxpyhvn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hongshengwenyu.top/gteywzxawx.html

[C13] 类型声明 / 类型注解
来源：http://hz.guowangkeji.top/gtslrgpwao.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sysykeji.top/gtqhqpmdow.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtroshmzfe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jiagoushi.top/gtjuoogkzr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigfzy.top/gtzntsdcpe.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gteqwwwvey.html

Go:   func add(a, b int) int
来源：http://hz.hysaishi.cn/gtpwzqaqui.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.andypj.xyz/gtnpvxttwm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.bjfxy.top/gtngvfixlv.html

[C14] 泛型函数
来源：http://hz.tian-w.cn/gtfcraklxm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gtrrnmpymf.html

PHP:  // 无泛型
来源：http://hz.yongpay.top/gtreqzymmt.html

JS:   // 无泛型
来源：http://hz.wangdashe.top/gtaaqphlkf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hnqzz.top/gtvyfihbws.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sweek.top/gteloylenz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.snrcjt.cn/gtghssfoqx.html

Ruby: # 无泛型
来源：http://hz.jiagoushi.top/gtwmvcaanb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.0kj1m.cn/gtsdrmoytp.html

[C15] 解构 / 展开参数
来源：http://hz.daxiang520.top/gtqnovggyf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhiwuduotai.top/gtxoeurzyo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aizwys.cn/gtddgsogep.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtdwwjdanm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.feifeiyinyue.top/gtgzoibslg.html

Java: // 无解构
来源：http://hz.shangyingyoupin.top/gtthdzpqtz.html

Go:   // 无解构
来源：http://hz.chenlongwang.top/gtyfbugsit.html

Ruby: a, b = pair
来源：http://hz.zhoulong.xyz/gtjclosfou.html

C#:   var (a, b) = pair;
来源：http://hz.yuxming.cn/gtvpmkrxdl.html

[C16] 函数 / 方法重载
来源：http://hz.jianghu66.top/gtndzmnxvb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhixingplan.top/gtyfimhzhe.html

PHP:  // 无重载
来源：http://hz.c1oappe.top/gtvyxhuype.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnqzz.top/gtxyiudmgb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jyoumei.cn/gtxdcriyfn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.birdmap.top/gtnayhjuoz.html

Go:   // 无重载：用不同函数名
来源：http://hz.yanxiufei.cn/gtcfmpxrwb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shanyushiyangkeji.top/gtsqfegbep.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sysykeji.top/gtwvjhrjwy.html

================================================================================
来源：http://hz.redwolf501.top/gthpoiiqlb.html

D. 数组 / 列表 / 集合
来源：http://hz.cqqwz.cn/gtskivmqge.html

================================================================================
来源：http://hz.zycfv.cn/gtmwveyxyi.html

[D01] 创建数组 / 列表
来源：http://hz.pengpengdd.cyou/gtzmgqzuel.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jianghu66.top/gtfbjyhtft.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ppjwa.cn/gtpohuuewf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guowangkeji.top/gtfewgndiq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hysaishi.cn/gtiyvrkhnj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhaomingkeji.xyz/gtqvquuggg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pengpengdd.cyou/gtjivvedhw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daxiang520.top/gteggaytte.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.svipenyu.cn/gttxezbhvz.html

[D02] 追加元素到末尾
来源：http://hz.yueranfly.top/gtevdiqxrn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gzhubu.top/gtmierxuzq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.dianchejie.cn/gtoptwkuce.html

JS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gtrnahdtdd.html

TS:   arr.push(4);
来源：http://hz.yj202588.top/gtnivxbgil.html

Java: list.add(4);
来源：http://hz.yj202588.top/gtwxrakehr.html

Go:   arr = append(arr, 4)
来源：http://hz.jinqigfzy.top/gtabvmlglw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ywan-chungtsiang.top/gtqevaiowq.html

C#:   list.Add(4);
来源：http://hz.hnqzz.top/gtmnsngrcv.html

[D03] 在指定位置插入元素
来源：http://hz.hywenlv.cn/gtaixcrfzs.html

Py:   arr.insert(0, 0)
来源：http://hz.ivvv.top/gtasiywxmm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yvedp.cn/gtgybvfyky.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yongpay.top/gtxgthbntm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.wangdashe.top/gtjtwoyifz.html

Java: list.add(0, 0);
来源：http://hz.tanke756.top/gtuhzhbapd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yangfankeji.com/gtunelfgno.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aizwys.cn/gtareepfwi.html

C#:   list.Insert(0, 0);
来源：http://hz.xziqi.cn/gtucyqvwuv.html

[D04] 删除元素
来源：http://hz.birdmap.top/gtwmbhbeau.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinyuanbaomall.cn/gtsovpaxzo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj202588.top/gtihchjpgh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guowangkeji.top/gtgajaohhw.html

TS:   arr.splice(0, 1);
来源：http://hz.jqgufenzy.top/gtlvwypalm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.haohaochexian.top/gtaxtpplsf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yangfankeji.com/gtktbitayx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.daxiang520.top/gtlnhwvbnc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhixingplan.top/gtbxchlpij.html

[D05] 访问与修改元素
来源：http://hz.iojbl.cn/gtkkuparis.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtylarfsag.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ivvv.top/gtrlszokyi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuanzhike.top/gtqhqdzxzq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangtech.top/gttfxygaom.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.kuanghao11.cn/gtpeedpbzo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.dianchejie.cn/gtigsbqbzy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.svipenyu.cn/gtkclldtkc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.quarkkingdee.top/gtrymzbzyn.html

[D06] 数组长度
来源：http://hz.nwbrower.top/gtsphacdav.html

Py:   len(arr)
来源：http://hz.chenjidiqi.icu/gtxoebvvra.html

PHP:  count($arr);
来源：http://hz.cqqwz.cn/gtctswmhaq.html

JS:   arr.length
来源：http://hz.smart0.xyz/gtzejqrrey.html

TS:   arr.length
来源：http://hz.yj202588.top/gtbikfosqg.html

Java: list.size();
来源：http://hz.chenjidiqi.icu/gtxjemqewf.html

Go:   len(arr)
来源：http://hz.hfpthk.cn/gttduovzzk.html

Ruby: arr.length; arr.size
来源：http://hz.yuanzhike.top/gthaouvagy.html

C#:   list.Count;
来源：http://hz.yueranfly.top/gtpncblcyr.html

[D07] 切片 / 取子数组
来源：http://hz.cqqwz.cn/gtchqkjcjn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinyuanbaomall.cn/gtnaafqkfd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cdnleiting.top/gteepliojg.html

JS:   arr.slice(1, 4);
来源：http://hz.pengpengdd.cyou/gtlsiewjhm.html

TS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtredbqyhh.html

Java: list.subList(1, 4);
来源：http://hz.xuanzx.com/gtuodtpvpp.html

Go:   arr[1:4]
来源：http://hz.svipenyu.cn/gtsmbnwzfl.html

Ruby: arr[1, 3]
来源：http://hz.tian-w.cn/gttdzagdfo.html

C#:   list.GetRange(1, 3);
来源：http://hz.cashguo.top/gtoexbqoax.html

[D08] 合并两个数组
来源：http://hz.sweek.top/gtqxlakpsa.html

Py:   a + b;  a.extend(b)
来源：http://hz.cqqwz.cn/gtoijxusia.html

PHP:  array_merge($a, $b);
来源：http://hz.andypj.xyz/gtjbuwrcbl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.snrcjt.cn/gttpscdyng.html

TS:   [...a, ...b];
来源：http://hz.chenjidiqi.icu/gtdpylbzjv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.guannengcc.top/gtwdynegif.html

Go:   append(a, b...)
来源：http://hz.gotoacloud.top/gtmvruxmkr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.52xcode.cn/gtuvmxvroo.html

C#:   a.Concat(b).ToList()
来源：http://hz.svipenyu.cn/gtnsfjaslr.html

[D09] 排序（升序）
来源：http://hz.zhaomingkeji.xyz/gtnfwrtgzl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cashguo.top/gtxijtvtzi.html

PHP:  sort($arr);
来源：http://hz.shanyushiyangtech.top/gtmefqigwl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.smart0.xyz/gtexxpejox.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhixingplan.top/gttekcpted.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhoulong.xyz/gtdwqrteza.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yangfankeji.com/gtnzscdtxq.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtbkusighd.html

C#:   list.Sort();
来源：http://hz.yangfankeji.com/gtgbyetkza.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ywan-chungtsiang.top/gtrcfiomwq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.dashuyun.cn/gtkpqjaimy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yanxiufei.cn/gtprnaodqs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sweek.top/gtzfjvwkdy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigfzy.top/gthydotzmb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jlsjyb.cn/gtngsbzocf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhoulong.xyz/gtdhxysnww.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tianlin.xyz/gtnioefpez.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fzhhl.top/gtkussspeu.html

[D11] 反转数组
来源：http://hz.yanxiufei.cn/gtrnaovbvg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cheryme.top/gtwrdpzazm.html

PHP:  array_reverse($arr);
来源：http://hz.svipenyu.cn/gtxqztxeip.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hywenlv.cn/gtulizzomx.html

TS:   [...arr].reverse();
来源：http://hz.meibo888.top/gtwpkxydoj.html

Java: Collections.reverse(list);
来源：http://hz.tianlin.xyz/gtzjkvfbxb.html

Go:   slices.Reverse(arr)
来源：http://hz.pycfn.com/gthkdwduzb.html

Ruby: arr.reverse
来源：http://hz.yangfankeji.com/gtiusvblrw.html

C#:   list.Reverse();
来源：http://hz.aizwys.cn/gtbsejhvmt.html

[D12] 查找元素下标
来源：http://hz.jinghuilouyu.cn/gtfvwypvvn.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhijiandao.cn/gtmqdbqqfj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinyuanbaomall.cn/gtuzuopiin.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gthprrfjxx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gtnyttbjxi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhixingplan.top/gtlgrdhmgr.html

Go:   slices.Index(arr, x)
来源：http://hz.hywenlv.cn/gtvrpqhasz.html

Ruby: arr.index(x)
来源：http://hz.gaohongyu789.top/gtpbwphdti.html

C#:   list.IndexOf(x);
来源：http://hz.ydjk.org.cn/gthautjvnv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jianghu66.top/gtrwjroyyj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yueranfly.top/gtfbckfuic.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.dianchejie.cn/gtkaimwkpo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jiagoushi.top/gtgmqvalac.html

TS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtnwtfocxd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yangfankeji.com/gtjxigryqf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.smart0.xyz/gtbyexyrgk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gtxujpgiiq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinqigufen.top/gtzvkfahoz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.havefunace.top/gtnjthsdup.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shanyushiyangtech.top/gtrxggtsxr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tianlin.xyz/gtpkarholl.html

JS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtmzuqxjab.html

TS:   arr.map(x => x * 2)
来源：http://hz.jiagoushi.top/gtgmgeugfp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hnqzz.top/gtcufscqks.html

Go:   // 手写循环
来源：http://hz.xinyue.icu/gtkhkrsnyd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenzaomai.com/gtvbfxfave.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgfzy.top/gtyetbonot.html

[D15] 去重
来源：http://hz.0kj1m.cn/gtbrcvhguo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gaohongyu789.top/gtqbsmbvsh.html

PHP:  array_unique($arr);
来源：http://hz.bjfxy.top/gtpwzaacse.html

JS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtuzxchbwc.html

TS:   [...new Set(arr)]
来源：http://hz.hnxiangtu.top/gtrdnprkqd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ybcxt.top/gtpsitsczz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ywan-chungtsiang.top/gtymdkrwds.html

Ruby: arr.uniq
来源：http://hz.xziqi.cn/gtmeufoyrv.html

C#:   list.Distinct().ToList()
来源：http://hz.gotoacloud.top/gtcnoqnnjt.html

[D16] 求和与平均值
来源：http://hz.fzhhl.top/gtefxwrwre.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.birdmap.top/gtxktoabzh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tanke756.top/gthyryshvr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtrvlcvxsd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtvvrdjmry.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gogol.net.cn/gtpudzrutv.html

Go:   // 手写循环累加
来源：http://hz.316326.xyz/gtgpughifm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxinkj.top/gtzidffimr.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinyuanbaomall.cn/gthynpjexw.html

[D17] 最大值与最小值
来源：http://hz.tianlin.xyz/gtrlwwclbn.html

Py:   max(arr);  min(arr)
来源：http://hz.quarkkingdee.top/gtclashhtj.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258.top/gtlofqdtql.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.havefunace.top/gtpvjcwrdz.html

TS:   Math.max(...arr);
来源：http://hz.guowangkeji.top/gtjmyhgjkn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cqqwz.cn/gtdmpkjend.html


<!-- 参考信息 -->