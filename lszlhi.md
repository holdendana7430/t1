代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://hz.jianghu66.top/gtpiaeypta.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yvedp.cn/gtipxzajan.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shzxlz.cn/gtugkkxsqc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yvedp.cn/gtysjyubdv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xziqi.cn/gtvduejgkw.html

[C07] 把函数作为参数传入
来源：http://hz.fzhhl.top/gtuhourypk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cdnleiting.top/gtczchvtnf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenlongwang.top/gtolqtyuhg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.andypj.xyz/gtjdnwnwvx.html

TS:   arr.map(String)
来源：http://hz.aibaodan.cn/gtnoiraqdy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yj20258888.top/gtmufmnsix.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.andypj.xyz/gttyqaldyc.html

Ruby: arr.map(&:upcase)
来源：http://hz.birdmap.top/gtjwnzxfoh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhengqikj.top/gtyinyiiqd.html

[C08] 闭包
来源：http://hz.yueranfly.top/gtvzwtbnmd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ybcxt.top/gtjfiodfjj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yongpay.top/gtmrfvmbvq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtuepubuui.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.havefunace.top/gtepqwlmyj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.0kj1m.cn/gtzivcnmfv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cqqwz.cn/gttmkinoqm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xziqi.cn/gthoihaftv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gtgnlbsjdo.html

[C09] 递归
来源：http://hz.aizwys.cn/gtvmuqmmak.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sysykeji.top/gtgjpahlbx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hnqzz.top/gtltrmmykp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hammf.cn/gtcxhlygrg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtyzwkzqsx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.smart0.xyz/gtyrsqswqh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.svipenyu.cn/gtxzekwstj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shanyushiyangkeji.top/gtfubzaauh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.aizwys.cn/gtepltwiur.html

[C10] 变量作用域
来源：http://hz.gaohongyu789.top/gtmqmiokvq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sufxvd.cn/gthbgdmsbk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gotoacloud.top/gtbkyyruze.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gaohongyu789.top/gtdqmeiqfm.html

TS:   同 JS
来源：http://hz.yj20258888.top/gtwkoiypsl.html

Java: 方法内为块级作用域
来源：http://hz.tian-w.cn/gtopkpcggr.html

Go:   花括号块级作用域
来源：http://hz.fzhhl.top/gtuqegwmrr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ydjk.org.cn/gtnceobfbo.html

C#:   块级作用域
来源：http://hz.jinghuilouyu.cn/gtoypjfenv.html

[C11] 模块导入与导出
来源：http://hz.daria6918.cn/gtngdslptt.html

Py:   from module import func
来源：http://hz.jqgfzy.top/gtyeakpqgy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jqgufenzy.top/gtbpzbozfj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.52xcode.cn/gtkvbjlgtn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gotoacloud.top/gtbafbzghx.html

Java: import java.util.List;
来源：http://hz.yanxiufei.cn/gthhiokrvd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cucudq.cn/gtnrcsgmpd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.meibo888.top/gtyqgjnomo.html

C#:   using System.Text;
来源：http://hz.daria6918.cn/gtwoysxvkx.html

[C12] 立即执行函数 IIFE
来源：http://hz.aibaodan.cn/gthiwemkeo.html

Py:   (lambda: print("run"))()
来源：http://hz.fzhhl.top/gtmgyssxxm.html

PHP:  (function () { echo "run"; })();
来源：http://hz.dianchejie.cn/gtekghzvaq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuanzx.com/gtfftkszvg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.kuanghao11.cn/gthxmrwpql.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.0kj1m.cn/gtgmydejga.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cdnleiting.top/gteuayxebq.html

Ruby: -> { puts "run" }.call
来源：http://hz.sxryk.cn/gtsxdakdlp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.c1oappe.top/gtmwfgzriw.html

[C13] 类型声明 / 类型注解
来源：http://hz.sysykeji.top/gtxedopkco.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xziqi.cn/gtzscsotfl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtuurwttvq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhaomingkeji.xyz/gthmgiapqw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pengpengdd.cyou/gtkejzxxcq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtmavfwccb.html

Go:   func add(a, b int) int
来源：http://hz.jianghu66.top/gtdocdoabs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shanyushiyangtech.top/gtvkaysksl.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shanyushiyangkeji.top/gtqmzddjec.html

[C14] 泛型函数
来源：http://hz.hnxiangtu.top/gtpxwamiqm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.aibaodan.cn/gteiamtbbz.html

PHP:  // 无泛型
来源：http://hz.pycfn.com/gtylzhcisi.html

JS:   // 无泛型
来源：http://hz.shangyingyoupin.top/gtiqaspktr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.daria6918.cn/gtrnxccocz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinghuilouyu.cn/gthycajmmh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ivvv.top/gtxgtasyon.html

Ruby: # 无泛型
来源：http://hz.guowangkeji.top/gtulmvqzgq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ehwqpu.com/gtjkzqctig.html

[C15] 解构 / 展开参数
来源：http://hz.shanyushiyangkeji.top/gtjxcepnrp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fzhhl.top/gtifpmjaue.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shanyushiyangkeji.top/gtlicnudxb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtgcofpgpq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gaohongyu789.top/gteqyygtlf.html

Java: // 无解构
来源：http://hz.nwbrower.top/gtwhrqbimr.html

Go:   // 无解构
来源：http://hz.guannengcc.top/gtfswtmsco.html

Ruby: a, b = pair
来源：http://hz.quarkkingdee.top/gtcpbxmdag.html

C#:   var (a, b) = pair;
来源：http://hz.snrcjt.cn/gtrhfhbyvu.html

[C16] 函数 / 方法重载
来源：http://hz.316326.xyz/gtdqksukzh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dianchejie.cn/gtmxyyjljd.html

PHP:  // 无重载
来源：http://hz.ivvv.top/gtkxaxjtjm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hfpthk.cn/gtzmdxttvr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuanzhike.top/gtdavdbwzm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gaohongyu789.top/gtwnjntepv.html

Go:   // 无重载：用不同函数名
来源：http://hz.yueranfly.top/gtwhbvblak.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ybcxt.top/gtddonuteg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yj20258.top/gtaagneimk.html

================================================================================
来源：http://hz.yongpay.top/gtuzgyhocj.html

D. 数组 / 列表 / 集合
来源：http://hz.xingfuxueyuan.xyz/gtsrvarsnb.html

================================================================================
来源：http://hz.daxiang520.top/gthfhotmhe.html

[D01] 创建数组 / 列表
来源：http://hz.ehwqpu.com/gtoiqfjpsl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhiwuduotai.top/gtvywzfjye.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ehwqpu.com/gtslycggeh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hywenlv.cn/gtbasjjhlx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guannengcc.top/gtsprylrdd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.wangdashe.top/gtbtlsltwa.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenlongwang.top/gtwokfteeh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.c1oappe.top/gtcznlvuzm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cucudq.cn/gtrdlcednf.html

[D02] 追加元素到末尾
来源：http://hz.yonumen.top/gtlpfotbsm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.haohaochexian.top/gtewjdzpvp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cashguo.top/gtixcpsrqt.html

JS:   arr.push(4);
来源：http://hz.dianchejie.cn/gtsmflqzlm.html

TS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtxnpnkimj.html

Java: list.add(4);
来源：http://hz.redwolf501.top/gtfsltmbgb.html

Go:   arr = append(arr, 4)
来源：http://hz.xuanzx.com/gtztvapipv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.snrcjt.cn/gtxjxfxhwa.html

C#:   list.Add(4);
来源：http://hz.iojbl.cn/gtbfwktryk.html

[D03] 在指定位置插入元素
来源：http://hz.52xcode.cn/gtyudavoqz.html

Py:   arr.insert(0, 0)
来源：http://hz.xziqi.cn/gtfkkclnqg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guannengcc.top/gttpxwkcep.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xinyue.icu/gtwieeofqm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.0kj1m.cn/gtmjnnlnac.html

Java: list.add(0, 0);
来源：http://hz.yj20258888.top/gtnjnwjnnq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xziqi.cn/gtqclfmjkv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ybcxt.top/gtibfsjdqm.html

C#:   list.Insert(0, 0);
来源：http://hz.cashguo.top/gtdlvemdey.html

[D04] 删除元素
来源：http://hz.chenjidiqi.icu/gtrgndsdzg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sysykeji.top/gthmunrnhx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenzaomai.com/gteynffbpc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hysaishi.cn/gtiheqhacs.html

TS:   arr.splice(0, 1);
来源：http://hz.yangfankeji.com/gtowaemihl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxuanxn.top/gtyowfosjh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.vqdsnc.cn/gtfyknxwzu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xziqi.cn/gtfppwzkjy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yangfankeji.com/gtjpzjueja.html

[D05] 访问与修改元素
来源：http://hz.zhijiandao.cn/gtyoxunmiw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtzsicaoxf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hnqzz.top/gtycpyjgax.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtgebguwyi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jianghu66.top/gttmugdauz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cheryme.top/gtqjfontax.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtaeaylabh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gtqovxwbun.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hysaishi.cn/gtjpkrthcy.html

[D06] 数组长度
来源：http://hz.yvedp.cn/gtvrysnzhz.html

Py:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtbgguquvu.html

PHP:  count($arr);
来源：http://hz.aizwys.cn/gtneqqvfdf.html

JS:   arr.length
来源：http://hz.yangfankeji.com/gtrwedgcgm.html

TS:   arr.length
来源：http://hz.snrcjt.cn/gtbyjrnouz.html

Java: list.size();
来源：http://hz.zhaomingkeji.xyz/gtiicksvzn.html

Go:   len(arr)
来源：http://hz.xuanzx.com/gtwhpcpiiq.html

Ruby: arr.length; arr.size
来源：http://hz.zhiwuduotai.top/gtndawuhsu.html

C#:   list.Count;
来源：http://hz.hammf.cn/gtkcshbjon.html

[D07] 切片 / 取子数组
来源：http://hz.cashguo.top/gtekqwnkfe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.redwolf501.top/gtqkydsccj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ehwqpu.com/gtisqmvkwy.html

JS:   arr.slice(1, 4);
来源：http://hz.tian-w.cn/gtzxpgftvs.html

TS:   arr.slice(1, 4);
来源：http://hz.52xcode.cn/gtperdulks.html

Java: list.subList(1, 4);
来源：http://hz.svipenyu.cn/gtzkldmgey.html

Go:   arr[1:4]
来源：http://hz.ppjwa.cn/gteenflxgc.html

Ruby: arr[1, 3]
来源：http://hz.iojbl.cn/gtsqnbbbef.html

C#:   list.GetRange(1, 3);
来源：http://hz.guannengcc.top/gtpnczzjim.html

[D08] 合并两个数组
来源：http://hz.snrcjt.cn/gtzkjehzlm.html

Py:   a + b;  a.extend(b)
来源：http://hz.yvedp.cn/gtvwqqiiuw.html

PHP:  array_merge($a, $b);
来源：http://hz.zhaomingkeji.xyz/gtrczyljhk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj202588.top/gtnmzcesjg.html

TS:   [...a, ...b];
来源：http://hz.fzhhl.top/gtlgzovlct.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jyoumei.cn/gtjsrbgszh.html

Go:   append(a, b...)
来源：http://hz.xziqi.cn/gtehokpaeq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.meibo888.top/gtwjcxjdyp.html

C#:   a.Concat(b).ToList()
来源：http://hz.feifeiyinyue.top/gtwrmdowfg.html

[D09] 排序（升序）
来源：http://hz.guowangkeji.top/gtranhcrql.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ivvv.top/gtweifnxuk.html

PHP:  sort($arr);
来源：http://hz.vqdsnc.cn/gtvmgqhden.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.wangdashe.top/gtswukdcoe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.svipenyu.cn/gtoumfeiex.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhaomingkeji.xyz/gtotlwlfzu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtrrbsqdmp.html

Ruby: arr.sort
来源：http://hz.xuanzx.com/gthpfrpznt.html

C#:   list.Sort();
来源：http://hz.c1oappe.top/gtlfifhgks.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.mhx1999.top/gtgdtfxdgg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yangfankeji.com/gtgblbdshg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cqqwz.cn/gtvlwycici.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nwbrower.top/gtvlenewwy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gtqstzhtsd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yanxiufei.cn/gtnldaqzsp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tian-w.cn/gtlyxuftmd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.wangshuangyany.cn/gtqgzrchxc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cdnleiting.top/gtgrykjmoi.html

[D11] 反转数组
来源：http://hz.wangdashe.top/gtegtmwxea.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.feifeiyinyue.top/gtasiifsbi.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258888.top/gtjqixxadv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ivvv.top/gtvptpjgcn.html

TS:   [...arr].reverse();
来源：http://hz.yj202588.top/gtlgvfgyyl.html

Java: Collections.reverse(list);
来源：http://hz.tanke756.top/gtovkwnjwr.html

Go:   slices.Reverse(arr)
来源：http://hz.cucudq.cn/gtomegzlhf.html

Ruby: arr.reverse
来源：http://hz.nanxinkj.top/gtlhynbwjn.html

C#:   list.Reverse();
来源：http://hz.yvedp.cn/gtmsgsaapm.html

[D12] 查找元素下标
来源：http://hz.zdqjudy.top/gtawrdwutb.html

Py:   arr.index(x);  x in arr
来源：http://hz.guannengcc.top/gtgrtlmlan.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nwbrower.top/gtwolmrwio.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pengpengdd.cyou/gtxfpnlzkm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtwurwxhlr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.dashuyun.cn/gtomnqjcuw.html

Go:   slices.Index(arr, x)
来源：http://hz.redwolf501.top/gtwpdmsksy.html

Ruby: arr.index(x)
来源：http://hz.cucudq.cn/gtvvggbtft.html

C#:   list.IndexOf(x);
来源：http://hz.yvedp.cn/gtxneazbgk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhongyouzk.top/gtiaqkdetj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhaomingkeji.xyz/gtmbrscdox.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.52xcode.cn/gtkpotqnaw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtsjsmlptd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sysykeji.top/gtixwovaby.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shangyingyoupin.top/gtmkvgrnvq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinqigfzy.top/gtlcbsrckp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gotoacloud.top/gtsinjkcih.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.aizwys.cn/gtyhfcupjr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.0kj1m.cn/gtmyshhjpy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shuidangran.top/gtdhugqvzs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj20258.top/gtwoejygbc.html

JS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtrnietzev.html

TS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtuomkkqty.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shzxlz.cn/gtljznkibs.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtljccbgkc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.snrcjt.cn/gtmzdcpgkt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yvedp.cn/gtcyatysed.html

[D15] 去重
来源：http://hz.shangyingyoupin.top/gthcywqgrk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.quarkkingdee.top/gtqymnietm.html

PHP:  array_unique($arr);
来源：http://hz.jlsjyb.cn/gthxzbtzer.html

JS:   [...new Set(arr)]
来源：http://hz.hammf.cn/gtosrnqtck.html

TS:   [...new Set(arr)]
来源：http://hz.tanke756.top/gtfwvlntng.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zycfv.cn/gtjvangdlq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yanxiufei.cn/gtpesqkidf.html

Ruby: arr.uniq
来源：http://hz.wangshuangyany.cn/gtewmjluec.html

C#:   list.Distinct().ToList()
来源：http://hz.ydjk.org.cn/gtlfkyiuuk.html

[D16] 求和与平均值
来源：http://hz.c1oappe.top/gtjmrqoapb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.birdmap.top/gtudqvbjag.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj20258888.top/gtekqygsgf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtpfcztvsv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sxryk.cn/gtrrzfcsts.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cucudq.cn/gtvsatumre.html

Go:   // 手写循环累加
来源：http://hz.guannengcc.top/gtylnboecp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ivvv.top/gtsegslizy.html

C#:   list.Sum();  list.Average()
来源：http://hz.iojbl.cn/gtfoqzyyzj.html

[D17] 最大值与最小值
来源：http://hz.hongshengwenyu.top/gtqwwwmcez.html

Py:   max(arr);  min(arr)
来源：http://hz.kuanghao11.cn/gtdppygxhw.html

PHP:  max($arr);  min($arr);
来源：http://hz.snrcjt.cn/gtchmzwldr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenzaomai.com/gtdskcojyt.html

TS:   Math.max(...arr);
来源：http://hz.yvedp.cn/gtkmgyyxgl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj202588.top/gteoqcsept.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.vqdsnc.cn/gtizyiiito.html

Ruby: arr.max;  arr.min
来源：http://hz.birdmap.top/gtumfjefzo.html

C#:   list.Max();  list.Min()
来源：http://hz.chenjidiqi.icu/gtstgokhaq.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgfzy.top/gtigjelibq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.andypj.xyz/gtelmuncjz.html

PHP:  array_merge(...$nested);
来源：http://hz.gaohongyu789.top/gtavogcjcl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jiagoushi.top/gtvhpsulxk.html

TS:   nested.flat();
来源：http://hz.hammf.cn/gtbtgvlvyd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xuanzx.com/gtxifrtgsg.html

Go:   // 手写双层循环
来源：http://hz.gogol.net.cn/gtackedfii.html

Ruby: nested.flatten
来源：http://hz.quarkkingdee.top/gtllcbubgp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hnqzz.top/gtuocfznad.html

[D19] 按字段分组
来源：http://hz.bjfxy.top/gtptyxphmp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gaohongyu789.top/gticdfxduy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhengqikj.top/gtuturnzud.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ehwqpu.com/gthssjvqfb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jyoumei.cn/gtjjiykmvc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cheryme.top/gtfivgtkvh.html

Go:   // 手写 map[string][]T
来源：http://hz.vqdsnc.cn/gtejheczvk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.vqdsnc.cn/gtzpgztgtg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.daxiang520.top/gtixqmilow.html

[D20] 统计每个元素出现次数
来源：http://hz.kuanghao11.cn/gttetmixhv.html

Py:   Counter(arr)
来源：http://hz.jianghu66.top/gtytcloymt.html

PHP:  array_count_values($arr);
来源：http://hz.xinyue.icu/gtejcwmrap.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenlongwang.top/gtiobdiwfm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhongyouzk.top/gtdfuckiae.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.aizwys.cn/gtfwkqwzyo.html

Go:   // 手写 map[T]int
来源：http://hz.daria6918.cn/gtgxifzxxk.html

Ruby: arr.tally
来源：http://hz.dianchejie.cn/gtvoiqvzvh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.havefunace.top/gttcerwwps.html

[D21] 判断是否包含某元素
来源：http://hz.316326.xyz/gtirqzjmnf.html

Py:   x in arr
来源：http://hz.cqqwz.cn/gtkhlzmmfm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuanzhike.top/gtvjkemfhe.html

JS:   arr.includes(x)
来源：http://hz.guowangkeji.top/gtxflgxrfy.html

TS:   arr.includes(x)
来源：http://hz.daria6918.cn/gtggknptxc.html

Java: list.contains(x)
来源：http://hz.gotoacloud.top/gtjvsxxonz.html

Go:   slices.Contains(arr, x)
来源：http://hz.daxiang520.top/gtsnlipovb.html

Ruby: arr.include?(x)
来源：http://hz.tian-w.cn/gtpeykpbqn.html

C#:   list.Contains(x)
来源：http://hz.sysykeji.top/gtfyfemnmt.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangshuangyany.cn/gtrjyinxwe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.smart0.xyz/gtdxpkccoo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhixingplan.top/gtbtgngydo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.quarkkingdee.top/gtmugtrrxv.html

TS:   [...arr];
来源：http://hz.zhijiandao.cn/gtegknjcoa.html

Java: new ArrayList<>(list);
来源：http://hz.andypj.xyz/gtnwqqvizt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.haohaochexian.top/gtcnvchfnm.html

Ruby: arr.dup;  arr.clone
来源：http://hz.tianlin.xyz/gtgkywcxxj.html

C#:   new List<int>(list);
来源：http://hz.tanke756.top/gtoqfytria.html

[D23] reduce 累积计算
来源：http://hz.zycfv.cn/gtdugchyqe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinghuilouyu.cn/gtwomemikn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shanyushiyangkeji.top/gtdhqsdvuz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.andypj.xyz/gtyofswitq.html


<!-- 参考信息 -->