代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://hz.xuetiantiany.cn/gtbgcsjjoi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yanxiufei.cn/gtjsdetnei.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.vqdsnc.cn/gtgpgjudpd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.quarkkingdee.top/gtfrpxuzac.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.vqdsnc.cn/gtmvsoqzgu.html

[C07] 把函数作为参数传入
来源：http://hz.chenlongwang.top/gtiepvhmsb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.52xcode.cn/gttwbptzuy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.fzhhl.top/gtyaezqxzw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.52xcode.cn/gtowyrcwel.html

TS:   arr.map(String)
来源：http://hz.jianghu66.top/gtdhiiqgul.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cheryme.top/gtsglenapj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258.top/gtdzozuori.html

Ruby: arr.map(&:upcase)
来源：http://hz.yonumen.top/gtzesimxmd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.daxiang520.top/gtpzizktlo.html

[C08] 闭包
来源：http://hz.yonumen.top/gtgnepaoge.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nanxuanxn.top/gtnfinjaex.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangkeji.top/gtdaxfuabk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gtvuvxelnh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtutmjfpnp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jqgfzy.top/gtqiiboahk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tianlin.xyz/gtwjcggtyr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sxryk.cn/gtetuuxomb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.daria6918.cn/gtavpfuiey.html

[C09] 递归
来源：http://hz.shanyushiyangkeji.top/gtujtqixga.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xinyue.icu/gtqvayzzeo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenlongwang.top/gtybmnyivt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yangfankeji.com/gtzdgxvjdm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gtjfvbplbn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yongpay.top/gtvazotxtu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.fzhhl.top/gtaaggnkim.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj202588.top/gtizqgckjd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daxiang520.top/gtteyvzlgy.html

[C10] 变量作用域
来源：http://hz.zhixingplan.top/gtdoofwmhb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hongshengwenyu.top/gtlypioykc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yj202588.top/gtvwwgxkdy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ehwqpu.com/gtgbcaxirf.html

TS:   同 JS
来源：http://hz.sweek.top/gtgxayeikj.html

Java: 方法内为块级作用域
来源：http://hz.nwbrower.top/gtveuztkhy.html

Go:   花括号块级作用域
来源：http://hz.tianlin.xyz/gtkqlzgkrs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.shuidangran.top/gtitezufhe.html

C#:   块级作用域
来源：http://hz.zhijiandao.cn/gtvxuzpyhu.html

[C11] 模块导入与导出
来源：http://hz.hnqzz.top/gtcufyozqa.html

Py:   from module import func
来源：http://hz.aizwys.cn/gtvcjsurae.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sweek.top/gtzmrrmkri.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.smart0.xyz/gtqhqqezex.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.52xcode.cn/gtphcdswbu.html

Java: import java.util.List;
来源：http://hz.xinyue.icu/gtommvewbw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.wangdashe.top/gtvzfkviut.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fzhhl.top/gtdftninyv.html

C#:   using System.Text;
来源：http://hz.birdmap.top/gtekjcskir.html

[C12] 立即执行函数 IIFE
来源：http://hz.cucudq.cn/gtwplzawbv.html

Py:   (lambda: print("run"))()
来源：http://hz.tian-w.cn/gtnjzxkfbp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj202588.top/gtpaqgpkkx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yongpay.top/gtuiekzkvq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.andypj.xyz/gtjfmwynwg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.redwolf501.top/gtotufaeih.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yonumen.top/gtyblaanxv.html

Ruby: -> { puts "run" }.call
来源：http://hz.xuetiantiany.cn/gtkisrcpgy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuxming.cn/gtkarilnkf.html

[C13] 类型声明 / 类型注解
来源：http://hz.hnqzz.top/gtucgpjuej.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.daria6918.cn/gtpulrodvo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ppjwa.cn/gtxwpdhkqs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xylfe.cn/gtidyferoc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.bjfxy.top/gtksqfixga.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtncztpnbo.html

Go:   func add(a, b int) int
来源：http://hz.ydjk.org.cn/gtzqnsqifl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jlsjyb.cn/gtthtokbge.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yongpay.top/gtnjwztdlb.html

[C14] 泛型函数
来源：http://hz.shuidangran.top/gteyggzfll.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ydzc1.top/gtbliyonbr.html

PHP:  // 无泛型
来源：http://hz.zhengqikj.top/gtmoepyjkq.html

JS:   // 无泛型
来源：http://hz.yongpay.top/gtupakljwz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xinyue.icu/gtxvgncbvw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yvedp.cn/gtpnwqgids.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xylfe.cn/gtactutghr.html

Ruby: # 无泛型
来源：http://hz.yonumen.top/gtdxsmyhit.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hysaishi.cn/gthjnxwxqc.html

[C15] 解构 / 展开参数
来源：http://hz.xinyue.icu/gtkdlxqnua.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.feifeiyinyue.top/gtmprtrsrk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hnxiangtu.top/gtmfmxpobr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jqgufenzy.top/gtzwdwyfzf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gotoacloud.top/gtvnrzedxj.html

Java: // 无解构
来源：http://hz.xziqi.cn/gtkjijcsbr.html

Go:   // 无解构
来源：http://hz.chenjidiqi.icu/gtlaqcfiir.html

Ruby: a, b = pair
来源：http://hz.hongshengwenyu.top/gtfelhhytx.html

C#:   var (a, b) = pair;
来源：http://hz.ydzc1.top/gtuklyxrti.html

[C16] 函数 / 方法重载
来源：http://hz.zycfv.cn/gtnyrorphz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhixingplan.top/gtuqtbxyej.html

PHP:  // 无重载
来源：http://hz.pycfn.com/gtyhbxbxgb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.kuanghao11.cn/gtqydjyaqb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jqgufenzy.top/gtowdxlihq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.316326.xyz/gtxfdnkzre.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtumuxvddq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cdnleiting.top/gtfrutebqe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yvedp.cn/gtkszzflbb.html

================================================================================
来源：http://hz.dashuyun.cn/gtacjmismp.html

D. 数组 / 列表 / 集合
来源：http://hz.zhengqikj.top/gtopmujozi.html

================================================================================
来源：http://hz.yj202588.top/gtnxrztbol.html

[D01] 创建数组 / 列表
来源：http://hz.aibaodan.cn/gtoidrrcpr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.quarkkingdee.top/gtsnpmkjsl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nanxinkj.top/gteerssiqm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.pengpengdd.cyou/gtlzvtyzbv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhiwuduotai.top/gtpsrilhjj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.guowangkeji.top/gtsbmegmtn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gotoacloud.top/gtobghpoqa.html

Ruby: arr = [1, 2, 3]
来源：http://hz.316326.xyz/gttkgyvlrj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aibaodan.cn/gtwsazzucp.html

[D02] 追加元素到末尾
来源：http://hz.zhixingplan.top/gtkxuszgyr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ivvv.top/gtxrqfomzz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuanzx.com/gtuzlvrwer.html

JS:   arr.push(4);
来源：http://hz.tian-w.cn/gtkodaqlnd.html

TS:   arr.push(4);
来源：http://hz.quarkkingdee.top/gtfxxcorwt.html

Java: list.add(4);
来源：http://hz.gogol.net.cn/gtbekcpkuv.html

Go:   arr = append(arr, 4)
来源：http://hz.xingfuxueyuan.xyz/gtvoctmsha.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuetiantiany.cn/gtzglatvvq.html

C#:   list.Add(4);
来源：http://hz.kuanghao11.cn/gtrattryhn.html

[D03] 在指定位置插入元素
来源：http://hz.jiagoushi.top/gtwbgunhzc.html

Py:   arr.insert(0, 0)
来源：http://hz.smart0.xyz/gtqnxepoag.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinghuilouyu.cn/gtaoadejyu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nanxinkj.top/gtbnvkkddl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.wangshuangyany.cn/gtssjyzpyc.html

Java: list.add(0, 0);
来源：http://hz.zhixingplan.top/gtytnwsowa.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gzhubu.top/gtxrbwtncf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hongshengwenyu.top/gtofduxysm.html

C#:   list.Insert(0, 0);
来源：http://hz.sxryk.cn/gtcastfpnd.html

[D04] 删除元素
来源：http://hz.mhx1999.top/gtnqngikxc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.c1oappe.top/gtvualigng.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.meibo888.top/gtvtsjqmyk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.xylfe.cn/gtprlfabgx.html

TS:   arr.splice(0, 1);
来源：http://hz.xylfe.cn/gtfvbpciij.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yanxiufei.cn/gtzetptxrf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hnxiangtu.top/gtqusswuhc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxinkj.top/gtykiohigv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.feifeiyinyue.top/gtxvxvgjdp.html

[D05] 访问与修改元素
来源：http://hz.aizwys.cn/gtcjvghfnb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtchjhllnv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.c1oappe.top/gtnqqjmvuu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj20258.top/gthsilhqdk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenlongwang.top/gtfnzckatq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yonumen.top/gtfmueiaqh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtvssnofuv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tian-w.cn/gtcqqxhhst.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ivvv.top/gtuhyubpqo.html

[D06] 数组长度
来源：http://hz.316326.xyz/gtykuetmdr.html

Py:   len(arr)
来源：http://hz.svipenyu.cn/gtmuguftig.html

PHP:  count($arr);
来源：http://hz.jinghuilouyu.cn/gtuaoltkkz.html

JS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtpuinuqwv.html

TS:   arr.length
来源：http://hz.jqgufenzy.top/gtzzauvakp.html

Java: list.size();
来源：http://hz.aibaodan.cn/gtuuacqjli.html

Go:   len(arr)
来源：http://hz.jinqigfzy.top/gtmvkdejki.html

Ruby: arr.length; arr.size
来源：http://hz.fengsongda.top/gtwfyvscxb.html

C#:   list.Count;
来源：http://hz.jqgufenzy.top/gtkzicugpw.html

[D07] 切片 / 取子数组
来源：http://hz.xinyue.icu/gtqygyyode.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xziqi.cn/gtamwaqvaf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yangfankeji.com/gtqwffioyc.html

JS:   arr.slice(1, 4);
来源：http://hz.aibaodan.cn/gtjbeoikzj.html

TS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gtjkytdwtq.html

Java: list.subList(1, 4);
来源：http://hz.jqgfzy.top/gtgwpcmfwl.html

Go:   arr[1:4]
来源：http://hz.hywenlv.cn/gterlhkjbf.html

Ruby: arr[1, 3]
来源：http://hz.zycfv.cn/gtwkdmkcnt.html

C#:   list.GetRange(1, 3);
来源：http://hz.sysykeji.top/gtvwswruhv.html

[D08] 合并两个数组
来源：http://hz.pycfn.com/gthqurxdrt.html

Py:   a + b;  a.extend(b)
来源：http://hz.xuetiantiany.cn/gtclmsmkyb.html

PHP:  array_merge($a, $b);
来源：http://hz.tanke756.top/gtmyojleea.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hfpthk.cn/gtlvjizuyc.html

TS:   [...a, ...b];
来源：http://hz.yvedp.cn/gttoguhkhx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hysaishi.cn/gtxonqvbfw.html

Go:   append(a, b...)
来源：http://hz.yueranfly.top/gtqpshvyuh.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenjidiqi.icu/gtmmzdoybu.html

C#:   a.Concat(b).ToList()
来源：http://hz.tianlin.xyz/gtcsxcmolp.html

[D09] 排序（升序）
来源：http://hz.jinghuilouyu.cn/gtxxyerpwk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtpknvfwuu.html

PHP:  sort($arr);
来源：http://hz.316326.xyz/gtsibxegnk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cqqwz.cn/gtnsotzdwt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinqigufen.top/gtpmntiyvm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nwbrower.top/gtybnqunol.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.dianchejie.cn/gtzrijnfev.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtubrqulef.html

C#:   list.Sort();
来源：http://hz.chenlongwang.top/gtvfdhnojz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.tian-w.cn/gtdsfnxxqi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydzc1.top/gtjsjaxpbq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ywan-chungtsiang.top/gtzavuztda.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.0kj1m.cn/gtgshbhvhh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.snrcjt.cn/gtugymnjzt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.52xcode.cn/gtofdptadg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yvedp.cn/gtyfkrnebp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenzaomai.com/gtrwypakzg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.meibo888.top/gtbmgxrnqf.html

[D11] 反转数组
来源：http://hz.ppjwa.cn/gtsvypqesn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhaomingkeji.xyz/gtxsisltdx.html

PHP:  array_reverse($arr);
来源：http://hz.dashuyun.cn/gthjddctto.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guowangkeji.top/gtuhdyxdid.html

TS:   [...arr].reverse();
来源：http://hz.mhx1999.top/gtgsjarprs.html

Java: Collections.reverse(list);
来源：http://hz.sxryk.cn/gtbwsqlkzb.html

Go:   slices.Reverse(arr)
来源：http://hz.xuetiantiany.cn/gttihoatbv.html

Ruby: arr.reverse
来源：http://hz.vqdsnc.cn/gtwqpgvvfm.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gtylyazaqv.html

[D12] 查找元素下标
来源：http://hz.snrcjt.cn/gtazwuzwln.html

Py:   arr.index(x);  x in arr
来源：http://hz.pycfn.com/gtyuqjkwdn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgufenzy.top/gtelvascqd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gtojzzcvfv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tanke756.top/gtfujyclua.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jiagoushi.top/gtvjycnylg.html

Go:   slices.Index(arr, x)
来源：http://hz.cheryme.top/gtoknwdquk.html

Ruby: arr.index(x)
来源：http://hz.yj20258888.top/gtqukchsnq.html

C#:   list.IndexOf(x);
来源：http://hz.yj20258888.top/gtfijjezjk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zycfv.cn/gtpxmyqlhd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnqzz.top/gtzjlweqbw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ybcxt.top/gtzlnwabuy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shuidangran.top/gtbrdxxjex.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sxryk.cn/gtvztjhbis.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hfpthk.cn/gtpeqqukif.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhengqikj.top/gtokltyeei.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ybcxt.top/gtteoonmya.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ydjk.org.cn/gtapdkbmzk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhiwuduotai.top/gtbdmwyqau.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhixingplan.top/gtddpnctxc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenzaomai.com/gthtezqdml.html

JS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gtbnnedjrj.html

TS:   arr.map(x => x * 2)
来源：http://hz.hnxiangtu.top/gtroqrdceu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.0kj1m.cn/gtujnuunms.html

Go:   // 手写循环
来源：http://hz.zhaomingkeji.xyz/gtvwptayqk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shanyushiyangkeji.top/gtdbexbcrc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgufenzy.top/gtxoxzzsaz.html

[D15] 去重
来源：http://hz.hywenlv.cn/gtjreltmjh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtfkzpzbzc.html

PHP:  array_unique($arr);
来源：http://hz.9152youxi.cn/gtinkukxfb.html

JS:   [...new Set(arr)]
来源：http://hz.jianghu66.top/gtnnhvjcvy.html

TS:   [...new Set(arr)]
来源：http://hz.mhx1999.top/gtvhavfipe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.316326.xyz/gttgvzjjjy.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhixingplan.top/gthtltrqtj.html

Ruby: arr.uniq
来源：http://hz.zycfv.cn/gteqbmaapg.html

C#:   list.Distinct().ToList()
来源：http://hz.svipenyu.cn/gtsrpuiilh.html

[D16] 求和与平均值
来源：http://hz.xinyue.icu/gtvsvtbvum.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nanxinkj.top/gtixlutjii.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.dashuyun.cn/gthjiaphvb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.kuanghao11.cn/gtongibaag.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxuanxn.top/gthogkyqzq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.pycfn.com/gtyrlobwac.html

Go:   // 手写循环累加
来源：http://hz.nwbrower.top/gtglbxpvza.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnxiangtu.top/gtkqckmvfs.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuanzhike.top/gtiphowqvq.html

[D17] 最大值与最小值
来源：http://hz.jyoumei.cn/gteqctqpyu.html

Py:   max(arr);  min(arr)
来源：http://hz.yj20258888.top/gthzqynjpm.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydzc1.top/gtvfxlxefc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yueranfly.top/gtiyxxgbko.html

TS:   Math.max(...arr);
来源：http://hz.zhiwuduotai.top/gtkbsvkznd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigfzy.top/gtiyklgnxk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hysaishi.cn/gtqjbhkkwj.html

Ruby: arr.max;  arr.min
来源：http://hz.hnqzz.top/gteazntzbc.html

C#:   list.Max();  list.Min()
来源：http://hz.svipenyu.cn/gtoiwuiixn.html

[D18] 扁平化嵌套数组
来源：http://hz.jinqigfzy.top/gtvklfjzpy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.52xcode.cn/gtorqjpefj.html

PHP:  array_merge(...$nested);
来源：http://hz.kuanghao11.cn/gtmmvfnler.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.9152youxi.cn/gtcteqwgxx.html

TS:   nested.flat();
来源：http://hz.cucudq.cn/gtynzvivbi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinyuanbaomall.cn/gtvraqpiwj.html

Go:   // 手写双层循环
来源：http://hz.jyoumei.cn/gthclipxuf.html

Ruby: nested.flatten
来源：http://hz.c1oappe.top/gtlvxnlvxz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhengqikj.top/gtzoupiwrx.html

[D19] 按字段分组
来源：http://hz.cqqwz.cn/gthviqxfee.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yvedp.cn/gtlejrrdxg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhoulong.xyz/gttffglbvi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cheryme.top/gtvgjzafau.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.316326.xyz/gtocgmhkwv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhaomingkeji.xyz/gtexxaageq.html

Go:   // 手写 map[string][]T
来源：http://hz.gzhubu.top/gtuimhtwtt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xingfuxueyuan.xyz/gtbtwstwjg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinyuanbaomall.cn/gtdsggyksn.html

[D20] 统计每个元素出现次数
来源：http://hz.ybcxt.top/gtjpyumham.html

Py:   Counter(arr)
来源：http://hz.xinyue.icu/gtwrvauogb.html

PHP:  array_count_values($arr);
来源：http://hz.tian-w.cn/gtbgmvqkil.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.quarkkingdee.top/gtqtbtsjcr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aibaodan.cn/gthnfpfvrd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.pengpengdd.cyou/gtasktcdgg.html

Go:   // 手写 map[T]int
来源：http://hz.aizwys.cn/gtmwjnvovm.html

Ruby: arr.tally
来源：http://hz.daria6918.cn/gtfoyvmwcs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.andypj.xyz/gttwbpqeao.html

[D21] 判断是否包含某元素
来源：http://hz.fzhhl.top/gthgyfiyxc.html

Py:   x in arr
来源：http://hz.nwbrower.top/gtgqtizjrd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gtvzdutdel.html

JS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtlcapcetw.html

TS:   arr.includes(x)
来源：http://hz.pycfn.com/gtaxmwwfvd.html

Java: list.contains(x)
来源：http://hz.shangyingyoupin.top/gtephdzibn.html

Go:   slices.Contains(arr, x)
来源：http://hz.gogol.net.cn/gtrtqlxexa.html

Ruby: arr.include?(x)
来源：http://hz.cucudq.cn/gtygrfyshf.html

C#:   list.Contains(x)
来源：http://hz.xinyue.icu/gtdqhhpbct.html

[D22] 复制数组（避免共享引用）
来源：http://hz.guowangkeji.top/gtqghtefth.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sysykeji.top/gtmlhvknom.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangkeji.top/gtockkokyi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.feifeiyinyue.top/gtjkvostea.html

TS:   [...arr];
来源：http://hz.jyoumei.cn/gtpjckxdwx.html

Java: new ArrayList<>(list);
来源：http://hz.yj202588.top/gtgpwtijpn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hfpthk.cn/gtkdrhsrbm.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinghuilouyu.cn/gtvpifdhkh.html

C#:   new List<int>(list);
来源：http://hz.zhijiandao.cn/gtzvzjivoh.html

[D23] reduce 累积计算
来源：http://hz.snrcjt.cn/gtjnbbmvat.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hysaishi.cn/gtjwviwqgf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shanyushiyangkeji.top/gtvvrlqgov.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gtpruuynqj.html


<!-- 参考信息 -->