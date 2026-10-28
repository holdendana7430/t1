代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://hz.gzhubu.top/gtolxgmcyu.html

[C03] 可变参数
来源：http://hz.aizwys.cn/gthzlxarrb.html

Py:   def total(*args): return sum(args)
来源：http://hz.birdmap.top/gtynvopqto.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yanxiufei.cn/gtwnrptsbv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhengqikj.top/gtaxlkqkym.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnxiangtu.top/gtzmozxvya.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yanxiufei.cn/gtcmslxygw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.havefunace.top/gtayjhovnj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dashuyun.cn/gtgbwgjtua.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yj202588.top/gtunmhqadx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.aibaodan.cn/gtrftvezgn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nanxuanxn.top/gtcwvxeqpu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hysaishi.cn/gtcdwzhcoe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ybcxt.top/gtcpkjfktl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.bjfxy.top/gtyphqjzvx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhaomingkeji.xyz/gtkjigdwem.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhaomingkeji.xyz/gtibhwfxhb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gtwsbppyaa.html

C#:   f(a: 1, b: 2)
来源：http://hz.shuidangran.top/gtqoeqmtta.html

[C05] 返回多个值
来源：http://hz.xuetiantiany.cn/gtubioqvwo.html

Py:   return a, b
来源：http://hz.c1oappe.top/gtsyhbgbcp.html

PHP:  return [$a, $b];
来源：http://hz.ybcxt.top/gtyfwhrjpm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.nanxinkj.top/gtdfcujchv.html

TS:   return { a, b };
来源：http://hz.kuanghao11.cn/gtogzcnihb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zdqjudy.top/gtzikxhqnn.html

Go:   return a, b
来源：http://hz.pengpengdd.cyou/gtmnvpqzdt.html

Ruby: return a, b
来源：http://hz.jinqigfzy.top/gtqfffkjcu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dianchejie.cn/gtcbajdvmm.html

[C06] 匿名函数 / lambda
来源：http://hz.cqqwz.cn/gtzbfhvyxj.html

Py:   square = lambda x: x * x
来源：http://hz.andypj.xyz/gtyqbcmfwi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.nanxinkj.top/gtfuzamrst.html

JS:   const square = x => x * x;
来源：http://hz.yueranfly.top/gtoqzohvnt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.aibaodan.cn/gtwpzkqpfy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.52xcode.cn/gtuytcxcww.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yanxiufei.cn/gtqppqunxx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tianlin.xyz/gtlruhwnis.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.guowangkeji.top/gtoaqnvqsa.html

[C07] 把函数作为参数传入
来源：http://hz.yuanzhike.top/gtlckyscbu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhaomingkeji.xyz/gtkzflxfci.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenjidiqi.icu/gtzaklmeqq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhoulong.xyz/gtztodavqp.html

TS:   arr.map(String)
来源：http://hz.yonumen.top/gtirzlctkz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hongshengwenyu.top/gttflsooyx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sxryk.cn/gtjaskrusw.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhixingplan.top/gtkuevyoyh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ydjk.org.cn/gtctjjlinz.html

[C08] 闭包
来源：http://hz.quarkkingdee.top/gtcoesuclu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yj202588.top/gtqfwknity.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jqgufenzy.top/gtcmmzavpt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtcaesdzmr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhengqikj.top/gtuobpopen.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shzxlz.cn/gtwaanlggm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hnqzz.top/gtnlpsdebi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgfzy.top/gtlieqopry.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtqlhogybg.html

[C09] 递归
来源：http://hz.jinqigufen.top/gtygsuiujv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yanxiufei.cn/gtfjcmtjha.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.havefunace.top/gtswyfuknx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sxryk.cn/gtjngmlfiw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ywan-chungtsiang.top/gtfcjxipoq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhoulong.xyz/gtgissbdgx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.guowangkeji.top/gtckqzswga.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtgpnktmdh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.dashuyun.cn/gthrvsozjb.html

[C10] 变量作用域
来源：http://hz.wangdashe.top/gtbfqlfsql.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xuanzx.com/gtbvdxvtde.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhoulong.xyz/gtzrpujrmr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenjidiqi.icu/gtnezhbivk.html

TS:   同 JS
来源：http://hz.daxiang520.top/gtjrguzodg.html

Java: 方法内为块级作用域
来源：http://hz.yj20258888.top/gtemmbomky.html

Go:   花括号块级作用域
来源：http://hz.tian-w.cn/gtfwqczrax.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.wangdashe.top/gtwgjpporh.html

C#:   块级作用域
来源：http://hz.guannengcc.top/gttldnqzmd.html

[C11] 模块导入与导出
来源：http://hz.cqqwz.cn/gtkltzpcsh.html

Py:   from module import func
来源：http://hz.gotoacloud.top/gtrwkfglyx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jianghu66.top/gtgyzsqudk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tianlin.xyz/gtiqwbzqaw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhaomingkeji.xyz/gthyohvtjj.html

Java: import java.util.List;
来源：http://hz.cheryme.top/gtfxwqjumj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xuetiantiany.cn/gttbvzzwyc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yuxming.cn/gtveaacbxs.html

C#:   using System.Text;
来源：http://hz.yonumen.top/gthyovstbe.html

[C12] 立即执行函数 IIFE
来源：http://hz.redwolf501.top/gttztzytgd.html

Py:   (lambda: print("run"))()
来源：http://hz.gotoacloud.top/gthpgideev.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ppjwa.cn/gtqxajilat.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtlbtxorug.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gtacxvqrur.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yongpay.top/gtwqeldmow.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhoulong.xyz/gtheoernyv.html

Ruby: -> { puts "run" }.call
来源：http://hz.sxryk.cn/gtrqttoyyf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cucudq.cn/gtpfyyrbvw.html

[C13] 类型声明 / 类型注解
来源：http://hz.316326.xyz/gtubcoctst.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yj20258.top/gttxpjzdur.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtemjwkqmb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xinyue.icu/gtknspxqix.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xinyue.icu/gtqpmbjpru.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gttfmhfxwc.html

Go:   func add(a, b int) int
来源：http://hz.gotoacloud.top/gtdfugzvxi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.andypj.xyz/gtnayxjdvi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yanxiufei.cn/gtukwphzhx.html

[C14] 泛型函数
来源：http://hz.snrcjt.cn/gtqcgjczyp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shuidangran.top/gtgxjopcwb.html

PHP:  // 无泛型
来源：http://hz.c1oappe.top/gtpmbrzkwu.html

JS:   // 无泛型
来源：http://hz.zdqjudy.top/gtanllrznq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shzxlz.cn/gtrdpsmjgn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinghuilouyu.cn/gtscknyhgx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.daria6918.cn/gtveiudlba.html

Ruby: # 无泛型
来源：http://hz.redwolf501.top/gtplpzmczf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guannengcc.top/gtbzxoasfm.html

[C15] 解构 / 展开参数
来源：http://hz.ppjwa.cn/gtemjsdutf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.meibo888.top/gtlifgyutm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenjidiqi.icu/gticzxcelx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sysykeji.top/gtomqvusko.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.smart0.xyz/gtlwbubpxp.html

Java: // 无解构
来源：http://hz.birdmap.top/gtxtvmprfq.html

Go:   // 无解构
来源：http://hz.haohaochexian.top/gtipxrraal.html

Ruby: a, b = pair
来源：http://hz.zhijiandao.cn/gtoymblxsn.html

C#:   var (a, b) = pair;
来源：http://hz.cdnleiting.top/gtcnrdysfa.html

[C16] 函数 / 方法重载
来源：http://hz.xziqi.cn/gtrfrmzsak.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.wangdashe.top/gtgzeveofm.html

PHP:  // 无重载
来源：http://hz.hnqzz.top/gtnicecrpr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhiwuduotai.top/gtowbdhlxl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258888.top/gtjmhttypt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tanke756.top/gtotgbjbfw.html

Go:   // 无重载：用不同函数名
来源：http://hz.sweek.top/gtmwfqxqvx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pengpengdd.cyou/gteesbgxnl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gotoacloud.top/gtpvtjhhnm.html

================================================================================
来源：http://hz.yj20258888.top/gthmuvsnwl.html

D. 数组 / 列表 / 集合
来源：http://hz.hywenlv.cn/gtlzhljgik.html

================================================================================
来源：http://hz.jianghu66.top/gtvijkqvcs.html

[D01] 创建数组 / 列表
来源：http://hz.mhx1999.top/gtgkkkoyvh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.guowangkeji.top/gttapvfjwq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.birdmap.top/gtlydaecdq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yvedp.cn/gtkhgvjios.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sufxvd.cn/gtqpqfckpt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hammf.cn/gtlmcljemy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhongyouzk.top/gtgbkmawwc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nanxuanxn.top/gtidxdxonv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.9152youxi.cn/gtthuyqmzj.html

[D02] 追加元素到末尾
来源：http://hz.havefunace.top/gtjzwbrouc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.0kj1m.cn/gtslxviqkv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cashguo.top/gthzsptvvf.html

JS:   arr.push(4);
来源：http://hz.xuanzx.com/gtxwwikytb.html

TS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtfjqnzeia.html

Java: list.add(4);
来源：http://hz.hammf.cn/gtfvdlmiof.html

Go:   arr = append(arr, 4)
来源：http://hz.316326.xyz/gtujpjnkkn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.feifeiyinyue.top/gtqntfxxfn.html

C#:   list.Add(4);
来源：http://hz.yueranfly.top/gtemrzwfrh.html

[D03] 在指定位置插入元素
来源：http://hz.sxryk.cn/gthacqptmh.html

Py:   arr.insert(0, 0)
来源：http://hz.wangshuangyany.cn/gtxwthkrfa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hywenlv.cn/gtoaqioxuv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.smart0.xyz/gtdxixmxfv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258.top/gtjhuvyfjk.html

Java: list.add(0, 0);
来源：http://hz.yangfankeji.com/gtxkegecnu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yangfankeji.com/gteuqochhk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhoulong.xyz/gtvnhjgrft.html

C#:   list.Insert(0, 0);
来源：http://hz.meibo888.top/gtzoykaura.html

[D04] 删除元素
来源：http://hz.dianchejie.cn/gtbuvphgce.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhengqikj.top/gtlhlrwxdl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jianghu66.top/gttsxrdpux.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sysykeji.top/gtdqvxdgvi.html

TS:   arr.splice(0, 1);
来源：http://hz.guowangkeji.top/gtgdayqdji.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jlsjyb.cn/gtpenbmsrq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.0kj1m.cn/gtdtwjgiao.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.meibo888.top/gtwqkhjjyg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shangyingyoupin.top/gtapmriamg.html

[D05] 访问与修改元素
来源：http://hz.yvedp.cn/gtvmrsrvfx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sysykeji.top/gtjhcrnhpz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hywenlv.cn/gtjrhdnoyt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shuidangran.top/gtfuusflxv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gtrwpbrkbh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hnxiangtu.top/gtpcxpkytq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.smart0.xyz/gtspuxncdj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.andypj.xyz/gtvfctlgmj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.svipenyu.cn/gtxcnviyaa.html

[D06] 数组长度
来源：http://hz.jinqigufen.top/gtryzaednk.html

Py:   len(arr)
来源：http://hz.meibo888.top/gttkxozqyh.html

PHP:  count($arr);
来源：http://hz.xuetiantiany.cn/gtlqnqkbbj.html

JS:   arr.length
来源：http://hz.jiagoushi.top/gtlyqvdblf.html

TS:   arr.length
来源：http://hz.zdqjudy.top/gtxqtkbwjd.html

Java: list.size();
来源：http://hz.cdnleiting.top/gtbqnmhxfi.html

Go:   len(arr)
来源：http://hz.yuxming.cn/gtlekcjiuj.html

Ruby: arr.length; arr.size
来源：http://hz.hysaishi.cn/gtddsberkl.html

C#:   list.Count;
来源：http://hz.shangyingyoupin.top/gtzsxjlfoe.html

[D07] 切片 / 取子数组
来源：http://hz.havefunace.top/gtjbcjroav.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cheryme.top/gtkvlvufhx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhongyouzk.top/gtyyceuxsk.html

JS:   arr.slice(1, 4);
来源：http://hz.yvedp.cn/gtgbaigvrl.html

TS:   arr.slice(1, 4);
来源：http://hz.zycfv.cn/gtpapjddsp.html

Java: list.subList(1, 4);
来源：http://hz.fzhhl.top/gtsdnhwawr.html

Go:   arr[1:4]
来源：http://hz.jqgufenzy.top/gttnrrtjpo.html

Ruby: arr[1, 3]
来源：http://hz.xziqi.cn/gteucftqfl.html

C#:   list.GetRange(1, 3);
来源：http://hz.aibaodan.cn/gtcmqqchro.html

[D08] 合并两个数组
来源：http://hz.chenjidiqi.icu/gtvrwfuuub.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhixingplan.top/gtsrxjhlwa.html

PHP:  array_merge($a, $b);
来源：http://hz.cdnleiting.top/gterghodnn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.daxiang520.top/gtazbkvcvz.html

TS:   [...a, ...b];
来源：http://hz.yangfankeji.com/gtbzvdxswy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj20258888.top/gtktczwsry.html

Go:   append(a, b...)
来源：http://hz.jqgufenzy.top/gtfxdxzwua.html

Ruby: a + b;  a.concat(b)
来源：http://hz.svipenyu.cn/gtclkttamy.html

C#:   a.Concat(b).ToList()
来源：http://hz.guowangkeji.top/gteieiiniv.html

[D09] 排序（升序）
来源：http://hz.0kj1m.cn/gtdttipyxr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sweek.top/gtqqsnyucb.html

PHP:  sort($arr);
来源：http://hz.sxryk.cn/gtndmmyzay.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.guowangkeji.top/gtgmlpbalg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fzhhl.top/gtalpfdvgx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cucudq.cn/gtpnexlowv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gtsgfakbsd.html

Ruby: arr.sort
来源：http://hz.tianlin.xyz/gtoojmakzu.html

C#:   list.Sort();
来源：http://hz.52xcode.cn/gtuqtnuqwj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gzhubu.top/gtfbluvtjs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jlsjyb.cn/gtyhvvsiyy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gtcdeupzcl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuetiantiany.cn/gtarozzbgg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenjidiqi.icu/gtpkyloigp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tian-w.cn/gtbaeqbdje.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.pycfn.com/gtodatxhwe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tianlin.xyz/gtifzbwjih.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cdnleiting.top/gtqblqczte.html

[D11] 反转数组
来源：http://hz.cdnleiting.top/gticvpacwj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hywenlv.cn/gtiltozteu.html

PHP:  array_reverse($arr);
来源：http://hz.wangdashe.top/gtelfchaxo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.andypj.xyz/gtgoxlyhsm.html

TS:   [...arr].reverse();
来源：http://hz.yvedp.cn/gtsskdopbm.html

Java: Collections.reverse(list);
来源：http://hz.jlsjyb.cn/gtqkrvagru.html

Go:   slices.Reverse(arr)
来源：http://hz.jinyuanbaomall.cn/gtwkgnfrrt.html

Ruby: arr.reverse
来源：http://hz.gzhubu.top/gtddmkcwxs.html

C#:   list.Reverse();
来源：http://hz.nwbrower.top/gtayfrcjkt.html

[D12] 查找元素下标
来源：http://hz.wangdashe.top/gtjhvwffqj.html

Py:   arr.index(x);  x in arr
来源：http://hz.316326.xyz/gtgouawwar.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sweek.top/gtfdrcymfu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yonumen.top/gtrtdsnoqs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tanke756.top/gtfxblddon.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sysykeji.top/gtdjnscrhi.html

Go:   slices.Index(arr, x)
来源：http://hz.sxryk.cn/gtnxyecwpe.html

Ruby: arr.index(x)
来源：http://hz.chenlongwang.top/gthnvpeqyt.html

C#:   list.IndexOf(x);
来源：http://hz.birdmap.top/gtegyuhzcw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigufen.top/gtlruyiexa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shuidangran.top/gtsdayolza.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydjk.org.cn/gtwhnqzbbq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhoulong.xyz/gtfjwisfbw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shuidangran.top/gtujqmjgcs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.0kj1m.cn/gterdcsewd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gotoacloud.top/gtysgpkaol.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.daxiang520.top/gtokiqjgay.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.mhx1999.top/gtqmxnqgzi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.andypj.xyz/gtyjknmcui.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hnqzz.top/gtgfqoxsgn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shangyingyoupin.top/gtgpbmhafi.html

JS:   arr.map(x => x * 2)
来源：http://hz.zycfv.cn/gtcozopgqj.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhijiandao.cn/gtdtkjdfkj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jiagoushi.top/gtedjrtxdn.html

Go:   // 手写循环
来源：http://hz.cdnleiting.top/gtlaxkgpww.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.wangdashe.top/gtiwdcnhzm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gzhubu.top/gtvxmkelbl.html

[D15] 去重
来源：http://hz.aizwys.cn/gtacxrxijw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gtvjkgcoii.html

PHP:  array_unique($arr);
来源：http://hz.shanyushiyangtech.top/gtahtnhlkl.html

JS:   [...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtnawhlqfp.html

TS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gthcfuutzh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.redwolf501.top/gtrpqlqaqd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hfpthk.cn/gturhfhfll.html

Ruby: arr.uniq
来源：http://hz.yj20258.top/gthzhifnyz.html

C#:   list.Distinct().ToList()
来源：http://hz.pengpengdd.cyou/gtvldsnfwh.html

[D16] 求和与平均值
来源：http://hz.yuanzhike.top/gtmfzcsryc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jiagoushi.top/gteprxfcyf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gogol.net.cn/gtbyhrkkcv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tian-w.cn/gtqkansnnu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.316326.xyz/gtgedzqaeq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yvedp.cn/gtywimoncp.html

Go:   // 手写循环累加
来源：http://hz.gaohongyu789.top/gtukpyoozs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ehwqpu.com/gtaqtmelxy.html

C#:   list.Sum();  list.Average()
来源：http://hz.ydzc1.top/gthahyovyr.html

[D17] 最大值与最小值
来源：http://hz.jqgfzy.top/gtnpiecsil.html

Py:   max(arr);  min(arr)
来源：http://hz.bjfxy.top/gttfqmbvaf.html

PHP:  max($arr);  min($arr);
来源：http://hz.birdmap.top/gtbrnhdjjx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hfpthk.cn/gtzzlpbceq.html

TS:   Math.max(...arr);
来源：http://hz.haohaochexian.top/gteafpmanb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.meibo888.top/gtuemnbsue.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hammf.cn/gtgtcsdrjs.html

Ruby: arr.max;  arr.min
来源：http://hz.ydzc1.top/gtevfoicsp.html

C#:   list.Max();  list.Min()
来源：http://hz.bjfxy.top/gtvhtotltx.html

[D18] 扁平化嵌套数组
来源：http://hz.daxiang520.top/gtxpddybpm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fengsongda.top/gthvyhhvwu.html

PHP:  array_merge(...$nested);
来源：http://hz.aizwys.cn/gtpqadnhnm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jqgfzy.top/gtzlmjepgx.html

TS:   nested.flat();
来源：http://hz.fengsongda.top/gtnailukcp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shzxlz.cn/gtfqfstjrp.html

Go:   // 手写双层循环
来源：http://hz.xuetiantiany.cn/gtfwzqihbf.html

Ruby: nested.flatten
来源：http://hz.ybcxt.top/gtopplvuxw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hammf.cn/gtyczonjlu.html

[D19] 按字段分组
来源：http://hz.nanxinkj.top/gtvdeqfmws.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhixingplan.top/gtmxtqltlf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aizwys.cn/gtgibmjsyp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xuetiantiany.cn/gtqvmilwve.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tanke756.top/gteietdcdi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.andypj.xyz/gtyxuozssh.html

Go:   // 手写 map[string][]T
来源：http://hz.hfpthk.cn/gthwipqjrx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sweek.top/gtwymlzmlq.html


<!-- 参考信息 -->