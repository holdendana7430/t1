代发 wailian999

[C02] 默认参数
来源：http://hz.zhixingplan.top/gtiotnitqf.html

Py:   def greet(name="World"): return name
来源：http://hz.yueranfly.top/gtoyjbipqn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xinyue.icu/gtpgknpbuy.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yvedp.cn/gtbydxapxa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj202588.top/gtxyudwjbr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jianghu66.top/gtxnqobudn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.andypj.xyz/gtwfnwitin.html

Ruby: def greet(name = "World") = name
来源：http://hz.gaohongyu789.top/gtfutrpeqk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangkeji.top/gtumnspidp.html

[C03] 可变参数
来源：http://hz.cucudq.cn/gtbmqvmdkn.html

Py:   def total(*args): return sum(args)
来源：http://hz.redwolf501.top/gtfvgejxnq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnqzz.top/gtdlkmyvah.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.vqdsnc.cn/gtvpkqltwf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.feifeiyinyue.top/gtnognrrmm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuanzx.com/gtmacqnnhe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yueranfly.top/gtklfcfkji.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.52xcode.cn/gtmhqewaup.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenlongwang.top/gtduqrvhuk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.nanxuanxn.top/gtuddnvyyv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.fengsongda.top/gtnvjfrlku.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ybcxt.top/gtbfzewzqv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtiphfqbju.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ivvv.top/gtsvhucozs.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ppjwa.cn/gtqmggyyta.html

Go:   // 无：用配置结构体参数
来源：http://hz.xuetiantiany.cn/gtxzfvspfm.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtzlmhzwhi.html

C#:   f(a: 1, b: 2)
来源：http://hz.zycfv.cn/gtpfoijtcv.html

[C05] 返回多个值
来源：http://hz.cqqwz.cn/gtlcxcmvhv.html

Py:   return a, b
来源：http://hz.yj20258888.top/gtgsjjsfga.html

PHP:  return [$a, $b];
来源：http://hz.xylfe.cn/gtmxzhaucj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.aizwys.cn/gtoppdrnos.html

TS:   return { a, b };
来源：http://hz.jqgfzy.top/gtvvrpufme.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhaomingkeji.xyz/gtyxyfyuqa.html

Go:   return a, b
来源：http://hz.zhengqikj.top/gtrolopajx.html

Ruby: return a, b
来源：http://hz.xinyue.icu/gtwwjystyv.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sweek.top/gtngdatrja.html

[C06] 匿名函数 / lambda
来源：http://hz.chenzaomai.com/gtvibsxemo.html

Py:   square = lambda x: x * x
来源：http://hz.ydjk.org.cn/gtadajutzh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yuxming.cn/gtpuuddwlt.html

JS:   const square = x => x * x;
来源：http://hz.pengpengdd.cyou/gtbosfwbrg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhaomingkeji.xyz/gtwvialgan.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.316326.xyz/gtkfmzdyuy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuxming.cn/gtxgqdazvb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shangyingyoupin.top/gtmqghpykf.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nanxuanxn.top/gtshuabkmr.html

[C07] 把函数作为参数传入
来源：http://hz.tian-w.cn/gtceravapp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.guowangkeji.top/gtglaosgrg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jinghuilouyu.cn/gtqpylgxsi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hammf.cn/gtpwczmrjb.html

TS:   arr.map(String)
来源：http://hz.nanxinkj.top/gtznujtnfn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shzxlz.cn/gtqqtoinwy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.nwbrower.top/gtcihxymmj.html

Ruby: arr.map(&:upcase)
来源：http://hz.shzxlz.cn/gtfldtenrd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.feifeiyinyue.top/gtbiwzlkyj.html

[C08] 闭包
来源：http://hz.yj202588.top/gtnneiwnhy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shangyingyoupin.top/gtslwenuxn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yangfankeji.com/gtwztsmhmp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.mhx1999.top/gtfodigjrr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtwbsvtjlx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gotoacloud.top/gttuwdoakk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ivvv.top/gtkijrpiat.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.gotoacloud.top/gtbnpyvhwk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtpatyqzmc.html

[C09] 递归
来源：http://hz.c1oappe.top/gtuwxhvhng.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtvqrxqgrm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.smart0.xyz/gtrjvexsdq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gttbicnrhg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.andypj.xyz/gtkbvqeqvy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.redwolf501.top/gtrkzvxpxv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinqigfzy.top/gtrgavhggd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sysykeji.top/gtcsickckt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigfzy.top/gtzxiyidfe.html

[C10] 变量作用域
来源：http://hz.xuetiantiany.cn/gtwfddfhoh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jiagoushi.top/gthhfrhvxt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jqgufenzy.top/gtoqhsfvtw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.haohaochexian.top/gtbtdvxjpo.html

TS:   同 JS
来源：http://hz.jiagoushi.top/gtmesmaakz.html

Java: 方法内为块级作用域
来源：http://hz.gaohongyu789.top/gtfbnllrvl.html

Go:   花括号块级作用域
来源：http://hz.havefunace.top/gtlborbrkr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.bjfxy.top/gtshdmuxyx.html

C#:   块级作用域
来源：http://hz.ydjk.org.cn/gtrxqtprfc.html

[C11] 模块导入与导出
来源：http://hz.tian-w.cn/gthzlzhmov.html

Py:   from module import func
来源：http://hz.hammf.cn/gtluzdhfmn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hysaishi.cn/gtjjzmzsvn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.fzhhl.top/gtissbinrd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xuanzx.com/gttnxvpagm.html

Java: import java.util.List;
来源：http://hz.dianchejie.cn/gtdmqvnqra.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hysaishi.cn/gttfppbcgd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xuetiantiany.cn/gtcokwwxyu.html

C#:   using System.Text;
来源：http://hz.cheryme.top/gtksxadfye.html

[C12] 立即执行函数 IIFE
来源：http://hz.xuanzx.com/gtmwwhjheu.html

Py:   (lambda: print("run"))()
来源：http://hz.kuanghao11.cn/gteeiizsxr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.aizwys.cn/gttijjoyhf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gttemgiqre.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinyuanbaomall.cn/gtghovfcbq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.mhx1999.top/gtbnmjpxxb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.quarkkingdee.top/gtrlztwwlf.html

Ruby: -> { puts "run" }.call
来源：http://hz.chenzaomai.com/gtinaiznju.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jlsjyb.cn/gthawcpkzt.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj202588.top/gtqwepzmgc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinyuanbaomall.cn/gtayqpypkq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtxthroavi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cashguo.top/gtymwymkha.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenlongwang.top/gtdcaksgfd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtxhauyzfk.html

Go:   func add(a, b int) int
来源：http://hz.shanyushiyangkeji.top/gtsfwmplzm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.smart0.xyz/gtxoocetrj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxuanxn.top/gtjpdtdqnx.html

[C14] 泛型函数
来源：http://hz.aibaodan.cn/gtmzgjhutu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yonumen.top/gtbwjaezzq.html

PHP:  // 无泛型
来源：http://hz.gaohongyu789.top/gtidxzupks.html

JS:   // 无泛型
来源：http://hz.zhengqikj.top/gtpaahnkqq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigfzy.top/gtusymtmbm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xingfuxueyuan.xyz/gtetnhembs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhixingplan.top/gtycjodhgo.html

Ruby: # 无泛型
来源：http://hz.jqgfzy.top/gtrsfkebrm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sxryk.cn/gtcbskqjwc.html

[C15] 解构 / 展开参数
来源：http://hz.hammf.cn/gtiswnvfql.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.quarkkingdee.top/gteumilwor.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yvedp.cn/gtvpprhnbc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtuchqjlnl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yangfankeji.com/gtcvcsqhow.html

Java: // 无解构
来源：http://hz.shanyushiyangkeji.top/gthwbqcbap.html

Go:   // 无解构
来源：http://hz.sysykeji.top/gtvyothxgw.html

Ruby: a, b = pair
来源：http://hz.yuxming.cn/gtyevewgty.html

C#:   var (a, b) = pair;
来源：http://hz.hfpthk.cn/gthxijwiqo.html

[C16] 函数 / 方法重载
来源：http://hz.ydjk.org.cn/gtibvvytlb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shanyushiyangkeji.top/gtxgsmyhky.html

PHP:  // 无重载
来源：http://hz.hammf.cn/gtulmgoukp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sufxvd.cn/gtuaevtphc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ehwqpu.com/gtvsdqodqm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.redwolf501.top/gtxzmuakvx.html

Go:   // 无重载：用不同函数名
来源：http://hz.pycfn.com/gtcxdiwfdw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.0kj1m.cn/gtiddliuwr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ppjwa.cn/gthbbnmbre.html

================================================================================
来源：http://hz.xinyue.icu/gtpgastals.html

D. 数组 / 列表 / 集合
来源：http://hz.yueranfly.top/gtsqldgehj.html

================================================================================
来源：http://hz.52xcode.cn/gtuojwdxwa.html

[D01] 创建数组 / 列表
来源：http://hz.hfpthk.cn/gtehartryv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jlsjyb.cn/gtkrasnmjj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.9152youxi.cn/gtlplcmlcr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.meibo888.top/gttnowfasr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.dashuyun.cn/gtzzdnqufp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jianghu66.top/gtarjdpvjz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shangyingyoupin.top/gttusaovyr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.guannengcc.top/gtxnjjpeaa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.c1oappe.top/gtkycurtqh.html

[D02] 追加元素到末尾
来源：http://hz.dashuyun.cn/gtyjifnhiz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuxming.cn/gtnsgbqqmd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuanzx.com/gtdszkqisx.html

JS:   arr.push(4);
来源：http://hz.xylfe.cn/gtjpbriefu.html

TS:   arr.push(4);
来源：http://hz.nanxuanxn.top/gtvoyzlhjr.html

Java: list.add(4);
来源：http://hz.yj20258888.top/gtnosvlxfb.html

Go:   arr = append(arr, 4)
来源：http://hz.xuetiantiany.cn/gthpvyptyi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.vqdsnc.cn/gtxpjsruii.html

C#:   list.Add(4);
来源：http://hz.aibaodan.cn/gtgioenaei.html

[D03] 在指定位置插入元素
来源：http://hz.jinqigfzy.top/gtaxxztrbs.html

Py:   arr.insert(0, 0)
来源：http://hz.daxiang520.top/gtizbwozft.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hysaishi.cn/gtqxxhxzlt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.vqdsnc.cn/gttyseoney.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.kuanghao11.cn/gtapyundvw.html

Java: list.add(0, 0);
来源：http://hz.zhaomingkeji.xyz/gtpbssygfl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aibaodan.cn/gttnuzqbto.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hnxiangtu.top/gtnjwwgeud.html

C#:   list.Insert(0, 0);
来源：http://hz.ehwqpu.com/gtihftltmt.html

[D04] 删除元素
来源：http://hz.xziqi.cn/gtsggkffeb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydjk.org.cn/gtawebshza.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.smart0.xyz/gtlxbucbwr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.guannengcc.top/gtfkzsvqeh.html

TS:   arr.splice(0, 1);
来源：http://hz.zhixingplan.top/gttwuilotr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxuanxn.top/gttescttek.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.svipenyu.cn/gtegqlvfci.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ywan-chungtsiang.top/gtexitqcpk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sufxvd.cn/gtfxmagcxh.html

[D05] 访问与修改元素
来源：http://hz.fzhhl.top/gtnxvylewr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtmgzusqwi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nwbrower.top/gtsikbdetd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuxming.cn/gttndmjscd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.meibo888.top/gtbnqgbqrj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gogol.net.cn/gtnpmrbdvk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yj20258888.top/gtanaomicu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtfmrxiiam.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aibaodan.cn/gtuzegimrh.html

[D06] 数组长度
来源：http://hz.svipenyu.cn/gtzeunhcln.html

Py:   len(arr)
来源：http://hz.jinqigufen.top/gtwwyfxmnc.html

PHP:  count($arr);
来源：http://hz.sweek.top/gteevyaapi.html

JS:   arr.length
来源：http://hz.wangshuangyany.cn/gtpadnyual.html

TS:   arr.length
来源：http://hz.jinqigfzy.top/gtdwircqtx.html

Java: list.size();
来源：http://hz.xinyue.icu/gttcbteyth.html

Go:   len(arr)
来源：http://hz.nanxuanxn.top/gtuvsoowrl.html

Ruby: arr.length; arr.size
来源：http://hz.chenjidiqi.icu/gtuheypveb.html

C#:   list.Count;
来源：http://hz.hammf.cn/gtchgpijzi.html

[D07] 切片 / 取子数组
来源：http://hz.xinyue.icu/gtttlnvial.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shzxlz.cn/gtlhdcvnqv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aizwys.cn/gtpbtvcppd.html

JS:   arr.slice(1, 4);
来源：http://hz.feifeiyinyue.top/gtoeoebqzh.html

TS:   arr.slice(1, 4);
来源：http://hz.hfpthk.cn/gtczkylsnq.html

Java: list.subList(1, 4);
来源：http://hz.shangyingyoupin.top/gtezvoubgf.html

Go:   arr[1:4]
来源：http://hz.jianghu66.top/gtoctlqyzv.html

Ruby: arr[1, 3]
来源：http://hz.sxryk.cn/gtkgrhheik.html

C#:   list.GetRange(1, 3);
来源：http://hz.meibo888.top/gtlfdtmxmf.html

[D08] 合并两个数组
来源：http://hz.yj20258.top/gtgthtbcaj.html

Py:   a + b;  a.extend(b)
来源：http://hz.cashguo.top/gtnmveeaed.html

PHP:  array_merge($a, $b);
来源：http://hz.cucudq.cn/gtvaialxwl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.daxiang520.top/gtnojmabdu.html

TS:   [...a, ...b];
来源：http://hz.ehwqpu.com/gtfddfllmg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinqigufen.top/gtkymrrnty.html

Go:   append(a, b...)
来源：http://hz.hysaishi.cn/gtekqkkjll.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cashguo.top/gtyrorlkyw.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinyuanbaomall.cn/gthnrewwhe.html

[D09] 排序（升序）
来源：http://hz.chenlongwang.top/gtjkwmuxci.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.birdmap.top/gtxaeuvpni.html

PHP:  sort($arr);
来源：http://hz.daria6918.cn/gtpqtgcgyn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yueranfly.top/gttlxxfgbx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pengpengdd.cyou/gtvrwkesdx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cucudq.cn/gtelpiorzx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinqigufen.top/gtjhpcixzq.html

Ruby: arr.sort
来源：http://hz.nanxuanxn.top/gtueflrfkv.html

C#:   list.Sort();
来源：http://hz.tian-w.cn/gtuiuacqzt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydzc1.top/gtfnqmjzlv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xuetiantiany.cn/gtxgenmynl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cqqwz.cn/gtizxlrrpe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shuidangran.top/gtztbtuifm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.c1oappe.top/gtjrzifjbq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zycfv.cn/gtjgrznfam.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shangyingyoupin.top/gtjsspedjz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daxiang520.top/gtilmviles.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhijiandao.cn/gtixpfmsdn.html

[D11] 反转数组
来源：http://hz.ybcxt.top/gtrztjuaxr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shuidangran.top/gtwgzpghsl.html

PHP:  array_reverse($arr);
来源：http://hz.aibaodan.cn/gtcnzaspyn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigfzy.top/gtwjvmdlto.html

TS:   [...arr].reverse();
来源：http://hz.redwolf501.top/gtchoweizt.html

Java: Collections.reverse(list);
来源：http://hz.316326.xyz/gtiqdzsnhi.html

Go:   slices.Reverse(arr)
来源：http://hz.chenzaomai.com/gtujmydthm.html

Ruby: arr.reverse
来源：http://hz.daxiang520.top/gtwobejfsj.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gtgtkzyzgl.html

[D12] 查找元素下标
来源：http://hz.cdnleiting.top/gtkuyuvfhp.html

Py:   arr.index(x);  x in arr
来源：http://hz.hnxiangtu.top/gtorexoebd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxuanxn.top/gtufrkpsjf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gaohongyu789.top/gtbrwntioy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cashguo.top/gtkezthixe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhongyouzk.top/gtmvlsojmm.html

Go:   slices.Index(arr, x)
来源：http://hz.jlsjyb.cn/gttpijsdxk.html

Ruby: arr.index(x)
来源：http://hz.cdnleiting.top/gtkueqxtec.html

C#:   list.IndexOf(x);
来源：http://hz.cashguo.top/gtntbyadxv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhixingplan.top/gtozrzhzkb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gotoacloud.top/gtafefdiuh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhijiandao.cn/gtjzkhltcw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gaohongyu789.top/gtnypzcrgq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shangyingyoupin.top/gtijwsdsmh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigufen.top/gthbisatnq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hongshengwenyu.top/gtydmxxdqv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.c1oappe.top/gtzmkgklmt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.aibaodan.cn/gtidpqgapp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ybcxt.top/gtwgufavsp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aibaodan.cn/gtoowtsija.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cdnleiting.top/gtatorkrzm.html

JS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gtedypaobt.html

TS:   arr.map(x => x * 2)
来源：http://hz.yonumen.top/gtxogisqaw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xingfuxueyuan.xyz/gtlnlqnhtz.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtjubrkhoh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenzaomai.com/gtgabpqhay.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhiwuduotai.top/gttxsotdin.html

[D15] 去重
来源：http://hz.dashuyun.cn/gtmbowyhqt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtsjuiosjr.html

PHP:  array_unique($arr);
来源：http://hz.cucudq.cn/gtyppfgbna.html

JS:   [...new Set(arr)]
来源：http://hz.wangshuangyany.cn/gtaqlwvkky.html

TS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gtuaxbfniz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xinyue.icu/gtzbbxkxyx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.smart0.xyz/gtjohuvpuh.html

Ruby: arr.uniq
来源：http://hz.hywenlv.cn/gtcrlympdi.html

C#:   list.Distinct().ToList()
来源：http://hz.sysykeji.top/gtkirzimsa.html

[D16] 求和与平均值
来源：http://hz.cucudq.cn/gtmktmwanj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangkeji.top/gtwcbbaxax.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guowangkeji.top/gtkvhirdbu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigfzy.top/gtnalqzwex.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.bjfxy.top/gtftbtgtvo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jqgfzy.top/gtiigtcziu.html

Go:   // 手写循环累加
来源：http://hz.jyoumei.cn/gtpjkxfdkg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sweek.top/gtxjxlidsi.html

C#:   list.Sum();  list.Average()
来源：http://hz.c1oappe.top/gtedktvzfr.html

[D17] 最大值与最小值
来源：http://hz.hnqzz.top/gtlyfdjjsm.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtjxlqoajc.html

PHP:  max($arr);  min($arr);
来源：http://hz.gzhubu.top/gtwypsnvsu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fengsongda.top/gtujwnbayd.html

TS:   Math.max(...arr);
来源：http://hz.hywenlv.cn/gtylfuoadp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hammf.cn/gtraoutizi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tian-w.cn/gtqowlhknq.html

Ruby: arr.max;  arr.min
来源：http://hz.sxryk.cn/gtfnliumun.html

C#:   list.Max();  list.Min()
来源：http://hz.fengsongda.top/gtwbasiblm.html

[D18] 扁平化嵌套数组
来源：http://hz.chenjidiqi.icu/gtokammkhs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhixingplan.top/gtdkntgtuh.html

PHP:  array_merge(...$nested);
来源：http://hz.ehwqpu.com/gtgolxnibc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.52xcode.cn/gtlymtroue.html

TS:   nested.flat();
来源：http://hz.52xcode.cn/gtobpfhxqe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.316326.xyz/gtgsoqtaoo.html

Go:   // 手写双层循环
来源：http://hz.wangdashe.top/gttrzudgrl.html

Ruby: nested.flatten
来源：http://hz.nwbrower.top/gtntfaoxqq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhengqikj.top/gtvbmqvmgx.html


<!-- 参考信息 -->