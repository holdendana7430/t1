代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtyabgnsrv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daxiang520.top/gtaesspgej.html

Ruby: def add(a, b); a + b; end
来源：http://hz.nanxinkj.top/gtcixyikun.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gthldaqsju.html

[C02] 默认参数
来源：http://hz.chenjidiqi.icu/gtcwvmkajq.html

Py:   def greet(name="World"): return name
来源：http://hz.cucudq.cn/gtxpptzbkn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tianlin.xyz/gtnzjrlyva.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.0kj1m.cn/gtavgcinsd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhongyouzk.top/gtwaqyfjdd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj20258.top/gtdvjpkrhf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yongpay.top/gtrdaaoofp.html

Ruby: def greet(name = "World") = name
来源：http://hz.9152youxi.cn/gttpsdfkgu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hongshengwenyu.top/gtqeyuwgpo.html

[C03] 可变参数
来源：http://hz.sufxvd.cn/gtbucgmgxq.html

Py:   def total(*args): return sum(args)
来源：http://hz.52xcode.cn/gtaqkojiry.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.snrcjt.cn/gttjzssibz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuxming.cn/gtgwpqphcf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.mhx1999.top/gtulgpvmun.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jyoumei.cn/gtddkpxvhv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yangfankeji.com/gtidkofhpv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhengqikj.top/gtwexjgukv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jianghu66.top/gtbxbsjdmv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sysykeji.top/gttwpcnyfp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ybcxt.top/gtmrdvjbpg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.dianchejie.cn/gtfaqvylcg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.svipenyu.cn/gtyyxqjlyv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.0kj1m.cn/gtatifmzkn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xingfuxueyuan.xyz/gtzevsdtvq.html

Go:   // 无：用配置结构体参数
来源：http://hz.yonumen.top/gtulgnaejf.html

Ruby: f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtfqhxwevq.html

C#:   f(a: 1, b: 2)
来源：http://hz.quarkkingdee.top/gtfxyrdxqo.html

[C05] 返回多个值
来源：http://hz.hywenlv.cn/gtjowtecob.html

Py:   return a, b
来源：http://hz.redwolf501.top/gtmvpgrnor.html

PHP:  return [$a, $b];
来源：http://hz.dianchejie.cn/gtewrneshp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ivvv.top/gtjhpxvpnt.html

TS:   return { a, b };
来源：http://hz.hnxiangtu.top/gtumdcklax.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xuanzx.com/gtwuizdjfj.html

Go:   return a, b
来源：http://hz.nanxuanxn.top/gtmgcfykwj.html

Ruby: return a, b
来源：http://hz.316326.xyz/gtysefxeme.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gtrkjgbwle.html

[C06] 匿名函数 / lambda
来源：http://hz.ivvv.top/gtilcqitgr.html

Py:   square = lambda x: x * x
来源：http://hz.yongpay.top/gtxmmumhvp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cdnleiting.top/gtfxiaewex.html

JS:   const square = x => x * x;
来源：http://hz.yuxming.cn/gtsfpagedn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.9152youxi.cn/gthzmtzqny.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ppjwa.cn/gtpxzyzkjn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jqgufenzy.top/gtqzsbhslv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.52xcode.cn/gtzrgifmgd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhoulong.xyz/gtnmecsznw.html

[C07] 把函数作为参数传入
来源：http://hz.meibo888.top/gtzrwecrnj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xziqi.cn/gtzewqftzv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jinqigfzy.top/gtvhhjjsyc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dianchejie.cn/gturspdaeq.html

TS:   arr.map(String)
来源：http://hz.vqdsnc.cn/gtlldcozem.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sweek.top/gtjajadtsy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yuanzhike.top/gtjltrabyn.html

Ruby: arr.map(&:upcase)
来源：http://hz.hnqzz.top/gtolzjxzgx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fengsongda.top/gtxxyraqwv.html

[C08] 闭包
来源：http://hz.hysaishi.cn/gtcjwszmyo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.birdmap.top/gttlvnjshz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258.top/gtgnhxvjkh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gttmtbwmue.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gtcuvsclqo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shanyushiyangkeji.top/gtxxtowfil.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhixingplan.top/gtiqwyzito.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.birdmap.top/gtqcvtrpnj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtxdjcnfmt.html

[C09] 递归
来源：http://hz.xuetiantiany.cn/gtcfijxiaj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.aibaodan.cn/gtyempxmjv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ehwqpu.com/gtblvviyoh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgfzy.top/gtyncjmxcw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jlsjyb.cn/gtxixpmwah.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hfpthk.cn/gtaqwxkzcz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.meibo888.top/gtodrufyag.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tianlin.xyz/gtuhforlgq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.tanke756.top/gtnkiewyyg.html

[C10] 变量作用域
来源：http://hz.sufxvd.cn/gtbnrtbycn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tian-w.cn/gtjqvporll.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhiwuduotai.top/gtkgktvfec.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.pengpengdd.cyou/gtlbiqiubf.html

TS:   同 JS
来源：http://hz.zhoulong.xyz/gtjgenvbyn.html

Java: 方法内为块级作用域
来源：http://hz.zdqjudy.top/gtxzhthbim.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangtech.top/gtjzvemoiw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhaomingkeji.xyz/gtyforcmjf.html

C#:   块级作用域
来源：http://hz.c1oappe.top/gtwandpgim.html

[C11] 模块导入与导出
来源：http://hz.smart0.xyz/gtjtqepwmu.html

Py:   from module import func
来源：http://hz.sufxvd.cn/gtpnkgxwsl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.9152youxi.cn/gttsubxyhh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnqzz.top/gtavietugj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fzhhl.top/gtvvpozfvl.html

Java: import java.util.List;
来源：http://hz.sysykeji.top/gtxnjtjmnb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.0kj1m.cn/gthqcryqyg.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.c1oappe.top/gthladdfwp.html

C#:   using System.Text;
来源：http://hz.ydjk.org.cn/gtizqlxctt.html

[C12] 立即执行函数 IIFE
来源：http://hz.sxryk.cn/gtxfmpsjql.html

Py:   (lambda: print("run"))()
来源：http://hz.xingfuxueyuan.xyz/gthhtzhmwg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nwbrower.top/gtugcrakdu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gtiylpbnzq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.316326.xyz/gtxmjrjpus.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nanxinkj.top/gtkydawtpw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.havefunace.top/gtzqzmbmjm.html

Ruby: -> { puts "run" }.call
来源：http://hz.jqgufenzy.top/gtjxlalzfi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.quarkkingdee.top/gtokqiecat.html

[C13] 类型声明 / 类型注解
来源：http://hz.ybcxt.top/gtwvvrhmfx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jqgfzy.top/gtvijobxlq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nwbrower.top/gtvlefzmau.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hysaishi.cn/gtxdysbfze.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jiagoushi.top/gtjnupyztf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtfeodrteh.html

Go:   func add(a, b int) int
来源：http://hz.meibo888.top/gtebroxook.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.kuanghao11.cn/gttxszmyzi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.kuanghao11.cn/gtmuvbftqk.html

[C14] 泛型函数
来源：http://hz.meibo888.top/gtcpnedlrx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.iojbl.cn/gtvmkudxpe.html

PHP:  // 无泛型
来源：http://hz.bjfxy.top/gtotyouyhd.html

JS:   // 无泛型
来源：http://hz.redwolf501.top/gtyglvyqpe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jlsjyb.cn/gtsvgymqna.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jqgfzy.top/gtdezcjest.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sysykeji.top/gtrtynwhuc.html

Ruby: # 无泛型
来源：http://hz.sxryk.cn/gtsfwzclpz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jyoumei.cn/gtlpovtrgw.html

[C15] 解构 / 展开参数
来源：http://hz.hfpthk.cn/gtsudojpko.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.haohaochexian.top/gtdbqnzhqj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zdqjudy.top/gtfudzbrel.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenzaomai.com/gtpxtiwosm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yuanzhike.top/gtwbhvpfgt.html

Java: // 无解构
来源：http://hz.jinyuanbaomall.cn/gtzovcsoqa.html

Go:   // 无解构
来源：http://hz.yvedp.cn/gtqgbudnyy.html

Ruby: a, b = pair
来源：http://hz.zhoulong.xyz/gtulofzbcq.html

C#:   var (a, b) = pair;
来源：http://hz.nwbrower.top/gtimicywml.html

[C16] 函数 / 方法重载
来源：http://hz.cdnleiting.top/gthxkdzjgf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.andypj.xyz/gtbniqaltx.html

PHP:  // 无重载
来源：http://hz.svipenyu.cn/gtsphdyzkx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.haohaochexian.top/gtokylqzwg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shanyushiyangkeji.top/gtybyfznvv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxuanxn.top/gtrcdltvpe.html

Go:   // 无重载：用不同函数名
来源：http://hz.wangdashe.top/gttfftklfo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhaomingkeji.xyz/gtubiigvhg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ybcxt.top/gtmsqpnasd.html

================================================================================
来源：http://hz.feifeiyinyue.top/gttdhwqvcy.html

D. 数组 / 列表 / 集合
来源：http://hz.hnxiangtu.top/gtngevsjlr.html

================================================================================
来源：http://hz.nanxinkj.top/gtaopegfsj.html

[D01] 创建数组 / 列表
来源：http://hz.gotoacloud.top/gtdggeeyxj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hywenlv.cn/gtcymzfjgz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinqigfzy.top/gtcmzrukbk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.svipenyu.cn/gtxraqoxyd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jqgufenzy.top/gtgajagxbg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuanzx.com/gtrtzihjnx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.iojbl.cn/gtpjaiyscu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cheryme.top/gtgsrsnagp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sxryk.cn/gtiukztzks.html

[D02] 追加元素到末尾
来源：http://hz.birdmap.top/gtfmonmfst.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zycfv.cn/gtaofvphsa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuetiantiany.cn/gtfarqdosq.html

JS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtjaulrokg.html

TS:   arr.push(4);
来源：http://hz.ydjk.org.cn/gtlaacaolo.html

Java: list.add(4);
来源：http://hz.cashguo.top/gtdoitjkzu.html

Go:   arr = append(arr, 4)
来源：http://hz.birdmap.top/gtnswlgxnc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhoulong.xyz/gteilaouni.html

C#:   list.Add(4);
来源：http://hz.jqgfzy.top/gtvqwdlioh.html

[D03] 在指定位置插入元素
来源：http://hz.wangdashe.top/gtollaiqsw.html

Py:   arr.insert(0, 0)
来源：http://hz.daria6918.cn/gtalwpjjqj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.havefunace.top/gtegdnwhsi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.andypj.xyz/gtizqvthfo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tianlin.xyz/gtxrhzheof.html

Java: list.add(0, 0);
来源：http://hz.daria6918.cn/gtplpiatip.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ydzc1.top/gtrkxjixvz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenjidiqi.icu/gtbgwfzbce.html

C#:   list.Insert(0, 0);
来源：http://hz.gaohongyu789.top/gtwihxjjyv.html

[D04] 删除元素
来源：http://hz.shzxlz.cn/gtnpeumegt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhengqikj.top/gtbddjryvn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gogol.net.cn/gtkairqrvz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.mhx1999.top/gtqqxudphf.html

TS:   arr.splice(0, 1);
来源：http://hz.zdqjudy.top/gtreejxetp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.c1oappe.top/gtiashcnap.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhiwuduotai.top/gtqwjsfqgl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.dianchejie.cn/gtuwrvxozu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aizwys.cn/gtgfbruedc.html

[D05] 访问与修改元素
来源：http://hz.52xcode.cn/gtqeavphqm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtvuafpfpx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hnqzz.top/gtwdosubuc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.redwolf501.top/gtefcsxgrx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.bjfxy.top/gtmdqlridg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jqgfzy.top/gtprdmpcby.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtdduknzkc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hammf.cn/gtztjebywk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aibaodan.cn/gtpmvoeazr.html

[D06] 数组长度
来源：http://hz.wangshuangyany.cn/gtqbcfnzle.html

Py:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtrxnxmjag.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gtulbtvzdt.html

JS:   arr.length
来源：http://hz.pengpengdd.cyou/gtcnpunxcs.html

TS:   arr.length
来源：http://hz.daria6918.cn/gtcwdojywo.html

Java: list.size();
来源：http://hz.yj20258888.top/gtkjtrxkxk.html

Go:   len(arr)
来源：http://hz.sufxvd.cn/gtzltkmrov.html

Ruby: arr.length; arr.size
来源：http://hz.ydjk.org.cn/gtekzqvgqf.html

C#:   list.Count;
来源：http://hz.shzxlz.cn/gtdoaybfrz.html

[D07] 切片 / 取子数组
来源：http://hz.sweek.top/gtklntvush.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yuxming.cn/gtvknqpuxj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.smart0.xyz/gtvjupisip.html

JS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtqtasoimq.html

TS:   arr.slice(1, 4);
来源：http://hz.nwbrower.top/gtnzhwdseg.html

Java: list.subList(1, 4);
来源：http://hz.hongshengwenyu.top/gtvqszkusk.html

Go:   arr[1:4]
来源：http://hz.xingfuxueyuan.xyz/gtnmwzsgyn.html

Ruby: arr[1, 3]
来源：http://hz.cucudq.cn/gttffzbmjk.html

C#:   list.GetRange(1, 3);
来源：http://hz.cqqwz.cn/gtywlkgrxh.html

[D08] 合并两个数组
来源：http://hz.guannengcc.top/gtdjcegwah.html

Py:   a + b;  a.extend(b)
来源：http://hz.vqdsnc.cn/gtbjmtfjmd.html

PHP:  array_merge($a, $b);
来源：http://hz.daria6918.cn/gtrvygkdcw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tanke756.top/gtfirbhwuv.html

TS:   [...a, ...b];
来源：http://hz.dashuyun.cn/gtlhlftljz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sxryk.cn/gtxakciyto.html

Go:   append(a, b...)
来源：http://hz.zhixingplan.top/gtuvnvhhsr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.meibo888.top/gtkstilepk.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinqigfzy.top/gtiiwncgha.html

[D09] 排序（升序）
来源：http://hz.xylfe.cn/gtgpoagkdt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtgsarfspf.html

PHP:  sort($arr);
来源：http://hz.jinyuanbaomall.cn/gtfozcwfls.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj202588.top/gtjorvedmb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.bjfxy.top/gtorfkzwht.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.guowangkeji.top/gtcyocqmsy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xinyue.icu/gtcefhufbr.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtcjlpwyus.html

C#:   list.Sort();
来源：http://hz.ydzc1.top/gtmihhycoz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daria6918.cn/gthcbzznpw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.snrcjt.cn/gtjacgxyso.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.meibo888.top/gtmylrzgdj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jqgufenzy.top/gtiiqpqpud.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yanxiufei.cn/gtwtymthyv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhiwuduotai.top/gttsuecynd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ehwqpu.com/gtnfmxauvr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yongpay.top/gtdmbnkexb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ehwqpu.com/gtpcapibfx.html

[D11] 反转数组
来源：http://hz.birdmap.top/gtlvcayjql.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.dashuyun.cn/gtjnwwdoxv.html

PHP:  array_reverse($arr);
来源：http://hz.jinyuanbaomall.cn/gtyabvjohl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.feifeiyinyue.top/gtgopdjcdo.html

TS:   [...arr].reverse();
来源：http://hz.jinyuanbaomall.cn/gtgllqrcwv.html

Java: Collections.reverse(list);
来源：http://hz.jlsjyb.cn/gtoofsbwht.html

Go:   slices.Reverse(arr)
来源：http://hz.jyoumei.cn/gtphyarehi.html

Ruby: arr.reverse
来源：http://hz.yonumen.top/gtovxmritw.html

C#:   list.Reverse();
来源：http://hz.zhijiandao.cn/gtgvlnlslj.html

[D12] 查找元素下标
来源：http://hz.ydzc1.top/gtxhsuvcys.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhijiandao.cn/gtmtcefiyz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhongyouzk.top/gtjrpisfro.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.redwolf501.top/gtbmeblrmi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gthwrckqvy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.0kj1m.cn/gtuhcgdbqd.html

Go:   slices.Index(arr, x)
来源：http://hz.bjfxy.top/gthsrlilmh.html

Ruby: arr.index(x)
来源：http://hz.jqgfzy.top/gtksdhnjfs.html

C#:   list.IndexOf(x);
来源：http://hz.jiagoushi.top/gtygnwfnsr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhaomingkeji.xyz/gtvgyzukvl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.guowangkeji.top/gtzhmrybly.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cheryme.top/gthewcupoe.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtxsleyyym.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xuetiantiany.cn/gtrgyxjfsg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.kuanghao11.cn/gtcaucgvsn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yongpay.top/gtbxfmjwud.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.mhx1999.top/gtwqeliayd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yanxiufei.cn/gtvutgzdra.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xylfe.cn/gtgqynjatg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.iojbl.cn/gtyznbbpot.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jqgufenzy.top/gttasvjzlq.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtnaxdinvp.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gteamvfdbi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangshuangyany.cn/gtgboqmltt.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gtypmnaiyz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cheryme.top/gtlxvntitq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.redwolf501.top/gtrrltdwnh.html

[D15] 去重
来源：http://hz.redwolf501.top/gtxdubgkcc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnxiangtu.top/gtqwsarkld.html

PHP:  array_unique($arr);
来源：http://hz.feifeiyinyue.top/gttbmxnaoo.html

JS:   [...new Set(arr)]
来源：http://hz.xinyue.icu/gtbamrmuuw.html

TS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gthrymncok.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cashguo.top/gtxvadzwhm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yuxming.cn/gtwzgiwcdl.html

Ruby: arr.uniq
来源：http://hz.yueranfly.top/gtmxsmfveq.html

C#:   list.Distinct().ToList()
来源：http://hz.yangfankeji.com/gtsbujwplc.html

[D16] 求和与平均值
来源：http://hz.yongpay.top/gtechpidpd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuanzhike.top/gtdlgicqct.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.mhx1999.top/gtrlzkyvtn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fzhhl.top/gtueshxuim.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cheryme.top/gtwzimaluz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.pengpengdd.cyou/gtvohoizuz.html

Go:   // 手写循环累加
来源：http://hz.shuidangran.top/gtcrvmagme.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shangyingyoupin.top/gtkjrhkxnt.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhiwuduotai.top/gteyssiwlo.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gtlfwfzfsp.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtnvicyvgh.html

PHP:  max($arr);  min($arr);
来源：http://hz.xylfe.cn/gtqcbfaubr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhijiandao.cn/gtsoxppffg.html

TS:   Math.max(...arr);
来源：http://hz.gzhubu.top/gtzdfrpyko.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jiagoushi.top/gtecithzjz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tanke756.top/gtlvvrnxip.html

Ruby: arr.max;  arr.min
来源：http://hz.zhongyouzk.top/gtpfzznwcu.html

C#:   list.Max();  list.Min()
来源：http://hz.cdnleiting.top/gtyhwprxkw.html

[D18] 扁平化嵌套数组
来源：http://hz.tian-w.cn/gtcqipsfak.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jinqigufen.top/gtkhcxmfgh.html

PHP:  array_merge(...$nested);
来源：http://hz.vqdsnc.cn/gtnxcbuobe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnxiangtu.top/gtbhaymdzm.html

TS:   nested.flat();
来源：http://hz.ehwqpu.com/gtgxtmotqt.html


<!-- 参考信息 -->