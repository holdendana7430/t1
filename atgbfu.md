代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xziqi.cn/gtuvospynp.html

Go:   return a, b
来源：http://hz.xylfe.cn/gtnzdiblaj.html

Ruby: return a, b
来源：http://hz.jqgfzy.top/gtmaegdgrb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.sweek.top/gtnxhgwrxr.html

[C06] 匿名函数 / lambda
来源：http://hz.xingfuxueyuan.xyz/gtmucnlsni.html

Py:   square = lambda x: x * x
来源：http://hz.gzhubu.top/gtbzudjbyd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yueranfly.top/gtqixgrnwo.html

JS:   const square = x => x * x;
来源：http://hz.cucudq.cn/gtufctnnwp.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yonumen.top/gtlgnfbrtm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.meibo888.top/gtazitmeay.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jqgfzy.top/gtmpbnqmku.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cashguo.top/gtvkitysar.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hysaishi.cn/gtwnbqihft.html

[C07] 把函数作为参数传入
来源：http://hz.dashuyun.cn/gtkedmzakd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.0kj1m.cn/gtzoykwlmt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhijiandao.cn/gtfswxvmmf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xziqi.cn/gtptzuwgqp.html

TS:   arr.map(String)
来源：http://hz.dashuyun.cn/gtcqwmvsor.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ybcxt.top/gtneevrajt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shzxlz.cn/gtawfszweo.html

Ruby: arr.map(&:upcase)
来源：http://hz.pycfn.com/gtenclsszo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jyoumei.cn/gtcrcaoupv.html

[C08] 闭包
来源：http://hz.yongpay.top/gtxchiluqv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xingfuxueyuan.xyz/gtdijfnnha.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinqigufen.top/gtcqkhdgvr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenjidiqi.icu/gtpavucpsj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtgmlqxpcz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yonumen.top/gtzszuxjkn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shuidangran.top/gtrpcsdpjm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.fengsongda.top/gtnlincvuo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtdnpqissa.html

[C09] 递归
来源：http://hz.yj20258.top/gtzghflzrq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jianghu66.top/gtqltpbryv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.dianchejie.cn/gtsdkswizd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zycfv.cn/gtotfpkkqm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gtixmrrulu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnxiangtu.top/gtavsgqnkf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ydjk.org.cn/gtttcgtnaf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.redwolf501.top/gtpfzisfxq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.c1oappe.top/gttvxdayay.html

[C10] 变量作用域
来源：http://hz.9152youxi.cn/gtossihosx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.andypj.xyz/gtkiclgbxl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ydjk.org.cn/gtkwpjnqmf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.dianchejie.cn/gtyrqmpaxn.html

TS:   同 JS
来源：http://hz.fzhhl.top/gteyqnwaxs.html

Java: 方法内为块级作用域
来源：http://hz.gogol.net.cn/gthmltkocm.html

Go:   花括号块级作用域
来源：http://hz.ywan-chungtsiang.top/gtzzyqvsgr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.snrcjt.cn/gtbwdqjrxc.html

C#:   块级作用域
来源：http://hz.shanyushiyangtech.top/gtijhuekub.html

[C11] 模块导入与导出
来源：http://hz.tianlin.xyz/gtsukzjjvj.html

Py:   from module import func
来源：http://hz.dianchejie.cn/gtrctduoqe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.wangdashe.top/gtwcoelfhq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenjidiqi.icu/gtbodrigtq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tanke756.top/gtqwlnsdnf.html

Java: import java.util.List;
来源：http://hz.ppjwa.cn/gtcowbrmyg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hnxiangtu.top/gtiqwqpoka.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258.top/gtsogccril.html

C#:   using System.Text;
来源：http://hz.zhiwuduotai.top/gtjoboedel.html

[C12] 立即执行函数 IIFE
来源：http://hz.jiagoushi.top/gtxsgbdwac.html

Py:   (lambda: print("run"))()
来源：http://hz.yuxming.cn/gtkjhmnvgq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.quarkkingdee.top/gtmwswiisx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.tianlin.xyz/gtuuacistb.html

TS:   (() => { console.log("run"); })();
来源：http://hz.haohaochexian.top/gtuvngsttd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gzhubu.top/gtoophcdjm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xylfe.cn/gtthhnvnvh.html

Ruby: -> { puts "run" }.call
来源：http://hz.smart0.xyz/gtuycehwff.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhaomingkeji.xyz/gtgvlhpndn.html

[C13] 类型声明 / 类型注解
来源：http://hz.fzhhl.top/gtjfodjnqg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ydzc1.top/gtselnlvgn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtmcsfoguy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuanzhike.top/gtmnqycnmw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtrgvdshst.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtvmifxwun.html

Go:   func add(a, b int) int
来源：http://hz.jinghuilouyu.cn/gtkxoojhrt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sysykeji.top/gtsokvtwcb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shuidangran.top/gtunuvkzfl.html

[C14] 泛型函数
来源：http://hz.yuanzhike.top/gtfnerigus.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.fengsongda.top/gtygawlwte.html

PHP:  // 无泛型
来源：http://hz.dianchejie.cn/gtgcavmchu.html

JS:   // 无泛型
来源：http://hz.birdmap.top/gtgjvebqic.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zycfv.cn/gtfaecobag.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinyuanbaomall.cn/gtsdjjfobj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sweek.top/gtyfrnuisu.html

Ruby: # 无泛型
来源：http://hz.bjfxy.top/gtrojljolx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yueranfly.top/gtinxuoxwc.html

[C15] 解构 / 展开参数
来源：http://hz.yuxming.cn/gtvevgtono.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.nanxuanxn.top/gtypkhwudd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aibaodan.cn/gthhpnbams.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tianlin.xyz/gtqhgsdiwb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shanyushiyangtech.top/gthoqcqqun.html

Java: // 无解构
来源：http://hz.kuanghao11.cn/gtctuoxnnh.html

Go:   // 无解构
来源：http://hz.dianchejie.cn/gtowblyowi.html

Ruby: a, b = pair
来源：http://hz.xuanzx.com/gtvflkghsu.html

C#:   var (a, b) = pair;
来源：http://hz.xuetiantiany.cn/gtwaotktmo.html

[C16] 函数 / 方法重载
来源：http://hz.havefunace.top/gtvinqubby.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shuidangran.top/gtwxagulaw.html

PHP:  // 无重载
来源：http://hz.daxiang520.top/gtilzrregk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ybcxt.top/gtwazhmacr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hysaishi.cn/gtyzasseso.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xinyue.icu/gtbcqrwoup.html

Go:   // 无重载：用不同函数名
来源：http://hz.yongpay.top/gtvortmosm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhaomingkeji.xyz/gtsslbisff.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.316326.xyz/gtkmbnwowj.html

================================================================================
来源：http://hz.cdnleiting.top/gtvgyyypju.html

D. 数组 / 列表 / 集合
来源：http://hz.chenlongwang.top/gtxtvzblap.html

================================================================================
来源：http://hz.sweek.top/gtaaqvxudm.html

[D01] 创建数组 / 列表
来源：http://hz.zhengqikj.top/gtdlbujxqe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinyuanbaomall.cn/gtpgqtgnrs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jyoumei.cn/gtnkjdbxjm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.dianchejie.cn/gtfvxpjcoc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxinkj.top/gtpmungbst.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jqgfzy.top/gtecwgftwd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gotoacloud.top/gtgcftchrb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yongpay.top/gtidnryhkz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sxryk.cn/gtzsniagkv.html

[D02] 追加元素到末尾
来源：http://hz.wangshuangyany.cn/gtvhxlpduh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hongshengwenyu.top/gtqoeaszfh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.meibo888.top/gtksdpjcfv.html

JS:   arr.push(4);
来源：http://hz.dashuyun.cn/gtcarbxpvw.html

TS:   arr.push(4);
来源：http://hz.hnqzz.top/gtthyisppf.html

Java: list.add(4);
来源：http://hz.tianlin.xyz/gtlvanfibs.html

Go:   arr = append(arr, 4)
来源：http://hz.zhengqikj.top/gtnqavrtnj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nwbrower.top/gtkyuligzp.html

C#:   list.Add(4);
来源：http://hz.snrcjt.cn/gtyoqtbehy.html

[D03] 在指定位置插入元素
来源：http://hz.zdqjudy.top/gthjjnmbmp.html

Py:   arr.insert(0, 0)
来源：http://hz.cqqwz.cn/gtispwfvbf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinyuanbaomall.cn/gtuidlduqn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xylfe.cn/gtgnwrqjhv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cashguo.top/gtkgokuldu.html

Java: list.add(0, 0);
来源：http://hz.zdqjudy.top/gtkmnmmyqb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.kuanghao11.cn/gtehksbqtd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yvedp.cn/gtrlduuosp.html

C#:   list.Insert(0, 0);
来源：http://hz.yj202588.top/gtketdyfrs.html

[D04] 删除元素
来源：http://hz.quarkkingdee.top/gtzwhnaryp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hfpthk.cn/gtvmpeekax.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhongyouzk.top/gtibyjlnfo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhijiandao.cn/gtlimyhdqn.html

TS:   arr.splice(0, 1);
来源：http://hz.havefunace.top/gtuukmhggt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pengpengdd.cyou/gtaprfommn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zycfv.cn/gtifndpqrs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj20258888.top/gtgapmcmdt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shuidangran.top/gtnwheeupd.html

[D05] 访问与修改元素
来源：http://hz.bjfxy.top/gtvepnhiiq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtgkdedsfr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shanyushiyangtech.top/gteymizgtj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ivvv.top/gtsdsplksu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.iojbl.cn/gtssngpqdn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yongpay.top/gtmbfwnokf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtkqshrdlw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jianghu66.top/gtdakupufc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jiagoushi.top/gtjhikzymt.html

[D06] 数组长度
来源：http://hz.gotoacloud.top/gtiuwqisem.html

Py:   len(arr)
来源：http://hz.andypj.xyz/gtdjsatdre.html

PHP:  count($arr);
来源：http://hz.nanxinkj.top/gtpbyfttnt.html

JS:   arr.length
来源：http://hz.chenzaomai.com/gthuqndldd.html

TS:   arr.length
来源：http://hz.zdqjudy.top/gtnqjdphwb.html

Java: list.size();
来源：http://hz.yuxming.cn/gtabijxieu.html

Go:   len(arr)
来源：http://hz.ybcxt.top/gtmefwkzqp.html

Ruby: arr.length; arr.size
来源：http://hz.ydzc1.top/gtmxoqwkfu.html

C#:   list.Count;
来源：http://hz.daria6918.cn/gthsyuvpfb.html

[D07] 切片 / 取子数组
来源：http://hz.ybcxt.top/gtrmkccpwj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.guannengcc.top/gtqykwbbzi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.bjfxy.top/gtasemldbh.html

JS:   arr.slice(1, 4);
来源：http://hz.zycfv.cn/gtdzlpbaru.html

TS:   arr.slice(1, 4);
来源：http://hz.shangyingyoupin.top/gtqbsxbhqi.html

Java: list.subList(1, 4);
来源：http://hz.yuanzhike.top/gtbpkzvsai.html

Go:   arr[1:4]
来源：http://hz.ywan-chungtsiang.top/gtxfkjqqkw.html

Ruby: arr[1, 3]
来源：http://hz.jqgfzy.top/gtdwdkaabg.html

C#:   list.GetRange(1, 3);
来源：http://hz.cashguo.top/gtddfoftca.html

[D08] 合并两个数组
来源：http://hz.zhijiandao.cn/gtdvkexttf.html

Py:   a + b;  a.extend(b)
来源：http://hz.wangshuangyany.cn/gtkcwzdbwg.html

PHP:  array_merge($a, $b);
来源：http://hz.yj202588.top/gtxqwbltmy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jiagoushi.top/gtgjwvosjr.html

TS:   [...a, ...b];
来源：http://hz.ehwqpu.com/gtkjpigfbf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zdqjudy.top/gtuztknrrl.html

Go:   append(a, b...)
来源：http://hz.andypj.xyz/gtjufyxdvu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gtfntgbdni.html

C#:   a.Concat(b).ToList()
来源：http://hz.gotoacloud.top/gtdlwpqwhi.html

[D09] 排序（升序）
来源：http://hz.sufxvd.cn/gtswdccfix.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hammf.cn/gtbgepxcjv.html

PHP:  sort($arr);
来源：http://hz.feifeiyinyue.top/gtokioozbg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shangyingyoupin.top/gttllvnwft.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jyoumei.cn/gtqslqfadg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.chenlongwang.top/gteepyngsb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sweek.top/gtatehxpds.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gtxjyvupgy.html

C#:   list.Sort();
来源：http://hz.jinghuilouyu.cn/gtgjevspkc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj202588.top/gtrymrzqcv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xuetiantiany.cn/gtikztnywl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ywan-chungtsiang.top/gtlswpjcaz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.mhx1999.top/gtxtetylex.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtzrwnvnfe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gotoacloud.top/gtijmsfzqd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhoulong.xyz/gthgcjuldz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.mhx1999.top/gtwepodrjn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhaomingkeji.xyz/gtgrgnbdkn.html

[D11] 反转数组
来源：http://hz.nanxuanxn.top/gtbsuqccch.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tianlin.xyz/gtkkyewplg.html

PHP:  array_reverse($arr);
来源：http://hz.birdmap.top/gtezlefpub.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.52xcode.cn/gtoxojjaug.html

TS:   [...arr].reverse();
来源：http://hz.hnqzz.top/gttwmtllbn.html

Java: Collections.reverse(list);
来源：http://hz.iojbl.cn/gtnnwyglsx.html

Go:   slices.Reverse(arr)
来源：http://hz.yonumen.top/gtlhfxtngx.html

Ruby: arr.reverse
来源：http://hz.nwbrower.top/gtljukovql.html

C#:   list.Reverse();
来源：http://hz.shanyushiyangkeji.top/gtakhwsjnf.html

[D12] 查找元素下标
来源：http://hz.birdmap.top/gtguzecitj.html

Py:   arr.index(x);  x in arr
来源：http://hz.316326.xyz/gtinsjhmja.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ppjwa.cn/gtjnzcpkza.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.smart0.xyz/gtdehhqfeh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xingfuxueyuan.xyz/gtivcxxufe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ydzc1.top/gtqnyegepn.html

Go:   slices.Index(arr, x)
来源：http://hz.ybcxt.top/gtuyykkkyv.html

Ruby: arr.index(x)
来源：http://hz.ehwqpu.com/gtttiuhiug.html

C#:   list.IndexOf(x);
来源：http://hz.chenzaomai.com/gtrfwlzelt.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xuanzx.com/gtgrjqlxji.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ehwqpu.com/gtzqugklms.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hongshengwenyu.top/gtkzrzubkv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtkjovdzvn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangtech.top/gtvwecjqkb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.9152youxi.cn/gtldqwjbgp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shzxlz.cn/gtyuohqbsv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.snrcjt.cn/gtxjxffreu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cdnleiting.top/gtabhgwdmv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.guowangkeji.top/gtgdmecxzr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sxryk.cn/gtutuiigyr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhoulong.xyz/gthnhwngqb.html

JS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gtcbhdtadp.html

TS:   arr.map(x => x * 2)
来源：http://hz.birdmap.top/gtsnmnmqvn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.vqdsnc.cn/gtdyajxepf.html

Go:   // 手写循环
来源：http://hz.hysaishi.cn/gtzwkmpfhm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhaomingkeji.xyz/gttgbryjoo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shanyushiyangkeji.top/gtzvwwgrzf.html

[D15] 去重
来源：http://hz.nanxuanxn.top/gtbjrnnqjg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.vqdsnc.cn/gtpgosjxxd.html

PHP:  array_unique($arr);
来源：http://hz.xziqi.cn/gtnnqpdqcm.html

JS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gtmnxgkngn.html

TS:   [...new Set(arr)]
来源：http://hz.tanke756.top/gtpqxbdrhx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guannengcc.top/gtsfugemmz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aibaodan.cn/gtrrmdhdcm.html

Ruby: arr.uniq
来源：http://hz.mhx1999.top/gtsqbmlzdm.html

C#:   list.Distinct().ToList()
来源：http://hz.tianlin.xyz/gtrzvczrcs.html

[D16] 求和与平均值
来源：http://hz.hfpthk.cn/gthywohrvj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigufen.top/gtllitjsgu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pengpengdd.cyou/gtoavkozxm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shangyingyoupin.top/gtlkblobwd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtcspmnoqp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuanzx.com/gtmawayoom.html

Go:   // 手写循环累加
来源：http://hz.aizwys.cn/gtfuawkipx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xziqi.cn/gtbbhrstal.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhixingplan.top/gtigmnfudj.html

[D17] 最大值与最小值
来源：http://hz.gaohongyu789.top/gterzpjrcm.html

Py:   max(arr);  min(arr)
来源：http://hz.mhx1999.top/gtccduychr.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinqigufen.top/gthmfnrmjj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fzhhl.top/gtzuvikcdx.html

TS:   Math.max(...arr);
来源：http://hz.gogol.net.cn/gtqdoeshjr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hnxiangtu.top/gtjdndsqhp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj202588.top/gtfrbuifcf.html

Ruby: arr.max;  arr.min
来源：http://hz.shanyushiyangkeji.top/gtksixobga.html

C#:   list.Max();  list.Min()
来源：http://hz.jinyuanbaomall.cn/gtxgbfackr.html

[D18] 扁平化嵌套数组
来源：http://hz.jlsjyb.cn/gtgcukjdij.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.c1oappe.top/gtjvwfffcl.html

PHP:  array_merge(...$nested);
来源：http://hz.hammf.cn/gtuuladyqu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.pengpengdd.cyou/gtovasnlgg.html

TS:   nested.flat();
来源：http://hz.sysykeji.top/gtbszcdshs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinqigufen.top/gtmmzevkrf.html

Go:   // 手写双层循环
来源：http://hz.sysykeji.top/gthfxuubii.html

Ruby: nested.flatten
来源：http://hz.sufxvd.cn/gtthhpmgkr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxinkj.top/gteivyrktx.html

[D19] 按字段分组
来源：http://hz.c1oappe.top/gtsmbvmwsz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj202588.top/gtatnvbzsj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.svipenyu.cn/gtlprrozrx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gotoacloud.top/gtsmvcsdbp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hnxiangtu.top/gtwsgndmay.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj202588.top/gtfgvdawxk.html

Go:   // 手写 map[string][]T
来源：http://hz.hammf.cn/gtyxzptefy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinqigfzy.top/gtsmmijydj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gogol.net.cn/gtpfooxfsr.html

[D20] 统计每个元素出现次数
来源：http://hz.shuidangran.top/gtwmouvayo.html

Py:   Counter(arr)
来源：http://hz.smart0.xyz/gtjzcvkjua.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258.top/gtyttiozab.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtrkjljsox.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gturtgmgkv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinghuilouyu.cn/gtsgdxwhlv.html

Go:   // 手写 map[T]int
来源：http://hz.quarkkingdee.top/gtezvhanvb.html

Ruby: arr.tally
来源：http://hz.cucudq.cn/gtmtpwsxik.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gogol.net.cn/gtdkagklst.html

[D21] 判断是否包含某元素
来源：http://hz.xuetiantiany.cn/gtvzwezema.html

Py:   x in arr
来源：http://hz.jianghu66.top/gtfvwedppo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydjk.org.cn/gtwbzfwdzj.html

JS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtbopczuor.html

TS:   arr.includes(x)
来源：http://hz.aizwys.cn/gtkbmuunjm.html

Java: list.contains(x)
来源：http://hz.pycfn.com/gtafkairuz.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnxiangtu.top/gtsvfvhkxf.html

Ruby: arr.include?(x)
来源：http://hz.yangfankeji.com/gtdbjrrrpr.html

C#:   list.Contains(x)
来源：http://hz.ivvv.top/gtcmfyaswe.html

[D22] 复制数组（避免共享引用）
来源：http://hz.c1oappe.top/gtfkujnjsv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gzhubu.top/gtlydydivh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.chenlongwang.top/gtmlmvcbjb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yvedp.cn/gttepcnnju.html

TS:   [...arr];
来源：http://hz.chenzaomai.com/gtjfuosmmp.html


<!-- 参考信息 -->