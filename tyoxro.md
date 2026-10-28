代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ybcxt.top/gtfaqeellc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hysaishi.cn/gtevinmykf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xylfe.cn/gthxgwyjbv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtwrzlrayb.html

[C02] 默认参数
来源：http://hz.hongshengwenyu.top/gtevmjnfiy.html

Py:   def greet(name="World"): return name
来源：http://hz.pengpengdd.cyou/gtcsmssare.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gzhubu.top/gtvqtmnayj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.mhx1999.top/gtdvkcvyiw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gotoacloud.top/gtynxdcjms.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinghuilouyu.cn/gtozmcmnyz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hongshengwenyu.top/gtvlpbmgwx.html

Ruby: def greet(name = "World") = name
来源：http://hz.hfpthk.cn/gtkxolvikn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.daxiang520.top/gtzrhvtmkd.html

[C03] 可变参数
来源：http://hz.yueranfly.top/gtefkqbjiw.html

Py:   def total(*args): return sum(args)
来源：http://hz.fengsongda.top/gtthcydjtw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yvedp.cn/gtlcdcvidi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtecwshyab.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jyoumei.cn/gtsvkuyhzn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xziqi.cn/gtivmcigdi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shuidangran.top/gtnfqpocvz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xingfuxueyuan.xyz/gtpnivzsfz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cucudq.cn/gtrerbulgo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.kuanghao11.cn/gtktpwyrke.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zycfv.cn/gtnafjtcxs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cashguo.top/gtrpcdniyw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.vqdsnc.cn/gthkxwoqvx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.fzhhl.top/gtwhpwbrgq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gogol.net.cn/gtsysisegs.html

Go:   // 无：用配置结构体参数
来源：http://hz.cdnleiting.top/gtwifdehgk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.havefunace.top/gtjlrhxgbz.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuanzx.com/gtsdefhbio.html

[C05] 返回多个值
来源：http://hz.zhengqikj.top/gtiyrfqxyz.html

Py:   return a, b
来源：http://hz.fzhhl.top/gttgykgjbq.html

PHP:  return [$a, $b];
来源：http://hz.yongpay.top/gtfyeizwme.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yj20258888.top/gtqmfdclrt.html

TS:   return { a, b };
来源：http://hz.yueranfly.top/gtksnziflu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ppjwa.cn/gtpitmakwx.html

Go:   return a, b
来源：http://hz.shanyushiyangtech.top/gtiyyhtkbx.html

Ruby: return a, b
来源：http://hz.fzhhl.top/gtqojqosfm.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yongpay.top/gtjtiuhuzb.html

[C06] 匿名函数 / lambda
来源：http://hz.cheryme.top/gtgfmnqaso.html

Py:   square = lambda x: x * x
来源：http://hz.zdqjudy.top/gtyulyiddi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yanxiufei.cn/gtprtybfkw.html

JS:   const square = x => x * x;
来源：http://hz.yangfankeji.com/gtilgwkxgb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.havefunace.top/gtguupybhi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hnxiangtu.top/gtwwhaqjnm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.nwbrower.top/gtufawbdjn.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhixingplan.top/gtbbjdduac.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hongshengwenyu.top/gtjqyiddsr.html

[C07] 把函数作为参数传入
来源：http://hz.tian-w.cn/gtwhuabtoc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xinyue.icu/gtwkxthopd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zdqjudy.top/gtixcqqblq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenjidiqi.icu/gtbmjhenbz.html

TS:   arr.map(String)
来源：http://hz.zhijiandao.cn/gtmsqxckqg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shangyingyoupin.top/gtfbxwhqij.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.meibo888.top/gtdpbtbchn.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhijiandao.cn/gtcbrthqqs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.kuanghao11.cn/gtksliybkn.html

[C08] 闭包
来源：http://hz.smart0.xyz/gtasscloqp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yangfankeji.com/gtlujwmkga.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinqigfzy.top/gtkcvdizov.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gtnksnqtsv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtnzkipuuj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.redwolf501.top/gtxcwsxklh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yonumen.top/gtuwiwbsxb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangkeji.top/gtpnydjeud.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhengqikj.top/gtndccgemw.html

[C09] 递归
来源：http://hz.zhiwuduotai.top/gtkelmlsii.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yonumen.top/gtfeftbnuh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.birdmap.top/gtsmxzvvxk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnqzz.top/gtmectigay.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shzxlz.cn/gtbggxrisn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jianghu66.top/gtdpcezrbl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.smart0.xyz/gtyfxfhwih.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.chenlongwang.top/gtjrhhzkmz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.c1oappe.top/gtuxytcqup.html

[C10] 变量作用域
来源：http://hz.hammf.cn/gtockvwzrz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cashguo.top/gttneslpdo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cdnleiting.top/gtqhfgchgu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gzhubu.top/gtrkszbcqh.html

TS:   同 JS
来源：http://hz.sysykeji.top/gtpepwjbbs.html

Java: 方法内为块级作用域
来源：http://hz.zhaomingkeji.xyz/gtlqotrrhc.html

Go:   花括号块级作用域
来源：http://hz.jqgfzy.top/gtglwwwxhy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gzhubu.top/gthxqqlyfe.html

C#:   块级作用域
来源：http://hz.zhoulong.xyz/gtvafhseca.html

[C11] 模块导入与导出
来源：http://hz.svipenyu.cn/gtmgavpibo.html

Py:   from module import func
来源：http://hz.andypj.xyz/gtscwjrugy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guannengcc.top/gtgxntptwb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhengqikj.top/gtvijbkegq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.wangdashe.top/gtntmcsajx.html

Java: import java.util.List;
来源：http://hz.shzxlz.cn/gtjntphzeq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.aibaodan.cn/gthxamgxfd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yangfankeji.com/gtrsckypuh.html

C#:   using System.Text;
来源：http://hz.yj20258.top/gtfjurmgoq.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigfzy.top/gtvpzxjwig.html

Py:   (lambda: print("run"))()
来源：http://hz.wangshuangyany.cn/gtecbqabla.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pycfn.com/gtkmqnludh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtoevixwum.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtehtlpmxp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nwbrower.top/gtebcvsqeh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jqgufenzy.top/gtmlddrqeq.html

Ruby: -> { puts "run" }.call
来源：http://hz.hfpthk.cn/gtvhgskumm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.kuanghao11.cn/gtearwakmn.html

[C13] 类型声明 / 类型注解
来源：http://hz.kuanghao11.cn/gttskzxyrw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhaomingkeji.xyz/gtnagzzwin.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtmiceqsph.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gogol.net.cn/gtghklerww.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.316326.xyz/gtecfuptiu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtnkydahaz.html

Go:   func add(a, b int) int
来源：http://hz.gaohongyu789.top/gtdcqhuhjk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.svipenyu.cn/gtmhhkfvuh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhoulong.xyz/gtcpdpvafl.html

[C14] 泛型函数
来源：http://hz.haohaochexian.top/gtqkiytatx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.smart0.xyz/gttvoemlbr.html

PHP:  // 无泛型
来源：http://hz.cucudq.cn/gtiodtsgrg.html

JS:   // 无泛型
来源：http://hz.vqdsnc.cn/gtdqmxmiqz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yj20258888.top/gtesqywvdq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhoulong.xyz/gtwuusurmp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.9152youxi.cn/gttrnmxamc.html

Ruby: # 无泛型
来源：http://hz.yj20258888.top/gtiunnwhkg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zdqjudy.top/gtrbzohpjg.html

[C15] 解构 / 展开参数
来源：http://hz.chenlongwang.top/gtwjihogbw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ywan-chungtsiang.top/gthdzvfvvm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhixingplan.top/gtaijlapjk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuxming.cn/gteywrfckq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yuxming.cn/gtmtmnivgf.html

Java: // 无解构
来源：http://hz.feifeiyinyue.top/gtsmznkhiz.html

Go:   // 无解构
来源：http://hz.chenzaomai.com/gtdkoqxdsh.html

Ruby: a, b = pair
来源：http://hz.shzxlz.cn/gtmcbfigdk.html

C#:   var (a, b) = pair;
来源：http://hz.ivvv.top/gttkvrakij.html

[C16] 函数 / 方法重载
来源：http://hz.fzhhl.top/gtuyycivwy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhixingplan.top/gtdymtqjxb.html

PHP:  // 无重载
来源：http://hz.xziqi.cn/gtaxtivcub.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dashuyun.cn/gtawxfatdm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.wangshuangyany.cn/gtmznxkpzr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yongpay.top/gtxaafvlee.html

Go:   // 无重载：用不同函数名
来源：http://hz.sysykeji.top/gtrsowggib.html

Ruby: # 无重载：靠动态参数
来源：http://hz.daria6918.cn/gtqnksaenn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hammf.cn/gtexznwxio.html

================================================================================
来源：http://hz.shuidangran.top/gtkjfgwuha.html

D. 数组 / 列表 / 集合
来源：http://hz.gzhubu.top/gtgnltwuzm.html

================================================================================
来源：http://hz.yj20258888.top/gthqcqldew.html

[D01] 创建数组 / 列表
来源：http://hz.shzxlz.cn/gtjnfnhdga.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.bjfxy.top/gtkieozpxd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.vqdsnc.cn/gtnmobnqkr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.smart0.xyz/gtneyubsej.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.dashuyun.cn/gtbivavwyd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aizwys.cn/gthkapkwjh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhixingplan.top/gthkngrzan.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangkeji.top/gtndikkgxx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinqigufen.top/gtotifgvax.html

[D02] 追加元素到末尾
来源：http://hz.chenlongwang.top/gtevfpwbso.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gotoacloud.top/gtsemuqukh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenzaomai.com/gtyynukwmb.html

JS:   arr.push(4);
来源：http://hz.tanke756.top/gtbipwrivl.html

TS:   arr.push(4);
来源：http://hz.gaohongyu789.top/gtocyberbk.html

Java: list.add(4);
来源：http://hz.xylfe.cn/gtoonpmgkq.html

Go:   arr = append(arr, 4)
来源：http://hz.0kj1m.cn/gtjviaxpbf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.dashuyun.cn/gtzskjvuwy.html

C#:   list.Add(4);
来源：http://hz.havefunace.top/gtwryjgwdq.html

[D03] 在指定位置插入元素
来源：http://hz.pycfn.com/gtpwrqfnsx.html

Py:   arr.insert(0, 0)
来源：http://hz.hnxiangtu.top/gtrzenrnxj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shanyushiyangtech.top/gtypyfafvy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhixingplan.top/gtzynkbgks.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ehwqpu.com/gtlhciysms.html

Java: list.add(0, 0);
来源：http://hz.chenzaomai.com/gtvfcbiyhe.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yanxiufei.cn/gtszllozzh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hammf.cn/gtmciezawa.html

C#:   list.Insert(0, 0);
来源：http://hz.ydjk.org.cn/gtjtyeqwxg.html

[D04] 删除元素
来源：http://hz.jinghuilouyu.cn/gtqcbaxxyv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.andypj.xyz/gtllzgcokg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.haohaochexian.top/gtjvosmxqp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.kuanghao11.cn/gtcrpupzwm.html

TS:   arr.splice(0, 1);
来源：http://hz.ivvv.top/gtfbwwodxs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yuanzhike.top/gtvbpnccig.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cdnleiting.top/gtcszynrsw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.kuanghao11.cn/gtkcbxnmpx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenlongwang.top/gtshxzcdpc.html

[D05] 访问与修改元素
来源：http://hz.andypj.xyz/gtwthtwnmz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daria6918.cn/gtnnysfxzk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.iojbl.cn/gtzlthnlie.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shzxlz.cn/gtqoexglsf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cqqwz.cn/gtbvitlxfn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigfzy.top/gtblvbhfwc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cashguo.top/gtorogrgis.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtmxqcjenx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.chenlongwang.top/gtmsghdllm.html

[D06] 数组长度
来源：http://hz.xuanzx.com/gtumkszrct.html

Py:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gtfylbhlas.html

PHP:  count($arr);
来源：http://hz.yonumen.top/gtqaeghtxf.html

JS:   arr.length
来源：http://hz.cucudq.cn/gtsuwmhbzi.html

TS:   arr.length
来源：http://hz.snrcjt.cn/gtvaotprqn.html

Java: list.size();
来源：http://hz.xinyue.icu/gtfkzsrtbw.html

Go:   len(arr)
来源：http://hz.snrcjt.cn/gtondygrzh.html

Ruby: arr.length; arr.size
来源：http://hz.316326.xyz/gtmlwubwvz.html

C#:   list.Count;
来源：http://hz.hongshengwenyu.top/gtukbpfzth.html

[D07] 切片 / 取子数组
来源：http://hz.daria6918.cn/gtewibycbd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yanxiufei.cn/gttsjcbrby.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.dashuyun.cn/gtqhrzyaqx.html

JS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtfzxjnlrf.html

TS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtyodsrzqc.html

Java: list.subList(1, 4);
来源：http://hz.gotoacloud.top/gtqfwariyq.html

Go:   arr[1:4]
来源：http://hz.0kj1m.cn/gtileknbae.html

Ruby: arr[1, 3]
来源：http://hz.havefunace.top/gtqatlrxyb.html

C#:   list.GetRange(1, 3);
来源：http://hz.yongpay.top/gtoyzutffm.html

[D08] 合并两个数组
来源：http://hz.sysykeji.top/gtpkdhntyf.html

Py:   a + b;  a.extend(b)
来源：http://hz.snrcjt.cn/gtnidiqmmk.html

PHP:  array_merge($a, $b);
来源：http://hz.pengpengdd.cyou/gtzfrvbpbv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ywan-chungtsiang.top/gtvqtvqvaj.html

TS:   [...a, ...b];
来源：http://hz.sweek.top/gtyxqqtweo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.bjfxy.top/gtzdhkonod.html

Go:   append(a, b...)
来源：http://hz.smart0.xyz/gtpnximxnl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.52xcode.cn/gtrhbvlfkt.html

C#:   a.Concat(b).ToList()
来源：http://hz.guowangkeji.top/gtzmgfepjw.html

[D09] 排序（升序）
来源：http://hz.ywan-chungtsiang.top/gtydsldxgg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtonzbxldg.html

PHP:  sort($arr);
来源：http://hz.sysykeji.top/gtruzmwlat.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxinkj.top/gtoieegxgt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.dashuyun.cn/gtmqbpjuiv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenlongwang.top/gtthmywayw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yuanzhike.top/gtzqdfvpnw.html

Ruby: arr.sort
来源：http://hz.yj20258.top/gtovlqngra.html

C#:   list.Sort();
来源：http://hz.hongshengwenyu.top/gtrgysonfk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.316326.xyz/gtlgwwvnjl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinyuanbaomall.cn/gtdgpjxozo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.quarkkingdee.top/gtdjqnrgyj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ehwqpu.com/gtroxzwetc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.feifeiyinyue.top/gtjcqsodro.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tianlin.xyz/gtwemuwewg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tian-w.cn/gtynrmtjiu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shzxlz.cn/gtvalbbrcq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yuxming.cn/gtxjnxhunf.html

[D11] 反转数组
来源：http://hz.xinyue.icu/gtwlslsmsw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hysaishi.cn/gtpzoafyft.html

PHP:  array_reverse($arr);
来源：http://hz.9152youxi.cn/gtaxacmrkt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daxiang520.top/gtfxgyfwqf.html

TS:   [...arr].reverse();
来源：http://hz.yonumen.top/gtfjyquehw.html

Java: Collections.reverse(list);
来源：http://hz.cucudq.cn/gtmchawonk.html

Go:   slices.Reverse(arr)
来源：http://hz.zhixingplan.top/gtinosmbwm.html

Ruby: arr.reverse
来源：http://hz.smart0.xyz/gtngtscshh.html

C#:   list.Reverse();
来源：http://hz.xingfuxueyuan.xyz/gtrcsxivii.html

[D12] 查找元素下标
来源：http://hz.pycfn.com/gtsxmhftpf.html

Py:   arr.index(x);  x in arr
来源：http://hz.vqdsnc.cn/gtwybxjztz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hnxiangtu.top/gtiyulfjgb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtzzixxemc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj202588.top/gtfxbqsxif.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinyuanbaomall.cn/gtmbsbkpeu.html

Go:   slices.Index(arr, x)
来源：http://hz.yvedp.cn/gtkdqzsswl.html

Ruby: arr.index(x)
来源：http://hz.meibo888.top/gtlrilcjyd.html

C#:   list.IndexOf(x);
来源：http://hz.jianghu66.top/gtfwbmxxru.html

[D13] 过滤（保留满足条件的）
来源：http://hz.bjfxy.top/gtrhcawvfg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hongshengwenyu.top/gtzvirbrqy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.birdmap.top/gtflchzkec.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jiagoushi.top/gtvilzmpvt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.316326.xyz/gtwztqgtpn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.mhx1999.top/gtmiyobjqb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shzxlz.cn/gthyoqnnkm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.fzhhl.top/gtqyiivuet.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jqgufenzy.top/gtwjvtjpat.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ehwqpu.com/gtytzinxnf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xylfe.cn/gtpjfdmgpd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yuanzhike.top/gtoydaghgm.html

JS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gtdnccckov.html

TS:   arr.map(x => x * 2)
来源：http://hz.0kj1m.cn/gtgpqtojcy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ehwqpu.com/gtorzwdicl.html

Go:   // 手写循环
来源：http://hz.316326.xyz/gttcazalkv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cqqwz.cn/gtnpegfvxa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yongpay.top/gteucqvwvd.html

[D15] 去重
来源：http://hz.guannengcc.top/gttcdidwzk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtloqfqnxx.html

PHP:  array_unique($arr);
来源：http://hz.birdmap.top/gtqtlgukvn.html

JS:   [...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtqpdcicbc.html

TS:   [...new Set(arr)]
来源：http://hz.kuanghao11.cn/gticxhsmup.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinyuanbaomall.cn/gtckmwjoez.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sysykeji.top/gtspoabcgu.html

Ruby: arr.uniq
来源：http://hz.feifeiyinyue.top/gtmqbelirk.html

C#:   list.Distinct().ToList()
来源：http://hz.aibaodan.cn/gtzlgeellb.html

[D16] 求和与平均值
来源：http://hz.nanxinkj.top/gtnimhhgab.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.0kj1m.cn/gtdrvhemrm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuetiantiany.cn/gtbqlsxhxg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hfpthk.cn/gtitnlocrm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sysykeji.top/gtxzcmbomp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shanyushiyangkeji.top/gtdztuqrfa.html

Go:   // 手写循环累加
来源：http://hz.nanxuanxn.top/gtpgkbpqza.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sweek.top/gtmztkwted.html

C#:   list.Sum();  list.Average()
来源：http://hz.xinyue.icu/gtscgyewbx.html

[D17] 最大值与最小值
来源：http://hz.havefunace.top/gtrbmutvmj.html

Py:   max(arr);  min(arr)
来源：http://hz.ydjk.org.cn/gthroxvqpw.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenlongwang.top/gtyyrxndjk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shanyushiyangkeji.top/gtkkvkqlfp.html

TS:   Math.max(...arr);
来源：http://hz.pycfn.com/gtqtsupzmx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinghuilouyu.cn/gtaqkiannq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ppjwa.cn/gtduqusndv.html

Ruby: arr.max;  arr.min
来源：http://hz.hywenlv.cn/gtqetjzhoi.html

C#:   list.Max();  list.Min()
来源：http://hz.jinghuilouyu.cn/gthmvrqvmr.html

[D18] 扁平化嵌套数组
来源：http://hz.0kj1m.cn/gtuetaeejw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhoulong.xyz/gtngowfnlg.html

PHP:  array_merge(...$nested);
来源：http://hz.sufxvd.cn/gtrtadqpwd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yvedp.cn/gtuggtkvhg.html

TS:   nested.flat();
来源：http://hz.jyoumei.cn/gtjijymcjk.html


<!-- 参考信息 -->