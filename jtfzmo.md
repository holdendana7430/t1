代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgfzy.top/gtmaeggvra.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.kuanghao11.cn/gtcxejcxhm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hfpthk.cn/gtiqwlywrv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.haohaochexian.top/gtkckbajpw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinqigfzy.top/gtuuhirtac.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hongshengwenyu.top/gtaikjggnt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.birdmap.top/gtcozvsuoe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinghuilouyu.cn/gtnpfrjkyl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cucudq.cn/gtrhaictox.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gttjscsgmp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.bjfxy.top/gtxnlbamkz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.wangshuangyany.cn/gtgdkbeict.html

Go:   // 无：用配置结构体参数
来源：http://hz.hnxiangtu.top/gtcmufxrjd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tianlin.xyz/gtyyfczeut.html

C#:   f(a: 1, b: 2)
来源：http://hz.havefunace.top/gtjjqgzqac.html

[C05] 返回多个值
来源：http://hz.cucudq.cn/gthvyynfzx.html

Py:   return a, b
来源：http://hz.gogol.net.cn/gtqsjxrkmj.html

PHP:  return [$a, $b];
来源：http://hz.cheryme.top/gtjzxmupgs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zycfv.cn/gtsmfpfhxo.html

TS:   return { a, b };
来源：http://hz.xuetiantiany.cn/gtqjngmklg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.aibaodan.cn/gtyhpfzutc.html

Go:   return a, b
来源：http://hz.bjfxy.top/gtvtovxwzt.html

Ruby: return a, b
来源：http://hz.zhiwuduotai.top/gtkdasxjmd.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gogol.net.cn/gtbekqrlki.html

[C06] 匿名函数 / lambda
来源：http://hz.zhiwuduotai.top/gtlbbqtowr.html

Py:   square = lambda x: x * x
来源：http://hz.ywan-chungtsiang.top/gtlqqwnswy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhixingplan.top/gtdmnvdobj.html

JS:   const square = x => x * x;
来源：http://hz.jinqigufen.top/gtqkycreza.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuanzhike.top/gtnifggooi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.meibo888.top/gtyiowtpbu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhijiandao.cn/gtajtcaind.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jlsjyb.cn/gtuykwqfay.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jqgufenzy.top/gtddbewwyw.html

[C07] 把函数作为参数传入
来源：http://hz.chenlongwang.top/gticmavcjm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cheryme.top/gtenjpoypn.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ppjwa.cn/gttofnruxr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xziqi.cn/gtypiqekhx.html

TS:   arr.map(String)
来源：http://hz.jinyuanbaomall.cn/gtbqrwnczy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.pycfn.com/gtgrrhpaae.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gzhubu.top/gtjoiqgiea.html

Ruby: arr.map(&:upcase)
来源：http://hz.havefunace.top/gtofmoholm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zycfv.cn/gtpjkmacsm.html

[C08] 闭包
来源：http://hz.sxryk.cn/gtjjagakwp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.bjfxy.top/gteegvbbih.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jianghu66.top/gtyqindgjw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xylfe.cn/gtrfiyjgfa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtawuhosdc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ydzc1.top/gtrybhgfli.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sufxvd.cn/gtfzyjjhym.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangtech.top/gtotwszvrj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gttduxmcei.html

[C09] 递归
来源：http://hz.zhoulong.xyz/gtmayxxecd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yvedp.cn/gtvnjmldga.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sysykeji.top/gtltecelex.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.haohaochexian.top/gthpvvtwse.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gtolrgowpq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shuidangran.top/gtutwgqrwq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.guannengcc.top/gtfktikodq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.smart0.xyz/gthebbpddr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yanxiufei.cn/gtilqagdzq.html

[C10] 变量作用域
来源：http://hz.shanyushiyangkeji.top/gtkihjoejn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhiwuduotai.top/gtsibaahwe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinghuilouyu.cn/gtsnwqelno.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.0kj1m.cn/gtkijrgbak.html

TS:   同 JS
来源：http://hz.jiagoushi.top/gtaxzdljrp.html

Java: 方法内为块级作用域
来源：http://hz.hnxiangtu.top/gtzchpwcvw.html

Go:   花括号块级作用域
来源：http://hz.nanxuanxn.top/gtmszoosrf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jqgfzy.top/gttcllmjmq.html

C#:   块级作用域
来源：http://hz.andypj.xyz/gtxrwfbrep.html

[C11] 模块导入与导出
来源：http://hz.jinghuilouyu.cn/gtzbawupow.html

Py:   from module import func
来源：http://hz.zhengqikj.top/gtdomohtqz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cheryme.top/gtwwibyfdt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnqzz.top/gtdttggnuh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fengsongda.top/gtcapjsvqz.html

Java: import java.util.List;
来源：http://hz.ybcxt.top/gtttgxvghh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj20258888.top/gtzywcbeua.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yonumen.top/gtpwulihub.html

C#:   using System.Text;
来源：http://hz.zhijiandao.cn/gtmpdbqnot.html

[C12] 立即执行函数 IIFE
来源：http://hz.yonumen.top/gtkwykbrof.html

Py:   (lambda: print("run"))()
来源：http://hz.nwbrower.top/gtqlupjflp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhiwuduotai.top/gtuglbfifg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.birdmap.top/gtelatpltt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guannengcc.top/gtfteypgwd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daxiang520.top/gtmrbqmqab.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gaohongyu789.top/gtwumisanx.html

Ruby: -> { puts "run" }.call
来源：http://hz.jqgfzy.top/gtekjjkxrr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.chenlongwang.top/gtmnsufmxi.html

[C13] 类型声明 / 类型注解
来源：http://hz.havefunace.top/gtdivvmyeb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cucudq.cn/gtxoophpaf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gthmldiqch.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.guowangkeji.top/gtytxipjed.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtqlfrevou.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtkcihlmjn.html

Go:   func add(a, b int) int
来源：http://hz.sufxvd.cn/gttnudomou.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydjk.org.cn/gtkkkqxuoh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.0kj1m.cn/gtgzcyovfm.html

[C14] 泛型函数
来源：http://hz.meibo888.top/gtsigtclpw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gogol.net.cn/gtbchhjcxr.html

PHP:  // 无泛型
来源：http://hz.zhoulong.xyz/gtkkucpept.html

JS:   // 无泛型
来源：http://hz.nwbrower.top/gthgpdmcsh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xziqi.cn/gtsbmshtkr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigfzy.top/gtzbslatqp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yangfankeji.com/gtqstfpvyl.html

Ruby: # 无泛型
来源：http://hz.jqgufenzy.top/gtyqmjxypb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sufxvd.cn/gtqjbyscsu.html

[C15] 解构 / 展开参数
来源：http://hz.jinghuilouyu.cn/gttnvxhxbo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jqgfzy.top/gtumxwlxus.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhijiandao.cn/gthusfgcxz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sxryk.cn/gtixamscrp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hammf.cn/gtmijwwezi.html

Java: // 无解构
来源：http://hz.havefunace.top/gtzqosplby.html

Go:   // 无解构
来源：http://hz.wangshuangyany.cn/gtrednfjiy.html

Ruby: a, b = pair
来源：http://hz.xingfuxueyuan.xyz/gtynffernv.html

C#:   var (a, b) = pair;
来源：http://hz.tianlin.xyz/gtoiiauotv.html

[C16] 函数 / 方法重载
来源：http://hz.yongpay.top/gtrojyecaj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.kuanghao11.cn/gteaweajrb.html

PHP:  // 无重载
来源：http://hz.aizwys.cn/gtxkiedenl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.havefunace.top/gtwrbaunro.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xingfuxueyuan.xyz/gtpinubqjx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gzhubu.top/gtxqnhhwtr.html

Go:   // 无重载：用不同函数名
来源：http://hz.jiagoushi.top/gtlxlcajyq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuanzhike.top/gtxrljwuwc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xuetiantiany.cn/gtbxdvkmtn.html

================================================================================
来源：http://hz.cheryme.top/gtrrxwuzfh.html

D. 数组 / 列表 / 集合
来源：http://hz.52xcode.cn/gtlvrobxmf.html

================================================================================
来源：http://hz.ehwqpu.com/gtgslkazdk.html

[D01] 创建数组 / 列表
来源：http://hz.feifeiyinyue.top/gtmxwjxvdk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhiwuduotai.top/gtfmzoemtv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hysaishi.cn/gtrafvdazs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ppjwa.cn/gtgsjqxgps.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xziqi.cn/gtstirzdyq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shangyingyoupin.top/gtsqlajeft.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.316326.xyz/gtajzwqiko.html

Ruby: arr = [1, 2, 3]
来源：http://hz.316326.xyz/gtiekiqnuv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tanke756.top/gtcliqrhoy.html

[D02] 追加元素到末尾
来源：http://hz.yj20258.top/gtmguytnsn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gzhubu.top/gtqycaiohe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aibaodan.cn/gtcjiihhyo.html

JS:   arr.push(4);
来源：http://hz.316326.xyz/gtzdhopmxz.html

TS:   arr.push(4);
来源：http://hz.hongshengwenyu.top/gtlbnpklxm.html

Java: list.add(4);
来源：http://hz.yj202588.top/gtfvxrjahb.html

Go:   arr = append(arr, 4)
来源：http://hz.cucudq.cn/gtkwzeqeyy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xinyue.icu/gtstyartcu.html

C#:   list.Add(4);
来源：http://hz.zdqjudy.top/gtetpdnbrh.html

[D03] 在指定位置插入元素
来源：http://hz.jlsjyb.cn/gtiutiiloc.html

Py:   arr.insert(0, 0)
来源：http://hz.hnqzz.top/gtdbhslkat.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.daxiang520.top/gtywfxabkl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinghuilouyu.cn/gtnkvoygyz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shanyushiyangkeji.top/gtcqhkinfp.html

Java: list.add(0, 0);
来源：http://hz.chenjidiqi.icu/gttdbqdbai.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.nanxuanxn.top/gtqrxpnsct.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gogol.net.cn/gtjrdjlwsj.html

C#:   list.Insert(0, 0);
来源：http://hz.pycfn.com/gtuuluaedv.html

[D04] 删除元素
来源：http://hz.gzhubu.top/gtuyrcflhh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinqigfzy.top/gtsyjibrfb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenlongwang.top/gtggnwyavu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ywan-chungtsiang.top/gtxnrhafin.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigfzy.top/gtyzcozzis.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.feifeiyinyue.top/gtllmwblzm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yongpay.top/gtvmsnregu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hammf.cn/gtkmnzxsem.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhongyouzk.top/gtuvonnpfn.html

[D05] 访问与修改元素
来源：http://hz.havefunace.top/gtjiyneklr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gtbdrisxjw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sxryk.cn/gtqzmwskhg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jyoumei.cn/gtrphsyjcs.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.birdmap.top/gtrgyhdlpr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj20258.top/gtfcfduugu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cashguo.top/gtcqttscav.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tian-w.cn/gtosqdgsql.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhengqikj.top/gtrqdkwmpm.html

[D06] 数组长度
来源：http://hz.dashuyun.cn/gtdzskjusi.html

Py:   len(arr)
来源：http://hz.cheryme.top/gtfahrsxne.html

PHP:  count($arr);
来源：http://hz.gzhubu.top/gtszpybqki.html

JS:   arr.length
来源：http://hz.jiagoushi.top/gtnfzdjorn.html

TS:   arr.length
来源：http://hz.jyoumei.cn/gtdurdhbdz.html

Java: list.size();
来源：http://hz.kuanghao11.cn/gtabxkfqrg.html

Go:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gthxtwcyma.html

Ruby: arr.length; arr.size
来源：http://hz.wangshuangyany.cn/gtzcxxukth.html

C#:   list.Count;
来源：http://hz.jinqigufen.top/gtsbhwymwr.html

[D07] 切片 / 取子数组
来源：http://hz.yanxiufei.cn/gtahaqrruj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xziqi.cn/gtqvopmims.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.redwolf501.top/gtzxevavwg.html

JS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gtyllmvfzt.html

TS:   arr.slice(1, 4);
来源：http://hz.hnxiangtu.top/gtrvwxxfxd.html

Java: list.subList(1, 4);
来源：http://hz.cqqwz.cn/gtnwaeupsv.html

Go:   arr[1:4]
来源：http://hz.pengpengdd.cyou/gtwkceuhtm.html

Ruby: arr[1, 3]
来源：http://hz.nanxinkj.top/gtlrhziihb.html

C#:   list.GetRange(1, 3);
来源：http://hz.jqgfzy.top/gttshcftpy.html

[D08] 合并两个数组
来源：http://hz.9152youxi.cn/gtfimvhkmr.html

Py:   a + b;  a.extend(b)
来源：http://hz.yangfankeji.com/gtxuwfakbt.html

PHP:  array_merge($a, $b);
来源：http://hz.yj202588.top/gtorghadpt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hongshengwenyu.top/gtigbsmhbd.html

TS:   [...a, ...b];
来源：http://hz.gzhubu.top/gtdxrophzl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gtvbudfogt.html

Go:   append(a, b...)
来源：http://hz.ppjwa.cn/gtcuxptcoh.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xylfe.cn/gtecwwoznv.html

C#:   a.Concat(b).ToList()
来源：http://hz.nanxinkj.top/gtooxrkvrr.html

[D09] 排序（升序）
来源：http://hz.ehwqpu.com/gtithegiyr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtfjububfs.html

PHP:  sort($arr);
来源：http://hz.316326.xyz/gtsqljuhml.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jianghu66.top/gtqftpeumk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xingfuxueyuan.xyz/gtntrztkqj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgfzy.top/gtncxbqrfz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.316326.xyz/gtkqdquzqz.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gtywqnvalf.html

C#:   list.Sort();
来源：http://hz.xingfuxueyuan.xyz/gtrxxxutfh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hywenlv.cn/gtornuzaaa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aizwys.cn/gtwdhqddvd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.meibo888.top/gtlzuhvpzw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gotoacloud.top/gtakpjfpri.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gtxmosmnmy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yanxiufei.cn/gtixntjwnw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shanyushiyangkeji.top/gtrrdjzggt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gotoacloud.top/gtcrzgqwdc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinghuilouyu.cn/gtiwspzeao.html

[D11] 反转数组
来源：http://hz.dianchejie.cn/gtkutbnjvm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhengqikj.top/gtuvlimqwz.html

PHP:  array_reverse($arr);
来源：http://hz.sxryk.cn/gtbufqqesu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yanxiufei.cn/gtligttnmx.html

TS:   [...arr].reverse();
来源：http://hz.chenjidiqi.icu/gtezpffubh.html

Java: Collections.reverse(list);
来源：http://hz.yonumen.top/gtxuddobfi.html

Go:   slices.Reverse(arr)
来源：http://hz.sysykeji.top/gtldjiqzww.html

Ruby: arr.reverse
来源：http://hz.hnqzz.top/gtmcqzpybf.html

C#:   list.Reverse();
来源：http://hz.aibaodan.cn/gtqdrfoehp.html

[D12] 查找元素下标
来源：http://hz.pengpengdd.cyou/gtshvntifl.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhaomingkeji.xyz/gtpimttawn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ivvv.top/gtqavrcpmh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnxiangtu.top/gtwqjfifyt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtujtfkybo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yuxming.cn/gtgkprunrg.html

Go:   slices.Index(arr, x)
来源：http://hz.nwbrower.top/gtudhlledv.html

Ruby: arr.index(x)
来源：http://hz.jianghu66.top/gtfmfsszvn.html

C#:   list.IndexOf(x);
来源：http://hz.nanxinkj.top/gtahpyscux.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jiagoushi.top/gttttcxdrl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jianghu66.top/gttvilvonj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.316326.xyz/gtsknrqyym.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jiagoushi.top/gttiaqwmhb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sxryk.cn/gtvmvlsipz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.kuanghao11.cn/gtpixkniop.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.guowangkeji.top/gtunszmtqp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ehwqpu.com/gtourpcneq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gotoacloud.top/gtguylgddg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.daxiang520.top/gtyoxcjnrz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.dashuyun.cn/gtlaboqxrf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.bjfxy.top/gtriyexvfr.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangtech.top/gtbpsymqkf.html

TS:   arr.map(x => x * 2)
来源：http://hz.0kj1m.cn/gtehsxqlsf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinghuilouyu.cn/gtorpprsys.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtzsiprrpk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jianghu66.top/gtpbvafyvq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shanyushiyangkeji.top/gtutoexrzf.html

[D15] 去重
来源：http://hz.jinqigufen.top/gtsmodopqa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.quarkkingdee.top/gtvleqsdnx.html

PHP:  array_unique($arr);
来源：http://hz.xingfuxueyuan.xyz/gtclsspvdw.html

JS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtqxlujedg.html

TS:   [...new Set(arr)]
来源：http://hz.yuanzhike.top/gtkdhyrqma.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtugeqhwmd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tian-w.cn/gtkdglgcpj.html

Ruby: arr.uniq
来源：http://hz.gzhubu.top/gtqptnrxof.html

C#:   list.Distinct().ToList()
来源：http://hz.jlsjyb.cn/gtqmhncrcy.html

[D16] 求和与平均值
来源：http://hz.gzhubu.top/gtiyxhaais.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shuidangran.top/gtppfpczkm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenlongwang.top/gtrjadnzuu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhixingplan.top/gthfqapbdb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtqjolszrc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xylfe.cn/gtfdzhopck.html

Go:   // 手写循环累加
来源：http://hz.yvedp.cn/gtueszopnj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hywenlv.cn/gtslwueylq.html

C#:   list.Sum();  list.Average()
来源：http://hz.ppjwa.cn/gtywcngyjl.html

[D17] 最大值与最小值
来源：http://hz.ydzc1.top/gttjknkkwv.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgfzy.top/gtlngznufh.html

PHP:  max($arr);  min($arr);
来源：http://hz.shanyushiyangtech.top/gthvcxdzxg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fzhhl.top/gtihrvaezk.html

TS:   Math.max(...arr);
来源：http://hz.aizwys.cn/gteowlndaf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.9152youxi.cn/gtstyojcqw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.quarkkingdee.top/gtzorkkexo.html

Ruby: arr.max;  arr.min
来源：http://hz.zhaomingkeji.xyz/gtfabmstof.html

C#:   list.Max();  list.Min()
来源：http://hz.jyoumei.cn/gtvmrwuxng.html

[D18] 扁平化嵌套数组
来源：http://hz.xinyue.icu/gttkivrtgt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xylfe.cn/gtelhsvpgv.html

PHP:  array_merge(...$nested);
来源：http://hz.9152youxi.cn/gtyekgznyt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.pengpengdd.cyou/gtqfomzefb.html

TS:   nested.flat();
来源：http://hz.ywan-chungtsiang.top/gtrzezwqkl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.meibo888.top/gtawvdszbz.html

Go:   // 手写双层循环
来源：http://hz.yangfankeji.com/gtzniehsdd.html

Ruby: nested.flatten
来源：http://hz.tian-w.cn/gtefvmzddh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shanyushiyangtech.top/gthirwgjdz.html

[D19] 按字段分组
来源：http://hz.hongshengwenyu.top/gthiognaoo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ydjk.org.cn/gtsyetpqvg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.quarkkingdee.top/gtrweqimxn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.fzhhl.top/gtkyrhsvdn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sxryk.cn/gtiotvqvvb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ivvv.top/gtuyucenwm.html

Go:   // 手写 map[string][]T
来源：http://hz.hammf.cn/gtykqsrlyj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yongpay.top/gtnijvaoae.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sysykeji.top/gtigylajfc.html

[D20] 统计每个元素出现次数
来源：http://hz.wangshuangyany.cn/gthrifirld.html

Py:   Counter(arr)
来源：http://hz.dashuyun.cn/gtsrsjpttf.html

PHP:  array_count_values($arr);
来源：http://hz.fzhhl.top/gtwttzhnum.html


<!-- 参考信息 -->