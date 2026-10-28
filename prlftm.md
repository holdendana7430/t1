代发 wailian999

Py:   return a, b
来源：http://hz.nanxinkj.top/gtkolgafpn.html

PHP:  return [$a, $b];
来源：http://hz.ppjwa.cn/gtxrpirpii.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.andypj.xyz/gtywoeimox.html

TS:   return { a, b };
来源：http://hz.ybcxt.top/gtzterkdqj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinyuanbaomall.cn/gtbjzmqtyi.html

Go:   return a, b
来源：http://hz.wangshuangyany.cn/gtsdzxpwrb.html

Ruby: return a, b
来源：http://hz.zdqjudy.top/gtliuxxqtw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jlsjyb.cn/gtnaxebcia.html

[C06] 匿名函数 / lambda
来源：http://hz.yvedp.cn/gtjygysgzp.html

Py:   square = lambda x: x * x
来源：http://hz.xingfuxueyuan.xyz/gthvyjonln.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hfpthk.cn/gtbcuugdlh.html

JS:   const square = x => x * x;
来源：http://hz.hammf.cn/gtokclcgfe.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ehwqpu.com/gtkxfqecpp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.0kj1m.cn/gtunnbjwgg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.snrcjt.cn/gtgqhidivo.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cdnleiting.top/gtnhedrqlo.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yvedp.cn/gtdyrcplwm.html

[C07] 把函数作为参数传入
来源：http://hz.jinqigufen.top/gttggbvgqk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yangfankeji.com/gtvillvuze.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jinghuilouyu.cn/gtfwgckfoq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xylfe.cn/gtjtxavhsp.html

TS:   arr.map(String)
来源：http://hz.feifeiyinyue.top/gtbiivqcve.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cheryme.top/gtqhupfsla.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenjidiqi.icu/gtonxualrm.html

Ruby: arr.map(&:upcase)
来源：http://hz.cqqwz.cn/gtbjvhzxqd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangshuangyany.cn/gtnjdniftl.html

[C08] 闭包
来源：http://hz.zhongyouzk.top/gtngghprzx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangtech.top/gthcwzusaf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hywenlv.cn/gtkfshlnap.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj20258888.top/gtkawrldso.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sysykeji.top/gtkklturnp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jqgufenzy.top/gtholkijtm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.kuanghao11.cn/gtdczpgosc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xziqi.cn/gtlvevfzin.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gthjogkftw.html

[C09] 递归
来源：http://hz.haohaochexian.top/gtoevrbjif.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jqgfzy.top/gtzewcofdx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sufxvd.cn/gtiumaiffh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aibaodan.cn/gtwkntgnek.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gtbffdibvg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.guowangkeji.top/gtprqwadgt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cdnleiting.top/gttckwxipg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dianchejie.cn/gtzilykixw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ppjwa.cn/gtzwwlpnfb.html

[C10] 变量作用域
来源：http://hz.hysaishi.cn/gtzborpfvb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.redwolf501.top/gtdxjpczdl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.c1oappe.top/gtnnknmwoy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.havefunace.top/gtbhodsgfi.html

TS:   同 JS
来源：http://hz.daxiang520.top/gtftcotjxb.html

Java: 方法内为块级作用域
来源：http://hz.zhiwuduotai.top/gtzoqtjscy.html

Go:   花括号块级作用域
来源：http://hz.zhongyouzk.top/gtzpgrqabw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.aizwys.cn/gtrickhvfg.html

C#:   块级作用域
来源：http://hz.gzhubu.top/gtiytlfmzu.html

[C11] 模块导入与导出
来源：http://hz.sufxvd.cn/gtdsvrsogy.html

Py:   from module import func
来源：http://hz.gzhubu.top/gtrigvbcdj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yangfankeji.com/gtxxsebhrc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shuidangran.top/gtnihhiewe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jqgufenzy.top/gtqehpodow.html

Java: import java.util.List;
来源：http://hz.c1oappe.top/gtjdvbieyb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj20258888.top/gtelrpdamf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shuidangran.top/gtoeqdkhgq.html

C#:   using System.Text;
来源：http://hz.yongpay.top/gtcrixdvfo.html

[C12] 立即执行函数 IIFE
来源：http://hz.0kj1m.cn/gtteywxyzx.html

Py:   (lambda: print("run"))()
来源：http://hz.fengsongda.top/gtognxjnsp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xziqi.cn/gtxagxplfm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuanzx.com/gtvwoyrfjc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cqqwz.cn/gtegxgxcmh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sweek.top/gtkjnrxjsa.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.wangshuangyany.cn/gteicoqiwk.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydzc1.top/gtoyplehfs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gaohongyu789.top/gthtuehavy.html

[C13] 类型声明 / 类型注解
来源：http://hz.zycfv.cn/gtwofhlekc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cashguo.top/gtveblyycb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtdxpqbvtq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.guowangkeji.top/gtnxhrobcf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gtifawelgu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtcdlcdkdm.html

Go:   func add(a, b int) int
来源：http://hz.jiagoushi.top/gtldlhqzbm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.dashuyun.cn/gtjsasakmh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gaohongyu789.top/gtclgykjtv.html

[C14] 泛型函数
来源：http://hz.ppjwa.cn/gtrqflqjuy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangtech.top/gtplybmfeb.html

PHP:  // 无泛型
来源：http://hz.fzhhl.top/gtkbwwcdnm.html

JS:   // 无泛型
来源：http://hz.jqgufenzy.top/gtjvhzhcoo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xingfuxueyuan.xyz/gtcahwfzlc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sysykeji.top/gtrzpeiovo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xingfuxueyuan.xyz/gtajviombz.html

Ruby: # 无泛型
来源：http://hz.fengsongda.top/gtybftcpjg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aibaodan.cn/gtdfykbggl.html

[C15] 解构 / 展开参数
来源：http://hz.nwbrower.top/gtvovuqsef.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.andypj.xyz/gtozoovhjt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gaohongyu789.top/gtohjxdyis.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sweek.top/gtuqahnmwy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jianghu66.top/gtvcepynjm.html

Java: // 无解构
来源：http://hz.xziqi.cn/gtetrrblfx.html

Go:   // 无解构
来源：http://hz.zycfv.cn/gtdnmfuonm.html

Ruby: a, b = pair
来源：http://hz.yongpay.top/gtnhzaavoc.html

C#:   var (a, b) = pair;
来源：http://hz.wangshuangyany.cn/gtlxhyimed.html

[C16] 函数 / 方法重载
来源：http://hz.jinghuilouyu.cn/gtsexxhaqj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xylfe.cn/gtcvyzqicp.html

PHP:  // 无重载
来源：http://hz.bjfxy.top/gtvmudezyp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xuetiantiany.cn/gtlpgovmvl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ybcxt.top/gtihkqedam.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.wangshuangyany.cn/gtntrgnwab.html

Go:   // 无重载：用不同函数名
来源：http://hz.meibo888.top/gtdqnamjqp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.snrcjt.cn/gthdbfrknk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hongshengwenyu.top/gtjjlmsrln.html

================================================================================
来源：http://hz.guannengcc.top/gttvncazte.html

D. 数组 / 列表 / 集合
来源：http://hz.dianchejie.cn/gtsszdtsty.html

================================================================================
来源：http://hz.haohaochexian.top/gtrlqzhikb.html

[D01] 创建数组 / 列表
来源：http://hz.ivvv.top/gturxdkqdh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhengqikj.top/gtwdezokpq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.bjfxy.top/gtacncmhrq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xziqi.cn/gtamfwysyh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.kuanghao11.cn/gtujukrlmn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.iojbl.cn/gtzehfwnkh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenjidiqi.icu/gtkfidiqxn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhiwuduotai.top/gthxphwikk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgfzy.top/gtstiespri.html

[D02] 追加元素到末尾
来源：http://hz.jinyuanbaomall.cn/gtelyegufc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xziqi.cn/gtbgwychxf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yangfankeji.com/gtvxdpbphq.html

JS:   arr.push(4);
来源：http://hz.nwbrower.top/gtwyiirumh.html

TS:   arr.push(4);
来源：http://hz.xylfe.cn/gtwkpvmzjt.html

Java: list.add(4);
来源：http://hz.zhixingplan.top/gtrayzdalp.html

Go:   arr = append(arr, 4)
来源：http://hz.dianchejie.cn/gtciqmmpwp.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daxiang520.top/gtdeuyhtpr.html

C#:   list.Add(4);
来源：http://hz.zhiwuduotai.top/gtibisayrn.html

[D03] 在指定位置插入元素
来源：http://hz.pycfn.com/gtgppnsnxh.html

Py:   arr.insert(0, 0)
来源：http://hz.zhaomingkeji.xyz/gtfcvxhmlg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.bjfxy.top/gtvkuplsvk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhaomingkeji.xyz/gtmjeifxtu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.birdmap.top/gtfmmcfqxq.html

Java: list.add(0, 0);
来源：http://hz.hongshengwenyu.top/gtycdxduou.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aizwys.cn/gtlfjijtrs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.guannengcc.top/gtlztdoyzq.html

C#:   list.Insert(0, 0);
来源：http://hz.zhongyouzk.top/gtzplrynuk.html

[D04] 删除元素
来源：http://hz.jqgfzy.top/gtyrwruggi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nanxuanxn.top/gtkmiihqxv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yj20258.top/gtqkxxsapj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hammf.cn/gtzlongqzt.html

TS:   arr.splice(0, 1);
来源：http://hz.316326.xyz/gtwwwhmlww.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tanke756.top/gtyydxcrib.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj202588.top/gtxbythluw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gogol.net.cn/gttmknyyib.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.dianchejie.cn/gthxyulseg.html

[D05] 访问与修改元素
来源：http://hz.birdmap.top/gtmzxbvxvd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sxryk.cn/gtuqeiynpt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.iojbl.cn/gtklsuxudn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shangyingyoupin.top/gtkprerpcp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.daria6918.cn/gteqcaegmq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xylfe.cn/gtnxwhpeeq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gzhubu.top/gtvozixtey.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtgxyempat.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhaomingkeji.xyz/gtxtwwxofg.html

[D06] 数组长度
来源：http://hz.iojbl.cn/gtpahaagen.html

Py:   len(arr)
来源：http://hz.aibaodan.cn/gtztpugtbn.html

PHP:  count($arr);
来源：http://hz.wangshuangyany.cn/gtxtkdjbnx.html

JS:   arr.length
来源：http://hz.andypj.xyz/gtouryxkkh.html

TS:   arr.length
来源：http://hz.hongshengwenyu.top/gtkadlbdmr.html

Java: list.size();
来源：http://hz.xziqi.cn/gtggpdkgba.html

Go:   len(arr)
来源：http://hz.ydjk.org.cn/gttvwvpqxp.html

Ruby: arr.length; arr.size
来源：http://hz.9152youxi.cn/gttqhandyd.html

C#:   list.Count;
来源：http://hz.nanxuanxn.top/gtxeusskzo.html

[D07] 切片 / 取子数组
来源：http://hz.ppjwa.cn/gthcvgevdb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cheryme.top/gtqmenzyus.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenzaomai.com/gtnbrcqkzo.html

JS:   arr.slice(1, 4);
来源：http://hz.gaohongyu789.top/gtfeayenzy.html

TS:   arr.slice(1, 4);
来源：http://hz.chenzaomai.com/gtdhqlkyvr.html

Java: list.subList(1, 4);
来源：http://hz.xuanzx.com/gtpevwjayy.html

Go:   arr[1:4]
来源：http://hz.hongshengwenyu.top/gtqaqhcqsn.html

Ruby: arr[1, 3]
来源：http://hz.pengpengdd.cyou/gtenhrxbjk.html

C#:   list.GetRange(1, 3);
来源：http://hz.cucudq.cn/gtjsjfszky.html

[D08] 合并两个数组
来源：http://hz.hywenlv.cn/gtykkxpekt.html

Py:   a + b;  a.extend(b)
来源：http://hz.cucudq.cn/gtatrfynqv.html

PHP:  array_merge($a, $b);
来源：http://hz.yuxming.cn/gtjdfmmpnh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gogol.net.cn/gtctedopcf.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangtech.top/gtgjmnoobp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.guannengcc.top/gtbuokncfc.html

Go:   append(a, b...)
来源：http://hz.jianghu66.top/gtrhbyfvnc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hywenlv.cn/gtodtuwtwh.html

C#:   a.Concat(b).ToList()
来源：http://hz.jiagoushi.top/gtrnhhbrgt.html

[D09] 排序（升序）
来源：http://hz.yueranfly.top/gtrznixlwi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtucwzxqss.html

PHP:  sort($arr);
来源：http://hz.zhijiandao.cn/gtygqzmtov.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cqqwz.cn/gtbanywspn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gotoacloud.top/gtmwfbgfcv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.52xcode.cn/gtplmlxrjv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.quarkkingdee.top/gtoxifedjx.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtdudfgtmf.html

C#:   list.Sort();
来源：http://hz.ybcxt.top/gtbjirctix.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgfzy.top/gtxjbnyaya.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhaomingkeji.xyz/gtdxxrnudy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtpzysfawj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnxiangtu.top/gtfhgrnhva.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shuidangran.top/gtfxyhespg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.9152youxi.cn/gtgzfpayak.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gzhubu.top/gtzkndprcp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydjk.org.cn/gtletyqeuf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ydjk.org.cn/gtussukjfe.html

[D11] 反转数组
来源：http://hz.sysykeji.top/gtkpznimxr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhiwuduotai.top/gtuhjujmqy.html

PHP:  array_reverse($arr);
来源：http://hz.fengsongda.top/gtnbuwpbfw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daria6918.cn/gtgnouayjg.html

TS:   [...arr].reverse();
来源：http://hz.havefunace.top/gtchtdllbe.html

Java: Collections.reverse(list);
来源：http://hz.c1oappe.top/gtejqpnwzk.html

Go:   slices.Reverse(arr)
来源：http://hz.shanyushiyangtech.top/gtchcvvqxs.html

Ruby: arr.reverse
来源：http://hz.cheryme.top/gtmjsvrmjg.html

C#:   list.Reverse();
来源：http://hz.pengpengdd.cyou/gtjhjsbfsq.html

[D12] 查找元素下标
来源：http://hz.zhijiandao.cn/gtnerefbfj.html

Py:   arr.index(x);  x in arr
来源：http://hz.cashguo.top/gtsxkzdfnc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pycfn.com/gtnahjgyrq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangkeji.top/gttmtqnwac.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.mhx1999.top/gthxjshpgt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhaomingkeji.xyz/gtjwovcdpc.html

Go:   slices.Index(arr, x)
来源：http://hz.daria6918.cn/gtrlhvzikm.html

Ruby: arr.index(x)
来源：http://hz.aibaodan.cn/gtxkynifza.html

C#:   list.IndexOf(x);
来源：http://hz.guannengcc.top/gtcimzofjs.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hnqzz.top/gtobebtvgb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ybcxt.top/gtsiszseqa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xylfe.cn/gtrlrizhlb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhiwuduotai.top/gtzrfbrpmj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shangyingyoupin.top/gtvhsphmdv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hfpthk.cn/gtvhzzzytn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ywan-chungtsiang.top/gtignbwwzm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yuxming.cn/gtazpvjcty.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daxiang520.top/gtkgsamciw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.pycfn.com/gtwzrmeovp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yonumen.top/gtxoitjpss.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.pycfn.com/gtwayxqqrv.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gtdqlwrivp.html

TS:   arr.map(x => x * 2)
来源：http://hz.jqgufenzy.top/gtcspatypz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.0kj1m.cn/gtwrjuybwt.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtoytmveme.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xuetiantiany.cn/gthxggmzdk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ehwqpu.com/gtolhuwbwp.html

[D15] 去重
来源：http://hz.xziqi.cn/gteqvgitxe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.snrcjt.cn/gtevejhrrp.html

PHP:  array_unique($arr);
来源：http://hz.fengsongda.top/gthpkmaxdf.html

JS:   [...new Set(arr)]
来源：http://hz.wangdashe.top/gtnbijlykg.html

TS:   [...new Set(arr)]
来源：http://hz.nanxinkj.top/gtqlfjrlyv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yangfankeji.com/gtrymxvkbr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jianghu66.top/gtewhalque.html

Ruby: arr.uniq
来源：http://hz.yj20258888.top/gtycrtnkvk.html

C#:   list.Distinct().ToList()
来源：http://hz.hammf.cn/gtgzdmkoax.html

[D16] 求和与平均值
来源：http://hz.meibo888.top/gtuncavqsl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gzhubu.top/gtuqufdejc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xingfuxueyuan.xyz/gtogvckdqr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tanke756.top/gtvekajozh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtvuipibxu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shanyushiyangkeji.top/gtofzjvluc.html

Go:   // 手写循环累加
来源：http://hz.zhengqikj.top/gtkpuwslgz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.fengsongda.top/gtpghnbiok.html

C#:   list.Sum();  list.Average()
来源：http://hz.vqdsnc.cn/gtovwmuuva.html

[D17] 最大值与最小值
来源：http://hz.52xcode.cn/gtqmthnyme.html

Py:   max(arr);  min(arr)
来源：http://hz.cucudq.cn/gtzcrmaowb.html

PHP:  max($arr);  min($arr);
来源：http://hz.c1oappe.top/gtjrpzgpcm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.aizwys.cn/gtchqudegv.html

TS:   Math.max(...arr);
来源：http://hz.zhoulong.xyz/gtydkpoyyj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cdnleiting.top/gtetvbqwdh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenjidiqi.icu/gtpnxgpyeb.html

Ruby: arr.max;  arr.min
来源：http://hz.iojbl.cn/gthuoxyued.html

C#:   list.Max();  list.Min()
来源：http://hz.gzhubu.top/gtlbiyoqvl.html

[D18] 扁平化嵌套数组
来源：http://hz.vqdsnc.cn/gtdzjbbugm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yonumen.top/gtipyeasnc.html

PHP:  array_merge(...$nested);
来源：http://hz.jinghuilouyu.cn/gtlkstclau.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sxryk.cn/gtwtentuza.html

TS:   nested.flat();
来源：http://hz.cqqwz.cn/gtehenawuq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.9152youxi.cn/gtnvcgseuu.html

Go:   // 手写双层循环
来源：http://hz.cucudq.cn/gtpxzajdko.html

Ruby: nested.flatten
来源：http://hz.nanxuanxn.top/gtisypdmde.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.52xcode.cn/gtmryamarm.html

[D19] 按字段分组
来源：http://hz.zhongyouzk.top/gtbczbgxfm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guannengcc.top/gtmbyycpes.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hysaishi.cn/gtafctvuko.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tanke756.top/gtysziigwl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gtnuneojir.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinghuilouyu.cn/gtidjnqoqu.html

Go:   // 手写 map[string][]T
来源：http://hz.svipenyu.cn/gtnirrlzga.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aibaodan.cn/gtyeuqsubw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.316326.xyz/gtxkiudqbh.html

[D20] 统计每个元素出现次数
来源：http://hz.cqqwz.cn/gtyscedthq.html

Py:   Counter(arr)
来源：http://hz.ppjwa.cn/gtfphxvhij.html

PHP:  array_count_values($arr);
来源：http://hz.cdnleiting.top/gtjaxghqbp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gtorqnyzbz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydjk.org.cn/gtzobmfteb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dianchejie.cn/gtsovtcevf.html

Go:   // 手写 map[T]int
来源：http://hz.chenzaomai.com/gtlyxpqlix.html

Ruby: arr.tally
来源：http://hz.zhiwuduotai.top/gthwsaajjb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gotoacloud.top/gthmcwfwla.html

[D21] 判断是否包含某元素
来源：http://hz.xuanzx.com/gthnekyhhp.html

Py:   x in arr
来源：http://hz.jlsjyb.cn/gtelwegrda.html

PHP:  in_array($x, $arr, true);
来源：http://hz.bjfxy.top/gtsqvjloxe.html

JS:   arr.includes(x)
来源：http://hz.fzhhl.top/gtwplsxylp.html

TS:   arr.includes(x)
来源：http://hz.ivvv.top/gtszzjozdm.html

Java: list.contains(x)
来源：http://hz.haohaochexian.top/gtpznvlvon.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgfzy.top/gtxgxbbgjd.html

Ruby: arr.include?(x)
来源：http://hz.ehwqpu.com/gtcswzdqom.html

C#:   list.Contains(x)
来源：http://hz.jiagoushi.top/gtaedfxhtr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhongyouzk.top/gtywdryxuc.html


<!-- 参考信息 -->