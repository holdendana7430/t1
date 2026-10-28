代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cashguo.top/gtryvxbjck.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zdqjudy.top/gtakjdueyq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hysaishi.cn/gtvcnpidjq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ppjwa.cn/gtbveppfst.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sweek.top/gtlshgxavn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.nanxinkj.top/gtkdmolcdr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yangfankeji.com/gtmufllmbn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.pycfn.com/gtagacoiym.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shuidangran.top/gtsyrlkjug.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gtozfccrfe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.fzhhl.top/gtpomlwbnh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinyuanbaomall.cn/gtpwfviwhh.html

Go:   // 无：用配置结构体参数
来源：http://hz.tianlin.xyz/gtgdpntfwy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sxryk.cn/gttagonhrc.html

C#:   f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gteilaqpeq.html

[C05] 返回多个值
来源：http://hz.aibaodan.cn/gtpkvbmhbb.html

Py:   return a, b
来源：http://hz.chenjidiqi.icu/gttmxyrpop.html

PHP:  return [$a, $b];
来源：http://hz.yuxming.cn/gttakcrdxz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jlsjyb.cn/gtjpifowaz.html

TS:   return { a, b };
来源：http://hz.gotoacloud.top/gtyzplyapi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xuetiantiany.cn/gttwjkdfmh.html

Go:   return a, b
来源：http://hz.hywenlv.cn/gtlmqrxkav.html

Ruby: return a, b
来源：http://hz.hnxiangtu.top/gtybrpayyj.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cqqwz.cn/gtokcoqsdx.html

[C06] 匿名函数 / lambda
来源：http://hz.yangfankeji.com/gtyjtxjxnb.html

Py:   square = lambda x: x * x
来源：http://hz.9152youxi.cn/gtspctsits.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xuanzx.com/gtvtikazye.html

JS:   const square = x => x * x;
来源：http://hz.aizwys.cn/gttdcjzjgb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.guowangkeji.top/gtxdrxxnap.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.quarkkingdee.top/gthozjpefd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.iojbl.cn/gttudvgdic.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jqgufenzy.top/gtuffwickb.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.316326.xyz/gtmaaiqiqo.html

[C07] 把函数作为参数传入
来源：http://hz.gzhubu.top/gtjmuaekbr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pengpengdd.cyou/gtxyexvhga.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ehwqpu.com/gttyookixj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.guowangkeji.top/gtmbynofqp.html

TS:   arr.map(String)
来源：http://hz.gaohongyu789.top/gtidiadqgp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tanke756.top/gttudwrxqt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hammf.cn/gtctjhsglo.html

Ruby: arr.map(&:upcase)
来源：http://hz.jiagoushi.top/gtqjrylsju.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cheryme.top/gtztbxlujc.html

[C08] 闭包
来源：http://hz.feifeiyinyue.top/gtksynbxjd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinghuilouyu.cn/gthxpwfruw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cashguo.top/gtqeskteoq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtrjgouszh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.haohaochexian.top/gtrsvxvmfu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yangfankeji.com/gtfahxiurd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhongyouzk.top/gtxcxuesso.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yuanzhike.top/gtxvfvtaif.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtmhogfzks.html

[C09] 递归
来源：http://hz.ivvv.top/gtxacdxsaq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinqigufen.top/gtousonvhb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.aibaodan.cn/gtsjnwainm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhoulong.xyz/gttwnlbbgy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gtmbeaizho.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jianghu66.top/gteaoykyab.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sxryk.cn/gtmlbodrmg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yongpay.top/gtxcwghvva.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.meibo888.top/gtjkrvuxdc.html

[C10] 变量作用域
来源：http://hz.daxiang520.top/gtshffsxwb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yueranfly.top/gtolstjnra.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gaohongyu789.top/gtlteumyos.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.tianlin.xyz/gtejznuwpz.html

TS:   同 JS
来源：http://hz.smart0.xyz/gtqgnanfth.html

Java: 方法内为块级作用域
来源：http://hz.dianchejie.cn/gtgyusmtaa.html

Go:   花括号块级作用域
来源：http://hz.ivvv.top/gtarpetvqg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dashuyun.cn/gtiqhudcxq.html

C#:   块级作用域
来源：http://hz.hammf.cn/gtnzvfttnl.html

[C11] 模块导入与导出
来源：http://hz.shanyushiyangtech.top/gtfknfwprk.html

Py:   from module import func
来源：http://hz.aizwys.cn/gtdlkpvldh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.daria6918.cn/gtfallqooj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gotoacloud.top/gtvgboujkd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yvedp.cn/gtrrtmxmck.html

Java: import java.util.List;
来源：http://hz.jyoumei.cn/gtfjfwyvbt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xingfuxueyuan.xyz/gtasvpsqzy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hywenlv.cn/gtcjgqevot.html

C#:   using System.Text;
来源：http://hz.ywan-chungtsiang.top/gtntkgrvyk.html

[C12] 立即执行函数 IIFE
来源：http://hz.0kj1m.cn/gteugkoohh.html

Py:   (lambda: print("run"))()
来源：http://hz.zhengqikj.top/gtucngxavr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zycfv.cn/gtrftzpvih.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jqgufenzy.top/gttbraqkgw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ppjwa.cn/gtislsteho.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hongshengwenyu.top/gttsmvxljx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.svipenyu.cn/gttdufavxw.html

Ruby: -> { puts "run" }.call
来源：http://hz.guannengcc.top/gtvlkrwbec.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yonumen.top/gtaqncwcfk.html

[C13] 类型声明 / 类型注解
来源：http://hz.feifeiyinyue.top/gtaoatyixo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.dianchejie.cn/gtiftbmdvy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtxzllscjd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj20258.top/gtxcfidjzx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.0kj1m.cn/gtucobodts.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtcfytqyxd.html

Go:   func add(a, b int) int
来源：http://hz.gaohongyu789.top/gtkfujhlpt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhiwuduotai.top/gtksajuknb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xuetiantiany.cn/gtjcmthzqf.html

[C14] 泛型函数
来源：http://hz.guowangkeji.top/gtqacuxxhk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sweek.top/gtilsljojn.html

PHP:  // 无泛型
来源：http://hz.snrcjt.cn/gtjqnsqqko.html

JS:   // 无泛型
来源：http://hz.sysykeji.top/gtqapczdxm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.0kj1m.cn/gtqdootfgb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenzaomai.com/gtjmqzdetl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sysykeji.top/gtudcppepz.html

Ruby: # 无泛型
来源：http://hz.hnxiangtu.top/gtaykwwlul.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuanzhike.top/gtspueettz.html

[C15] 解构 / 展开参数
来源：http://hz.hysaishi.cn/gtbolqfity.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jiagoushi.top/gtitlhiekf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.quarkkingdee.top/gtooceinma.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtqnirbaoh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shanyushiyangkeji.top/gtlimblggt.html

Java: // 无解构
来源：http://hz.pengpengdd.cyou/gtqytbggww.html

Go:   // 无解构
来源：http://hz.cucudq.cn/gtybabzmvs.html

Ruby: a, b = pair
来源：http://hz.0kj1m.cn/gthxbcpogw.html

C#:   var (a, b) = pair;
来源：http://hz.snrcjt.cn/gtexxhtfzt.html

[C16] 函数 / 方法重载
来源：http://hz.jinghuilouyu.cn/gtkirqcnrz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.svipenyu.cn/gttdmylruz.html

PHP:  // 无重载
来源：http://hz.jianghu66.top/gtmpnibwjv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tanke756.top/gtiiiqopwh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hnqzz.top/gtacrxucpc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.fzhhl.top/gtijenjgyj.html

Go:   // 无重载：用不同函数名
来源：http://hz.redwolf501.top/gtgcwyyxyl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.birdmap.top/gtrmvpzyze.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenzaomai.com/gtzejovqhb.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdmytnmfn.html

D. 数组 / 列表 / 集合
来源：http://hz.jqgfzy.top/gtlsqejxfj.html

================================================================================
来源：http://hz.snrcjt.cn/gtmobkgfdi.html

[D01] 创建数组 / 列表
来源：http://hz.shanyushiyangtech.top/gtcspczahq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ydzc1.top/gtfcispdni.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sysykeji.top/gtaoysnhjf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.0kj1m.cn/gtqadcqlvm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.dashuyun.cn/gtujtblzpo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhoulong.xyz/gthiitjaza.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.havefunace.top/gtijevhajy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cqqwz.cn/gtdgqrzjdb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgufenzy.top/gtrbfigole.html

[D02] 追加元素到末尾
来源：http://hz.ivvv.top/gtsugclisf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.wangdashe.top/gtxjfaiatx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nwbrower.top/gtawmrqhmb.html

JS:   arr.push(4);
来源：http://hz.gaohongyu789.top/gtqhkwocye.html

TS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtbjqwcuwx.html

Java: list.add(4);
来源：http://hz.yonumen.top/gtzvfeanhc.html

Go:   arr = append(arr, 4)
来源：http://hz.hywenlv.cn/gtnwjpqbpb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuanzx.com/gtisqkencn.html

C#:   list.Add(4);
来源：http://hz.yangfankeji.com/gtoyofadlm.html

[D03] 在指定位置插入元素
来源：http://hz.nwbrower.top/gtlwhxyqvv.html

Py:   arr.insert(0, 0)
来源：http://hz.zhiwuduotai.top/gthrszwxyq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jianghu66.top/gtmwwjnzuc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.c1oappe.top/gtrxapksuo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258.top/gtzpxfmzjs.html

Java: list.add(0, 0);
来源：http://hz.jianghu66.top/gthelsvxoa.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hongshengwenyu.top/gtsygoavse.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sysykeji.top/gteoaihjnc.html

C#:   list.Insert(0, 0);
来源：http://hz.hammf.cn/gtupfzewfp.html

[D04] 删除元素
来源：http://hz.birdmap.top/gtelusceox.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.pengpengdd.cyou/gtdarmlpdj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.cqqwz.cn/gtykjhmccr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xinyue.icu/gtihvdbxzi.html

TS:   arr.splice(0, 1);
来源：http://hz.quarkkingdee.top/gtqvvuyish.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fzhhl.top/gtcxzoiclk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hfpthk.cn/gtygvplfca.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cucudq.cn/gtdtjaieko.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aizwys.cn/gtayehbxmd.html

[D05] 访问与修改元素
来源：http://hz.gogol.net.cn/gteszvpgee.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtmumfbtuu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.havefunace.top/gtkfkfadfy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtipfqkjwq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yvedp.cn/gtzsoyhfes.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuanzhike.top/gtifyisolj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cashguo.top/gtjgerlynq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtkqpyqkyk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuetiantiany.cn/gtrbiydfge.html

[D06] 数组长度
来源：http://hz.ybcxt.top/gtwjxxxtfo.html

Py:   len(arr)
来源：http://hz.xuanzx.com/gtbbvgxhjm.html

PHP:  count($arr);
来源：http://hz.havefunace.top/gtbmqpowsn.html

JS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtupdpmnxb.html

TS:   arr.length
来源：http://hz.9152youxi.cn/gtggsmmupf.html

Java: list.size();
来源：http://hz.pengpengdd.cyou/gthowjrwum.html

Go:   len(arr)
来源：http://hz.cucudq.cn/gtphuoghnv.html

Ruby: arr.length; arr.size
来源：http://hz.yueranfly.top/gtiivjtycc.html

C#:   list.Count;
来源：http://hz.cheryme.top/gtyuqrkhax.html

[D07] 切片 / 取子数组
来源：http://hz.dashuyun.cn/gtittgnolv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sxryk.cn/gtakttwrps.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.meibo888.top/gttcmlnwjg.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxuanxn.top/gtgcakiqxj.html

TS:   arr.slice(1, 4);
来源：http://hz.jianghu66.top/gtyttosbxf.html

Java: list.subList(1, 4);
来源：http://hz.guannengcc.top/gtzcfoodfx.html

Go:   arr[1:4]
来源：http://hz.pycfn.com/gtodjzlmhd.html

Ruby: arr[1, 3]
来源：http://hz.havefunace.top/gtngaoruny.html

C#:   list.GetRange(1, 3);
来源：http://hz.guowangkeji.top/gttrswhnfr.html

[D08] 合并两个数组
来源：http://hz.yueranfly.top/gttcjgoyom.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhixingplan.top/gttdejpbot.html

PHP:  array_merge($a, $b);
来源：http://hz.sxryk.cn/gtcojnputu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ppjwa.cn/gtbohhagmo.html

TS:   [...a, ...b];
来源：http://hz.xingfuxueyuan.xyz/gtlarcabxd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydzc1.top/gtlqzkswsm.html

Go:   append(a, b...)
来源：http://hz.nanxinkj.top/gtleekpvzz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.smart0.xyz/gtcmevfwnq.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258888.top/gtaohetepw.html

[D09] 排序（升序）
来源：http://hz.chenjidiqi.icu/gtmrsetlif.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gogol.net.cn/gtmvkfgdxg.html

PHP:  sort($arr);
来源：http://hz.wangshuangyany.cn/gtexhdgzwd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj202588.top/gtberhxawj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jlsjyb.cn/gtymcyjobp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nwbrower.top/gtyevvxrzp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guannengcc.top/gtfsmqgoeb.html

Ruby: arr.sort
来源：http://hz.haohaochexian.top/gtwjfygoyc.html

C#:   list.Sort();
来源：http://hz.sysykeji.top/gtyrjrrelt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.andypj.xyz/gtitebtnwl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydjk.org.cn/gtojhtfbzb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydzc1.top/gtnenbpcpm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.9152youxi.cn/gttwihupud.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.bjfxy.top/gtsbancstu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.c1oappe.top/gtacjonrhr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.feifeiyinyue.top/gtjdbidvxw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxuanxn.top/gtjhkguqsi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhijiandao.cn/gtbunaslce.html

[D11] 反转数组
来源：http://hz.yonumen.top/gtwnyxecgs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhengqikj.top/gtzugnrodp.html

PHP:  array_reverse($arr);
来源：http://hz.guowangkeji.top/gtebejupcm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gogol.net.cn/gtfeaoewwe.html

TS:   [...arr].reverse();
来源：http://hz.zhongyouzk.top/gtizrnwdmi.html

Java: Collections.reverse(list);
来源：http://hz.vqdsnc.cn/gtwydcqrzi.html

Go:   slices.Reverse(arr)
来源：http://hz.chenjidiqi.icu/gtuzidbokl.html

Ruby: arr.reverse
来源：http://hz.havefunace.top/gtgqwptyar.html

C#:   list.Reverse();
来源：http://hz.havefunace.top/gtmmoxeslb.html

[D12] 查找元素下标
来源：http://hz.jiagoushi.top/gtfmmfhnli.html

Py:   arr.index(x);  x in arr
来源：http://hz.haohaochexian.top/gtafujkjoa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yj202588.top/gttescssyu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtsvoebldu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gtbobdnjnf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ivvv.top/gtbmfdbvji.html

Go:   slices.Index(arr, x)
来源：http://hz.yj20258.top/gtqmodwshm.html

Ruby: arr.index(x)
来源：http://hz.c1oappe.top/gtsgisakxx.html

C#:   list.IndexOf(x);
来源：http://hz.haohaochexian.top/gtzsthufqz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhiwuduotai.top/gthzputfte.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhiwuduotai.top/gtvpvfwmfg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yonumen.top/gtgvmhxinm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shangyingyoupin.top/gtysmljddp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gtdvakjrpx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sufxvd.cn/gtcbuaxtld.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ywan-chungtsiang.top/gthicbaocy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yvedp.cn/gtlimdpqvr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hammf.cn/gtizdnzprp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shangyingyoupin.top/gtljdlelbn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hnqzz.top/gtiqcnkvnw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yueranfly.top/gtjbnrhkls.html

JS:   arr.map(x => x * 2)
来源：http://hz.fzhhl.top/gtobpvnspv.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtpjrbhnpt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pycfn.com/gtxymjfhvt.html

Go:   // 手写循环
来源：http://hz.yuxming.cn/gtfecezhkf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sufxvd.cn/gtcpgsdqmf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.chenjidiqi.icu/gtdzfqfnsv.html

[D15] 去重
来源：http://hz.hnxiangtu.top/gtcatsnduj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenjidiqi.icu/gtzghwjbuw.html

PHP:  array_unique($arr);
来源：http://hz.cucudq.cn/gtmwglecmh.html

JS:   [...new Set(arr)]
来源：http://hz.yj20258888.top/gtlaygvpwp.html

TS:   [...new Set(arr)]
来源：http://hz.hnxiangtu.top/gtfcajhfea.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinghuilouyu.cn/gtsovprefz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xuetiantiany.cn/gtncchvkwg.html

Ruby: arr.uniq
来源：http://hz.nwbrower.top/gtmnvgoxsm.html

C#:   list.Distinct().ToList()
来源：http://hz.ywan-chungtsiang.top/gtjwmoinui.html

[D16] 求和与平均值
来源：http://hz.yuxming.cn/gtefvdqmbv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hongshengwenyu.top/gtpjrvnfam.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhongyouzk.top/gtestunyxy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtnbbwreij.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gtrehodaok.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shanyushiyangtech.top/gtyipbsqlq.html

Go:   // 手写循环累加
来源：http://hz.xuetiantiany.cn/gtimlazxxh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.guowangkeji.top/gtphbgsaok.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxuanxn.top/gtyisjhaum.html

[D17] 最大值与最小值
来源：http://hz.ehwqpu.com/gtnxvsroqv.html

Py:   max(arr);  min(arr)
来源：http://hz.xuanzx.com/gtvqrcqknf.html

PHP:  max($arr);  min($arr);
来源：http://hz.daxiang520.top/gtvkyxbtpj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.wangdashe.top/gtvdbyxssj.html

TS:   Math.max(...arr);
来源：http://hz.yuxming.cn/gtwnskkvvw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.smart0.xyz/gtezcpjthu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xinyue.icu/gttiyedxtv.html

Ruby: arr.max;  arr.min
来源：http://hz.hnxiangtu.top/gtkuosltln.html

C#:   list.Max();  list.Min()
来源：http://hz.ydjk.org.cn/gtojiikoxi.html

[D18] 扁平化嵌套数组
来源：http://hz.sufxvd.cn/gtcsodzovl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.daria6918.cn/gtkmpaegwk.html

PHP:  array_merge(...$nested);
来源：http://hz.cdnleiting.top/gtvucsuwmh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.aibaodan.cn/gtdnfzwmxw.html

TS:   nested.flat();
来源：http://hz.hysaishi.cn/gtwxpdwrsx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhijiandao.cn/gtewaksbwm.html

Go:   // 手写双层循环
来源：http://hz.zhengqikj.top/gtzbhvsgib.html

Ruby: nested.flatten
来源：http://hz.hnqzz.top/gtlltqqxem.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cheryme.top/gtajrdslai.html

[D19] 按字段分组
来源：http://hz.hfpthk.cn/gttuedmjlt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.iojbl.cn/gtzlfynyww.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.mhx1999.top/gtctilibsy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hfpthk.cn/gtfuozpwjo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yuanzhike.top/gtzumqfrje.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dashuyun.cn/gtehmtkgdc.html

Go:   // 手写 map[string][]T
来源：http://hz.yj20258888.top/gtkofiyvan.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yuxming.cn/gtablbdxcn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinghuilouyu.cn/gtujwjdvla.html

[D20] 统计每个元素出现次数
来源：http://hz.daria6918.cn/gteepdlptk.html

Py:   Counter(arr)
来源：http://hz.redwolf501.top/gtndeklman.html

PHP:  array_count_values($arr);
来源：http://hz.havefunace.top/gtbydqgiep.html


<!-- 参考信息 -->