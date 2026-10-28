代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://hz.aibaodan.cn/gtfcccyngg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhijiandao.cn/gtffudsjqb.html

[C08] 闭包
来源：http://hz.xuanzx.com/gtmiolkfwz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nwbrower.top/gttiomvpdo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.9152youxi.cn/gtwjwmyink.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.sweek.top/gtkxkzwqql.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gttxyneybc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.aizwys.cn/gthrnaemal.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yonumen.top/gtbayxzsec.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.nanxuanxn.top/gtabqyxlze.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yonumen.top/gtiixhnmub.html

[C09] 递归
来源：http://hz.yongpay.top/gttwvelvye.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.0kj1m.cn/gtxedgfkqk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hammf.cn/gtzecmhapy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.snrcjt.cn/gtqaojaqph.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhoulong.xyz/gtibqgiipj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenlongwang.top/gtyioawaan.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xuetiantiany.cn/gtdglwlnmf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.c1oappe.top/gtgrmuvgbv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.wangdashe.top/gtpmhzudiq.html

[C10] 变量作用域
来源：http://hz.yonumen.top/gtyifnctxb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dashuyun.cn/gtstezjvel.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cucudq.cn/gturrputwd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ppjwa.cn/gtqwvhskge.html

TS:   同 JS
来源：http://hz.birdmap.top/gtltwcjqcj.html

Java: 方法内为块级作用域
来源：http://hz.c1oappe.top/gtcqrootqh.html

Go:   花括号块级作用域
来源：http://hz.yanxiufei.cn/gtkhmgnerc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.redwolf501.top/gtdjtivflv.html

C#:   块级作用域
来源：http://hz.jinghuilouyu.cn/gttpmvycvv.html

[C11] 模块导入与导出
来源：http://hz.iojbl.cn/gtzmkapjup.html

Py:   from module import func
来源：http://hz.havefunace.top/gtmevcuyrj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.wangshuangyany.cn/gteytosjej.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gotoacloud.top/gtlofmwxxl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jinqigfzy.top/gtzrftrurf.html

Java: import java.util.List;
来源：http://hz.ybcxt.top/gtxgglmwyo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yuxming.cn/gtmfaemari.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fzhhl.top/gtuqlaigjf.html

C#:   using System.Text;
来源：http://hz.yongpay.top/gtpcsodmzv.html

[C12] 立即执行函数 IIFE
来源：http://hz.xuetiantiany.cn/gtjuhmgzbq.html

Py:   (lambda: print("run"))()
来源：http://hz.wangshuangyany.cn/gtcauhsoxx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hfpthk.cn/gtsfulreix.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jiagoushi.top/gtvqhbucij.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nwbrower.top/gtmqpaftrp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.birdmap.top/gtieqjksje.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ivvv.top/gtwsyauarq.html

Ruby: -> { puts "run" }.call
来源：http://hz.feifeiyinyue.top/gtnbfolnrb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.vqdsnc.cn/gtolpfzxom.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258888.top/gtelonjoou.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.0kj1m.cn/gtauwavbhm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtnnpqnsrh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nanxuanxn.top/gtgusrsdrb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.vqdsnc.cn/gtrhfuauid.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtduelmujr.html

Go:   func add(a, b int) int
来源：http://hz.sufxvd.cn/gtrvfxixya.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangshuangyany.cn/gtghwrgoin.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenzaomai.com/gtsmbrjiig.html

[C14] 泛型函数
来源：http://hz.chenlongwang.top/gtkgkfdisn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nanxuanxn.top/gtvkqvbppy.html

PHP:  // 无泛型
来源：http://hz.tanke756.top/gtvwlvcmxt.html

JS:   // 无泛型
来源：http://hz.jinghuilouyu.cn/gtukbgafnv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.daria6918.cn/gtjkjovrsj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jyoumei.cn/gtnjhmwwcc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.316326.xyz/gtlrnhyits.html

Ruby: # 无泛型
来源：http://hz.yonumen.top/gtqobwcrun.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj20258888.top/gtegpedtcx.html

[C15] 解构 / 展开参数
来源：http://hz.vqdsnc.cn/gtlgmuqoqu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.chenjidiqi.icu/gtoxylzxtb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gogol.net.cn/gtcpxrpmmh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ybcxt.top/gtqnekymvy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenjidiqi.icu/gtqpxxmdcl.html

Java: // 无解构
来源：http://hz.yueranfly.top/gtnycbglyk.html

Go:   // 无解构
来源：http://hz.yongpay.top/gtedmaruin.html

Ruby: a, b = pair
来源：http://hz.quarkkingdee.top/gtyuunenny.html

C#:   var (a, b) = pair;
来源：http://hz.jinqigufen.top/gtyvgeosyu.html

[C16] 函数 / 方法重载
来源：http://hz.yuanzhike.top/gtrvkubdrx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zycfv.cn/gthgofyddl.html

PHP:  // 无重载
来源：http://hz.yvedp.cn/gtxcmmhvgt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gzhubu.top/gtkrlgfxnx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xziqi.cn/gtwsikvecm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj20258.top/gtnhkblbbh.html

Go:   // 无重载：用不同函数名
来源：http://hz.ywan-chungtsiang.top/gtxgpcjgvi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pycfn.com/gtdofvxteh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenzaomai.com/gtelpeavzi.html

================================================================================
来源：http://hz.hfpthk.cn/gtbejzvxtm.html

D. 数组 / 列表 / 集合
来源：http://hz.shangyingyoupin.top/gttwljpkgf.html

================================================================================
来源：http://hz.dianchejie.cn/gtwrabkklw.html

[D01] 创建数组 / 列表
来源：http://hz.tian-w.cn/gtyoazaiii.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hammf.cn/gtlaflqacy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuanzhike.top/gtggfukzya.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shanyushiyangkeji.top/gtflapsvpe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cucudq.cn/gtcgvapquy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtrvhwurmf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.dianchejie.cn/gtqcnuhmuh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shzxlz.cn/gtisooymjl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sxryk.cn/gtfcxsbryg.html

[D02] 追加元素到末尾
来源：http://hz.xingfuxueyuan.xyz/gtgehgnpef.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.0kj1m.cn/gtsusrrfxr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhongyouzk.top/gtdrpuopfq.html

JS:   arr.push(4);
来源：http://hz.ehwqpu.com/gtohsesqdy.html

TS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gtrsdihyeu.html

Java: list.add(4);
来源：http://hz.yj20258.top/gtwijwzxkh.html

Go:   arr = append(arr, 4)
来源：http://hz.c1oappe.top/gtdizlhsmh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.snrcjt.cn/gtsomqgwff.html

C#:   list.Add(4);
来源：http://hz.cucudq.cn/gtpegcfifq.html

[D03] 在指定位置插入元素
来源：http://hz.zhiwuduotai.top/gtuaozgoql.html

Py:   arr.insert(0, 0)
来源：http://hz.hnxiangtu.top/gtpglhsiqs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.dianchejie.cn/gtrbzulfzv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xylfe.cn/gthggjvapq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.quarkkingdee.top/gtpalrhxtq.html

Java: list.add(0, 0);
来源：http://hz.gzhubu.top/gtnnnzrmcb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.guannengcc.top/gtcxmewntu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.nwbrower.top/gtmpvfwpng.html

C#:   list.Insert(0, 0);
来源：http://hz.hnxiangtu.top/gtljduvafp.html

[D04] 删除元素
来源：http://hz.kuanghao11.cn/gtkwglnpbd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.pycfn.com/gtkuiklkog.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sufxvd.cn/gtjmhlbnry.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.havefunace.top/gtfhgvmlnx.html

TS:   arr.splice(0, 1);
来源：http://hz.gzhubu.top/gtzlditamw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sxryk.cn/gtgxgfunok.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shanyushiyangkeji.top/gtdhupavep.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pengpengdd.cyou/gtajwsgand.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangdashe.top/gttigmjfuf.html

[D05] 访问与修改元素
来源：http://hz.hammf.cn/gtatczsmab.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtcbrasszp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.pycfn.com/gtjtklhzmo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj20258.top/gtzxcjyjrg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yanxiufei.cn/gtdpwaqilb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sysykeji.top/gttiohetoe.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtassepfid.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtkwvabtqx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hnqzz.top/gthoverlkw.html

[D06] 数组长度
来源：http://hz.aibaodan.cn/gtxxoxpsjn.html

Py:   len(arr)
来源：http://hz.jqgfzy.top/gtlknyiwou.html

PHP:  count($arr);
来源：http://hz.jqgufenzy.top/gtawskvjrs.html

JS:   arr.length
来源：http://hz.hfpthk.cn/gtexxjbcyw.html

TS:   arr.length
来源：http://hz.zhoulong.xyz/gtimwgwyhd.html

Java: list.size();
来源：http://hz.pengpengdd.cyou/gtyqbldshp.html

Go:   len(arr)
来源：http://hz.hfpthk.cn/gtxhtuetdf.html

Ruby: arr.length; arr.size
来源：http://hz.tian-w.cn/gtatarmqps.html

C#:   list.Count;
来源：http://hz.guannengcc.top/gtnwztrvol.html

[D07] 切片 / 取子数组
来源：http://hz.fengsongda.top/gtozlhcmoo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yuanzhike.top/gtlgtkjfxk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zdqjudy.top/gtfsjzqxbc.html

JS:   arr.slice(1, 4);
来源：http://hz.xinyue.icu/gtzeouqbdo.html

TS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gtwjgimtxf.html

Java: list.subList(1, 4);
来源：http://hz.hongshengwenyu.top/gtsvueplnf.html

Go:   arr[1:4]
来源：http://hz.mhx1999.top/gtmpzbwgre.html

Ruby: arr[1, 3]
来源：http://hz.pengpengdd.cyou/gtzjmktxtk.html

C#:   list.GetRange(1, 3);
来源：http://hz.316326.xyz/gtwpdvbxrf.html

[D08] 合并两个数组
来源：http://hz.xuanzx.com/gtegqbaeri.html

Py:   a + b;  a.extend(b)
来源：http://hz.hongshengwenyu.top/gtyghgjpap.html

PHP:  array_merge($a, $b);
来源：http://hz.ivvv.top/gtgjtsdehp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.316326.xyz/gttxkhyeql.html

TS:   [...a, ...b];
来源：http://hz.ybcxt.top/gthifnfcvp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.kuanghao11.cn/gtmselcwrk.html

Go:   append(a, b...)
来源：http://hz.cheryme.top/gtgrgbuubr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hongshengwenyu.top/gtcxouieln.html

C#:   a.Concat(b).ToList()
来源：http://hz.hywenlv.cn/gtiucbhzkq.html

[D09] 排序（升序）
来源：http://hz.jlsjyb.cn/gtxswdudso.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtjgstvxun.html

PHP:  sort($arr);
来源：http://hz.quarkkingdee.top/gtcexrasbb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnxiangtu.top/gtirjwpahm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinyuanbaomall.cn/gtasazyrcz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sufxvd.cn/gtfqgouxat.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zdqjudy.top/gtwmmmbwcj.html

Ruby: arr.sort
来源：http://hz.aizwys.cn/gtgajnbvhv.html

C#:   list.Sort();
来源：http://hz.xinyue.icu/gtmeohvtql.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.feifeiyinyue.top/gtusrfptcb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yonumen.top/gtnryyxvyx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.iojbl.cn/gtnhhlnyco.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuanzhike.top/gtdjnqddhj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenzaomai.com/gtqbfkttyh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenzaomai.com/gteqizcdrd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuxming.cn/gteibsfhov.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xziqi.cn/gtwpyrneod.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigfzy.top/gtapthayqu.html

[D11] 反转数组
来源：http://hz.cqqwz.cn/gtbqejbpds.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangkeji.top/gtadyyncgr.html

PHP:  array_reverse($arr);
来源：http://hz.haohaochexian.top/gtoetijsbw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yongpay.top/gtpmpoimun.html

TS:   [...arr].reverse();
来源：http://hz.yj20258888.top/gtpyrdgtqu.html

Java: Collections.reverse(list);
来源：http://hz.ywan-chungtsiang.top/gtautqnlwc.html

Go:   slices.Reverse(arr)
来源：http://hz.zhaomingkeji.xyz/gtgcnozuzf.html

Ruby: arr.reverse
来源：http://hz.ehwqpu.com/gtvlvgleof.html

C#:   list.Reverse();
来源：http://hz.ehwqpu.com/gtxeikpyvm.html

[D12] 查找元素下标
来源：http://hz.yuxming.cn/gtmzpuyrxl.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhijiandao.cn/gtomjdxkfk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xinyue.icu/gtwcmbfpyz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.smart0.xyz/gtviohasmv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtqojwxkbg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.52xcode.cn/gtpkhqyvwl.html

Go:   slices.Index(arr, x)
来源：http://hz.cdnleiting.top/gtsqpziyfm.html

Ruby: arr.index(x)
来源：http://hz.bjfxy.top/gtvmqrhvsd.html

C#:   list.IndexOf(x);
来源：http://hz.jinghuilouyu.cn/gtqhgikrrg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sufxvd.cn/gtvxgoppjz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.9152youxi.cn/gtguuhzrme.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhengqikj.top/gthhglrnpy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj202588.top/gtnoqdgmho.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangtech.top/gtvgjloyxk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aibaodan.cn/gtcikogabg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinqigfzy.top/gtbvivzrld.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yanxiufei.cn/gtlxrxmbeb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yueranfly.top/gthowqyefh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.316326.xyz/gtycgteary.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cqqwz.cn/gtbjdkhkzx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tian-w.cn/gtloxuvciz.html

JS:   arr.map(x => x * 2)
来源：http://hz.ybcxt.top/gtstqdyxpd.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhaomingkeji.xyz/gthjaixkap.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cucudq.cn/gttidhhzqb.html

Go:   // 手写循环
来源：http://hz.nwbrower.top/gtcztveebx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.316326.xyz/gtauvyilmy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xinyue.icu/gtszmufrup.html

[D15] 去重
来源：http://hz.haohaochexian.top/gtljjynfun.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtkjeomqrl.html

PHP:  array_unique($arr);
来源：http://hz.9152youxi.cn/gthcdsusec.html

JS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtuyoezytk.html

TS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtmibxfaxo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jiagoushi.top/gtpzcxkhky.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.haohaochexian.top/gtgqbnrlin.html

Ruby: arr.uniq
来源：http://hz.chenzaomai.com/gtvapgetof.html

C#:   list.Distinct().ToList()
来源：http://hz.zycfv.cn/gtillfmkhe.html

[D16] 求和与平均值
来源：http://hz.hywenlv.cn/gteolgayzo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gaohongyu789.top/gtuxhtubdt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gaohongyu789.top/gtlmfwslvm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daria6918.cn/gtdbwlhflc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hysaishi.cn/gtpeizaqsf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cdnleiting.top/gtvjopbncc.html

Go:   // 手写循环累加
来源：http://hz.zhaomingkeji.xyz/gtjftctxob.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.feifeiyinyue.top/gtknoipidq.html

C#:   list.Sum();  list.Average()
来源：http://hz.yueranfly.top/gtxxxacezu.html

[D17] 最大值与最小值
来源：http://hz.kuanghao11.cn/gtooyklqjp.html

Py:   max(arr);  min(arr)
来源：http://hz.guannengcc.top/gtdkegdiww.html

PHP:  max($arr);  min($arr);
来源：http://hz.ywan-chungtsiang.top/gtpifrkjxq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.52xcode.cn/gtlgwgimxe.html

TS:   Math.max(...arr);
来源：http://hz.jqgfzy.top/gtxxmbhwqa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gaohongyu789.top/gtdzhkxkoz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gotoacloud.top/gtratqmxoh.html

Ruby: arr.max;  arr.min
来源：http://hz.ehwqpu.com/gtxxwyjdpi.html

C#:   list.Max();  list.Min()
来源：http://hz.zhengqikj.top/gttsgwefja.html

[D18] 扁平化嵌套数组
来源：http://hz.daria6918.cn/gtaovtfora.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258.top/gtqdxoutiv.html

PHP:  array_merge(...$nested);
来源：http://hz.mhx1999.top/gtzyodjfdk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhijiandao.cn/gtheqrcyla.html

TS:   nested.flat();
来源：http://hz.gzhubu.top/gtdkbfjhim.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.svipenyu.cn/gtsawxmdih.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangkeji.top/gthsvelcpj.html

Ruby: nested.flatten
来源：http://hz.fzhhl.top/gtcgobyjxb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.havefunace.top/gtqyghzxhf.html

[D19] 按字段分组
来源：http://hz.hnqzz.top/gtplxzpmql.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hammf.cn/gtfecbkfzi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sweek.top/gtniuuadvt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.dashuyun.cn/gtdhjyotjj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yuanzhike.top/gtoapwcizj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.birdmap.top/gtllnvfitc.html

Go:   // 手写 map[string][]T
来源：http://hz.shangyingyoupin.top/gtcljbzzbi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nanxuanxn.top/gtyynzxwbt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sufxvd.cn/gtmalfrwfi.html

[D20] 统计每个元素出现次数
来源：http://hz.daria6918.cn/gtzlwzabbg.html

Py:   Counter(arr)
来源：http://hz.bjfxy.top/gtakidblmn.html

PHP:  array_count_values($arr);
来源：http://hz.xuanzx.com/gtlyfcxfiy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.bjfxy.top/gtceaqghhh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yonumen.top/gtspgxolfp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ppjwa.cn/gtfquxmohm.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigufen.top/gtckqfqjxt.html

Ruby: arr.tally
来源：http://hz.mhx1999.top/gttzjlpbyq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hongshengwenyu.top/gtjudtotjk.html

[D21] 判断是否包含某元素
来源：http://hz.jinqigufen.top/gtrowrviqu.html

Py:   x in arr
来源：http://hz.316326.xyz/gtevawnoid.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhixingplan.top/gtdvdcnlxb.html

JS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtrpdyfpdl.html

TS:   arr.includes(x)
来源：http://hz.jqgfzy.top/gtixcarrti.html

Java: list.contains(x)
来源：http://hz.fzhhl.top/gtmphatmbh.html

Go:   slices.Contains(arr, x)
来源：http://hz.haohaochexian.top/gtaflzhlsu.html

Ruby: arr.include?(x)
来源：http://hz.smart0.xyz/gtunjurunp.html

C#:   list.Contains(x)
来源：http://hz.snrcjt.cn/gtkvrtcpas.html

[D22] 复制数组（避免共享引用）
来源：http://hz.feifeiyinyue.top/gtscusrbpq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.pycfn.com/gtizzmatck.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aizwys.cn/gtldoxmgeo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hnqzz.top/gtblneclof.html

TS:   [...arr];
来源：http://hz.havefunace.top/gtbnmwnmrq.html

Java: new ArrayList<>(list);
来源：http://hz.xinyue.icu/gtbiqessyk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenjidiqi.icu/gtlijmbzhz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.birdmap.top/gtjazhchuw.html

C#:   new List<int>(list);
来源：http://hz.dashuyun.cn/gtdtuvsnac.html

[D23] reduce 累积计算
来源：http://hz.jinghuilouyu.cn/gtciaxzzqd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hywenlv.cn/gttxcrtgmj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.meibo888.top/gtzmixlkfs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnqzz.top/gthezwrsci.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.andypj.xyz/gtjrfxdqyv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.haohaochexian.top/gtrjhdvtaf.html

Go:   // 手写循环
来源：http://hz.aibaodan.cn/gtnrjgkuoo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangkeji.top/gtxlbpewwu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.52xcode.cn/gtkpzvodbe.html

[D24] 字典 / Map 基本操作
来源：http://hz.guowangkeji.top/gtxsnqdrcf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aibaodan.cn/gtjofqyfir.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.havefunace.top/gtmsdxdakp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj202588.top/gtzbocdalt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cheryme.top/gtyoykdfcs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hammf.cn/gtohmnwgta.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jqgfzy.top/gtpkqnieyo.html


<!-- 参考信息 -->