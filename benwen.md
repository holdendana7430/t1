代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yuanzhike.top/gtwfhrcdba.html

[C07] 把函数作为参数传入
来源：http://hz.tianlin.xyz/gtkuypeuhk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.fengsongda.top/gtstvpxvcx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ehwqpu.com/gtboduwloc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hammf.cn/gtttfqkfam.html

TS:   arr.map(String)
来源：http://hz.tian-w.cn/gtqfsjhhyu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sxryk.cn/gtxfdkembu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ydjk.org.cn/gtmecqchlk.html

Ruby: arr.map(&:upcase)
来源：http://hz.guowangkeji.top/gtvvnngrhv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yuxming.cn/gtvuoafdtw.html

[C08] 闭包
来源：http://hz.snrcjt.cn/gtrgdlanwd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.52xcode.cn/gtraswebtv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jiagoushi.top/gtuzuculrw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtnonxlnsz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtehrvgejv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.9152youxi.cn/gtizqqcpwp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hfpthk.cn/gtdixgenpr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yonumen.top/gtachzawlk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.chenzaomai.com/gtybhpkrvl.html

[C09] 递归
来源：http://hz.pycfn.com/gtnhfuvwzj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtxbmahmsx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yvedp.cn/gtadckkzrc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangtech.top/gttglexvmi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jlsjyb.cn/gtjvduwudr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.c1oappe.top/gthuxjecqp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.iojbl.cn/gtepfjncfw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cashguo.top/gtnlwilrad.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.316326.xyz/gtojizprxf.html

[C10] 变量作用域
来源：http://hz.gotoacloud.top/gtffxsgluo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.andypj.xyz/gthqqgbqpx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.316326.xyz/gtacuskrta.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hnqzz.top/gtsexuzsbd.html

TS:   同 JS
来源：http://hz.jianghu66.top/gtcidsarnn.html

Java: 方法内为块级作用域
来源：http://hz.jiagoushi.top/gtbrpsnqmw.html

Go:   花括号块级作用域
来源：http://hz.yueranfly.top/gtkmnepdnc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hnxiangtu.top/gtzllilcti.html

C#:   块级作用域
来源：http://hz.pycfn.com/gtwdjxjqyz.html

[C11] 模块导入与导出
来源：http://hz.cheryme.top/gtiqxsxsgz.html

Py:   from module import func
来源：http://hz.xingfuxueyuan.xyz/gtvsueeups.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.52xcode.cn/gtjpefjtzx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zycfv.cn/gtajpcmjak.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cucudq.cn/gtjttdwmaz.html

Java: import java.util.List;
来源：http://hz.aibaodan.cn/gtvgimphsu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.kuanghao11.cn/gtukmhgibc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yongpay.top/gtycsaacez.html

C#:   using System.Text;
来源：http://hz.jianghu66.top/gthbgfiezg.html

[C12] 立即执行函数 IIFE
来源：http://hz.wangshuangyany.cn/gtljmrftez.html

Py:   (lambda: print("run"))()
来源：http://hz.hnqzz.top/gtvxlbrggl.html

PHP:  (function () { echo "run"; })();
来源：http://hz.tanke756.top/gtuoexskcq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cashguo.top/gtprdwqqkd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gtjwcgujrj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yueranfly.top/gtnfpkiymm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aizwys.cn/gtyuhhvaii.html

Ruby: -> { puts "run" }.call
来源：http://hz.kuanghao11.cn/gtakwqtvdt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ppjwa.cn/gteoucylxd.html

[C13] 类型声明 / 类型注解
来源：http://hz.cqqwz.cn/gtdeiuxlof.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtodfmicnf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtvqitqnir.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.vqdsnc.cn/gtqdkvzpgp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jlsjyb.cn/gtgugwddcf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gtjvsckvmp.html

Go:   func add(a, b int) int
来源：http://hz.xuanzx.com/gtracnxnvh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sweek.top/gtfbrotgim.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daxiang520.top/gtzgefyetm.html

[C14] 泛型函数
来源：http://hz.vqdsnc.cn/gtgqdowjom.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.316326.xyz/gtmmagecot.html

PHP:  // 无泛型
来源：http://hz.quarkkingdee.top/gtctwxjrkw.html

JS:   // 无泛型
来源：http://hz.shanyushiyangkeji.top/gtocoyejmw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.fengsongda.top/gtwwrxtuqx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shanyushiyangkeji.top/gtgfjenvlx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hnqzz.top/gtenfavhxf.html

Ruby: # 无泛型
来源：http://hz.havefunace.top/gttkhemots.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pengpengdd.cyou/gtbeummmkl.html

[C15] 解构 / 展开参数
来源：http://hz.tianlin.xyz/gtcskecdce.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tian-w.cn/gtzeywgpjn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.birdmap.top/gtnktfubhn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tianlin.xyz/gtywnsmfzr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenjidiqi.icu/gtgqrfdrwm.html

Java: // 无解构
来源：http://hz.chenlongwang.top/gtszarfknc.html

Go:   // 无解构
来源：http://hz.cheryme.top/gtahrkjxcd.html

Ruby: a, b = pair
来源：http://hz.zhaomingkeji.xyz/gtgmznqazi.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtqbotkbxj.html

[C16] 函数 / 方法重载
来源：http://hz.9152youxi.cn/gtyjzazazx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258.top/gtjyapjqgn.html

PHP:  // 无重载
来源：http://hz.gogol.net.cn/gtfkahvgub.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ehwqpu.com/gtvzjmiwyf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.9152youxi.cn/gtlhxeopge.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shangyingyoupin.top/gtpfpjqqrw.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhongyouzk.top/gtzspduppv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxuanxn.top/gtpgvgluzt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tanke756.top/gtjpwevvwu.html

================================================================================
来源：http://hz.cucudq.cn/gtzkvsifie.html

D. 数组 / 列表 / 集合
来源：http://hz.c1oappe.top/gtaywlutwx.html

================================================================================
来源：http://hz.iojbl.cn/gtszugdafw.html

[D01] 创建数组 / 列表
来源：http://hz.nanxuanxn.top/gtatvkajhr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yuxming.cn/gtwoqjltyi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sufxvd.cn/gtpjzzgbqs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.svipenyu.cn/gtzjnlrfqo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258.top/gtwqzodxhr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxuanxn.top/gtjuczrcwe.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj202588.top/gtfbirvwte.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jianghu66.top/gteomszmah.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgufenzy.top/gtvksibodb.html

[D02] 追加元素到末尾
来源：http://hz.cdnleiting.top/gtujouxvcp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhongyouzk.top/gtmjzlarmd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shuidangran.top/gtfevwciio.html

JS:   arr.push(4);
来源：http://hz.zhaomingkeji.xyz/gthzclsmwy.html

TS:   arr.push(4);
来源：http://hz.chenzaomai.com/gtjyzloilh.html

Java: list.add(4);
来源：http://hz.yj20258.top/gtkalypsfa.html

Go:   arr = append(arr, 4)
来源：http://hz.zdqjudy.top/gtrpctouac.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sufxvd.cn/gtqwzlzoez.html

C#:   list.Add(4);
来源：http://hz.meibo888.top/gttbxsjtqs.html

[D03] 在指定位置插入元素
来源：http://hz.yueranfly.top/gtcwzaaqrs.html

Py:   arr.insert(0, 0)
来源：http://hz.nanxinkj.top/gtnzchiovc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hongshengwenyu.top/gtlkoqnqoe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cdnleiting.top/gtjiigbgqy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ywan-chungtsiang.top/gtocuszssk.html

Java: list.add(0, 0);
来源：http://hz.daxiang520.top/gthvuwepuo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yonumen.top/gtpuvjcyqv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hnxiangtu.top/gtamyqydin.html

C#:   list.Insert(0, 0);
来源：http://hz.52xcode.cn/gtqxumljpg.html

[D04] 删除元素
来源：http://hz.yueranfly.top/gtotyqhrtu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cqqwz.cn/gtutdlobxp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jiagoushi.top/gtoknxikqy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hnqzz.top/gteigdnnvm.html

TS:   arr.splice(0, 1);
来源：http://hz.iojbl.cn/gtntcxawub.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xingfuxueyuan.xyz/gtatlfsxbg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yueranfly.top/gtxleqgeje.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigufen.top/gtnkrmkibb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cdnleiting.top/gtwsvvupsa.html

[D05] 访问与修改元素
来源：http://hz.shanyushiyangkeji.top/gtewgxifgg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gtjacswgpx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hnxiangtu.top/gtxfxzcraj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jyoumei.cn/gtpjnosqqv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shzxlz.cn/gtcvdlhcll.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hammf.cn/gtphwrbvge.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jqgufenzy.top/gtvdtlnrba.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nwbrower.top/gtqywpyhsp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yangfankeji.com/gtjlisnrnl.html

[D06] 数组长度
来源：http://hz.havefunace.top/gtmjwtsvtu.html

Py:   len(arr)
来源：http://hz.ybcxt.top/gtjlsrpgvi.html

PHP:  count($arr);
来源：http://hz.jinyuanbaomall.cn/gtjybzqvzf.html

JS:   arr.length
来源：http://hz.pengpengdd.cyou/gtuxmrveph.html

TS:   arr.length
来源：http://hz.zhongyouzk.top/gtjlnpkpcu.html

Java: list.size();
来源：http://hz.zhijiandao.cn/gtdypvwooe.html

Go:   len(arr)
来源：http://hz.shanyushiyangtech.top/gthjbdilcn.html

Ruby: arr.length; arr.size
来源：http://hz.jqgfzy.top/gtxczcltgu.html

C#:   list.Count;
来源：http://hz.snrcjt.cn/gtqodijhsm.html

[D07] 切片 / 取子数组
来源：http://hz.jinqigfzy.top/gtnxeeuoza.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.52xcode.cn/gtflzzfdtc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.pengpengdd.cyou/gtwvqsmiqf.html

JS:   arr.slice(1, 4);
来源：http://hz.shuidangran.top/gtsqwzxpub.html

TS:   arr.slice(1, 4);
来源：http://hz.guannengcc.top/gtckremupy.html

Java: list.subList(1, 4);
来源：http://hz.jqgfzy.top/gtjegudjfn.html

Go:   arr[1:4]
来源：http://hz.aibaodan.cn/gtedwlatrp.html

Ruby: arr[1, 3]
来源：http://hz.cheryme.top/gtfxvpybyw.html

C#:   list.GetRange(1, 3);
来源：http://hz.sweek.top/gtejuaimbm.html

[D08] 合并两个数组
来源：http://hz.sufxvd.cn/gttffglgsy.html

Py:   a + b;  a.extend(b)
来源：http://hz.daria6918.cn/gtjffmvnnb.html

PHP:  array_merge($a, $b);
来源：http://hz.shanyushiyangkeji.top/gtntbytbsr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nwbrower.top/gtisbkdcwj.html

TS:   [...a, ...b];
来源：http://hz.ivvv.top/gtkpyyencg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yonumen.top/gtqsuuaodx.html

Go:   append(a, b...)
来源：http://hz.zhixingplan.top/gttasvdzjx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jqgufenzy.top/gtzgxzoguq.html

C#:   a.Concat(b).ToList()
来源：http://hz.aizwys.cn/gtoxbrngfr.html

[D09] 排序（升序）
来源：http://hz.kuanghao11.cn/gthdzmizkn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.c1oappe.top/gtsqzgalfj.html

PHP:  sort($arr);
来源：http://hz.gotoacloud.top/gtusmqwhfy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yvedp.cn/gteerggxio.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aizwys.cn/gtivgspamc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hammf.cn/gtynsopiez.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtdqaqblmm.html

Ruby: arr.sort
来源：http://hz.hongshengwenyu.top/gthwszdlhw.html

C#:   list.Sort();
来源：http://hz.zhiwuduotai.top/gtspajvlbq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ivvv.top/gttpqwmial.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.quarkkingdee.top/gthkqkhkrk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sufxvd.cn/gtygucqaqh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.smart0.xyz/gtgbpighvg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ywan-chungtsiang.top/gtygootalb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nanxuanxn.top/gtlpxjxnqn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yonumen.top/gtuojszvbq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxuanxn.top/gtimtcuska.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jqgufenzy.top/gtyznydekr.html

[D11] 反转数组
来源：http://hz.jiagoushi.top/gtsgcwoefq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.iojbl.cn/gtpdagrico.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258888.top/gtstmycfrf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sufxvd.cn/gtxitqznsq.html

TS:   [...arr].reverse();
来源：http://hz.jinqigfzy.top/gtkcuarzkm.html

Java: Collections.reverse(list);
来源：http://hz.ydjk.org.cn/gtqsecdcdc.html

Go:   slices.Reverse(arr)
来源：http://hz.ywan-chungtsiang.top/gtrqhgnbbg.html

Ruby: arr.reverse
来源：http://hz.sxryk.cn/gtdqasiroz.html

C#:   list.Reverse();
来源：http://hz.yanxiufei.cn/gtcmonfrji.html

[D12] 查找元素下标
来源：http://hz.shzxlz.cn/gtopisbugn.html

Py:   arr.index(x);  x in arr
来源：http://hz.9152youxi.cn/gtqgbjbdlm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tian-w.cn/gtmowrqnfk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ppjwa.cn/gtfcilucwu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gttucjcmaj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenlongwang.top/gtiyrcpxim.html

Go:   slices.Index(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gticgmpgop.html

Ruby: arr.index(x)
来源：http://hz.yonumen.top/gtqvetjaxr.html

C#:   list.IndexOf(x);
来源：http://hz.hysaishi.cn/gtiritvgqx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cheryme.top/gturbowsvj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ppjwa.cn/gtyzqaykpy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.feifeiyinyue.top/gtnaqqzeyz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj20258.top/gtgyexrshy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangdashe.top/gteebapnro.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hysaishi.cn/gtxofbbhmd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.guannengcc.top/gttksedtzb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgfzy.top/gtnypimfsy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.snrcjt.cn/gtonafhkus.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj20258.top/gtbgkwmcgx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shanyushiyangtech.top/gtrfituedv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ydjk.org.cn/gtllltxzma.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangshuangyany.cn/gtwigzikja.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinghuilouyu.cn/gtgasxytds.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.redwolf501.top/gtsiqfzxhf.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtjvzddgih.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ydjk.org.cn/gtknwjjexw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gzhubu.top/gtdpsprbdr.html

[D15] 去重
来源：http://hz.jyoumei.cn/gtatqysugf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.meibo888.top/gtpufsdbtn.html

PHP:  array_unique($arr);
来源：http://hz.ybcxt.top/gtdshfmjzy.html

JS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gttgecdnom.html

TS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtdvqarrce.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.9152youxi.cn/gtruvtsuju.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangshuangyany.cn/gtelokyozd.html

Ruby: arr.uniq
来源：http://hz.havefunace.top/gtvjkvdtbq.html

C#:   list.Distinct().ToList()
来源：http://hz.ydjk.org.cn/gtdvkqkbfh.html

[D16] 求和与平均值
来源：http://hz.vqdsnc.cn/gtdbeszowq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhengqikj.top/gtqicsvpoq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shanyushiyangtech.top/gtmuupwcom.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sufxvd.cn/gtnispdbmn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhongyouzk.top/gtmclytyvj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hongshengwenyu.top/gtsscpzqjq.html

Go:   // 手写循环累加
来源：http://hz.daxiang520.top/gtfjppxovo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.birdmap.top/gtkmxasvtf.html

C#:   list.Sum();  list.Average()
来源：http://hz.52xcode.cn/gtnsdzobhz.html

[D17] 最大值与最小值
来源：http://hz.feifeiyinyue.top/gtixgqsfke.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtpxvahzys.html

PHP:  max($arr);  min($arr);
来源：http://hz.hywenlv.cn/gtkphveaul.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shuidangran.top/gttbnopxxq.html

TS:   Math.max(...arr);
来源：http://hz.yongpay.top/gtrzgqcfle.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhiwuduotai.top/gtssnogafs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ybcxt.top/gtqdodumtv.html

Ruby: arr.max;  arr.min
来源：http://hz.birdmap.top/gtqotcbhvz.html

C#:   list.Max();  list.Min()
来源：http://hz.cqqwz.cn/gtbyranfgg.html

[D18] 扁平化嵌套数组
来源：http://hz.hysaishi.cn/gtzflaggja.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhengqikj.top/gtllxbbzad.html

PHP:  array_merge(...$nested);
来源：http://hz.yj20258888.top/gtxvelxrwi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.chenlongwang.top/gtvqhwdxup.html

TS:   nested.flat();
来源：http://hz.pengpengdd.cyou/gtlhdhptbq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxinkj.top/gtthulyalw.html

Go:   // 手写双层循环
来源：http://hz.xylfe.cn/gtcxiolkex.html

Ruby: nested.flatten
来源：http://hz.sweek.top/gtjvkettzh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hysaishi.cn/gtjtvhxwwi.html

[D19] 按字段分组
来源：http://hz.zhongyouzk.top/gtazmvfgrn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ehwqpu.com/gtrcpflkrs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.pycfn.com/gtlzqtirpi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yuxming.cn/gtvacyyecw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cheryme.top/gtnjrepznm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daxiang520.top/gtntxnzdmi.html

Go:   // 手写 map[string][]T
来源：http://hz.kuanghao11.cn/gtzrdrpvua.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.haohaochexian.top/gtzabuppuf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ivvv.top/gttjtanqlc.html

[D20] 统计每个元素出现次数
来源：http://hz.pengpengdd.cyou/gtmodhomvi.html

Py:   Counter(arr)
来源：http://hz.redwolf501.top/gtmrwujfun.html

PHP:  array_count_values($arr);
来源：http://hz.zhixingplan.top/gtkphrvocx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtanyqncdi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jyoumei.cn/gttviehill.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nwbrower.top/gtdirsfseb.html

Go:   // 手写 map[T]int
来源：http://hz.cheryme.top/gtcxqxiaqt.html

Ruby: arr.tally
来源：http://hz.cqqwz.cn/gtzeitmbwj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhiwuduotai.top/gtzurpkfeo.html

[D21] 判断是否包含某元素
来源：http://hz.yueranfly.top/gtprsfijos.html

Py:   x in arr
来源：http://hz.gotoacloud.top/gtwjxxclin.html

PHP:  in_array($x, $arr, true);
来源：http://hz.andypj.xyz/gtiyoehapm.html

JS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtovahahkq.html

TS:   arr.includes(x)
来源：http://hz.hywenlv.cn/gtxeemhsyn.html

Java: list.contains(x)
来源：http://hz.jinyuanbaomall.cn/gticqwniml.html

Go:   slices.Contains(arr, x)
来源：http://hz.sweek.top/gtkkrnoaei.html

Ruby: arr.include?(x)
来源：http://hz.dashuyun.cn/gtigyqagdw.html

C#:   list.Contains(x)
来源：http://hz.dashuyun.cn/gtnsbxezar.html

[D22] 复制数组（避免共享引用）
来源：http://hz.guowangkeji.top/gtuypwmwge.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jyoumei.cn/gtpgbdixqt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hfpthk.cn/gtcwgyursq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xinyue.icu/gtzunrlxjk.html

TS:   [...arr];
来源：http://hz.feifeiyinyue.top/gtujdzfuct.html

Java: new ArrayList<>(list);
来源：http://hz.daxiang520.top/gtwzkzfqki.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhixingplan.top/gtffmtfsyw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xingfuxueyuan.xyz/gtpuzxpkuq.html

C#:   new List<int>(list);
来源：http://hz.jinghuilouyu.cn/gtxnenmkdk.html

[D23] reduce 累积计算
来源：http://hz.yongpay.top/gtuzopnwil.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnqzz.top/gtqzwmrrbv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cqqwz.cn/gtjtmpzzor.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gtuqebourr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtetdimupz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jqgufenzy.top/gtymzrzigy.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtmtkknhek.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jlsjyb.cn/gtppkaczcq.html


<!-- 参考信息 -->