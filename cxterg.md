代发 wailian999

Go:   a && b || !c
来源：http://hz.xziqi.cn/gtmzzdwunz.html

Ruby: a && b || !c
来源：http://hz.xuanzx.com/gtkquwqpyn.html

C#:   a && b || !c
来源：http://hz.ppjwa.cn/gtfbscebye.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yj20258888.top/gtcalvzooe.html

Py:   if not data: return
来源：http://hz.ydjk.org.cn/gtqfwkovcm.html

PHP:  if (!$data) { return; }
来源：http://hz.ehwqpu.com/gthgrikfkx.html

JS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtiwpfjxtr.html

TS:   if (!data) return;
来源：http://hz.yonumen.top/gtbodbuqwa.html

Java: if (data == null) return;
来源：http://hz.daria6918.cn/gtyuvgtmah.html

Go:   if data == nil { return }
来源：http://hz.vqdsnc.cn/gtoagszhkx.html

Ruby: return if data.nil?
来源：http://hz.316326.xyz/gtmgdihqnl.html

C#:   if (data == null) return;
来源：http://hz.gaohongyu789.top/gtkofipibx.html

================================================================================
来源：http://hz.0kj1m.cn/gtgkbddfwa.html

C. 函数与作用域
来源：http://hz.chenzaomai.com/gtlnpuidgh.html

================================================================================
来源：http://hz.andypj.xyz/gttplinvck.html

[C01] 定义函数
来源：http://hz.aizwys.cn/gtldrorfts.html

Py:   def add(a, b): return a + b
来源：http://hz.hysaishi.cn/gtyhuurmtp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sweek.top/gtjmvlmkkn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenzaomai.com/gtynicdskz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dianchejie.cn/gtldtousfi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gtcskcahbf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daria6918.cn/gtwitjtuzg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jqgfzy.top/gtsilolnft.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtmilrzqvl.html

[C02] 默认参数
来源：http://hz.ehwqpu.com/gtcvccoxdb.html

Py:   def greet(name="World"): return name
来源：http://hz.zhoulong.xyz/gthqrjowcr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nanxuanxn.top/gtolcbsadd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shangyingyoupin.top/gtyqwsqkvc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yongpay.top/gtrzpcvkhc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shzxlz.cn/gtlsuvpuul.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhaomingkeji.xyz/gtmygknkbi.html

Ruby: def greet(name = "World") = name
来源：http://hz.ydzc1.top/gtpfwwkdkh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinqigfzy.top/gtwosjzatp.html

[C03] 可变参数
来源：http://hz.guannengcc.top/gtyzfktaja.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258.top/gtesmyvuhe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hysaishi.cn/gtksydxpdh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xylfe.cn/gtvhvevruy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yanxiufei.cn/gtfzvgpnuc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shanyushiyangkeji.top/gtyhoqslvu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.fzhhl.top/gtgakpsoiz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.52xcode.cn/gtnlrlwuyu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.iojbl.cn/gtqyqbcuij.html

[C04] 命名参数 / 关键字参数
来源：http://hz.dashuyun.cn/gtypimrkbo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.gogol.net.cn/gtdyhlhwel.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.kuanghao11.cn/gtlkhstxzm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtkrgnwhoy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.pycfn.com/gtuxiccyye.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shanyushiyangtech.top/gtebmxavtj.html

Go:   // 无：用配置结构体参数
来源：http://hz.tian-w.cn/gtlmnhsbiu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtqslbyibj.html

C#:   f(a: 1, b: 2)
来源：http://hz.sweek.top/gtbfcgmukq.html

[C05] 返回多个值
来源：http://hz.zhengqikj.top/gtnvzcripl.html

Py:   return a, b
来源：http://hz.xuanzx.com/gtoboxnwpr.html

PHP:  return [$a, $b];
来源：http://hz.dianchejie.cn/gtclhplgra.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yonumen.top/gtyuwvxzzg.html

TS:   return { a, b };
来源：http://hz.guowangkeji.top/gthltfjlpt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gotoacloud.top/gtfwzdigro.html

Go:   return a, b
来源：http://hz.fzhhl.top/gturbxwejy.html

Ruby: return a, b
来源：http://hz.jinqigufen.top/gtdtfbpnag.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.mhx1999.top/gtbyuxbxgk.html

[C06] 匿名函数 / lambda
来源：http://hz.tanke756.top/gtjcgqmfdz.html

Py:   square = lambda x: x * x
来源：http://hz.aibaodan.cn/gtdrdkximg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cqqwz.cn/gtrkllpmdz.html

JS:   const square = x => x * x;
来源：http://hz.xuetiantiany.cn/gtjmjuqjac.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.nanxinkj.top/gtnotfstxj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sxryk.cn/gtkontgntz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nwbrower.top/gtbmevoygm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.smart0.xyz/gticbygzps.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.birdmap.top/gtyguoijyu.html

[C07] 把函数作为参数传入
来源：http://hz.aibaodan.cn/gthnqbwpzy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pycfn.com/gtvbpgqcbw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.snrcjt.cn/gtmzuwruat.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sysykeji.top/gtauidcomu.html

TS:   arr.map(String)
来源：http://hz.zhongyouzk.top/gtmmzqjdtp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hysaishi.cn/gtboqwrjwp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.bjfxy.top/gtdpskblki.html

Ruby: arr.map(&:upcase)
来源：http://hz.gaohongyu789.top/gthjswgmje.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ywan-chungtsiang.top/gtcweydiov.html

[C08] 闭包
来源：http://hz.sysykeji.top/gtronkumef.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ehwqpu.com/gtwhxkfqds.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xingfuxueyuan.xyz/gtbyzlejyx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtifiymgbz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gtewiidsle.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shuidangran.top/gtepfsjrja.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gotoacloud.top/gtqpvilabr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhaomingkeji.xyz/gtcltisrhy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtvvxrfvce.html

[C09] 递归
来源：http://hz.kuanghao11.cn/gtpbgukszo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.9152youxi.cn/gtddzparyj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gotoacloud.top/gttbxdzkhi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhijiandao.cn/gtlolqlukn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yanxiufei.cn/gtpiunhqoh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xylfe.cn/gtimoozirq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yueranfly.top/gtmjheadqm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.52xcode.cn/gtiadysmjn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxuanxn.top/gthbpxbqim.html

[C10] 变量作用域
来源：http://hz.nanxuanxn.top/gtlhbwwxux.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ivvv.top/gtrxazmjsi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jyoumei.cn/gtmgcwkeyz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xylfe.cn/gtwtwscldv.html

TS:   同 JS
来源：http://hz.xuetiantiany.cn/gtfmonsbgh.html

Java: 方法内为块级作用域
来源：http://hz.meibo888.top/gttwfldrxb.html

Go:   花括号块级作用域
来源：http://hz.gzhubu.top/gtvlmflhbj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yangfankeji.com/gtcatxhjlp.html

C#:   块级作用域
来源：http://hz.yj20258.top/gtzqoeprzx.html

[C11] 模块导入与导出
来源：http://hz.feifeiyinyue.top/gtmmvqqrmm.html

Py:   from module import func
来源：http://hz.fengsongda.top/gthogdjxnx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hongshengwenyu.top/gtbxdodpgn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cashguo.top/gtqazacsof.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.smart0.xyz/gtbybfqppo.html

Java: import java.util.List;
来源：http://hz.kuanghao11.cn/gtnrusvife.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinghuilouyu.cn/gtdbbgflbs.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sufxvd.cn/gtfdodzrgb.html

C#:   using System.Text;
来源：http://hz.yuanzhike.top/gtdrhbnkys.html

[C12] 立即执行函数 IIFE
来源：http://hz.fengsongda.top/gtzsukaqlj.html

Py:   (lambda: print("run"))()
来源：http://hz.nwbrower.top/gtpzbixjfn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yanxiufei.cn/gteqgxjbpm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtdftkcllb.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gtdharkhyd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hysaishi.cn/gtjhgsdhtf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxinkj.top/gtcqnwgizf.html

Ruby: -> { puts "run" }.call
来源：http://hz.kuanghao11.cn/gtdlkqrkxx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.316326.xyz/gtlbzjtoii.html

[C13] 类型声明 / 类型注解
来源：http://hz.wangshuangyany.cn/gtdvdvtvjj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.dianchejie.cn/gtkpbjenmb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gtowlhmasd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dianchejie.cn/gtkpwiafzr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtrqgiecpu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.guannengcc.top/gtjobndmid.html

Go:   func add(a, b int) int
来源：http://hz.dashuyun.cn/gtolqbclhp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinghuilouyu.cn/gtvpgwsdzw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhengqikj.top/gttrjwlmml.html

[C14] 泛型函数
来源：http://hz.0kj1m.cn/gtrllyzbke.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.pengpengdd.cyou/gthwrphxob.html

PHP:  // 无泛型
来源：http://hz.sysykeji.top/gttnrqwswd.html

JS:   // 无泛型
来源：http://hz.chenlongwang.top/gtbanbysda.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shzxlz.cn/gtnsoloqzg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cucudq.cn/gtexltnbzx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.0kj1m.cn/gttgmkyviq.html

Ruby: # 无泛型
来源：http://hz.jlsjyb.cn/gtfsxsjqgf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.nanxinkj.top/gtfrkhpsse.html

[C15] 解构 / 展开参数
来源：http://hz.hywenlv.cn/gtfcaxprns.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sysykeji.top/gtsyvgjcjy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.redwolf501.top/gtvtndatkd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.fengsongda.top/gtalcpazpy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cqqwz.cn/gtwcpywdpq.html

Java: // 无解构
来源：http://hz.iojbl.cn/gtcaxczxao.html

Go:   // 无解构
来源：http://hz.sweek.top/gtccbyfipc.html

Ruby: a, b = pair
来源：http://hz.nanxuanxn.top/gtrpcxogdv.html

C#:   var (a, b) = pair;
来源：http://hz.ybcxt.top/gtjgerqdor.html

[C16] 函数 / 方法重载
来源：http://hz.0kj1m.cn/gtybbtrotg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fengsongda.top/gtakhwhspn.html

PHP:  // 无重载
来源：http://hz.shanyushiyangtech.top/gtyyusheir.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gotoacloud.top/gtmdvzcolg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.quarkkingdee.top/gtlmzkukoc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gogol.net.cn/gtchqfngrg.html

Go:   // 无重载：用不同函数名
来源：http://hz.ywan-chungtsiang.top/gtchaselwx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xziqi.cn/gtepdagucc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ppjwa.cn/gtpfcwqrqu.html

================================================================================
来源：http://hz.52xcode.cn/gtbccvyovt.html

D. 数组 / 列表 / 集合
来源：http://hz.tian-w.cn/gtxzjgkpep.html

================================================================================
来源：http://hz.svipenyu.cn/gtvvwgojgb.html

[D01] 创建数组 / 列表
来源：http://hz.jianghu66.top/gtxtoubbox.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnxiangtu.top/gtccpfgcsw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenlongwang.top/gtjioxtxbg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.kuanghao11.cn/gtxwsiozcn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shzxlz.cn/gtfezonfxp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxuanxn.top/gtfzmninaa.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zycfv.cn/gtuiuggkos.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhaomingkeji.xyz/gtaydzcoxj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zdqjudy.top/gtdhvfwpet.html

[D02] 追加元素到末尾
来源：http://hz.xuetiantiany.cn/gtaihglvcs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.guowangkeji.top/gtfcpsmflu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.daxiang520.top/gtrmvvexhr.html

JS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtdilizwiw.html

TS:   arr.push(4);
来源：http://hz.quarkkingdee.top/gtanpuwtoa.html

Java: list.add(4);
来源：http://hz.jianghu66.top/gthnlcznkt.html

Go:   arr = append(arr, 4)
来源：http://hz.bjfxy.top/gtfvyivbag.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.vqdsnc.cn/gtdxsywhle.html

C#:   list.Add(4);
来源：http://hz.wangshuangyany.cn/gtmdtkncjl.html

[D03] 在指定位置插入元素
来源：http://hz.sufxvd.cn/gtvijpuoqq.html

Py:   arr.insert(0, 0)
来源：http://hz.yj20258888.top/gtnnojbzxh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhiwuduotai.top/gtgggrtavx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nanxinkj.top/gtvcjbxxya.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jiagoushi.top/gttakpimum.html

Java: list.add(0, 0);
来源：http://hz.hysaishi.cn/gtvnnibnao.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yanxiufei.cn/gtlgughbmn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sxryk.cn/gtfalwjbui.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258888.top/gtjyjuuerp.html

[D04] 删除元素
来源：http://hz.jianghu66.top/gtfarugwok.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.kuanghao11.cn/gtkwhbcahb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj20258888.top/gtxptwgsbc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenlongwang.top/gtdpolxjfk.html

TS:   arr.splice(0, 1);
来源：http://hz.jinghuilouyu.cn/gtxozywqmv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxuanxn.top/gttvlktmvi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ydjk.org.cn/gtzwaoladc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.dashuyun.cn/gtsrrgyyir.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yuxming.cn/gtszextcci.html

[D05] 访问与修改元素
来源：http://hz.zhoulong.xyz/gthlkczjqu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtckvthwmj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigufen.top/gtkqucohvc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cucudq.cn/gtfpirvvru.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ydjk.org.cn/gtbkxdbumc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shuidangran.top/gtkkoylbzc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guannengcc.top/gtsbyrajdq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtrcbvgekk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yonumen.top/gtyohrctjy.html

[D06] 数组长度
来源：http://hz.wangshuangyany.cn/gtouoaukhu.html

Py:   len(arr)
来源：http://hz.aizwys.cn/gtfbzqotpf.html

PHP:  count($arr);
来源：http://hz.jiagoushi.top/gtkbtyfscm.html

JS:   arr.length
来源：http://hz.jyoumei.cn/gtxkkbhgbb.html

TS:   arr.length
来源：http://hz.sweek.top/gtbgrvcxxe.html

Java: list.size();
来源：http://hz.shangyingyoupin.top/gtqqsbfaqf.html

Go:   len(arr)
来源：http://hz.fengsongda.top/gthjyhvjul.html

Ruby: arr.length; arr.size
来源：http://hz.yanxiufei.cn/gtxxsrelxv.html

C#:   list.Count;
来源：http://hz.hongshengwenyu.top/gtyiqufywq.html

[D07] 切片 / 取子数组
来源：http://hz.tian-w.cn/gtutqlxioy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shzxlz.cn/gtevwkefik.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.316326.xyz/gtjhbkdzdz.html

JS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtfiburcnm.html

TS:   arr.slice(1, 4);
来源：http://hz.redwolf501.top/gtrngucgxi.html

Java: list.subList(1, 4);
来源：http://hz.ydjk.org.cn/gtpbzlmfyl.html

Go:   arr[1:4]
来源：http://hz.daria6918.cn/gtshktflbl.html

Ruby: arr[1, 3]
来源：http://hz.haohaochexian.top/gtgbyezfbf.html

C#:   list.GetRange(1, 3);
来源：http://hz.ppjwa.cn/gtuapnvoek.html

[D08] 合并两个数组
来源：http://hz.tian-w.cn/gtnmozueoe.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenjidiqi.icu/gtzrvbnryr.html

PHP:  array_merge($a, $b);
来源：http://hz.hnxiangtu.top/gthjuozzut.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.fengsongda.top/gtnkhxwjfm.html

TS:   [...a, ...b];
来源：http://hz.zhixingplan.top/gturiffach.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xylfe.cn/gtqkhxwqhx.html

Go:   append(a, b...)
来源：http://hz.316326.xyz/gtcotscbjs.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cheryme.top/gtdzltmpvm.html

C#:   a.Concat(b).ToList()
来源：http://hz.jiagoushi.top/gtgbzbxtde.html

[D09] 排序（升序）
来源：http://hz.jyoumei.cn/gtlvethoyi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtkzetnfzk.html

PHP:  sort($arr);
来源：http://hz.zhengqikj.top/gtbaxzqjak.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jyoumei.cn/gtvflhjxge.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.c1oappe.top/gttjbptock.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.daxiang520.top/gtuwalypdc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gtclvhirky.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtunpcpaef.html

C#:   list.Sort();
来源：http://hz.yvedp.cn/gtqltbowpn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj202588.top/gtgxjkwyiz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jlsjyb.cn/gtimwlqzeo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.smart0.xyz/gtkjeqopao.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtaeetsgif.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fengsongda.top/gtgpsowrdy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.andypj.xyz/gtfaeshvui.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigfzy.top/gtwlxazxzs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cucudq.cn/gtjhianatk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.quarkkingdee.top/gtlcccctqo.html

[D11] 反转数组
来源：http://hz.gzhubu.top/gtlxmiamuf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.pengpengdd.cyou/gttbkekumh.html

PHP:  array_reverse($arr);
来源：http://hz.cdnleiting.top/gtttideasb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258888.top/gtcfbsrikf.html

TS:   [...arr].reverse();
来源：http://hz.sysykeji.top/gthycodlbu.html

Java: Collections.reverse(list);
来源：http://hz.iojbl.cn/gtnenzcmya.html

Go:   slices.Reverse(arr)
来源：http://hz.hongshengwenyu.top/gtymdcvbxk.html

Ruby: arr.reverse
来源：http://hz.hfpthk.cn/gthitbzcqc.html

C#:   list.Reverse();
来源：http://hz.hammf.cn/gtkpkfpkel.html

[D12] 查找元素下标
来源：http://hz.yj202588.top/gtgipcsccb.html

Py:   arr.index(x);  x in arr
来源：http://hz.yuanzhike.top/gttihpsemr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.feifeiyinyue.top/gtikxntlqd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dianchejie.cn/gtrxdgnntm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ybcxt.top/gtsikmvmfm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuetiantiany.cn/gtnabhjayw.html

Go:   slices.Index(arr, x)
来源：http://hz.snrcjt.cn/gtpkwdxicl.html

Ruby: arr.index(x)
来源：http://hz.yanxiufei.cn/gtenduaolw.html

C#:   list.IndexOf(x);
来源：http://hz.meibo888.top/gtqczudkij.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hysaishi.cn/gtxkxfvitm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.snrcjt.cn/gtsleisape.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shanyushiyangtech.top/gtrjnrjfdv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtwyenaisf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cdnleiting.top/gtvjlkacss.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.guowangkeji.top/gtonneahtn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.c1oappe.top/gttytlfiuj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ywan-chungtsiang.top/gtiouamvma.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yonumen.top/gtcfxkdluv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jqgfzy.top/gtikjswllz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.9152youxi.cn/gtgsffmicq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jqgfzy.top/gtdhvxexws.html

JS:   arr.map(x => x * 2)
来源：http://hz.yueranfly.top/gtlvcgodwa.html

TS:   arr.map(x => x * 2)
来源：http://hz.gzhubu.top/gtrjqsptwj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cqqwz.cn/gtvcfombqt.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtvptlanna.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.fzhhl.top/gtlppejcti.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gotoacloud.top/gtasalpbgc.html

[D15] 去重
来源：http://hz.smart0.xyz/gtggijduvc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinghuilouyu.cn/gtftmjmopb.html

PHP:  array_unique($arr);
来源：http://hz.xuetiantiany.cn/gtpqolisex.html

JS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtamdxffkc.html

TS:   [...new Set(arr)]
来源：http://hz.pycfn.com/gtisspgvhc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jlsjyb.cn/gtlgbjevny.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pengpengdd.cyou/gtyrlldhup.html

Ruby: arr.uniq
来源：http://hz.yangfankeji.com/gtjcpalhiu.html

C#:   list.Distinct().ToList()
来源：http://hz.dianchejie.cn/gtkixxyybf.html

[D16] 求和与平均值
来源：http://hz.zhixingplan.top/gtarniibqv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ehwqpu.com/gtdczuctos.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tanke756.top/gtwmsfixgu.html


<!-- 参考信息 -->