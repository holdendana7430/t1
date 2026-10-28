代发 wailian999

================================================================================
来源：http://hz.cdnleiting.top/gtieqktfgi.html

C. 函数与作用域
来源：http://hz.ivvv.top/gtqopczrvu.html

================================================================================
来源：http://hz.c1oappe.top/gtuqgokgdv.html

[C01] 定义函数
来源：http://hz.yvedp.cn/gtradfqouq.html

Py:   def add(a, b): return a + b
来源：http://hz.svipenyu.cn/gtltxqgmtv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtvjhjofgt.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cqqwz.cn/gtjbwrxztz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenzaomai.com/gthbllinou.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gtququdyun.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zycfv.cn/gtdcjwwrzm.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xuetiantiany.cn/gtttxaqrgp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtukyxenhy.html

[C02] 默认参数
来源：http://hz.sufxvd.cn/gtiexcnuyq.html

Py:   def greet(name="World"): return name
来源：http://hz.sysykeji.top/gtqezmlxcd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dianchejie.cn/gtpahthlzk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jqgufenzy.top/gtooyijzpy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtztkqfoxq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xziqi.cn/gtrklqnryr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sysykeji.top/gtmddutqbr.html

Ruby: def greet(name = "World") = name
来源：http://hz.hywenlv.cn/gtrquwuafe.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangkeji.top/gtttolesfn.html

[C03] 可变参数
来源：http://hz.wangdashe.top/gthhjhsftu.html

Py:   def total(*args): return sum(args)
来源：http://hz.xingfuxueyuan.xyz/gtasjnkava.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jqgfzy.top/gthxxzhdsl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangdashe.top/gtbyzrxwup.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shzxlz.cn/gtxnozivcj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yuxming.cn/gtzmzkoskm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.svipenyu.cn/gtkxjbcnao.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sweek.top/gtubjudhkc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtktcphfkx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shanyushiyangtech.top/gtagiqrqsc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xylfe.cn/gtywmcwimf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ywan-chungtsiang.top/gtukhdnfrz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jqgfzy.top/gtkzaryuai.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sufxvd.cn/gtdkuazvwo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhiwuduotai.top/gthhyophxr.html

Go:   // 无：用配置结构体参数
来源：http://hz.0kj1m.cn/gtvbelcgth.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gthnukydyd.html

C#:   f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtmydmzcoc.html

[C05] 返回多个值
来源：http://hz.52xcode.cn/gtqeijuoro.html

Py:   return a, b
来源：http://hz.guannengcc.top/gtgyeensmt.html

PHP:  return [$a, $b];
来源：http://hz.shzxlz.cn/gtwdygdvry.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zycfv.cn/gtagdbrfsc.html

TS:   return { a, b };
来源：http://hz.svipenyu.cn/gtbsoivswq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhoulong.xyz/gtevpftzvj.html

Go:   return a, b
来源：http://hz.andypj.xyz/gtalytgmcy.html

Ruby: return a, b
来源：http://hz.zhoulong.xyz/gtklqdujoy.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sufxvd.cn/gteoyukulv.html

[C06] 匿名函数 / lambda
来源：http://hz.hfpthk.cn/gtmrsjwkmn.html

Py:   square = lambda x: x * x
来源：http://hz.yanxiufei.cn/gtgptbjhdo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.fzhhl.top/gtkzxzlbin.html

JS:   const square = x => x * x;
来源：http://hz.chenlongwang.top/gtmxbtnzwg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xylfe.cn/gtirowtefq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhiwuduotai.top/gtpuvwibyj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.aizwys.cn/gttesfziik.html

Ruby: square = ->(x) { x * x }
来源：http://hz.snrcjt.cn/gtbmxahgfg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.redwolf501.top/gtgjmedjga.html

[C07] 把函数作为参数传入
来源：http://hz.chenlongwang.top/gtlgxiwflp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.316326.xyz/gtdcbnkppp.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.wangdashe.top/gtctdqpnoi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yanxiufei.cn/gthahqbdjl.html

TS:   arr.map(String)
来源：http://hz.0kj1m.cn/gtxnkwhbzm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhijiandao.cn/gtlubrjdmk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jqgufenzy.top/gtvvvrncxc.html

Ruby: arr.map(&:upcase)
来源：http://hz.jinqigfzy.top/gttooxabfr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhoulong.xyz/gtlbupwpuu.html

[C08] 闭包
来源：http://hz.zhiwuduotai.top/gtwgnwjxdm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hysaishi.cn/gtfjbeieaa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhiwuduotai.top/gtfpjrgtzq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gtykxuwvay.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.vqdsnc.cn/gtsxnhasnq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ivvv.top/gthqgfvvja.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yueranfly.top/gtmynklskq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydzc1.top/gtgqzcwyfe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xylfe.cn/gtfxodwhwf.html

[C09] 递归
来源：http://hz.guannengcc.top/gthdwxycpv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.kuanghao11.cn/gtkjsmizvo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.9152youxi.cn/gtdmgmztpr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgfzy.top/gtbfqtszgm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258888.top/gtgexwdxrw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.nanxuanxn.top/gtgggttcmh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zdqjudy.top/gtmicpioxl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.nanxuanxn.top/gtnzkstjkq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zdqjudy.top/gtzwxhtwke.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtaxcpisdo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xuetiantiany.cn/gthzsjsawn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.snrcjt.cn/gtkqsuzglb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jianghu66.top/gtjtqqrvzj.html

TS:   同 JS
来源：http://hz.quarkkingdee.top/gttvhfbcgr.html

Java: 方法内为块级作用域
来源：http://hz.iojbl.cn/gtyeywsevx.html

Go:   花括号块级作用域
来源：http://hz.chenzaomai.com/gtndayppsz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ehwqpu.com/gtxwwwlrnc.html

C#:   块级作用域
来源：http://hz.chenlongwang.top/gtxcnwnrqn.html

[C11] 模块导入与导出
来源：http://hz.gaohongyu789.top/gtfjduwcwn.html

Py:   from module import func
来源：http://hz.yanxiufei.cn/gtymshvyfc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.havefunace.top/gttipyfyiy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.quarkkingdee.top/gtlvvoawzw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gogol.net.cn/gtqxylnpub.html

Java: import java.util.List;
来源：http://hz.hfpthk.cn/gtajwatlen.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.fzhhl.top/gtxnqwhekt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cheryme.top/gtjhiweuxw.html

C#:   using System.Text;
来源：http://hz.daria6918.cn/gtoxoowfjz.html

[C12] 立即执行函数 IIFE
来源：http://hz.gaohongyu789.top/gtnzbygeow.html

Py:   (lambda: print("run"))()
来源：http://hz.zhaomingkeji.xyz/gtnbbmcryh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xuanzx.com/gtqpusxfuf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gtjxvaqaon.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tanke756.top/gtrvmpyzos.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhiwuduotai.top/gtrxwusqsk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aibaodan.cn/gtjfwkoikd.html

Ruby: -> { puts "run" }.call
来源：http://hz.gzhubu.top/gtamupapdl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pycfn.com/gtospyifxa.html

[C13] 类型声明 / 类型注解
来源：http://hz.yvedp.cn/gtbwcrjwnd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangdashe.top/gtcnwcblgw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gthprrpjjo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ywan-chungtsiang.top/gtrycuhjqp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.meibo888.top/gtngzgpbch.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sxryk.cn/gtjgehaeeb.html

Go:   func add(a, b int) int
来源：http://hz.aibaodan.cn/gtxourygws.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ehwqpu.com/gteflkgfpj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.316326.xyz/gtxgpyploa.html

[C14] 泛型函数
来源：http://hz.guannengcc.top/gtsgrgqjcx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.meibo888.top/gtaenyvehp.html

PHP:  // 无泛型
来源：http://hz.tanke756.top/gtixncorxu.html

JS:   // 无泛型
来源：http://hz.hnxiangtu.top/gtcpygvaad.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xingfuxueyuan.xyz/gtuwbxdrjx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.havefunace.top/gtiiiajzyn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jinghuilouyu.cn/gtybhhtysa.html

Ruby: # 无泛型
来源：http://hz.dianchejie.cn/gthuhppfww.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aizwys.cn/gtnitntqnm.html

[C15] 解构 / 展开参数
来源：http://hz.ehwqpu.com/gtergbatwu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgfzy.top/gteutokdbg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenzaomai.com/gtbwzsrxcx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jyoumei.cn/gtzgsndxqz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ywan-chungtsiang.top/gtvvxaqpsw.html

Java: // 无解构
来源：http://hz.jyoumei.cn/gtwqferxrp.html

Go:   // 无解构
来源：http://hz.yonumen.top/gtzxkrcznt.html

Ruby: a, b = pair
来源：http://hz.cashguo.top/gtnzxwsyhk.html

C#:   var (a, b) = pair;
来源：http://hz.fengsongda.top/gtlrjxnfnn.html

[C16] 函数 / 方法重载
来源：http://hz.aizwys.cn/gtwkuljoya.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhoulong.xyz/gtqwdmdsal.html

PHP:  // 无重载
来源：http://hz.vqdsnc.cn/gtcbljlroc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gotoacloud.top/gtdhgprrsq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yanxiufei.cn/gtsprtfhwx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhiwuduotai.top/gtqexkqaet.html

Go:   // 无重载：用不同函数名
来源：http://hz.ivvv.top/gtyhtrobek.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yanxiufei.cn/gtrqkrgzxq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cdnleiting.top/gthsjrlaqw.html

================================================================================
来源：http://hz.smart0.xyz/gtctmqufuy.html

D. 数组 / 列表 / 集合
来源：http://hz.hfpthk.cn/gtdxwtxhpj.html

================================================================================
来源：http://hz.jlsjyb.cn/gtysolilvh.html

[D01] 创建数组 / 列表
来源：http://hz.ppjwa.cn/gtoptnyjtc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhoulong.xyz/gtmnnxfepl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhoulong.xyz/gtsbjxmrqi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aibaodan.cn/gtfgaaxgki.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.52xcode.cn/gtsiypcldz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shuidangran.top/gtuzxwdhuo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj20258888.top/gtoybbevkw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nwbrower.top/gtyfjgqyul.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.haohaochexian.top/gtvslgslwt.html

[D02] 追加元素到末尾
来源：http://hz.yangfankeji.com/gttamingwa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gzhubu.top/gtcsewalko.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.quarkkingdee.top/gthoadhpkz.html

JS:   arr.push(4);
来源：http://hz.yueranfly.top/gtrxrzegpn.html

TS:   arr.push(4);
来源：http://hz.redwolf501.top/gtpxawuepd.html

Java: list.add(4);
来源：http://hz.jqgfzy.top/gtsawpdtny.html

Go:   arr = append(arr, 4)
来源：http://hz.xuanzx.com/gtthfjxcgo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zdqjudy.top/gtivbawuqz.html

C#:   list.Add(4);
来源：http://hz.vqdsnc.cn/gtolnibgxo.html

[D03] 在指定位置插入元素
来源：http://hz.cucudq.cn/gtgvdtkwxl.html

Py:   arr.insert(0, 0)
来源：http://hz.redwolf501.top/gttugnfdbm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhixingplan.top/gtxxkmvpfo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.andypj.xyz/gtcuohukpu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.vqdsnc.cn/gtdyojpece.html

Java: list.add(0, 0);
来源：http://hz.gotoacloud.top/gtxtgtjsre.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yueranfly.top/gtnnxltsyt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.feifeiyinyue.top/gtmyykjdph.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtamtrkrfl.html

[D04] 删除元素
来源：http://hz.sufxvd.cn/gtczpkuzxs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.havefunace.top/gtjezmprta.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gogol.net.cn/gtqsinqhvs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ywan-chungtsiang.top/gtcjgyilww.html

TS:   arr.splice(0, 1);
来源：http://hz.svipenyu.cn/gtcmruzuck.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tianlin.xyz/gtgfehbayt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.birdmap.top/gtesuvrjht.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shuidangran.top/gtqbfiyuoo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.vqdsnc.cn/gtudqaaypk.html

[D05] 访问与修改元素
来源：http://hz.meibo888.top/gthmqhxout.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenjidiqi.icu/gtehjhskvs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.haohaochexian.top/gtfzzzysgs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ivvv.top/gtcbsydehn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gtmtwnbazl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhoulong.xyz/gtksxsqbtp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.redwolf501.top/gtfynivbip.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtnujzcclb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yueranfly.top/gtaseukixi.html

[D06] 数组长度
来源：http://hz.meibo888.top/gtfwlodvli.html

Py:   len(arr)
来源：http://hz.zhengqikj.top/gthydfdvya.html

PHP:  count($arr);
来源：http://hz.zhongyouzk.top/gtbfrfqeal.html

JS:   arr.length
来源：http://hz.cqqwz.cn/gtfpwazpsd.html

TS:   arr.length
来源：http://hz.nanxinkj.top/gtviuwswzc.html

Java: list.size();
来源：http://hz.hongshengwenyu.top/gtintxcels.html

Go:   len(arr)
来源：http://hz.aibaodan.cn/gteztmgqhs.html

Ruby: arr.length; arr.size
来源：http://hz.nanxuanxn.top/gtpqaptlll.html

C#:   list.Count;
来源：http://hz.xinyue.icu/gtangwqddd.html

[D07] 切片 / 取子数组
来源：http://hz.bjfxy.top/gtdoxjxoej.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sysykeji.top/gtvszavged.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xinyue.icu/gtwzidoqso.html

JS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gtmhcqjlqm.html

TS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtvwgkceug.html

Java: list.subList(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtdqmkzrsi.html

Go:   arr[1:4]
来源：http://hz.nanxinkj.top/gtgnvbtgro.html

Ruby: arr[1, 3]
来源：http://hz.svipenyu.cn/gtiusunshp.html

C#:   list.GetRange(1, 3);
来源：http://hz.haohaochexian.top/gtutftqlrt.html

[D08] 合并两个数组
来源：http://hz.bjfxy.top/gtacencduo.html

Py:   a + b;  a.extend(b)
来源：http://hz.sufxvd.cn/gtosevalze.html

PHP:  array_merge($a, $b);
来源：http://hz.birdmap.top/gtothnguay.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cdnleiting.top/gtujhoydaa.html

TS:   [...a, ...b];
来源：http://hz.aizwys.cn/gttiyuojmu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinyuanbaomall.cn/gtuntdrbti.html

Go:   append(a, b...)
来源：http://hz.zdqjudy.top/gtkxndcyem.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yuanzhike.top/gtqqswzyfn.html

C#:   a.Concat(b).ToList()
来源：http://hz.gaohongyu789.top/gtsywqiptg.html

[D09] 排序（升序）
来源：http://hz.yvedp.cn/gtybpshhnt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hammf.cn/gtzfopwgfg.html

PHP:  sort($arr);
来源：http://hz.0kj1m.cn/gtyixawkhq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgufenzy.top/gtesftnstz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.smart0.xyz/gtcowikkjl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gaohongyu789.top/gtvikdwjrn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangtech.top/gtiirvynyv.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gtrxqkvjnb.html

C#:   list.Sort();
来源：http://hz.pycfn.com/gtviubyxmt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.birdmap.top/gtnqtchbah.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jyoumei.cn/gtvlxgydkr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydzc1.top/gtyxrnobfz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hammf.cn/gtofnzpdza.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tianlin.xyz/gtrikpnwez.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tanke756.top/gtllepynhv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shzxlz.cn/gtykzeehuc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cheryme.top/gtbsderito.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinyuanbaomall.cn/gtnstrwbfj.html

[D11] 反转数组
来源：http://hz.xingfuxueyuan.xyz/gtrtqhkgqb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sysykeji.top/gthsqgzmpv.html

PHP:  array_reverse($arr);
来源：http://hz.shuidangran.top/gtwyqrrvle.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shuidangran.top/gtvkldlrez.html

TS:   [...arr].reverse();
来源：http://hz.haohaochexian.top/gtxahxaooy.html

Java: Collections.reverse(list);
来源：http://hz.jlsjyb.cn/gtjkgculeh.html

Go:   slices.Reverse(arr)
来源：http://hz.iojbl.cn/gtzovzjxes.html

Ruby: arr.reverse
来源：http://hz.vqdsnc.cn/gtcjzyiobc.html

C#:   list.Reverse();
来源：http://hz.jianghu66.top/gtgllnqnla.html

[D12] 查找元素下标
来源：http://hz.c1oappe.top/gtivzcfbed.html

Py:   arr.index(x);  x in arr
来源：http://hz.hnqzz.top/gtplbukkia.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgfzy.top/gtpuwwwerp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydzc1.top/gtkjxprleo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.9152youxi.cn/gtuajlyegz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ywan-chungtsiang.top/gtygclacsy.html

Go:   slices.Index(arr, x)
来源：http://hz.dianchejie.cn/gtzgzafwks.html

Ruby: arr.index(x)
来源：http://hz.zhongyouzk.top/gtytoerdxp.html

C#:   list.IndexOf(x);
来源：http://hz.yueranfly.top/gthzezpewk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangdashe.top/gtuntkwnin.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.quarkkingdee.top/gtodlfhqyy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhiwuduotai.top/gtfaiskfjm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cdnleiting.top/gtrkzftqzh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtgnyczkst.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jlsjyb.cn/gtxelewchl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jianghu66.top/gtxqbgajvu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.quarkkingdee.top/gtkdwrlxly.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinqigufen.top/gtryqwsver.html

[D14] 映射转换（每个元素变形）
来源：http://hz.0kj1m.cn/gttgqixssy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gzhubu.top/gtoiiwxeiv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangshuangyany.cn/gtaquvaofq.html

JS:   arr.map(x => x * 2)
来源：http://hz.zycfv.cn/gtcywveynp.html

TS:   arr.map(x => x * 2)
来源：http://hz.jqgufenzy.top/gtxmfbihzd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xuetiantiany.cn/gtytnwlxty.html

Go:   // 手写循环
来源：http://hz.birdmap.top/gtagtsmcka.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xuetiantiany.cn/gtfersstzk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.redwolf501.top/gtcioerphl.html

[D15] 去重
来源：http://hz.gzhubu.top/gtjdgwutmw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.feifeiyinyue.top/gtuhnrrzpv.html

PHP:  array_unique($arr);
来源：http://hz.ydjk.org.cn/gtfftnevrt.html

JS:   [...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtqkakeoew.html

TS:   [...new Set(arr)]
来源：http://hz.shzxlz.cn/gtcdtxdabv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xinyue.icu/gtuzcxonrp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xylfe.cn/gtudvblxiq.html

Ruby: arr.uniq
来源：http://hz.chenzaomai.com/gtpcrtxlgo.html

C#:   list.Distinct().ToList()
来源：http://hz.gzhubu.top/gtvvcuotsj.html

[D16] 求和与平均值
来源：http://hz.fzhhl.top/gtbcdnvule.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cdnleiting.top/gtowvyhyvb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.svipenyu.cn/gtposdvzwy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhoulong.xyz/gtodtsqkkb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtjndzyszv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yonumen.top/gtjjcghjhh.html

Go:   // 手写循环累加
来源：http://hz.daxiang520.top/gtegwapoas.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinqigufen.top/gtnatllzpw.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhixingplan.top/gtfohabetr.html

[D17] 最大值与最小值
来源：http://hz.sufxvd.cn/gtvvyvicyz.html

Py:   max(arr);  min(arr)
来源：http://hz.chenzaomai.com/gttbkbwjvt.html

PHP:  max($arr);  min($arr);
来源：http://hz.cheryme.top/gtqnqrtzgn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.snrcjt.cn/gtijaodcho.html

TS:   Math.max(...arr);
来源：http://hz.sxryk.cn/gtmixnwqvg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ydjk.org.cn/gtkoqrbuib.html


<!-- 参考信息 -->