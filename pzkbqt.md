代发 wailian999

[C02] 默认参数
来源：http://hz.zycfv.cn/gtkliwcmbu.html

Py:   def greet(name="World"): return name
来源：http://hz.316326.xyz/gtliyixeoe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.pengpengdd.cyou/gtahkaazqb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nwbrower.top/gtszvytbmi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yonumen.top/gthkkdeyjb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gaohongyu789.top/gtwmtriasx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.wangshuangyany.cn/gtigfufjuo.html

Ruby: def greet(name = "World") = name
来源：http://hz.xingfuxueyuan.xyz/gtgwsoaujt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nanxinkj.top/gtssldwspq.html

[C03] 可变参数
来源：http://hz.mhx1999.top/gtxqnnbyry.html

Py:   def total(*args): return sum(args)
来源：http://hz.c1oappe.top/gtkcjkllle.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xylfe.cn/gtgxygylmk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ybcxt.top/gtclgfaknh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhengqikj.top/gtsnejtcwh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yangfankeji.com/gtslgzryfi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tanke756.top/gtzyqsluhz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xingfuxueyuan.xyz/gtkrufcgyx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.quarkkingdee.top/gtqyswwoti.html

[C04] 命名参数 / 关键字参数
来源：http://hz.meibo888.top/gtfjgwagnp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.feifeiyinyue.top/gtwuejztas.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ydzc1.top/gtehitlmsb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.feifeiyinyue.top/gthekkoljb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zdqjudy.top/gtemnjxxow.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yvedp.cn/gtkierkjii.html

Go:   // 无：用配置结构体参数
来源：http://hz.bjfxy.top/gtezzebtlk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gtffwmflbp.html

C#:   f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtqjhdhaxc.html

[C05] 返回多个值
来源：http://hz.pengpengdd.cyou/gttzxwicpe.html

Py:   return a, b
来源：http://hz.sufxvd.cn/gtkdflsgza.html

PHP:  return [$a, $b];
来源：http://hz.zhixingplan.top/gtugkbncav.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shangyingyoupin.top/gtgmcrhqqq.html

TS:   return { a, b };
来源：http://hz.zhoulong.xyz/gtlmszjtor.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gotoacloud.top/gttkuacqyl.html

Go:   return a, b
来源：http://hz.guowangkeji.top/gtzwbpcqhu.html

Ruby: return a, b
来源：http://hz.316326.xyz/gtykzdcbuu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.feifeiyinyue.top/gtokhiwktr.html

[C06] 匿名函数 / lambda
来源：http://hz.xinyue.icu/gteffkftab.html

Py:   square = lambda x: x * x
来源：http://hz.sysykeji.top/gtcrbthtgt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.snrcjt.cn/gtcsgraxny.html

JS:   const square = x => x * x;
来源：http://hz.zhoulong.xyz/gtwjokifpj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.tian-w.cn/gtgihibmvv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhixingplan.top/gtpaeepnay.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenzaomai.com/gtaaodmote.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhengqikj.top/gtffmuinsj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zycfv.cn/gtoubtodii.html

[C07] 把函数作为参数传入
来源：http://hz.sufxvd.cn/gtehmrzduz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yvedp.cn/gttnagecxy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhongyouzk.top/gtsaonqntu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.0kj1m.cn/gtnwkxcbxq.html

TS:   arr.map(String)
来源：http://hz.jiagoushi.top/gtltmwntgl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxinkj.top/gtcqmiobsw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jyoumei.cn/gtcpjxqhpj.html

Ruby: arr.map(&:upcase)
来源：http://hz.ivvv.top/gtcyunjlth.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xinyue.icu/gtoeauaynr.html

[C08] 闭包
来源：http://hz.zhaomingkeji.xyz/gtxrezttpg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhoulong.xyz/gtugepqsxj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ivvv.top/gtknmocnwc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtpcyaoegv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.svipenyu.cn/gtsholqtph.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.snrcjt.cn/gtimfajcxv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shangyingyoupin.top/gtccodjmme.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydzc1.top/gtnzfsnnqc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtkskkwpgf.html

[C09] 递归
来源：http://hz.nanxuanxn.top/gtspfbneii.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.guowangkeji.top/gtiocoqrvc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenzaomai.com/gtdyuvjqkl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxinkj.top/gtkdxtckby.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gtcnsbjvpo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gtlimshbtu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.mhx1999.top/gtbwdevemf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.havefunace.top/gtwfvivssc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenjidiqi.icu/gttundyynt.html

[C10] 变量作用域
来源：http://hz.sysykeji.top/gtyyqkvlze.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.aizwys.cn/gtfwrieqgg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hammf.cn/gtciggjopo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gotoacloud.top/gtlokfnrgh.html

TS:   同 JS
来源：http://hz.jqgufenzy.top/gtyydkjhxu.html

Java: 方法内为块级作用域
来源：http://hz.sufxvd.cn/gtppchckpk.html

Go:   花括号块级作用域
来源：http://hz.cqqwz.cn/gtfzjtopoa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yongpay.top/gtdhaphkgc.html

C#:   块级作用域
来源：http://hz.hysaishi.cn/gtolgrjoxo.html

[C11] 模块导入与导出
来源：http://hz.jlsjyb.cn/gtmfnlwzto.html

Py:   from module import func
来源：http://hz.gotoacloud.top/gtiamzqseu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xingfuxueyuan.xyz/gtxmvxlkbd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xziqi.cn/gtgffvyyqv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daxiang520.top/gtzvrwovat.html

Java: import java.util.List;
来源：http://hz.pengpengdd.cyou/gtnpgghcsw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ywan-chungtsiang.top/gtxtlaubov.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj202588.top/gtjqfvsqyo.html

C#:   using System.Text;
来源：http://hz.yangfankeji.com/gtuxxnffyt.html

[C12] 立即执行函数 IIFE
来源：http://hz.tianlin.xyz/gtafjyvmkz.html

Py:   (lambda: print("run"))()
来源：http://hz.birdmap.top/gtsjckbkln.html

PHP:  (function () { echo "run"; })();
来源：http://hz.smart0.xyz/gtzpjccrqo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.316326.xyz/gtnpparrhf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xingfuxueyuan.xyz/gtwlgdtyek.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangkeji.top/gtpllqhkjw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydzc1.top/gtucnsttvs.html

Ruby: -> { puts "run" }.call
来源：http://hz.snrcjt.cn/gtjmstiprm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.fzhhl.top/gtieklnfor.html

[C13] 类型声明 / 类型注解
来源：http://hz.0kj1m.cn/gtlaluotos.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangshuangyany.cn/gtjylgppls.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.birdmap.top/gttpwezxmj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.gogol.net.cn/gtxmslhqcc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtrgnsmvyl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yvedp.cn/gtuxuurusd.html

Go:   func add(a, b int) int
来源：http://hz.tianlin.xyz/gtvxcdbxay.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj20258888.top/gtoiszpmgf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.dashuyun.cn/gtuawiumjq.html

[C14] 泛型函数
来源：http://hz.gotoacloud.top/gtxygzyyxn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangkeji.top/gtgcybloot.html

PHP:  // 无泛型
来源：http://hz.birdmap.top/gtquuuaeux.html

JS:   // 无泛型
来源：http://hz.jinqigfzy.top/gtotoogknv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhengqikj.top/gtugspunbr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.iojbl.cn/gthidgzvke.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.vqdsnc.cn/gtdbbyhuxt.html

Ruby: # 无泛型
来源：http://hz.zhaomingkeji.xyz/gthaopoici.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yvedp.cn/gtbztxhiwg.html

[C15] 解构 / 展开参数
来源：http://hz.jinqigfzy.top/gthkqeebrt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.vqdsnc.cn/gtcntmkjsf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sxryk.cn/gtnmqzawst.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shangyingyoupin.top/gtlkkxnewo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ehwqpu.com/gtjarxzluk.html

Java: // 无解构
来源：http://hz.pengpengdd.cyou/gtwvdiayef.html

Go:   // 无解构
来源：http://hz.wangshuangyany.cn/gtmtkijktn.html

Ruby: a, b = pair
来源：http://hz.fzhhl.top/gtfncvljyo.html

C#:   var (a, b) = pair;
来源：http://hz.yvedp.cn/gtdrvmefnw.html

[C16] 函数 / 方法重载
来源：http://hz.tanke756.top/gtggnqszrr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yongpay.top/gtiajnsoeu.html

PHP:  // 无重载
来源：http://hz.quarkkingdee.top/gtulpbsjrp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ywan-chungtsiang.top/gtpfzgjpwk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jlsjyb.cn/gtmxygadfh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.haohaochexian.top/gtrihhqysl.html

Go:   // 无重载：用不同函数名
来源：http://hz.hywenlv.cn/gtbbqboeds.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangdashe.top/gtgyukrrls.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydzc1.top/gtibeedamj.html

================================================================================
来源：http://hz.nwbrower.top/gtafwrplza.html

D. 数组 / 列表 / 集合
来源：http://hz.ydzc1.top/gteaivqznu.html

================================================================================
来源：http://hz.gzhubu.top/gttjngyxgw.html

[D01] 创建数组 / 列表
来源：http://hz.yj202588.top/gtfnclvvyr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xylfe.cn/gttsmnptgi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jianghu66.top/gtssbjpqwz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aizwys.cn/gtuxehmnam.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xinyue.icu/gtnxrrqfel.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtojjvhpsw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhongyouzk.top/gtudwymvsu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aibaodan.cn/gtqglzwrdg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cashguo.top/gtjeosbhgw.html

[D02] 追加元素到末尾
来源：http://hz.svipenyu.cn/gtpjrxfpon.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yonumen.top/gtlqlkmipy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cucudq.cn/gtbkvqcbxi.html

JS:   arr.push(4);
来源：http://hz.iojbl.cn/gtzkyigctr.html

TS:   arr.push(4);
来源：http://hz.316326.xyz/gtjinxhkse.html

Java: list.add(4);
来源：http://hz.jinqigufen.top/gtorokvuuo.html

Go:   arr = append(arr, 4)
来源：http://hz.ehwqpu.com/gttajjjmjw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.0kj1m.cn/gtrkpvzxgd.html

C#:   list.Add(4);
来源：http://hz.shzxlz.cn/gtbtnvbmko.html

[D03] 在指定位置插入元素
来源：http://hz.wangdashe.top/gtirrgdvnz.html

Py:   arr.insert(0, 0)
来源：http://hz.zycfv.cn/gturjrtyld.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hywenlv.cn/gtywcgpapm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhaomingkeji.xyz/gtkonkkryb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.bjfxy.top/gtzxcxtbfs.html

Java: list.add(0, 0);
来源：http://hz.redwolf501.top/gtsxlhviep.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.bjfxy.top/gtlzmccgbt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.52xcode.cn/gthaqgkjji.html

C#:   list.Insert(0, 0);
来源：http://hz.zhijiandao.cn/gtfetuuqun.html

[D04] 删除元素
来源：http://hz.gotoacloud.top/gtrubkoelv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hysaishi.cn/gtxfbpdnjk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhixingplan.top/gtjxpacuho.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxuanxn.top/gthqytbcbd.html

TS:   arr.splice(0, 1);
来源：http://hz.yanxiufei.cn/gtwqtccxku.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xinyue.icu/gtzxqybwty.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgfzy.top/gteogsnxaa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenzaomai.com/gttjbccjcw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.dianchejie.cn/gtcfsfwlxk.html

[D05] 访问与修改元素
来源：http://hz.yonumen.top/gtgyjpxnnd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gtkfqmbxse.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ywan-chungtsiang.top/gtltumczsf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tianlin.xyz/gtdymtwlsi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jlsjyb.cn/gtxkxontiq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fengsongda.top/gtlroblvnb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtnybsoylt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.meibo888.top/gtldiaazgv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtestauhgf.html

[D06] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtxdrhyqkc.html

Py:   len(arr)
来源：http://hz.cashguo.top/gtjnvabaqd.html

PHP:  count($arr);
来源：http://hz.c1oappe.top/gtchsztdxm.html

JS:   arr.length
来源：http://hz.havefunace.top/gtwvuokpee.html

TS:   arr.length
来源：http://hz.0kj1m.cn/gthqxoocgj.html

Java: list.size();
来源：http://hz.yanxiufei.cn/gteizcyfmf.html

Go:   len(arr)
来源：http://hz.daria6918.cn/gtmyjllpli.html

Ruby: arr.length; arr.size
来源：http://hz.sysykeji.top/gtmgbaysdh.html

C#:   list.Count;
来源：http://hz.xinyue.icu/gtwrfaiqbz.html

[D07] 切片 / 取子数组
来源：http://hz.hnxiangtu.top/gtxojnstbd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.aizwys.cn/gtqnycpsqb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.quarkkingdee.top/gtvtxtobrv.html

JS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gtyvqpicfu.html

TS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtcfvgwtkk.html

Java: list.subList(1, 4);
来源：http://hz.wangshuangyany.cn/gtjoqxnaej.html

Go:   arr[1:4]
来源：http://hz.zhiwuduotai.top/gtlynbjrmr.html

Ruby: arr[1, 3]
来源：http://hz.hywenlv.cn/gtutfewkwo.html

C#:   list.GetRange(1, 3);
来源：http://hz.sweek.top/gtblgsfiex.html

[D08] 合并两个数组
来源：http://hz.yvedp.cn/gtihnxhnqm.html

Py:   a + b;  a.extend(b)
来源：http://hz.iojbl.cn/gtkqdqspdf.html

PHP:  array_merge($a, $b);
来源：http://hz.9152youxi.cn/gtngltukaa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.daxiang520.top/gtatdkuduv.html

TS:   [...a, ...b];
来源：http://hz.ppjwa.cn/gtsmevafsi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.andypj.xyz/gtgkfvaagm.html

Go:   append(a, b...)
来源：http://hz.haohaochexian.top/gtsgluxxta.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gzhubu.top/gtddfxmjpw.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinghuilouyu.cn/gtjtkgdtcq.html

[D09] 排序（升序）
来源：http://hz.hysaishi.cn/gtiecqexti.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gttjfigqfx.html

PHP:  sort($arr);
来源：http://hz.zhiwuduotai.top/gtmncilugb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.0kj1m.cn/gtawhrlntr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.daria6918.cn/gtfluvjohx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.birdmap.top/gtqchsgfcb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhoulong.xyz/gtlzgydoub.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtdvrjwuyd.html

C#:   list.Sort();
来源：http://hz.shuidangran.top/gtgrbcqwoq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ivvv.top/gtkxkqgewd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yueranfly.top/gtavmvcxsv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydjk.org.cn/gtqntftkwi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ybcxt.top/gtiaabbcxn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gtoveqigoy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nwbrower.top/gtxjlunwfl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cdnleiting.top/gtommwmaof.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zycfv.cn/gtbjivzlny.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yanxiufei.cn/gtagmljizh.html

[D11] 反转数组
来源：http://hz.yonumen.top/gtflcesrvp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.chenlongwang.top/gtxyngikgd.html

PHP:  array_reverse($arr);
来源：http://hz.haohaochexian.top/gttsrklafb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fengsongda.top/gtzdljshbq.html

TS:   [...arr].reverse();
来源：http://hz.xziqi.cn/gtupqphxkw.html

Java: Collections.reverse(list);
来源：http://hz.svipenyu.cn/gtttqlrapj.html

Go:   slices.Reverse(arr)
来源：http://hz.shzxlz.cn/gtuqvjhfmx.html

Ruby: arr.reverse
来源：http://hz.cdnleiting.top/gtuivkduyd.html

C#:   list.Reverse();
来源：http://hz.cqqwz.cn/gtfpjhpuvg.html

[D12] 查找元素下标
来源：http://hz.yj202588.top/gttrzlawmx.html

Py:   arr.index(x);  x in arr
来源：http://hz.dashuyun.cn/gtiksjglqc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yueranfly.top/gtufutjyqp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aibaodan.cn/gtswqpmglq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fengsongda.top/gtqjhuians.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxuanxn.top/gtedllsoxw.html

Go:   slices.Index(arr, x)
来源：http://hz.yvedp.cn/gtdzeywgqx.html

Ruby: arr.index(x)
来源：http://hz.pengpengdd.cyou/gtzgyurwpy.html

C#:   list.IndexOf(x);
来源：http://hz.jinqigfzy.top/gtglqvwsix.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhoulong.xyz/gtpubccpqd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnxiangtu.top/gtlqdoagmx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jlsjyb.cn/gtcgiomyfu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtuusueocs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gogol.net.cn/gtxbjdjisi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sufxvd.cn/gtbympdiuu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.andypj.xyz/gtkgfhuemc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gzhubu.top/gtresrzwme.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.9152youxi.cn/gtwoeohbpb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jiagoushi.top/gtuirktaix.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.daxiang520.top/gtgwzfqtxz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.svipenyu.cn/gtuogwidzc.html

JS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gthjwwqwuf.html

TS:   arr.map(x => x * 2)
来源：http://hz.mhx1999.top/gttqkhfrgi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xuanzx.com/gtoljkrmol.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtfvtpygyu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ywan-chungtsiang.top/gtelelcvtc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.birdmap.top/gtqmwnohsl.html

[D15] 去重
来源：http://hz.yj20258.top/gtmikyghjv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydzc1.top/gtwzvckmwv.html

PHP:  array_unique($arr);
来源：http://hz.jinyuanbaomall.cn/gtmqcgbikd.html

JS:   [...new Set(arr)]
来源：http://hz.nanxuanxn.top/gtzmrnlwrd.html

TS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gtkxrfibua.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gzhubu.top/gthwosmvpu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aizwys.cn/gtvntzhpim.html

Ruby: arr.uniq
来源：http://hz.ydzc1.top/gtasekeiac.html

C#:   list.Distinct().ToList()
来源：http://hz.cqqwz.cn/gtldyweqet.html

[D16] 求和与平均值
来源：http://hz.ehwqpu.com/gtzaidiciy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.0kj1m.cn/gtggtpoqpv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yanxiufei.cn/gtbcnwryrc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtnseuypsp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gtwqpuvumz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenlongwang.top/gtwewgrbwa.html

Go:   // 手写循环累加
来源：http://hz.sweek.top/gtjacjfbnw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.quarkkingdee.top/gtagvpcnod.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinyuanbaomall.cn/gtxiarjcgm.html

[D17] 最大值与最小值
来源：http://hz.0kj1m.cn/gtjzugpttm.html

Py:   max(arr);  min(arr)
来源：http://hz.hammf.cn/gtejolboty.html

PHP:  max($arr);  min($arr);
来源：http://hz.ppjwa.cn/gtjvbtryfu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenzaomai.com/gtkddepqbr.html

TS:   Math.max(...arr);
来源：http://hz.shangyingyoupin.top/gtgscrjvli.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dashuyun.cn/gtmlvthumf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.andypj.xyz/gtmdwwiqrg.html

Ruby: arr.max;  arr.min
来源：http://hz.yvedp.cn/gtdbzpiyah.html

C#:   list.Max();  list.Min()
来源：http://hz.hfpthk.cn/gtvurnljhe.html

[D18] 扁平化嵌套数组
来源：http://hz.sysykeji.top/gtmjwnunjj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shanyushiyangtech.top/gtrewbgmaj.html

PHP:  array_merge(...$nested);
来源：http://hz.zhengqikj.top/gtxtthtpfi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangshuangyany.cn/gtndlhqzom.html

TS:   nested.flat();
来源：http://hz.hysaishi.cn/gtvqhghtji.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sxryk.cn/gtyoylzpqh.html

Go:   // 手写双层循环
来源：http://hz.zhoulong.xyz/gtktncgkwl.html

Ruby: nested.flatten
来源：http://hz.ppjwa.cn/gtjxtyuekq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shanyushiyangkeji.top/gtvpmgilhw.html


<!-- 参考信息 -->