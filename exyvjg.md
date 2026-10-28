代发 wailian999

Py:   def add(a, b): return a + b
来源：http://hz.quarkkingdee.top/gtmzztxatr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtsuwwgsek.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.vqdsnc.cn/gthpxvxpmz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gttpjbwtfw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gtxyzsrnxy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.c1oappe.top/gtuhsmnslp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shuidangran.top/gtywdchjur.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gtotpmglfw.html

[C02] 默认参数
来源：http://hz.zycfv.cn/gteiqdqzsr.html

Py:   def greet(name="World"): return name
来源：http://hz.zhixingplan.top/gtnxpllmyg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.pycfn.com/gtbrutvqqn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.havefunace.top/gtfnhrqcww.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhixingplan.top/gtekilhjal.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xingfuxueyuan.xyz/gtejarjcqt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.0kj1m.cn/gtsprkxvbw.html

Ruby: def greet(name = "World") = name
来源：http://hz.dashuyun.cn/gtpqvmbzbc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.smart0.xyz/gtcbvnfcmc.html

[C03] 可变参数
来源：http://hz.sysykeji.top/gtuqgrxefs.html

Py:   def total(*args): return sum(args)
来源：http://hz.svipenyu.cn/gtlvnqpmmo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pengpengdd.cyou/gtmhouwkzm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxinkj.top/gtsdsyevnd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pycfn.com/gtctqdhjgg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.0kj1m.cn/gtpoqmqyss.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.pengpengdd.cyou/gtvsapydzj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj202588.top/gtuennwbae.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yj20258888.top/gtcdjlpazl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hywenlv.cn/gtngsdzcoh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.havefunace.top/gtzhntgbtv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hywenlv.cn/gtmrsnqtnr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtaxujlajn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sysykeji.top/gtatpipvlg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.fengsongda.top/gtvymsstpr.html

Go:   // 无：用配置结构体参数
来源：http://hz.ybcxt.top/gtmdzqzodv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sufxvd.cn/gtjievkbbt.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtpkquoirp.html

[C05] 返回多个值
来源：http://hz.316326.xyz/gtrscrthne.html

Py:   return a, b
来源：http://hz.52xcode.cn/gtjzfbutis.html

PHP:  return [$a, $b];
来源：http://hz.shanyushiyangkeji.top/gttjsvoecs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydjk.org.cn/gtwjuuvyzm.html

TS:   return { a, b };
来源：http://hz.yvedp.cn/gtfvntktzb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.snrcjt.cn/gticndgnap.html

Go:   return a, b
来源：http://hz.jiagoushi.top/gtwstmkvkm.html

Ruby: return a, b
来源：http://hz.aibaodan.cn/gtuydlzfco.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.316326.xyz/gtugbxkwvr.html

[C06] 匿名函数 / lambda
来源：http://hz.kuanghao11.cn/gtudwiwlml.html

Py:   square = lambda x: x * x
来源：http://hz.svipenyu.cn/gttrslsicy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zycfv.cn/gtfdnlnxuo.html

JS:   const square = x => x * x;
来源：http://hz.mhx1999.top/gtyjvknfny.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gaohongyu789.top/gtgddvtczv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yueranfly.top/gtbauthxzf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenlongwang.top/gtlctqkeyr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.bjfxy.top/gtpuxtegjt.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gaohongyu789.top/gtqueeegbw.html

[C07] 把函数作为参数传入
来源：http://hz.iojbl.cn/gtpdrpekrs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenjidiqi.icu/gtdlimnnat.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.wangshuangyany.cn/gtrgkswwgt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sxryk.cn/gtausjshwx.html

TS:   arr.map(String)
来源：http://hz.tian-w.cn/gtzzxhtvhg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.aizwys.cn/gthbegysdf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.fzhhl.top/gtbtsgmsnw.html

Ruby: arr.map(&:upcase)
来源：http://hz.sysykeji.top/gtjesljfpl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hongshengwenyu.top/gtmypdvlxb.html

[C08] 闭包
来源：http://hz.jinyuanbaomall.cn/gtaknuljki.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ivvv.top/gtitgktnpl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhoulong.xyz/gtyqperave.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.andypj.xyz/gtkqdacndw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yanxiufei.cn/gtnjefomkz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gaohongyu789.top/gtssbvmgty.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.havefunace.top/gtvegwouxp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.quarkkingdee.top/gtskwtbmzp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtuiasmsam.html

[C09] 递归
来源：http://hz.andypj.xyz/gtlsmiahds.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ydjk.org.cn/gtsrsaaiix.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.birdmap.top/gtafqpyhmy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gotoacloud.top/gtmqwhygsa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.mhx1999.top/gtprhrzucl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ydjk.org.cn/gtawsfrote.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.9152youxi.cn/gtuchvtmyi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tanke756.top/gtzethwhao.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.wangshuangyany.cn/gtxvpoenwc.html

[C10] 变量作用域
来源：http://hz.cdnleiting.top/gtlyfdnmmg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.bjfxy.top/gtdfwpoelz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.haohaochexian.top/gtogzknblu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shangyingyoupin.top/gtcdajjsct.html

TS:   同 JS
来源：http://hz.jqgufenzy.top/gtccbowrye.html

Java: 方法内为块级作用域
来源：http://hz.yongpay.top/gtlfjigaks.html

Go:   花括号块级作用域
来源：http://hz.hywenlv.cn/gtyoqygsgt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.wangshuangyany.cn/gtgwyzljnb.html

C#:   块级作用域
来源：http://hz.yj20258.top/gtfjnmzhix.html

[C11] 模块导入与导出
来源：http://hz.bjfxy.top/gtkfyegatm.html

Py:   from module import func
来源：http://hz.yj20258888.top/gtmwsqxucy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.mhx1999.top/gtluzxoagt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.svipenyu.cn/gttjirwyuw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cashguo.top/gtqmqlaotm.html

Java: import java.util.List;
来源：http://hz.ppjwa.cn/gtjcihxtye.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.snrcjt.cn/gtaeddgjzt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.tianlin.xyz/gtphcaadvn.html

C#:   using System.Text;
来源：http://hz.kuanghao11.cn/gtkmvgvcpg.html

[C12] 立即执行函数 IIFE
来源：http://hz.ywan-chungtsiang.top/gtddmfytzi.html

Py:   (lambda: print("run"))()
来源：http://hz.c1oappe.top/gtvrboodmi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.andypj.xyz/gtrdfnxcdd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydzc1.top/gtbfgdpxhl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tianlin.xyz/gtaqgjeava.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yonumen.top/gtzhvmxbdz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.daria6918.cn/gtqsrhldhn.html

Ruby: -> { puts "run" }.call
来源：http://hz.meibo888.top/gtxdmlfbdw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shanyushiyangtech.top/gtwlizmsbt.html

[C13] 类型声明 / 类型注解
来源：http://hz.haohaochexian.top/gtiltpjjio.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yuanzhike.top/gtyzchpffg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtzyswmiey.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.mhx1999.top/gtyeikkkdf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtrkyalpsc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtvxxwggne.html

Go:   func add(a, b int) int
来源：http://hz.yj20258.top/gtbzvdzppt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yangfankeji.com/gtuicktfsg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aibaodan.cn/gtredvndww.html

[C14] 泛型函数
来源：http://hz.nanxinkj.top/gtzpdbpacb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hfpthk.cn/gtjkgrftzp.html

PHP:  // 无泛型
来源：http://hz.shuidangran.top/gtptytqhww.html

JS:   // 无泛型
来源：http://hz.dashuyun.cn/gteycbbwjt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tianlin.xyz/gttlcfvdna.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cucudq.cn/gtygatiobi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.316326.xyz/gtorbvsfax.html

Ruby: # 无泛型
来源：http://hz.cheryme.top/gtggzwsdxq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guowangkeji.top/gtdpmlljyr.html

[C15] 解构 / 展开参数
来源：http://hz.aizwys.cn/gtqrkuebxu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gogol.net.cn/gtcoavolmc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.316326.xyz/gtsnfhhscp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jiagoushi.top/gtytpnnkvf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ivvv.top/gtnueyzuur.html

Java: // 无解构
来源：http://hz.yj20258888.top/gtyinwdpuc.html

Go:   // 无解构
来源：http://hz.jinqigfzy.top/gthdbqscsa.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtpshznioh.html

C#:   var (a, b) = pair;
来源：http://hz.ppjwa.cn/gtpxzvujhy.html

[C16] 函数 / 方法重载
来源：http://hz.xingfuxueyuan.xyz/gtlkhbjyuj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.316326.xyz/gtjwenzuuu.html

PHP:  // 无重载
来源：http://hz.yj20258.top/gthhxzubbt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nwbrower.top/gtgocrshok.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hywenlv.cn/gtkfwvliqh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cashguo.top/gtnlwmbgji.html

Go:   // 无重载：用不同函数名
来源：http://hz.daxiang520.top/gtlagqhdxz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cqqwz.cn/gtgpgfrjrz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.birdmap.top/gtctenwkhx.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtznnnsyam.html

D. 数组 / 列表 / 集合
来源：http://hz.shanyushiyangtech.top/gttwqijcsm.html

================================================================================
来源：http://hz.hammf.cn/gtxqxbknhi.html

[D01] 创建数组 / 列表
来源：http://hz.smart0.xyz/gtmsriqbju.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gogol.net.cn/gtvqanaehv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gogol.net.cn/gtzaelnbhc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xuetiantiany.cn/gtsuyhftsu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinqigfzy.top/gtiqhocjwh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guannengcc.top/gtjpejvlfc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.pengpengdd.cyou/gtaxniskdu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.guowangkeji.top/gtkhlfyodt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jianghu66.top/gtnpsyrdkl.html

[D02] 追加元素到末尾
来源：http://hz.jinghuilouyu.cn/gtdzvhgwjh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.meibo888.top/gtlzuiawny.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shzxlz.cn/gtnzculpus.html

JS:   arr.push(4);
来源：http://hz.yangfankeji.com/gtxgfojnvg.html

TS:   arr.push(4);
来源：http://hz.yj202588.top/gtznbvlpyz.html

Java: list.add(4);
来源：http://hz.yonumen.top/gttdebzqql.html

Go:   arr = append(arr, 4)
来源：http://hz.fzhhl.top/gtgmxmdsrt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shzxlz.cn/gtpgkrrzfr.html

C#:   list.Add(4);
来源：http://hz.sufxvd.cn/gtfwemhpfz.html

[D03] 在指定位置插入元素
来源：http://hz.tian-w.cn/gtljcryksx.html

Py:   arr.insert(0, 0)
来源：http://hz.ehwqpu.com/gtkokzinsp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xinyue.icu/gtjqgoqcrk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tianlin.xyz/gtazlpacpq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xingfuxueyuan.xyz/gtdkmfnklc.html

Java: list.add(0, 0);
来源：http://hz.0kj1m.cn/gtmyvvkfxv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.smart0.xyz/gtrnebpwnj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgufenzy.top/gtpxymlhjf.html

C#:   list.Insert(0, 0);
来源：http://hz.ywan-chungtsiang.top/gtcjnugole.html

[D04] 删除元素
来源：http://hz.jinqigufen.top/gthcrioggk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.pengpengdd.cyou/gtxxzjtslv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.nwbrower.top/gtzgrnnkbr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.c1oappe.top/gtxraicgjf.html

TS:   arr.splice(0, 1);
来源：http://hz.yongpay.top/gtxvcuqtlh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fengsongda.top/gtvyorhilq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xinyue.icu/gtnlbzvuln.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jianghu66.top/gtosvtwqqv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.0kj1m.cn/gtsgzddbbp.html

[D05] 访问与修改元素
来源：http://hz.tanke756.top/gtwpeslmvd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tian-w.cn/gthwqpicxa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gotoacloud.top/gtdzagfdbn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.snrcjt.cn/gterxgtbdp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhijiandao.cn/gtiqddojdi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guowangkeji.top/gtuyafpkla.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nwbrower.top/gtmruradtd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtyagyaxbw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sxryk.cn/gtjsyoogzu.html

[D06] 数组长度
来源：http://hz.pycfn.com/gtxfxkhtfl.html

Py:   len(arr)
来源：http://hz.gzhubu.top/gtsyvpjyuw.html

PHP:  count($arr);
来源：http://hz.bjfxy.top/gtuimlsnxc.html

JS:   arr.length
来源：http://hz.jianghu66.top/gtoebvchgc.html

TS:   arr.length
来源：http://hz.tian-w.cn/gtewgummls.html

Java: list.size();
来源：http://hz.316326.xyz/gtffwggrug.html

Go:   len(arr)
来源：http://hz.yueranfly.top/gtkvdtkysd.html

Ruby: arr.length; arr.size
来源：http://hz.pycfn.com/gtvwkgncgs.html

C#:   list.Count;
来源：http://hz.hywenlv.cn/gtxpwczaqj.html

[D07] 切片 / 取子数组
来源：http://hz.hywenlv.cn/gtkpdkeoip.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.tianlin.xyz/gtoxgysypg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhoulong.xyz/gticiibhfm.html

JS:   arr.slice(1, 4);
来源：http://hz.cashguo.top/gtxdlcvrpd.html

TS:   arr.slice(1, 4);
来源：http://hz.zhongyouzk.top/gtimlgmqft.html

Java: list.subList(1, 4);
来源：http://hz.fzhhl.top/gtdvdwwvvi.html

Go:   arr[1:4]
来源：http://hz.yuanzhike.top/gtvjhccnou.html

Ruby: arr[1, 3]
来源：http://hz.svipenyu.cn/gtfiioukgh.html

C#:   list.GetRange(1, 3);
来源：http://hz.svipenyu.cn/gtpvrnbrvc.html

[D08] 合并两个数组
来源：http://hz.yueranfly.top/gtdgzqkjeu.html

Py:   a + b;  a.extend(b)
来源：http://hz.tianlin.xyz/gtdgaxrhqv.html

PHP:  array_merge($a, $b);
来源：http://hz.zhijiandao.cn/gtenhlnoyg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xziqi.cn/gtgqociomb.html

TS:   [...a, ...b];
来源：http://hz.shangyingyoupin.top/gtjjxzajyx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhoulong.xyz/gtkntpspaj.html

Go:   append(a, b...)
来源：http://hz.aizwys.cn/gtvbqusqkm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenlongwang.top/gtcdbywvbo.html

C#:   a.Concat(b).ToList()
来源：http://hz.nanxinkj.top/gtywqoajjf.html

[D09] 排序（升序）
来源：http://hz.jianghu66.top/gtyttxbvfa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtxeomseza.html

PHP:  sort($arr);
来源：http://hz.hywenlv.cn/gtucrwplkj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhiwuduotai.top/gtivdajawa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.pengpengdd.cyou/gtgaxfgpsh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.316326.xyz/gtxzdoqnyz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.mhx1999.top/gtgixudhff.html

Ruby: arr.sort
来源：http://hz.svipenyu.cn/gttkjabjmw.html

C#:   list.Sort();
来源：http://hz.iojbl.cn/gtewmepjkx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xylfe.cn/gtjrilrelk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinyuanbaomall.cn/gtxshajpua.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yonumen.top/gtaigrtjqg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.0kj1m.cn/gtjxrjiwin.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangshuangyany.cn/gtqueofhzt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhongyouzk.top/gtdyizwlfl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.mhx1999.top/gtbdovlizh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jiagoushi.top/gtknqvjctr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.haohaochexian.top/gtxdnsngxo.html

[D11] 反转数组
来源：http://hz.shanyushiyangkeji.top/gtkktgcwst.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zycfv.cn/gtnqksvpqp.html

PHP:  array_reverse($arr);
来源：http://hz.hnqzz.top/gtzcktqavr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tanke756.top/gtytqvuipi.html

TS:   [...arr].reverse();
来源：http://hz.xuanzx.com/gtaehqggbh.html

Java: Collections.reverse(list);
来源：http://hz.jinqigufen.top/gtzhaenylw.html

Go:   slices.Reverse(arr)
来源：http://hz.hammf.cn/gtqkesklln.html

Ruby: arr.reverse
来源：http://hz.zhongyouzk.top/gtattvdfrp.html

C#:   list.Reverse();
来源：http://hz.yj20258.top/gtrcipylgl.html

[D12] 查找元素下标
来源：http://hz.aizwys.cn/gtoooktbmc.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhixingplan.top/gtnvuvevbb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yueranfly.top/gtoxlhvjdl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.feifeiyinyue.top/gtsuopnshw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hfpthk.cn/gtugoymwib.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ywan-chungtsiang.top/gtpcpjqmpz.html

Go:   slices.Index(arr, x)
来源：http://hz.sweek.top/gtcpeilqqj.html

Ruby: arr.index(x)
来源：http://hz.iojbl.cn/gtaubtwnke.html

C#:   list.IndexOf(x);
来源：http://hz.mhx1999.top/gtmwpxauam.html

[D13] 过滤（保留满足条件的）
来源：http://hz.daxiang520.top/gtepetmkhq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ybcxt.top/gtxqqckhya.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.316326.xyz/gtrrxvjpat.html

JS:   arr.filter(x => x > 3)
来源：http://hz.316326.xyz/gtjfvwvlfu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtgyqhjlwz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenzaomai.com/gtpnddqvqs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.haohaochexian.top/gtjxsbyjiv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.fzhhl.top/gtxxtqfoki.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jiagoushi.top/gtsjajbinv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.birdmap.top/gtpzvtgqjo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jqgufenzy.top/gttlhqzxob.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fzhhl.top/gtrxejejth.html

JS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtefqhrcga.html

TS:   arr.map(x => x * 2)
来源：http://hz.yangfankeji.com/gtfyluneze.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.fzhhl.top/gtgphbsduy.html

Go:   // 手写循环
来源：http://hz.vqdsnc.cn/gtzuxrxusd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hysaishi.cn/gtyimslxlv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pycfn.com/gtthownawi.html

[D15] 去重
来源：http://hz.cheryme.top/gtpkjjknil.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gtprjjslez.html

PHP:  array_unique($arr);
来源：http://hz.zhaomingkeji.xyz/gtfdakosbv.html

JS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtsyybxxih.html

TS:   [...new Set(arr)]
来源：http://hz.hnxiangtu.top/gtzebzdufv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shanyushiyangtech.top/gtdbvqowpx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinyuanbaomall.cn/gtwldaibcr.html

Ruby: arr.uniq
来源：http://hz.hfpthk.cn/gtqaherxjr.html

C#:   list.Distinct().ToList()
来源：http://hz.yvedp.cn/gtxifizwpe.html

[D16] 求和与平均值
来源：http://hz.zhongyouzk.top/gtfxwghxfp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigufen.top/gtmkrsiito.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.smart0.xyz/gttecxiwgi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenzaomai.com/gtzoidsqtc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gtvzpkzsgo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hammf.cn/gtchgecwiw.html

Go:   // 手写循环累加
来源：http://hz.svipenyu.cn/gtmwtdptjf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.redwolf501.top/gtwdctpydn.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinyuanbaomall.cn/gtnskylmpl.html

[D17] 最大值与最小值
来源：http://hz.kuanghao11.cn/gtqzotxvdg.html

Py:   max(arr);  min(arr)
来源：http://hz.svipenyu.cn/gtnkjbtgjm.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gtpudpoavg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jqgufenzy.top/gtwywvqghm.html

TS:   Math.max(...arr);
来源：http://hz.redwolf501.top/gtkxkjplzr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xylfe.cn/gtyrziwegr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.iojbl.cn/gtqznthwfe.html

Ruby: arr.max;  arr.min
来源：http://hz.sufxvd.cn/gtymphwgkv.html

C#:   list.Max();  list.Min()
来源：http://hz.wangshuangyany.cn/gtzjjouqpm.html

[D18] 扁平化嵌套数组
来源：http://hz.zhijiandao.cn/gthdelggex.html


<!-- 参考信息 -->