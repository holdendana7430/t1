代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtvnxjeyog.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxinkj.top/gtcmbbambr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shzxlz.cn/gtkqbptekz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtxzomimzt.html

[C02] 默认参数
来源：http://hz.quarkkingdee.top/gtcvytzxnc.html

Py:   def greet(name="World"): return name
来源：http://hz.yueranfly.top/gtqolktzsw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinqigfzy.top/gtmypepfst.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtgyilwtkq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhongyouzk.top/gtqkdtabmc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinghuilouyu.cn/gtvvqrhsad.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yongpay.top/gtoqgkysug.html

Ruby: def greet(name = "World") = name
来源：http://hz.kuanghao11.cn/gtdhzekfbr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sweek.top/gtkwklmseu.html

[C03] 可变参数
来源：http://hz.ivvv.top/gtxbsohzeh.html

Py:   def total(*args): return sum(args)
来源：http://hz.yangfankeji.com/gtlifgcgsk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zdqjudy.top/gttouvzagz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pycfn.com/gtbrtzpoww.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtvesatrqh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cqqwz.cn/gtcwmwwojp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.aizwys.cn/gtolcwkcrl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenzaomai.com/gtrdihlwnd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhaomingkeji.xyz/gtydjviypq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gaohongyu789.top/gtwbqxqvht.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.aibaodan.cn/gtyoypwrgy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gaohongyu789.top/gtwwfrxcyv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yongpay.top/gtqjlmneis.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jiagoushi.top/gtrlbjjmcb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhengqikj.top/gtagrxjrhi.html

Go:   // 无：用配置结构体参数
来源：http://hz.gzhubu.top/gtjenvbaeo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtezfiwmuc.html

C#:   f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtvuxtrurz.html

[C05] 返回多个值
来源：http://hz.guowangkeji.top/gtrtrrahxp.html

Py:   return a, b
来源：http://hz.xuanzx.com/gtnmgvaune.html

PHP:  return [$a, $b];
来源：http://hz.snrcjt.cn/gtbgqwxhxs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sysykeji.top/gtwvkeyilh.html

TS:   return { a, b };
来源：http://hz.gogol.net.cn/gtkfzprrrk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.wangdashe.top/gtsxscwloq.html

Go:   return a, b
来源：http://hz.tian-w.cn/gtkehqfdvw.html

Ruby: return a, b
来源：http://hz.ydzc1.top/gtjgshcqfv.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj20258888.top/gtbqrfvylk.html

[C06] 匿名函数 / lambda
来源：http://hz.bjfxy.top/gtmzzhlfdb.html

Py:   square = lambda x: x * x
来源：http://hz.daria6918.cn/gtcqjyrmdn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj20258888.top/gtyiltpglm.html

JS:   const square = x => x * x;
来源：http://hz.sysykeji.top/gtstzplely.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dashuyun.cn/gtadgngfns.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.andypj.xyz/gtcsdsleim.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenzaomai.com/gtmfjxlvuq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.quarkkingdee.top/gtzzhdxcmj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ehwqpu.com/gtuyjeimmp.html

[C07] 把函数作为参数传入
来源：http://hz.guannengcc.top/gteogsnphn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shanyushiyangtech.top/gtjattzvvv.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.nwbrower.top/gtnspiukcd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xuanzx.com/gtkytpnjuo.html

TS:   arr.map(String)
来源：http://hz.yanxiufei.cn/gtaptgorcq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhengqikj.top/gtsxnlwsif.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhengqikj.top/gtcdieuuut.html

Ruby: arr.map(&:upcase)
来源：http://hz.tanke756.top/gtegaaphdc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.bjfxy.top/gtqdjitwgj.html

[C08] 闭包
来源：http://hz.jyoumei.cn/gtzrztofus.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yueranfly.top/gtprabkndl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hnxiangtu.top/gtoawsqyja.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtxktfvcgf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinghuilouyu.cn/gtcouuatgg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.snrcjt.cn/gtstgmxqiv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shuidangran.top/gtlzzjrmre.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.dashuyun.cn/gtckjpsyxb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gtdcmxqpjd.html

[C09] 递归
来源：http://hz.daria6918.cn/gtfmgjvizp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhengqikj.top/gtsfcogwuw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shzxlz.cn/gtubzoatnx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ywan-chungtsiang.top/gtffwrbtgb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ivvv.top/gtadsjksfm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.fengsongda.top/gtppitbjra.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ydzc1.top/gtscpymrhg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtauefelps.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydzc1.top/gtsldnorce.html

[C10] 变量作用域
来源：http://hz.yongpay.top/gtnnbsxvdm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.316326.xyz/gtshlbfoje.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gogol.net.cn/gtjxetqdgx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yj20258888.top/gtldtymsoy.html

TS:   同 JS
来源：http://hz.quarkkingdee.top/gtfztpczdr.html

Java: 方法内为块级作用域
来源：http://hz.zycfv.cn/gtkkvgdqbw.html

Go:   花括号块级作用域
来源：http://hz.smart0.xyz/gtcllnvpro.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhixingplan.top/gtacxgnkhi.html

C#:   块级作用域
来源：http://hz.jqgfzy.top/gtsacvdoiv.html

[C11] 模块导入与导出
来源：http://hz.jlsjyb.cn/gtfkohxzyp.html

Py:   from module import func
来源：http://hz.yj20258888.top/gtbgtghabk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ivvv.top/gtluiugwjw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.316326.xyz/gtvhtssqhk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jiagoushi.top/gtowdzxgwo.html

Java: import java.util.List;
来源：http://hz.sufxvd.cn/gtduerleon.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hnqzz.top/gtnzalwluk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.tian-w.cn/gtgdyatdat.html

C#:   using System.Text;
来源：http://hz.zhiwuduotai.top/gtyiwxwqgl.html

[C12] 立即执行函数 IIFE
来源：http://hz.birdmap.top/gteawsnkbz.html

Py:   (lambda: print("run"))()
来源：http://hz.redwolf501.top/gtkkmbnkmo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhiwuduotai.top/gtmtxccrtv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yueranfly.top/gtubvwfmgo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhongyouzk.top/gtqxnolyck.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.andypj.xyz/gtygtlxqep.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.pycfn.com/gtpcolipnj.html

Ruby: -> { puts "run" }.call
来源：http://hz.andypj.xyz/gtzhnnibdj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuxming.cn/gtyhyhpdiz.html

[C13] 类型声明 / 类型注解
来源：http://hz.daria6918.cn/gtxpekbsta.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nwbrower.top/gtafakuxbq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtgykidaaj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.feifeiyinyue.top/gtkkygdgtl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtdajrimiy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtglsuafxk.html

Go:   func add(a, b int) int
来源：http://hz.dashuyun.cn/gtszbjmxjo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhengqikj.top/gtnfsfwmkj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xylfe.cn/gtcccpyxwr.html

[C14] 泛型函数
来源：http://hz.andypj.xyz/gtpjgfpleb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gogol.net.cn/gtocjtguar.html

PHP:  // 无泛型
来源：http://hz.jqgfzy.top/gtpnftknhk.html

JS:   // 无泛型
来源：http://hz.jqgufenzy.top/gtljoaaxor.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gogol.net.cn/gtlhhmapqd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xinyue.icu/gtnxvhimmu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shzxlz.cn/gtbqgormyu.html

Ruby: # 无泛型
来源：http://hz.ehwqpu.com/gtkgsqgjdu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.bjfxy.top/gtksmtdolt.html

[C15] 解构 / 展开参数
来源：http://hz.redwolf501.top/gtrlkxnute.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gteamqijms.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ydjk.org.cn/gtjifvzysa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhoulong.xyz/gttffnugoo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fzhhl.top/gtrbsekdbd.html

Java: // 无解构
来源：http://hz.nanxinkj.top/gtthnvheqn.html

Go:   // 无解构
来源：http://hz.9152youxi.cn/gtufaitige.html

Ruby: a, b = pair
来源：http://hz.sufxvd.cn/gtvwwtkhbj.html

C#:   var (a, b) = pair;
来源：http://hz.quarkkingdee.top/gtkjcxitxf.html

[C16] 函数 / 方法重载
来源：http://hz.xinyue.icu/gtcvejufjs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gzhubu.top/gtcteyxduv.html

PHP:  // 无重载
来源：http://hz.xylfe.cn/gtxiwxvvgj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sweek.top/gthyphpaej.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.kuanghao11.cn/gtwthvzfgr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tianlin.xyz/gthtxpdfof.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgufenzy.top/gtgjnijsln.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sxryk.cn/gtihwlseye.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.0kj1m.cn/gtfityjhju.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtkbqjnvdq.html

D. 数组 / 列表 / 集合
来源：http://hz.cucudq.cn/gthjbpauzd.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtenwihbtk.html

[D01] 创建数组 / 列表
来源：http://hz.zhengqikj.top/gtiwxuutrr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.iojbl.cn/gtzdbenyhe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.chenjidiqi.icu/gtnvfuskbt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jqgufenzy.top/gtskjuddqa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhixingplan.top/gtgngifinn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xingfuxueyuan.xyz/gtpdaiiinj.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sysykeji.top/gtsnbnnaxn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenzaomai.com/gtsxggqyfa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinyuanbaomall.cn/gtmcdlkfom.html

[D02] 追加元素到末尾
来源：http://hz.haohaochexian.top/gtemjesxwf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.feifeiyinyue.top/gtoagmthpb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jianghu66.top/gtoilziyac.html

JS:   arr.push(4);
来源：http://hz.smart0.xyz/gtuoflnnke.html

TS:   arr.push(4);
来源：http://hz.jqgfzy.top/gtedxmxtsz.html

Java: list.add(4);
来源：http://hz.cqqwz.cn/gtyorutktp.html

Go:   arr = append(arr, 4)
来源：http://hz.sufxvd.cn/gtazbeusfh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.havefunace.top/gtygqhimyk.html

C#:   list.Add(4);
来源：http://hz.yj202588.top/gtajtxvayo.html

[D03] 在指定位置插入元素
来源：http://hz.hnxiangtu.top/gtnfpywyvy.html

Py:   arr.insert(0, 0)
来源：http://hz.cucudq.cn/gtmnsvzuii.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.dianchejie.cn/gtxhdzyxdg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yj20258.top/gtsleagjgy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shzxlz.cn/gtzychogfy.html

Java: list.add(0, 0);
来源：http://hz.hammf.cn/gtakaumgav.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aibaodan.cn/gtimbjkakl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gzhubu.top/gtcuwngwpb.html

C#:   list.Insert(0, 0);
来源：http://hz.daxiang520.top/gtnxopkmpa.html

[D04] 删除元素
来源：http://hz.jinghuilouyu.cn/gtniggotsm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jianghu66.top/gtzksfrkcr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gogol.net.cn/gtyzlbkyzp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yvedp.cn/gtwpihbbhn.html

TS:   arr.splice(0, 1);
来源：http://hz.gaohongyu789.top/gtacequnjm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydjk.org.cn/gtkbcvfhor.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sysykeji.top/gtpqrxwozl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhongyouzk.top/gtpyaqqftr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fengsongda.top/gtxkhpkqnd.html

[D05] 访问与修改元素
来源：http://hz.jianghu66.top/gtrjlhlpsx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtvcyescpa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtwczsdjao.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aibaodan.cn/gtspxorsjx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinqigfzy.top/gtqqntzsof.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yvedp.cn/gtwqksrkgm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jqgfzy.top/gtllkcgiop.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jqgufenzy.top/gtmotcmijb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.mhx1999.top/gtejkmmtlz.html

[D06] 数组长度
来源：http://hz.xuetiantiany.cn/gtwnvaiduu.html

Py:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gtrfynohxb.html

PHP:  count($arr);
来源：http://hz.fengsongda.top/gtpcpauliw.html

JS:   arr.length
来源：http://hz.chenlongwang.top/gtrqhnrwgz.html

TS:   arr.length
来源：http://hz.hongshengwenyu.top/gthjkngqbv.html

Java: list.size();
来源：http://hz.feifeiyinyue.top/gtxeupfeht.html

Go:   len(arr)
来源：http://hz.redwolf501.top/gtzyqbhone.html

Ruby: arr.length; arr.size
来源：http://hz.sweek.top/gtnzvbwika.html

C#:   list.Count;
来源：http://hz.chenjidiqi.icu/gtzwgiljbb.html

[D07] 切片 / 取子数组
来源：http://hz.xuetiantiany.cn/gtdaxxdlxm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuanzx.com/gtnpihchda.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenlongwang.top/gtqpsekgay.html

JS:   arr.slice(1, 4);
来源：http://hz.jqgufenzy.top/gtuorrsbwz.html

TS:   arr.slice(1, 4);
来源：http://hz.sxryk.cn/gtokrxuyiy.html

Java: list.subList(1, 4);
来源：http://hz.zhengqikj.top/gtmiecrebn.html

Go:   arr[1:4]
来源：http://hz.haohaochexian.top/gteiucnmwc.html

Ruby: arr[1, 3]
来源：http://hz.smart0.xyz/gtyscmytrt.html

C#:   list.GetRange(1, 3);
来源：http://hz.shzxlz.cn/gtmfufnfej.html

[D08] 合并两个数组
来源：http://hz.chenlongwang.top/gtqwswfeyo.html

Py:   a + b;  a.extend(b)
来源：http://hz.zycfv.cn/gtfkpeezxl.html

PHP:  array_merge($a, $b);
来源：http://hz.nanxinkj.top/gtoqjedpah.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.chenlongwang.top/gtksaccoyf.html

TS:   [...a, ...b];
来源：http://hz.gaohongyu789.top/gtgxqmuzfh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangtech.top/gtjxhosjlo.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gteiwdsebw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.feifeiyinyue.top/gtcgidiczy.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinghuilouyu.cn/gtyjdloszy.html

[D09] 排序（升序）
来源：http://hz.havefunace.top/gtecrszpwf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yonumen.top/gtmnxchkvh.html

PHP:  sort($arr);
来源：http://hz.yj20258.top/gtywsjlqqp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.pycfn.com/gtxiccgknp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinyuanbaomall.cn/gtovfepxvb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj20258.top/gtkhrpwsse.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hfpthk.cn/gtgcxsoozz.html

Ruby: arr.sort
来源：http://hz.fzhhl.top/gtkjqmjwsd.html

C#:   list.Sort();
来源：http://hz.ivvv.top/gtwlitnhxf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.dashuyun.cn/gtkvizmjsg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hnqzz.top/gtnahdsmsj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.meibo888.top/gtvysvyobs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sysykeji.top/gtmhctyzgl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ppjwa.cn/gtqywbzuee.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yanxiufei.cn/gtbyvztnrc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jqgfzy.top/gtlxpaozfn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhoulong.xyz/gtomhoyrep.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhengqikj.top/gtplfhtetw.html

[D11] 反转数组
来源：http://hz.ydzc1.top/gtblkxviij.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tianlin.xyz/gtdzplgjdd.html

PHP:  array_reverse($arr);
来源：http://hz.zhixingplan.top/gtgdrbwyyr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hywenlv.cn/gtodnjhqlk.html

TS:   [...arr].reverse();
来源：http://hz.zycfv.cn/gtcheuipzx.html

Java: Collections.reverse(list);
来源：http://hz.cashguo.top/gtgdiijlou.html

Go:   slices.Reverse(arr)
来源：http://hz.dashuyun.cn/gtmwihpivq.html

Ruby: arr.reverse
来源：http://hz.cdnleiting.top/gtdreauolc.html

C#:   list.Reverse();
来源：http://hz.jinqigufen.top/gtjfienoep.html

[D12] 查找元素下标
来源：http://hz.zdqjudy.top/gtxajzkxvk.html

Py:   arr.index(x);  x in arr
来源：http://hz.andypj.xyz/gternxobmp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.guowangkeji.top/gtzvmwofmw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.andypj.xyz/gttcrossgr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangkeji.top/gthwahdaaj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gaohongyu789.top/gtwjhvblkp.html

Go:   slices.Index(arr, x)
来源：http://hz.gaohongyu789.top/gtohykrerm.html

Ruby: arr.index(x)
来源：http://hz.yvedp.cn/gtoptxesct.html

C#:   list.IndexOf(x);
来源：http://hz.yueranfly.top/gtevicnith.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ppjwa.cn/gtnhcgxjsb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.guannengcc.top/gtefnvkcjc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cashguo.top/gtzkaqahld.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xingfuxueyuan.xyz/gtenchjycx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtcorubfdn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aizwys.cn/gtmcicfeqh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258888.top/gtpyqujhha.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aizwys.cn/gtctcfzbhn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhiwuduotai.top/gtmkrzdmvp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenzaomai.com/gtsvluxopl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xziqi.cn/gtdypmnepl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gzhubu.top/gtvrheenbv.html

JS:   arr.map(x => x * 2)
来源：http://hz.quarkkingdee.top/gtctuqtumo.html

TS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtknzydlde.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangtech.top/gtlnfopfjl.html

Go:   // 手写循环
来源：http://hz.xuetiantiany.cn/gtqsumqvqz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.316326.xyz/gtumcvfuuk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yongpay.top/gtzcqrxqyg.html

[D15] 去重
来源：http://hz.zycfv.cn/gtirjplzon.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtistoqehf.html

PHP:  array_unique($arr);
来源：http://hz.ivvv.top/gtdabouxqc.html

JS:   [...new Set(arr)]
来源：http://hz.tanke756.top/gtkotltrvi.html

TS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtbfecfdqx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigufen.top/gtlqmekqaf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.quarkkingdee.top/gtwmnqmwac.html

Ruby: arr.uniq
来源：http://hz.shzxlz.cn/gtithntfpf.html

C#:   list.Distinct().ToList()
来源：http://hz.yj202588.top/gtyqapasqb.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangtech.top/gtqwwasfji.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yonumen.top/gtmwipoeuu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xylfe.cn/gtxvhwnmya.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gtpuvxkola.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhiwuduotai.top/gtxlycenci.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nwbrower.top/gttyzbxlzr.html

Go:   // 手写循环累加
来源：http://hz.fzhhl.top/gtcrzldgws.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hfpthk.cn/gtsmqlcvex.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuanzhike.top/gtvhhtjyrh.html

[D17] 最大值与最小值
来源：http://hz.cdnleiting.top/gtmfgylcnu.html

Py:   max(arr);  min(arr)
来源：http://hz.fengsongda.top/gtmksconqs.html

PHP:  max($arr);  min($arr);
来源：http://hz.xziqi.cn/gtojpkhkix.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.316326.xyz/gtmtexqzyv.html

TS:   Math.max(...arr);
来源：http://hz.jqgfzy.top/gtsmysvdel.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yueranfly.top/gtmwzslmna.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgufenzy.top/gtvpmclftl.html

Ruby: arr.max;  arr.min
来源：http://hz.feifeiyinyue.top/gtciephxok.html

C#:   list.Max();  list.Min()
来源：http://hz.c1oappe.top/gtrbgaluwy.html

[D18] 扁平化嵌套数组
来源：http://hz.aizwys.cn/gtnkgohujo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj202588.top/gtwiyxngdt.html

PHP:  array_merge(...$nested);
来源：http://hz.zhoulong.xyz/gtfsuznojq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhaomingkeji.xyz/gtwtpeoaix.html

TS:   nested.flat();
来源：http://hz.sysykeji.top/gtcqlackvc.html


<!-- 参考信息 -->