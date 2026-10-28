代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gtzmqwsyke.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guannengcc.top/gtkgkmgkgr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinyuanbaomall.cn/gtjpylizqt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gthdgwvtvk.html

[C02] 默认参数
来源：http://hz.hfpthk.cn/gtwsngtiel.html

Py:   def greet(name="World"): return name
来源：http://hz.nanxuanxn.top/gtvlzwekxa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hongshengwenyu.top/gtwwtpgqef.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinqigfzy.top/gtmcrtgixn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.fengsongda.top/gtyxglunbb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xuetiantiany.cn/gtlmudznxl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ppjwa.cn/gtuderedkv.html

Ruby: def greet(name = "World") = name
来源：http://hz.kuanghao11.cn/gtrmmdrctb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cucudq.cn/gtbqzyiwkf.html

[C03] 可变参数
来源：http://hz.ywan-chungtsiang.top/gtcczfazgg.html

Py:   def total(*args): return sum(args)
来源：http://hz.hywenlv.cn/gtejmohgeu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhiwuduotai.top/gtkmwazzlv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangshuangyany.cn/gtzancljxo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sxryk.cn/gtmdjwzipe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.andypj.xyz/gtkklsbsfj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yonumen.top/gtdbppumqd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhixingplan.top/gtoogcsokf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cashguo.top/gtrjvgzlxi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.52xcode.cn/gtlvgvjqng.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinqigufen.top/gtnvyyifds.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinghuilouyu.cn/gtsrbparnr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hongshengwenyu.top/gtvjqcqgaw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.316326.xyz/gtyjekfzoz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shangyingyoupin.top/gtdtsqbcfv.html

Go:   // 无：用配置结构体参数
来源：http://hz.hfpthk.cn/gtgnilumnl.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtnlxynhir.html

C#:   f(a: 1, b: 2)
来源：http://hz.daxiang520.top/gtqkwbhvoq.html

[C05] 返回多个值
来源：http://hz.andypj.xyz/gtaynopzeh.html

Py:   return a, b
来源：http://hz.chenzaomai.com/gtxktaiwha.html

PHP:  return [$a, $b];
来源：http://hz.yueranfly.top/gtpedgcyxf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.svipenyu.cn/gtzcdrcnmq.html

TS:   return { a, b };
来源：http://hz.yanxiufei.cn/gtudevhlor.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhoulong.xyz/gtcbffmcdj.html

Go:   return a, b
来源：http://hz.sysykeji.top/gtomtyfyhp.html

Ruby: return a, b
来源：http://hz.jinyuanbaomall.cn/gtxrwfpkbp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnqzz.top/gtzulcvhck.html

[C06] 匿名函数 / lambda
来源：http://hz.tianlin.xyz/gthgktkcms.html

Py:   square = lambda x: x * x
来源：http://hz.nwbrower.top/gtvktvaqch.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ybcxt.top/gtqqatkvlq.html

JS:   const square = x => x * x;
来源：http://hz.ppjwa.cn/gtmuwpzmwv.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jianghu66.top/gtjejpanjr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhijiandao.cn/gtmjamsqgb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jiagoushi.top/gtwtaioxfa.html

Ruby: square = ->(x) { x * x }
来源：http://hz.c1oappe.top/gtoxekyrhc.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.mhx1999.top/gtgjvlrulc.html

[C07] 把函数作为参数传入
来源：http://hz.zhixingplan.top/gtbwqzrmxz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenlongwang.top/gtsgvizfwr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.aibaodan.cn/gtdfojlkmk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yvedp.cn/gtbvyqqjwx.html

TS:   arr.map(String)
来源：http://hz.c1oappe.top/gtyczsgnmk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hfpthk.cn/gtjsmdookq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hysaishi.cn/gtfaxjofke.html

Ruby: arr.map(&:upcase)
来源：http://hz.xuetiantiany.cn/gtzrytwryr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtmwwzkbpj.html

[C08] 闭包
来源：http://hz.gogol.net.cn/gtizzkafml.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cucudq.cn/gtvnsqihlg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.snrcjt.cn/gtbdwmanpc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtfmgfmywr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinghuilouyu.cn/gtirxlxmjw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yuanzhike.top/gtwazmplni.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tian-w.cn/gtnsxyjwtk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangtech.top/gtohqxqfbi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj202588.top/gtosgoiegi.html

[C09] 递归
来源：http://hz.ydzc1.top/gtjiinhqtd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.guannengcc.top/gtdsrvdhdf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.daxiang520.top/gtatyjkvvh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gtqnhzmtho.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.redwolf501.top/gtfxychzxx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhoulong.xyz/gtohulliqu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.iojbl.cn/gtqfaaihbx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtvapsaqte.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yj202588.top/gtvacavvge.html

[C10] 变量作用域
来源：http://hz.316326.xyz/gtbkzjmktv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenlongwang.top/gtaqaoxnrk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yongpay.top/gtdwackbrm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.smart0.xyz/gtyfrnyejc.html

TS:   同 JS
来源：http://hz.shanyushiyangkeji.top/gtnlujfmaj.html

Java: 方法内为块级作用域
来源：http://hz.316326.xyz/gtjbbfdjgo.html

Go:   花括号块级作用域
来源：http://hz.9152youxi.cn/gtootovrtn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zdqjudy.top/gtzfuybkhg.html

C#:   块级作用域
来源：http://hz.316326.xyz/gtuojfcdwi.html

[C11] 模块导入与导出
来源：http://hz.ehwqpu.com/gtbzzjdfeh.html

Py:   from module import func
来源：http://hz.gogol.net.cn/gtfhwvyukf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ybcxt.top/gtotwnymrb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cheryme.top/gtmmrrqeqg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.haohaochexian.top/gtwkkpenlf.html

Java: import java.util.List;
来源：http://hz.pengpengdd.cyou/gtibowthhw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinghuilouyu.cn/gtjprjpxye.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.tian-w.cn/gteiwkurjo.html

C#:   using System.Text;
来源：http://hz.zhaomingkeji.xyz/gtkxbqwddn.html

[C12] 立即执行函数 IIFE
来源：http://hz.vqdsnc.cn/gtommlwhwc.html

Py:   (lambda: print("run"))()
来源：http://hz.havefunace.top/gtlazipvwz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.redwolf501.top/gtkqbumdla.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hfpthk.cn/gtqzelnobf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jqgfzy.top/gtuckkdies.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xingfuxueyuan.xyz/gtwfowhwpu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xuanzx.com/gtqmahxmnt.html

Ruby: -> { puts "run" }.call
来源：http://hz.meibo888.top/gtzcngcbte.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tian-w.cn/gtukexajoc.html

[C13] 类型声明 / 类型注解
来源：http://hz.tian-w.cn/gtfldleurj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtggaphclj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xylfe.cn/gtzsihztqt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.wangdashe.top/gtpzwvbqos.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangshuangyany.cn/gtvaraakog.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gtpcitftud.html

Go:   func add(a, b int) int
来源：http://hz.chenjidiqi.icu/gtdfgeqznj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.c1oappe.top/gtzylczbdf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.c1oappe.top/gtfoogskiz.html

[C14] 泛型函数
来源：http://hz.andypj.xyz/gtfxdhyqfd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yuxming.cn/gtakqxwhno.html

PHP:  // 无泛型
来源：http://hz.dianchejie.cn/gtugeqpwtd.html

JS:   // 无泛型
来源：http://hz.guowangkeji.top/gtdinzzoyq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hnqzz.top/gtogixvbaa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zdqjudy.top/gtzmxamkxu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jiagoushi.top/gtdxhmurji.html

Ruby: # 无泛型
来源：http://hz.birdmap.top/gtlcjraygn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ybcxt.top/gtyggnyvkt.html

[C15] 解构 / 展开参数
来源：http://hz.shangyingyoupin.top/gtidikmhni.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.birdmap.top/gtdguyotdb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yangfankeji.com/gtmwcyevtj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.andypj.xyz/gtketoxhad.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj20258888.top/gtfrfwfbos.html

Java: // 无解构
来源：http://hz.bjfxy.top/gtmzizsqmv.html

Go:   // 无解构
来源：http://hz.snrcjt.cn/gtbmwdzksp.html

Ruby: a, b = pair
来源：http://hz.aizwys.cn/gtxvawhqwu.html

C#:   var (a, b) = pair;
来源：http://hz.sxryk.cn/gtmevmbyhe.html

[C16] 函数 / 方法重载
来源：http://hz.daria6918.cn/gtwbgmutqi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gotoacloud.top/gtyjcwvrsl.html

PHP:  // 无重载
来源：http://hz.zhixingplan.top/gtmlxyzzuu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yongpay.top/gtwputjnog.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.0kj1m.cn/gtefixkqqq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ywan-chungtsiang.top/gtqjtvtriy.html

Go:   // 无重载：用不同函数名
来源：http://hz.andypj.xyz/gtswbzfwkf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cdnleiting.top/gtcieltitq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xinyue.icu/gtyioaqlho.html

================================================================================
来源：http://hz.sufxvd.cn/gtytrjiujw.html

D. 数组 / 列表 / 集合
来源：http://hz.xinyue.icu/gtguhhhdky.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqvieevht.html

[D01] 创建数组 / 列表
来源：http://hz.nwbrower.top/gtytovrolj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.redwolf501.top/gtdtjdppxn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.bjfxy.top/gteiitgosx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hysaishi.cn/gthjqbamos.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shanyushiyangtech.top/gtyndckqmy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gaohongyu789.top/gtuoravcks.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinqigufen.top/gtfhnsdvbf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.redwolf501.top/gtndxcdwit.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pycfn.com/gtdrutvdds.html

[D02] 追加元素到末尾
来源：http://hz.andypj.xyz/gtlzbynxsd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shangyingyoupin.top/gtogyrzjeh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ivvv.top/gtdedspxlq.html

JS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtlprspjrs.html

TS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtilsuyros.html

Java: list.add(4);
来源：http://hz.xylfe.cn/gtqhkwtwor.html

Go:   arr = append(arr, 4)
来源：http://hz.jinyuanbaomall.cn/gtzupdrzmt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xylfe.cn/gtpvqkrtsp.html

C#:   list.Add(4);
来源：http://hz.meibo888.top/gtftgiclfs.html

[D03] 在指定位置插入元素
来源：http://hz.jyoumei.cn/gtehmhesoh.html

Py:   arr.insert(0, 0)
来源：http://hz.sxryk.cn/gtevjfrqxv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.c1oappe.top/gtqsobxvwe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.quarkkingdee.top/gtkhtngarw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gotoacloud.top/gtpqpziusv.html

Java: list.add(0, 0);
来源：http://hz.hywenlv.cn/gtillijdma.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenjidiqi.icu/gtgscnayiq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shuidangran.top/gtpftcodsu.html

C#:   list.Insert(0, 0);
来源：http://hz.xuetiantiany.cn/gtwhjzlulj.html

[D04] 删除元素
来源：http://hz.hnxiangtu.top/gtykfvcyjr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ehwqpu.com/gtyaqjicmo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhengqikj.top/gtsrqiiqjf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zdqjudy.top/gtzbmbucyn.html

TS:   arr.splice(0, 1);
来源：http://hz.xylfe.cn/gtrjztenwg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.kuanghao11.cn/gttrwtraad.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.aizwys.cn/gttlpxlilm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jqgufenzy.top/gthehtqohq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yvedp.cn/gtialkhwbu.html

[D05] 访问与修改元素
来源：http://hz.shzxlz.cn/gtkfghffwq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtwgjfhcgy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yvedp.cn/gtvrqkdhzp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shuidangran.top/gtpijsyxlu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yueranfly.top/gtdbyqrzni.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.birdmap.top/gtwbexbvza.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.wangshuangyany.cn/gtuphrlrwu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtdxdfxlll.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhongyouzk.top/gtlbxghyrl.html

[D06] 数组长度
来源：http://hz.ehwqpu.com/gtmnpuenem.html

Py:   len(arr)
来源：http://hz.ehwqpu.com/gtsextkaic.html

PHP:  count($arr);
来源：http://hz.pycfn.com/gtmtprgicq.html

JS:   arr.length
来源：http://hz.cheryme.top/gthlwphret.html

TS:   arr.length
来源：http://hz.jiagoushi.top/gtgdfyojgy.html

Java: list.size();
来源：http://hz.sweek.top/gtivdmtvri.html

Go:   len(arr)
来源：http://hz.iojbl.cn/gtglslyeix.html

Ruby: arr.length; arr.size
来源：http://hz.ehwqpu.com/gttwgtgaco.html

C#:   list.Count;
来源：http://hz.316326.xyz/gtigzqktim.html

[D07] 切片 / 取子数组
来源：http://hz.guannengcc.top/gtzlfwwujd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhengqikj.top/gtqtnwkuvz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xuanzx.com/gtqycfjkto.html

JS:   arr.slice(1, 4);
来源：http://hz.yvedp.cn/gtbzypqmbp.html

TS:   arr.slice(1, 4);
来源：http://hz.chenjidiqi.icu/gtkeqebuwv.html

Java: list.subList(1, 4);
来源：http://hz.jinghuilouyu.cn/gtkdbookub.html

Go:   arr[1:4]
来源：http://hz.zhixingplan.top/gtwzewcsvz.html

Ruby: arr[1, 3]
来源：http://hz.hywenlv.cn/gtsvpqmjph.html

C#:   list.GetRange(1, 3);
来源：http://hz.cqqwz.cn/gtjetljbby.html

[D08] 合并两个数组
来源：http://hz.chenzaomai.com/gtbeutwvjq.html

Py:   a + b;  a.extend(b)
来源：http://hz.xuetiantiany.cn/gtylmkmqzk.html

PHP:  array_merge($a, $b);
来源：http://hz.316326.xyz/gtmmliwlse.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.vqdsnc.cn/gtxdaiqkdv.html

TS:   [...a, ...b];
来源：http://hz.iojbl.cn/gtbqmpbgvn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.dashuyun.cn/gtgimsmezz.html

Go:   append(a, b...)
来源：http://hz.sufxvd.cn/gtjqbocqmu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yongpay.top/gtlvvcdjot.html

C#:   a.Concat(b).ToList()
来源：http://hz.daxiang520.top/gtptvkgaff.html

[D09] 排序（升序）
来源：http://hz.hnxiangtu.top/gtnvfuksrd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtgsrwhwwt.html

PHP:  sort($arr);
来源：http://hz.tianlin.xyz/gthoiunart.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.quarkkingdee.top/gtfdqjstwb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tian-w.cn/gtavhhdyoi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ydjk.org.cn/gtyazybvlw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtrhgheizx.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtsedbhgrx.html

C#:   list.Sort();
来源：http://hz.shangyingyoupin.top/gtmyeeegek.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhengqikj.top/gtkbetgyty.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nanxuanxn.top/gtxzfsmmcu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hongshengwenyu.top/gtblrflpdr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhengqikj.top/gtsozxqwbt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ppjwa.cn/gtecbhhjyk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xuanzx.com/gtedfokcqc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jyoumei.cn/gtzpvxycbx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jianghu66.top/gtwtvbnkxg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cashguo.top/gtrezmalay.html

[D11] 反转数组
来源：http://hz.fzhhl.top/gtbjimkgeb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.quarkkingdee.top/gtgpuidgob.html

PHP:  array_reverse($arr);
来源：http://hz.wangshuangyany.cn/gtvikujgdu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gaohongyu789.top/gtildwxshr.html

TS:   [...arr].reverse();
来源：http://hz.dashuyun.cn/gtbznvqqfc.html

Java: Collections.reverse(list);
来源：http://hz.redwolf501.top/gtitonqzfp.html

Go:   slices.Reverse(arr)
来源：http://hz.shanyushiyangkeji.top/gtakizcenf.html

Ruby: arr.reverse
来源：http://hz.xinyue.icu/gtifouzvdw.html

C#:   list.Reverse();
来源：http://hz.sweek.top/gtamqhhmlp.html

[D12] 查找元素下标
来源：http://hz.yanxiufei.cn/gtbyeeqodo.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinqigfzy.top/gtllcwtbep.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.fengsongda.top/gtgbbmegyx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtevbcqbor.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aizwys.cn/gtpidaafmk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ivvv.top/gttiwjpvck.html

Go:   slices.Index(arr, x)
来源：http://hz.ehwqpu.com/gtwhnjhebt.html

Ruby: arr.index(x)
来源：http://hz.hammf.cn/gtgqmnfpry.html

C#:   list.IndexOf(x);
来源：http://hz.yueranfly.top/gtebnrdddv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.aibaodan.cn/gtmxjhalpo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yangfankeji.com/gtjgrxcjwt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.0kj1m.cn/gtjkuwrsxv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtqbcpstck.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtcyjsaypk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aizwys.cn/gtdfusewyq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.dashuyun.cn/gtnmtaqjuq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gotoacloud.top/gtvdgtipuh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinqigufen.top/gtalekooyx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yangfankeji.com/gtpixbacnb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinghuilouyu.cn/gthbluooet.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jqgufenzy.top/gtfqttcxiz.html

JS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gtmzkcruye.html

TS:   arr.map(x => x * 2)
来源：http://hz.jlsjyb.cn/gteyheofyh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhoulong.xyz/gtykfgdoxn.html

Go:   // 手写循环
来源：http://hz.0kj1m.cn/gtvpgbstzf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xziqi.cn/gtfpamvlyy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cucudq.cn/gtucuopbfy.html

[D15] 去重
来源：http://hz.svipenyu.cn/gtmujzlfub.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinqigufen.top/gtycfyxktb.html

PHP:  array_unique($arr);
来源：http://hz.gogol.net.cn/gtkrhuwmlb.html

JS:   [...new Set(arr)]
来源：http://hz.jinqigufen.top/gtabinrjla.html

TS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtxcasogtg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guannengcc.top/gtcwqrhuxx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xziqi.cn/gtfgysaoor.html

Ruby: arr.uniq
来源：http://hz.yangfankeji.com/gtcisyrjbu.html

C#:   list.Distinct().ToList()
来源：http://hz.yvedp.cn/gtpskacxzp.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangkeji.top/gtohdsvxld.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydjk.org.cn/gtbltsgnkx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tanke756.top/gtbqukfcgf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sysykeji.top/gtlluwvcxs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtpvjbexpq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuanzx.com/gtilpwfubj.html

Go:   // 手写循环累加
来源：http://hz.jqgfzy.top/gttyrcelsp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.iojbl.cn/gtobvrtcbp.html

C#:   list.Sum();  list.Average()
来源：http://hz.dianchejie.cn/gtnffgtyqr.html

[D17] 最大值与最小值
来源：http://hz.birdmap.top/gtjydzitem.html

Py:   max(arr);  min(arr)
来源：http://hz.redwolf501.top/gtaixonbhm.html

PHP:  max($arr);  min($arr);
来源：http://hz.guowangkeji.top/gtvlsgybgv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cheryme.top/gtzfywlrqm.html

TS:   Math.max(...arr);
来源：http://hz.iojbl.cn/gtcoajsjeu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtwpnnmplh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.pycfn.com/gtbcraftxk.html

Ruby: arr.max;  arr.min
来源：http://hz.xuanzx.com/gtrlnmikqb.html

C#:   list.Max();  list.Min()
来源：http://hz.yonumen.top/gtnertpoex.html

[D18] 扁平化嵌套数组
来源：http://hz.shuidangran.top/gtnpqjhcqj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gotoacloud.top/gtjwfsnjzh.html

PHP:  array_merge(...$nested);
来源：http://hz.nanxinkj.top/gtdcnfxtof.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.chenjidiqi.icu/gtxvzmiadx.html

TS:   nested.flat();
来源：http://hz.yvedp.cn/gtvtlwfmmd.html


<!-- 参考信息 -->