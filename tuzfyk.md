代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.9152youxi.cn/gtefiwxodm.html

TS:   arr.map(String)
来源：http://hz.jianghu66.top/gtcjqfojgm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ivvv.top/gtuzyikibj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jlsjyb.cn/gtosybuuoi.html

Ruby: arr.map(&:upcase)
来源：http://hz.0kj1m.cn/gtcibkbwvn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.iojbl.cn/gtytxwpsvm.html

[C08] 闭包
来源：http://hz.shangyingyoupin.top/gtjbkeuevb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.birdmap.top/gtkvstxduf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.fzhhl.top/gtrkygqkkl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtwyzpdyhv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gteazqxxwe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xinyue.icu/gttnnegoiq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinqigfzy.top/gtspbnfvks.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.wangshuangyany.cn/gthdhlfnhk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yonumen.top/gthxvgmhnf.html

[C09] 递归
来源：http://hz.cdnleiting.top/gttfwevyjd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xingfuxueyuan.xyz/gthyxyqtvw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ydjk.org.cn/gtoapjpqoj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtrfulqusd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jianghu66.top/gtawsdusak.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xuetiantiany.cn/gtbqflovsc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhengqikj.top/gtrzmpzexb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sysykeji.top/gthfqemael.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sweek.top/gtwbksxbxm.html

[C10] 变量作用域
来源：http://hz.shanyushiyangtech.top/gturjghbgy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sxryk.cn/gtjhbchcgo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shuidangran.top/gteuqnwxrs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.haohaochexian.top/gturgteuip.html

TS:   同 JS
来源：http://hz.aibaodan.cn/gtfmeggwbv.html

Java: 方法内为块级作用域
来源：http://hz.shangyingyoupin.top/gthfrprubn.html

Go:   花括号块级作用域
来源：http://hz.hywenlv.cn/gtthlwvfoz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.fzhhl.top/gtfcdpacpb.html

C#:   块级作用域
来源：http://hz.bjfxy.top/gtfyhfidgh.html

[C11] 模块导入与导出
来源：http://hz.jyoumei.cn/gtmeoiynca.html

Py:   from module import func
来源：http://hz.ywan-chungtsiang.top/gtbrbvycwl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.aibaodan.cn/gtmenlmorf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinghuilouyu.cn/gtjxuusiql.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.smart0.xyz/gtbtvaotiz.html

Java: import java.util.List;
来源：http://hz.jianghu66.top/gtyoolcxgx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nanxuanxn.top/gtzdfpnnuw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.0kj1m.cn/gtvbwhqsnj.html

C#:   using System.Text;
来源：http://hz.wangdashe.top/gtyblpctxg.html

[C12] 立即执行函数 IIFE
来源：http://hz.cqqwz.cn/gtqeamijtm.html

Py:   (lambda: print("run"))()
来源：http://hz.jqgufenzy.top/gtbaqlwtmo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sufxvd.cn/gthjaupyln.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtupuaesiw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.kuanghao11.cn/gthlsxepkp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yj20258888.top/gthzqevfar.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sweek.top/gthczoyaol.html

Ruby: -> { puts "run" }.call
来源：http://hz.cheryme.top/gtvvqxmgwz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aizwys.cn/gthpetbsms.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258888.top/gtrbuwvjnc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinyuanbaomall.cn/gtdnbivggt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtzjlkhmfx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pengpengdd.cyou/gtthoqouak.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigfzy.top/gtukpkcxtv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtxohpwsme.html

Go:   func add(a, b int) int
来源：http://hz.yvedp.cn/gtwwikjcvq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhaomingkeji.xyz/gttjmuxglo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jinghuilouyu.cn/gtmhlbyplp.html

[C14] 泛型函数
来源：http://hz.vqdsnc.cn/gtkqhjsyzo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ydjk.org.cn/gtvykoubfj.html

PHP:  // 无泛型
来源：http://hz.zhongyouzk.top/gtvwbhtist.html

JS:   // 无泛型
来源：http://hz.yongpay.top/gthiiaurxz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gzhubu.top/gtkhfgdgyi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigufen.top/gttivifirt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ydzc1.top/gteywnnaro.html

Ruby: # 无泛型
来源：http://hz.zhijiandao.cn/gtuchlyzvd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ywan-chungtsiang.top/gtwzuanztx.html

[C15] 解构 / 展开参数
来源：http://hz.vqdsnc.cn/gtqzgjaiyq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zycfv.cn/gtdkausrwn.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhiwuduotai.top/gtpbvaptcz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gtlnefgpyk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yuxming.cn/gtlpyqouxs.html

Java: // 无解构
来源：http://hz.sweek.top/gtewlsefrb.html

Go:   // 无解构
来源：http://hz.shanyushiyangkeji.top/gtxfzjqwkf.html

Ruby: a, b = pair
来源：http://hz.yj202588.top/gtvjewnbzv.html

C#:   var (a, b) = pair;
来源：http://hz.ydzc1.top/gtflfrfqll.html

[C16] 函数 / 方法重载
来源：http://hz.jinghuilouyu.cn/gtqvpgpznl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jlsjyb.cn/gtehxbhkfs.html

PHP:  // 无重载
来源：http://hz.jinghuilouyu.cn/gtoicboddj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jyoumei.cn/gtlatsiwjl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hysaishi.cn/gtcsxuqjdp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinghuilouyu.cn/gtqrtbqfsd.html

Go:   // 无重载：用不同函数名
来源：http://hz.yvedp.cn/gtcsvjgbvp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cucudq.cn/gtvqpzkqey.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.mhx1999.top/gtkmygcycz.html

================================================================================
来源：http://hz.hnqzz.top/gtbrksxqvn.html

D. 数组 / 列表 / 集合
来源：http://hz.wangshuangyany.cn/gtmfpyehon.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpjiqdbxq.html

[D01] 创建数组 / 列表
来源：http://hz.sweek.top/gtfdselfma.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.mhx1999.top/gtkyagxibo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.iojbl.cn/gtdgebkxox.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhoulong.xyz/gtejxqqsvi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.daxiang520.top/gtdkfmzdui.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.svipenyu.cn/gteqzlwknx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ppjwa.cn/gtpdrwjqwc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhixingplan.top/gttyjfzbot.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.tian-w.cn/gtfpoibzjg.html

[D02] 追加元素到末尾
来源：http://hz.ywan-chungtsiang.top/gtfuieawzs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.guowangkeji.top/gtrjrkcftb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuanzx.com/gtdxvphlen.html

JS:   arr.push(4);
来源：http://hz.guowangkeji.top/gtikgvrimz.html

TS:   arr.push(4);
来源：http://hz.ydjk.org.cn/gtbzpzvtyu.html

Java: list.add(4);
来源：http://hz.guannengcc.top/gtozbvuamu.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxinkj.top/gtdopghuag.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.9152youxi.cn/gtojdwbdrb.html

C#:   list.Add(4);
来源：http://hz.yj202588.top/gtncibzruc.html

[D03] 在指定位置插入元素
来源：http://hz.wangdashe.top/gtgvuyuepy.html

Py:   arr.insert(0, 0)
来源：http://hz.52xcode.cn/gtempenckm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ehwqpu.com/gtabkyupyn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shuidangran.top/gtfaswvqak.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnxiangtu.top/gtjtcyuzmv.html

Java: list.add(0, 0);
来源：http://hz.ydjk.org.cn/gtxmkwtvxe.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinghuilouyu.cn/gtrkbskeuz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinghuilouyu.cn/gtrblblzkk.html

C#:   list.Insert(0, 0);
来源：http://hz.hongshengwenyu.top/gtilqwbuen.html

[D04] 删除元素
来源：http://hz.zhoulong.xyz/gtbfcsnhia.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.mhx1999.top/gtfllqtnoz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gogol.net.cn/gtcjmgrmii.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.52xcode.cn/gtfbyngeyw.html

TS:   arr.splice(0, 1);
来源：http://hz.zhoulong.xyz/gtvlpzuvmr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yonumen.top/gtidhsxxvv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.feifeiyinyue.top/gtjhxvhxcp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.birdmap.top/gtcbwqtntz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sweek.top/gtfldwnalc.html

[D05] 访问与修改元素
来源：http://hz.yuxming.cn/gtehxsmort.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtoqguurno.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hfpthk.cn/gtfulctbyq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ivvv.top/gtsucjdtjr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenlongwang.top/gtmcymaqmv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhoulong.xyz/gtcksellts.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtigjgrvmk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xinyue.icu/gtnnjnhlnz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.pengpengdd.cyou/gtsgzdkram.html

[D06] 数组长度
来源：http://hz.gotoacloud.top/gtpetxxmrn.html

Py:   len(arr)
来源：http://hz.guowangkeji.top/gtetehnunr.html

PHP:  count($arr);
来源：http://hz.sysykeji.top/gtdgoehxjd.html

JS:   arr.length
来源：http://hz.ybcxt.top/gtgtxqhsti.html

TS:   arr.length
来源：http://hz.dianchejie.cn/gtzqyuiviz.html

Java: list.size();
来源：http://hz.aibaodan.cn/gtvvhgzmiz.html

Go:   len(arr)
来源：http://hz.fengsongda.top/gtaozshabe.html

Ruby: arr.length; arr.size
来源：http://hz.iojbl.cn/gtxhzmgpnc.html

C#:   list.Count;
来源：http://hz.aizwys.cn/gttauoigty.html

[D07] 切片 / 取子数组
来源：http://hz.fengsongda.top/gtwfwpfzwd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cheryme.top/gtdovlvpvf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.kuanghao11.cn/gtgyupjfny.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtpakjkmfo.html

TS:   arr.slice(1, 4);
来源：http://hz.zdqjudy.top/gtbaqnqnkk.html

Java: list.subList(1, 4);
来源：http://hz.hammf.cn/gthrehrzmo.html

Go:   arr[1:4]
来源：http://hz.yangfankeji.com/gthgdwmdij.html

Ruby: arr[1, 3]
来源：http://hz.dashuyun.cn/gthihhuexq.html

C#:   list.GetRange(1, 3);
来源：http://hz.xinyue.icu/gtnkhewrrj.html

[D08] 合并两个数组
来源：http://hz.hysaishi.cn/gtrfkrnhrw.html

Py:   a + b;  a.extend(b)
来源：http://hz.cashguo.top/gtoxkaelgt.html

PHP:  array_merge($a, $b);
来源：http://hz.xingfuxueyuan.xyz/gtcnwyjbkp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hnxiangtu.top/gtjnlwwnej.html

TS:   [...a, ...b];
来源：http://hz.cqqwz.cn/gtkdntaeyx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.dashuyun.cn/gtkfrtbhot.html

Go:   append(a, b...)
来源：http://hz.hysaishi.cn/gtpkqtgqvw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhaomingkeji.xyz/gtpekkmfrw.html

C#:   a.Concat(b).ToList()
来源：http://hz.havefunace.top/gtcglpbswn.html

[D09] 排序（升序）
来源：http://hz.chenzaomai.com/gtawuhzpob.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gturqhvkjo.html

PHP:  sort($arr);
来源：http://hz.yj202588.top/gtrfzgkmwn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hongshengwenyu.top/gtxegxrwgw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cashguo.top/gtxnnhlwvn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.svipenyu.cn/gtkzgtcxtr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yongpay.top/gtpociwdgo.html

Ruby: arr.sort
来源：http://hz.gogol.net.cn/gtlbxazzda.html

C#:   list.Sort();
来源：http://hz.iojbl.cn/gtwliqzgip.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hfpthk.cn/gthywbatan.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenjidiqi.icu/gtundoqedu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtnbxrhnhh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtuiogukeg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhengqikj.top/gtddmetagq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yongpay.top/gtgnojihxr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.fengsongda.top/gtffvgasgu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj20258.top/gtfbhcepmq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tian-w.cn/gtnmbtmlkx.html

[D11] 反转数组
来源：http://hz.vqdsnc.cn/gtcceqltzg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jqgfzy.top/gtiuylrxhy.html

PHP:  array_reverse($arr);
来源：http://hz.hywenlv.cn/gtryuacyqa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dianchejie.cn/gtpavejsca.html

TS:   [...arr].reverse();
来源：http://hz.9152youxi.cn/gtijipjmzu.html

Java: Collections.reverse(list);
来源：http://hz.sysykeji.top/gtjygmfwji.html

Go:   slices.Reverse(arr)
来源：http://hz.guowangkeji.top/gtlmfylyue.html

Ruby: arr.reverse
来源：http://hz.zhengqikj.top/gtexjvkppn.html

C#:   list.Reverse();
来源：http://hz.guowangkeji.top/gtjkppzwwm.html

[D12] 查找元素下标
来源：http://hz.aibaodan.cn/gtcknmyehk.html

Py:   arr.index(x);  x in arr
来源：http://hz.cdnleiting.top/gtcbpfghpf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yj202588.top/gtymqddycp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtfypsaqrp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tianlin.xyz/gtelasxxkb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhixingplan.top/gtsddzyodv.html

Go:   slices.Index(arr, x)
来源：http://hz.meibo888.top/gtuvctphqo.html

Ruby: arr.index(x)
来源：http://hz.yangfankeji.com/gthdkxyfnj.html

C#:   list.IndexOf(x);
来源：http://hz.zhijiandao.cn/gtgmuhycdv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.meibo888.top/gttzofjvoo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sxryk.cn/gtzbjwbbbl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jianghu66.top/gtanxkszsx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hfpthk.cn/gtarphltxo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtskhqronl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sxryk.cn/gtpvikqzjc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shanyushiyangtech.top/gtstnaqtzc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jianghu66.top/gthnrcsstj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhiwuduotai.top/gthbnssnkv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.kuanghao11.cn/gtesstkwzv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.kuanghao11.cn/gtmdwwthsf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.smart0.xyz/gtaebjypto.html

JS:   arr.map(x => x * 2)
来源：http://hz.gaohongyu789.top/gtsjrrudsf.html

TS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtigfdupib.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.havefunace.top/gtqrgdscuy.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gthnhbcssm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhongyouzk.top/gtmvuhungq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtpttowpae.html

[D15] 去重
来源：http://hz.dianchejie.cn/gtirazzrsd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sweek.top/gtusekwmzm.html

PHP:  array_unique($arr);
来源：http://hz.hfpthk.cn/gtozgizqvi.html

JS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtmftffrwa.html

TS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtisqpvgov.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.redwolf501.top/gtblglhmkl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cheryme.top/gtlbvhjdgb.html

Ruby: arr.uniq
来源：http://hz.yuxming.cn/gtelkzeibc.html

C#:   list.Distinct().ToList()
来源：http://hz.zdqjudy.top/gthyxoqudu.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gtudsegqzd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ivvv.top/gtzjhvmaso.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yuanzhike.top/gtehofifid.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtsyhueqgv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cheryme.top/gtlvcmdjbr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tian-w.cn/gtdvuiiwdy.html

Go:   // 手写循环累加
来源：http://hz.yuxming.cn/gtyqjmmhcs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cdnleiting.top/gtsxtfnduy.html

C#:   list.Sum();  list.Average()
来源：http://hz.jlsjyb.cn/gteqgxbcrm.html

[D17] 最大值与最小值
来源：http://hz.aibaodan.cn/gtilsgqckf.html

Py:   max(arr);  min(arr)
来源：http://hz.chenjidiqi.icu/gtbglsymzn.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydzc1.top/gtfrljnfik.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sweek.top/gtvarccvtu.html

TS:   Math.max(...arr);
来源：http://hz.birdmap.top/gtngwaisdl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hnxiangtu.top/gtpeqwuhvi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sweek.top/gtmyipduvg.html

Ruby: arr.max;  arr.min
来源：http://hz.hnqzz.top/gtdezpcggo.html

C#:   list.Max();  list.Min()
来源：http://hz.guannengcc.top/gtuaitwdvk.html

[D18] 扁平化嵌套数组
来源：http://hz.yuanzhike.top/gtzdwdalsz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cashguo.top/gtjioysyae.html

PHP:  array_merge(...$nested);
来源：http://hz.ppjwa.cn/gtwacgsmpk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guannengcc.top/gtavohhdhl.html

TS:   nested.flat();
来源：http://hz.nanxinkj.top/gtdxudevmy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.pycfn.com/gtbuemnkmw.html

Go:   // 手写双层循环
来源：http://hz.dashuyun.cn/gtjkbkaesq.html

Ruby: nested.flatten
来源：http://hz.yj20258888.top/gtuvlihmav.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shzxlz.cn/gtkhzokyxx.html

[D19] 按字段分组
来源：http://hz.ywan-chungtsiang.top/gtbymwxrbh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.fzhhl.top/gtsxzamcmh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dianchejie.cn/gtqjjwkple.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cheryme.top/gtnpnchpsf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenzaomai.com/gtwxbpcjkr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ydjk.org.cn/gttqurvpri.html

Go:   // 手写 map[string][]T
来源：http://hz.chenjidiqi.icu/gtaduutzsn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hammf.cn/gtoeqhrezd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinqigufen.top/gthpzcdxis.html

[D20] 统计每个元素出现次数
来源：http://hz.iojbl.cn/gtdncsfauf.html

Py:   Counter(arr)
来源：http://hz.hysaishi.cn/gtxxgghwca.html

PHP:  array_count_values($arr);
来源：http://hz.yvedp.cn/gtbcfoxrby.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhoulong.xyz/gtvenywtlj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ppjwa.cn/gtrkckmktt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sxryk.cn/gtsckvaheu.html

Go:   // 手写 map[T]int
来源：http://hz.yj202588.top/gtkdmjusyk.html

Ruby: arr.tally
来源：http://hz.tanke756.top/gtzxyvcezw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ybcxt.top/gttkthxyau.html

[D21] 判断是否包含某元素
来源：http://hz.jinghuilouyu.cn/gttrtwousu.html

Py:   x in arr
来源：http://hz.chenjidiqi.icu/gtsqsteyul.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhiwuduotai.top/gtzgoqdqfp.html

JS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtaqvllmwb.html

TS:   arr.includes(x)
来源：http://hz.yangfankeji.com/gtnfwowyzs.html

Java: list.contains(x)
来源：http://hz.redwolf501.top/gtajwijdqi.html

Go:   slices.Contains(arr, x)
来源：http://hz.c1oappe.top/gtltwejntn.html

Ruby: arr.include?(x)
来源：http://hz.wangdashe.top/gtnkiauwti.html

C#:   list.Contains(x)
来源：http://hz.jianghu66.top/gtmlsrpqqx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.0kj1m.cn/gtgzaersvr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.wangshuangyany.cn/gtbtzbxpnm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangshuangyany.cn/gturraeozi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hywenlv.cn/gtoxpkvjvv.html

TS:   [...arr];
来源：http://hz.ivvv.top/gtwikurtdx.html

Java: new ArrayList<>(list);
来源：http://hz.chenjidiqi.icu/gtksvvbydu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ppjwa.cn/gteltufixe.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hnxiangtu.top/gtcwcgogwa.html

C#:   new List<int>(list);
来源：http://hz.aibaodan.cn/gtagopolgx.html

[D23] reduce 累积计算
来源：http://hz.jinyuanbaomall.cn/gthdkasawh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj20258.top/gtrxoyztdu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ppjwa.cn/gtwejzogxz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tanke756.top/gtmmdypkow.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gttvlflbxa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xylfe.cn/gtkrrmdqfy.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtmytsktqx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jianghu66.top/gtnkejfaoi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.haohaochexian.top/gtqrmkbwho.html

[D24] 字典 / Map 基本操作
来源：http://hz.yonumen.top/gteaiqpecg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ivvv.top/gteoirnbsc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xinyue.icu/gtqflxjtnl.html


<!-- 参考信息 -->