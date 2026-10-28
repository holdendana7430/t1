代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jqgfzy.top/gtirrdxdso.html

Go:   return a, b
来源：http://hz.jinghuilouyu.cn/gttrqhvsgv.html

Ruby: return a, b
来源：http://hz.shzxlz.cn/gtmuzhyjdn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gogol.net.cn/gtscbfjhtn.html

[C06] 匿名函数 / lambda
来源：http://hz.cdnleiting.top/gtlgkpufcd.html

Py:   square = lambda x: x * x
来源：http://hz.cashguo.top/gtwkztrbbo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangtech.top/gtnslmedaf.html

JS:   const square = x => x * x;
来源：http://hz.jiagoushi.top/gtdgrmzypl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.dianchejie.cn/gtcxqwojxw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhaomingkeji.xyz/gtoaafyawi.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jiagoushi.top/gtbbpxayin.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yueranfly.top/gttlmbkfjm.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtivkgaotg.html

[C07] 把函数作为参数传入
来源：http://hz.ybcxt.top/gtksezwtta.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jianghu66.top/gtzwmgqdpr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tanke756.top/gtlsrncgyo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daxiang520.top/gtfahaohqp.html

TS:   arr.map(String)
来源：http://hz.yj202588.top/gtbcroogjh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuxming.cn/gteraooijz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.nanxuanxn.top/gtgcolacrd.html

Ruby: arr.map(&:upcase)
来源：http://hz.fengsongda.top/gtzxctuzxm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.tanke756.top/gtejcisuey.html

[C08] 闭包
来源：http://hz.zhaomingkeji.xyz/gtbnzupest.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangdashe.top/gtvgtzirmg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ybcxt.top/gthgfyzadg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nanxuanxn.top/gtifpejczg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtnrdpgfgq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.haohaochexian.top/gthsfegemy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yanxiufei.cn/gtbxhbssem.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zdqjudy.top/gtgdjpvnnp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ybcxt.top/gtqrapqjyl.html

[C09] 递归
来源：http://hz.zdqjudy.top/gttuzhlkwr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.pycfn.com/gtxejzlhqm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.daxiang520.top/gtizkcpddy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydzc1.top/gtwzdohaxd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cheryme.top/gtjkcmcfld.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xuetiantiany.cn/gtnuruhewi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gzhubu.top/gtgulcbezk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtoswtywdt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangkeji.top/gtsekdbdup.html

[C10] 变量作用域
来源：http://hz.xuanzx.com/gtilaafbyp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.vqdsnc.cn/gtnncddgpj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinyuanbaomall.cn/gtvlpoeljt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.havefunace.top/gtjdlvikxi.html

TS:   同 JS
来源：http://hz.shanyushiyangkeji.top/gtomyqetat.html

Java: 方法内为块级作用域
来源：http://hz.svipenyu.cn/gtjenpeisi.html

Go:   花括号块级作用域
来源：http://hz.meibo888.top/gtoctaqdkh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj20258888.top/gtztxxyund.html

C#:   块级作用域
来源：http://hz.vqdsnc.cn/gtuevtsdwo.html

[C11] 模块导入与导出
来源：http://hz.ppjwa.cn/gttekqnlkl.html

Py:   from module import func
来源：http://hz.jianghu66.top/gtikdnhzel.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinghuilouyu.cn/gtuqiqclwn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.aizwys.cn/gtwxstloxj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.iojbl.cn/gthdlqvugm.html

Java: import java.util.List;
来源：http://hz.wangdashe.top/gtsvcswlbd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gaohongyu789.top/gtfklzlmrn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yvedp.cn/gtgwivfxeh.html

C#:   using System.Text;
来源：http://hz.cheryme.top/gtuftewkqh.html

[C12] 立即执行函数 IIFE
来源：http://hz.haohaochexian.top/gtudlilmir.html

Py:   (lambda: print("run"))()
来源：http://hz.ppjwa.cn/gtnbfjudep.html

PHP:  (function () { echo "run"; })();
来源：http://hz.bjfxy.top/gtzwajwuab.html

JS:   (() => { console.log("run"); })();
来源：http://hz.tianlin.xyz/gtuvvuqqyq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jqgufenzy.top/gtpeoqeery.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.0kj1m.cn/gteumysmbq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhongyouzk.top/gtbsmxvsff.html

Ruby: -> { puts "run" }.call
来源：http://hz.xylfe.cn/gtoryukmhd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj202588.top/gttdmxlejr.html

[C13] 类型声明 / 类型注解
来源：http://hz.gzhubu.top/gtevoosfka.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nanxinkj.top/gtssaiiuql.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtrsbnpxif.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhengqikj.top/gtzrbdolxj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.meibo888.top/gthsedvkto.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtrflltkkb.html

Go:   func add(a, b int) int
来源：http://hz.hysaishi.cn/gtrnayfrez.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.kuanghao11.cn/gtnqnpfsbq.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yuxming.cn/gtaozjtzcm.html

[C14] 泛型函数
来源：http://hz.iojbl.cn/gtmxqvwold.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.feifeiyinyue.top/gtufhepgyb.html

PHP:  // 无泛型
来源：http://hz.ivvv.top/gtofelkjjg.html

JS:   // 无泛型
来源：http://hz.hysaishi.cn/gtbinkspsc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.andypj.xyz/gtnumiltxx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhoulong.xyz/gtnswtxyge.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhengqikj.top/gtklgoxhdj.html

Ruby: # 无泛型
来源：http://hz.cqqwz.cn/gtstuaqfbk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinghuilouyu.cn/gtnaqugehh.html

[C15] 解构 / 展开参数
来源：http://hz.pengpengdd.cyou/gtfmemawot.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yuxming.cn/gtckaprqna.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aizwys.cn/gtqyvohfhd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ppjwa.cn/gtnjkzofvi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ehwqpu.com/gtpuwqkpjg.html

Java: // 无解构
来源：http://hz.cucudq.cn/gtkikzckfy.html

Go:   // 无解构
来源：http://hz.yueranfly.top/gtlxxhrulp.html

Ruby: a, b = pair
来源：http://hz.jiagoushi.top/gtobqzguhv.html

C#:   var (a, b) = pair;
来源：http://hz.sufxvd.cn/gtbyeqiygv.html

[C16] 函数 / 方法重载
来源：http://hz.tanke756.top/gtlxpiylzc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hfpthk.cn/gtwvtfcvdw.html

PHP:  // 无重载
来源：http://hz.jinyuanbaomall.cn/gtwfbgqmxj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.birdmap.top/gtrdoqpksy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jiagoushi.top/gtfccxqtnr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tian-w.cn/gthdjzwabh.html

Go:   // 无重载：用不同函数名
来源：http://hz.shanyushiyangkeji.top/gtniddsblo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ydzc1.top/gtiidiyiut.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gotoacloud.top/gtipkxctiz.html

================================================================================
来源：http://hz.meibo888.top/gtxluxbsjl.html

D. 数组 / 列表 / 集合
来源：http://hz.yuanzhike.top/gtzeykmxjp.html

================================================================================
来源：http://hz.dianchejie.cn/gtwlluajhs.html

[D01] 创建数组 / 列表
来源：http://hz.quarkkingdee.top/gtnqwvosxo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yuanzhike.top/gtwmvhnicn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sufxvd.cn/gtaxuvzzsp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.quarkkingdee.top/gtcalkjnoc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hammf.cn/gthllonqcq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yanxiufei.cn/gtuzsudbwu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cheryme.top/gtagygbhdc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yuxming.cn/gteqgwauef.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shzxlz.cn/gtvskmuubc.html

[D02] 追加元素到末尾
来源：http://hz.quarkkingdee.top/gtdsrlptoh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.wangdashe.top/gteoizdkcq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hnxiangtu.top/gtsrkymvcf.html

JS:   arr.push(4);
来源：http://hz.jqgfzy.top/gtvtwmrwyd.html

TS:   arr.push(4);
来源：http://hz.hnxiangtu.top/gtcyhdjlpy.html

Java: list.add(4);
来源：http://hz.ydjk.org.cn/gttrmzviki.html

Go:   arr = append(arr, 4)
来源：http://hz.gaohongyu789.top/gtrkrgdwwl.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.andypj.xyz/gtssmybrwt.html

C#:   list.Add(4);
来源：http://hz.jiagoushi.top/gttinidrnz.html

[D03] 在指定位置插入元素
来源：http://hz.quarkkingdee.top/gtpoacagda.html

Py:   arr.insert(0, 0)
来源：http://hz.hnxiangtu.top/gtwrxrlzcy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhixingplan.top/gtkmnrsyhg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shangyingyoupin.top/gtdpijrvtw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hywenlv.cn/gtzblawfza.html

Java: list.add(0, 0);
来源：http://hz.zhaomingkeji.xyz/gtawkrhamo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xingfuxueyuan.xyz/gtqaluewry.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yuanzhike.top/gthxktzlxw.html

C#:   list.Insert(0, 0);
来源：http://hz.wangshuangyany.cn/gtbmcdnlct.html

[D04] 删除元素
来源：http://hz.jiagoushi.top/gtlpeyakha.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shanyushiyangkeji.top/gtcqitwwfe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ybcxt.top/gtkfvkfmgl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cdnleiting.top/gtygazsrsg.html

TS:   arr.splice(0, 1);
来源：http://hz.zhiwuduotai.top/gtsutlrctm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gaohongyu789.top/gtstbdqwmy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hammf.cn/gtytnbfohd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shzxlz.cn/gtmvrwszxt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tanke756.top/gtuwzemrzc.html

[D05] 访问与修改元素
来源：http://hz.iojbl.cn/gtwtaiybij.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtbhckvodv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jiagoushi.top/gtjxazdivn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ehwqpu.com/gtrzqhnjql.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xuetiantiany.cn/gtqtprqcnk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.pengpengdd.cyou/gtlqbpolks.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gtbsuajkfq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtryweoijc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.c1oappe.top/gtszdlcfll.html

[D06] 数组长度
来源：http://hz.chenlongwang.top/gtqbnexzyh.html

Py:   len(arr)
来源：http://hz.jqgufenzy.top/gtizgmivsf.html

PHP:  count($arr);
来源：http://hz.aizwys.cn/gtzqtboqit.html

JS:   arr.length
来源：http://hz.jqgfzy.top/gtdkcxixot.html

TS:   arr.length
来源：http://hz.9152youxi.cn/gtftbmjyfj.html

Java: list.size();
来源：http://hz.wangdashe.top/gtwtrxotah.html

Go:   len(arr)
来源：http://hz.sufxvd.cn/gtjgpealai.html

Ruby: arr.length; arr.size
来源：http://hz.sysykeji.top/gteidwpbuz.html

C#:   list.Count;
来源：http://hz.zhixingplan.top/gtwpqtaowm.html

[D07] 切片 / 取子数组
来源：http://hz.pengpengdd.cyou/gttmjtulci.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.chenjidiqi.icu/gtjsvwbokf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gzhubu.top/gtbdmmfeep.html

JS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtflhbrvif.html

TS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtclbffsej.html

Java: list.subList(1, 4);
来源：http://hz.gotoacloud.top/gtjptirkcs.html

Go:   arr[1:4]
来源：http://hz.cucudq.cn/gtjmsxyhjp.html

Ruby: arr[1, 3]
来源：http://hz.cqqwz.cn/gtuynxosoo.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhaomingkeji.xyz/gtgkusyrtl.html

[D08] 合并两个数组
来源：http://hz.hnqzz.top/gtkmhhvmfb.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinqigufen.top/gtqzhtjtsl.html

PHP:  array_merge($a, $b);
来源：http://hz.52xcode.cn/gtqmtctzoh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.daria6918.cn/gtfsqmfqki.html

TS:   [...a, ...b];
来源：http://hz.havefunace.top/gtfnsynogf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ivvv.top/gtbpkopckw.html

Go:   append(a, b...)
来源：http://hz.fengsongda.top/gthbtjjhci.html

Ruby: a + b;  a.concat(b)
来源：http://hz.kuanghao11.cn/gtiqateomo.html

C#:   a.Concat(b).ToList()
来源：http://hz.xylfe.cn/gtcezghdbi.html

[D09] 排序（升序）
来源：http://hz.52xcode.cn/gtinodxaaz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gtfbklyfxb.html

PHP:  sort($arr);
来源：http://hz.daxiang520.top/gtiuydexzr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgfzy.top/gtmabdtibt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhongyouzk.top/gtgwktuxlo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yongpay.top/gttwvcepyl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gtjonkszma.html

Ruby: arr.sort
来源：http://hz.c1oappe.top/gtruhwjzew.html

C#:   list.Sort();
来源：http://hz.sweek.top/gtcontqmba.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cashguo.top/gtyyalmeyz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cashguo.top/gtevboncej.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gogol.net.cn/gtsiolbjgh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinghuilouyu.cn/gthcpyomhp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yvedp.cn/gtiirdduyf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hongshengwenyu.top/gtofpjdnau.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.pycfn.com/gtkzmzjajk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hongshengwenyu.top/gtzbhejqyy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.pycfn.com/gtukxqslhj.html

[D11] 反转数组
来源：http://hz.mhx1999.top/gtidpiqrzu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jianghu66.top/gtdogjmodi.html

PHP:  array_reverse($arr);
来源：http://hz.gotoacloud.top/gtzmkuhotu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hnqzz.top/gtnzwattif.html

TS:   [...arr].reverse();
来源：http://hz.hfpthk.cn/gtzwgfvvkf.html

Java: Collections.reverse(list);
来源：http://hz.yuanzhike.top/gtxddpcbui.html

Go:   slices.Reverse(arr)
来源：http://hz.pengpengdd.cyou/gthizsikbc.html

Ruby: arr.reverse
来源：http://hz.zhijiandao.cn/gtxfvtkaqs.html

C#:   list.Reverse();
来源：http://hz.svipenyu.cn/gtvyiqugjd.html

[D12] 查找元素下标
来源：http://hz.xingfuxueyuan.xyz/gtnbhcoput.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenlongwang.top/gtfdyzkxhe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hnxiangtu.top/gtxmceiuna.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenjidiqi.icu/gtuoimlwzw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangkeji.top/gtazqmqjfo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sufxvd.cn/gtknswyipj.html

Go:   slices.Index(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtnydqftnv.html

Ruby: arr.index(x)
来源：http://hz.tianlin.xyz/gtwbzxbndc.html

C#:   list.IndexOf(x);
来源：http://hz.bjfxy.top/gtvpqlaidp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangshuangyany.cn/gtdrbmyqlt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shzxlz.cn/gtvpqywgtv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cashguo.top/gtwnbuijzt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnxiangtu.top/gtdsjsfmyk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.c1oappe.top/gtrvcczgps.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gzhubu.top/gtbvsnfdhd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shanyushiyangkeji.top/gtenqutqew.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinghuilouyu.cn/gtltsvzpmt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.nanxinkj.top/gthxffmzdi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.mhx1999.top/gtkotrxesx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shzxlz.cn/gtghraunti.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.smart0.xyz/gtcsowfkkc.html

JS:   arr.map(x => x * 2)
来源：http://hz.daria6918.cn/gtocoezppp.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj202588.top/gttxoxqwfh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.fzhhl.top/gtpkzqyyxs.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtwywozgaw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.wangdashe.top/gtmbuwbmwc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shanyushiyangtech.top/gtjpzxtwuh.html

[D15] 去重
来源：http://hz.52xcode.cn/gtelpzbdmh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sysykeji.top/gtjszlgddd.html

PHP:  array_unique($arr);
来源：http://hz.pycfn.com/gtwmcmosnc.html

JS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtojvldoqk.html

TS:   [...new Set(arr)]
来源：http://hz.jinqigfzy.top/gtfllhkmnq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258888.top/gtqhnshjdb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zdqjudy.top/gtfjhgzano.html

Ruby: arr.uniq
来源：http://hz.jinqigufen.top/gtpgjixyhd.html

C#:   list.Distinct().ToList()
来源：http://hz.ivvv.top/gtpvsqhkzd.html

[D16] 求和与平均值
来源：http://hz.zhiwuduotai.top/gtmpnkdhdl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xinyue.icu/gtlaqqoukf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.316326.xyz/gtfosimfih.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtmgpmbbqd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fengsongda.top/gtixeimewk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.kuanghao11.cn/gtnbnulqlu.html

Go:   // 手写循环累加
来源：http://hz.jiagoushi.top/gtvxnatsny.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xinyue.icu/gtywqlyddj.html

C#:   list.Sum();  list.Average()
来源：http://hz.sysykeji.top/gtiutcskzh.html

[D17] 最大值与最小值
来源：http://hz.ydjk.org.cn/gtwqeawmlh.html

Py:   max(arr);  min(arr)
来源：http://hz.svipenyu.cn/gtutivqbue.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxinkj.top/gtziqymndp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.aibaodan.cn/gttogtvlfp.html

TS:   Math.max(...arr);
来源：http://hz.zhaomingkeji.xyz/gtxkxglfkc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gotoacloud.top/gtjgqvzwph.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hfpthk.cn/gtbzkvtinm.html

Ruby: arr.max;  arr.min
来源：http://hz.zhaomingkeji.xyz/gtodfgojeq.html

C#:   list.Max();  list.Min()
来源：http://hz.jlsjyb.cn/gtoahjtwoq.html

[D18] 扁平化嵌套数组
来源：http://hz.nwbrower.top/gtjmcerylc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aibaodan.cn/gtkegweyzi.html

PHP:  array_merge(...$nested);
来源：http://hz.xziqi.cn/gtebkkkpgg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sufxvd.cn/gtkzfxlixx.html

TS:   nested.flat();
来源：http://hz.316326.xyz/gtxtdlkqcj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.birdmap.top/gtgyntnqbw.html

Go:   // 手写双层循环
来源：http://hz.dianchejie.cn/gtbgxvxogi.html

Ruby: nested.flatten
来源：http://hz.xinyue.icu/gtayqqqwqv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.fzhhl.top/gtjrdpswiq.html

[D19] 按字段分组
来源：http://hz.wangshuangyany.cn/gtvdxxlkrz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yvedp.cn/gtdofbfnap.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zycfv.cn/gtumaawutk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.pengpengdd.cyou/gtlsmdmwlz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.havefunace.top/gtgpfijbcg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ydjk.org.cn/gtuquduslb.html

Go:   // 手写 map[string][]T
来源：http://hz.nwbrower.top/gtwwoqaytm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.birdmap.top/gtwgxooliv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhoulong.xyz/gtxcofybbn.html

[D20] 统计每个元素出现次数
来源：http://hz.shanyushiyangkeji.top/gtlzhjchgj.html

Py:   Counter(arr)
来源：http://hz.hfpthk.cn/gtbqznjjnh.html

PHP:  array_count_values($arr);
来源：http://hz.jianghu66.top/gtlmqryhir.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.c1oappe.top/gtqdwvgbwm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gtaxsbhkpc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hongshengwenyu.top/gtnxcqsarh.html

Go:   // 手写 map[T]int
来源：http://hz.xuanzx.com/gtjkiftikr.html

Ruby: arr.tally
来源：http://hz.cashguo.top/gttihfbrsn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.0kj1m.cn/gtqjpylvdq.html

[D21] 判断是否包含某元素
来源：http://hz.sweek.top/gtuyxigrxg.html

Py:   x in arr
来源：http://hz.shanyushiyangkeji.top/gtjdgpxwab.html

PHP:  in_array($x, $arr, true);
来源：http://hz.redwolf501.top/gtbtjspqlf.html

JS:   arr.includes(x)
来源：http://hz.gogol.net.cn/gttpyqawwf.html

TS:   arr.includes(x)
来源：http://hz.meibo888.top/gtnpwtuoyz.html

Java: list.contains(x)
来源：http://hz.shuidangran.top/gtegznjzhc.html

Go:   slices.Contains(arr, x)
来源：http://hz.shanyushiyangtech.top/gtaxdebiss.html

Ruby: arr.include?(x)
来源：http://hz.dianchejie.cn/gtjhojkzze.html

C#:   list.Contains(x)
来源：http://hz.dashuyun.cn/gtuwxnxpby.html

[D22] 复制数组（避免共享引用）
来源：http://hz.iojbl.cn/gtcactyfds.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhengqikj.top/gtcxifyacy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhaomingkeji.xyz/gtxcorqoyh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.c1oappe.top/gtqymgiuze.html

TS:   [...arr];
来源：http://hz.shanyushiyangtech.top/gtnibivyyy.html


<!-- 参考信息 -->