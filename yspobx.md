代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://hz.svipenyu.cn/gtngujtamy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.iojbl.cn/gtjigjnlpl.html

[C08] 闭包
来源：http://hz.jinqigfzy.top/gtujfoptkn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.bjfxy.top/gtyjffyvkq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.bjfxy.top/gtewjmdyan.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtvejjekss.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtomeixqih.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.aizwys.cn/gtbavkmstt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinqigfzy.top/gtylsezhiz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yuanzhike.top/gtztgnawkt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gthmuegdwn.html

[C09] 递归
来源：http://hz.yongpay.top/gtcbgjacxp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.aizwys.cn/gtcjuixpnk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hongshengwenyu.top/gtpkbppmmg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnxiangtu.top/gtvvdsnbhw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhixingplan.top/gtvvtwrzxm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yanxiufei.cn/gtpqnudppw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinghuilouyu.cn/gtfxurvomk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yonumen.top/gtjrjyhsaj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.meibo888.top/gtoatnxaso.html

[C10] 变量作用域
来源：http://hz.quarkkingdee.top/gtlcufrbbv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenlongwang.top/gtoqnqczlk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tanke756.top/gtjlfzxyne.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cucudq.cn/gtiuhrzngb.html

TS:   同 JS
来源：http://hz.ydjk.org.cn/gtwpyvlkob.html

Java: 方法内为块级作用域
来源：http://hz.52xcode.cn/gtjmplpede.html

Go:   花括号块级作用域
来源：http://hz.xziqi.cn/gtilztdsib.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.aizwys.cn/gtssienhao.html

C#:   块级作用域
来源：http://hz.yongpay.top/gtpbhevohu.html

[C11] 模块导入与导出
来源：http://hz.nwbrower.top/gtlzgvakdc.html

Py:   from module import func
来源：http://hz.yonumen.top/gthterugwl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xylfe.cn/gtjbxvzzyu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.haohaochexian.top/gtzrfoggjd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guannengcc.top/gtqedfwypu.html

Java: import java.util.List;
来源：http://hz.yuxming.cn/gtavsukpnu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.9152youxi.cn/gtqdmbplsu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xingfuxueyuan.xyz/gtxcgdynsw.html

C#:   using System.Text;
来源：http://hz.hongshengwenyu.top/gtidhtokwp.html

[C12] 立即执行函数 IIFE
来源：http://hz.hywenlv.cn/gtotbyuuuq.html

Py:   (lambda: print("run"))()
来源：http://hz.tian-w.cn/gtbokbhrvt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj20258888.top/gtitdcgslm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.c1oappe.top/gtujrcgpda.html

TS:   (() => { console.log("run"); })();
来源：http://hz.quarkkingdee.top/gtdkynfjgq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.52xcode.cn/gtvificxui.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jiagoushi.top/gtjjedxbeh.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhongyouzk.top/gtewwoozax.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hfpthk.cn/gtvflaqvnt.html

[C13] 类型声明 / 类型注解
来源：http://hz.ybcxt.top/gtnblsiakr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhoulong.xyz/gtcwrnenhm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jlsjyb.cn/gtqpzydkji.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.316326.xyz/gtrkdljijr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuetiantiany.cn/gtgpdthlkv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gteennuond.html

Go:   func add(a, b int) int
来源：http://hz.hongshengwenyu.top/gtipzfhqxd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gotoacloud.top/gtrdtxmqpa.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hfpthk.cn/gtgbzfchqn.html

[C14] 泛型函数
来源：http://hz.nanxinkj.top/gtcqpxmure.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.aizwys.cn/gtginouogg.html

PHP:  // 无泛型
来源：http://hz.daria6918.cn/gtprjnqeav.html

JS:   // 无泛型
来源：http://hz.jianghu66.top/gtlvvxouwt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.snrcjt.cn/gtsldunsyv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xingfuxueyuan.xyz/gtgpckatem.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hywenlv.cn/gtvbprolar.html

Ruby: # 无泛型
来源：http://hz.shzxlz.cn/gtjhcdcqvf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hammf.cn/gtktmjpvdp.html

[C15] 解构 / 展开参数
来源：http://hz.yuanzhike.top/gtguqaoiya.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cheryme.top/gtjqvvmnmt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.9152youxi.cn/gthunxkalf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinqigfzy.top/gtkfyicaln.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.redwolf501.top/gtnzfjtrnv.html

Java: // 无解构
来源：http://hz.sweek.top/gtxbumjpbm.html

Go:   // 无解构
来源：http://hz.ehwqpu.com/gtqmzyktwo.html

Ruby: a, b = pair
来源：http://hz.sysykeji.top/gtztyunktl.html

C#:   var (a, b) = pair;
来源：http://hz.svipenyu.cn/gtaucvvalz.html

[C16] 函数 / 方法重载
来源：http://hz.gaohongyu789.top/gttagvfazp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jyoumei.cn/gtywukcbzy.html

PHP:  // 无重载
来源：http://hz.yuxming.cn/gtbueseprs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tian-w.cn/gtbjangttb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.birdmap.top/gtjivqnakl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jqgfzy.top/gtvrpcvgpm.html

Go:   // 无重载：用不同函数名
来源：http://hz.cashguo.top/gtzcagrdze.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ppjwa.cn/gtfwigilsx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jqgufenzy.top/gtnuetalzw.html

================================================================================
来源：http://hz.hammf.cn/gtgirqtkep.html

D. 数组 / 列表 / 集合
来源：http://hz.jqgfzy.top/gtesmwusly.html

================================================================================
来源：http://hz.pycfn.com/gtduumbtoc.html

[D01] 创建数组 / 列表
来源：http://hz.wangdashe.top/gtuujzfowf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.pycfn.com/gthczhgzuh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.havefunace.top/gtlfuzdqgc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gotoacloud.top/gtkapknlab.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yongpay.top/gtbcqcxfzy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.fengsongda.top/gtufoewbqh.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenzaomai.com/gtaqbgpghm.html

Ruby: arr = [1, 2, 3]
来源：http://hz.iojbl.cn/gtipnbmkvm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xingfuxueyuan.xyz/gtzyxerwgq.html

[D02] 追加元素到末尾
来源：http://hz.ppjwa.cn/gtektvfmzg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenjidiqi.icu/gtrcexztfg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yonumen.top/gttgdbvmik.html

JS:   arr.push(4);
来源：http://hz.cucudq.cn/gtspsdohsq.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtknuyyfct.html

Java: list.add(4);
来源：http://hz.aibaodan.cn/gtirpfcpet.html

Go:   arr = append(arr, 4)
来源：http://hz.jqgufenzy.top/gtzzjzkycp.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.bjfxy.top/gtrsuynkwa.html

C#:   list.Add(4);
来源：http://hz.fzhhl.top/gtdqjyhogg.html

[D03] 在指定位置插入元素
来源：http://hz.vqdsnc.cn/gtvjhiepec.html

Py:   arr.insert(0, 0)
来源：http://hz.dianchejie.cn/gtnktwmvoa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhoulong.xyz/gtowechjij.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.andypj.xyz/gtbshjmsjd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.meibo888.top/gtosablqka.html

Java: list.add(0, 0);
来源：http://hz.svipenyu.cn/gtzklmpjfy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.bjfxy.top/gtbowhcyul.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.bjfxy.top/gtzrcomowi.html

C#:   list.Insert(0, 0);
来源：http://hz.yueranfly.top/gtculmftpt.html

[D04] 删除元素
来源：http://hz.daxiang520.top/gtkiaycmmg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hywenlv.cn/gtvrywuelx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.birdmap.top/gtrqpvoykl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shuidangran.top/gtcyttmoib.html

TS:   arr.splice(0, 1);
来源：http://hz.yuxming.cn/gtxwnbpttc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ybcxt.top/gtzffpvcai.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhengqikj.top/gtpeptndjr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xingfuxueyuan.xyz/gtfhvpsftr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ppjwa.cn/gtwmcabrhg.html

[D05] 访问与修改元素
来源：http://hz.xuetiantiany.cn/gtwnferxnt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gthsdkxryb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guannengcc.top/gtyrrielir.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ehwqpu.com/gtjxwgdovc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj20258888.top/gtcxvhbsuv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigfzy.top/gttqwbjwne.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shangyingyoupin.top/gtlexyzxzs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jyoumei.cn/gttjrfaenv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.tianlin.xyz/gthtpaovau.html

[D06] 数组长度
来源：http://hz.c1oappe.top/gtvzxhlehv.html

Py:   len(arr)
来源：http://hz.zhiwuduotai.top/gtvgcavtws.html

PHP:  count($arr);
来源：http://hz.pengpengdd.cyou/gtztsgrmfg.html

JS:   arr.length
来源：http://hz.jinqigfzy.top/gtnvbfrzzz.html

TS:   arr.length
来源：http://hz.yongpay.top/gtonyyqmdd.html

Java: list.size();
来源：http://hz.feifeiyinyue.top/gtyljekngt.html

Go:   len(arr)
来源：http://hz.shzxlz.cn/gtnmxmlcum.html

Ruby: arr.length; arr.size
来源：http://hz.vqdsnc.cn/gtspndopyd.html

C#:   list.Count;
来源：http://hz.vqdsnc.cn/gtgrmskvud.html

[D07] 切片 / 取子数组
来源：http://hz.316326.xyz/gthijcnmjs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinghuilouyu.cn/gtyltiqlhx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.iojbl.cn/gtrsmbtxrs.html

JS:   arr.slice(1, 4);
来源：http://hz.ydjk.org.cn/gtonwroals.html

TS:   arr.slice(1, 4);
来源：http://hz.bjfxy.top/gtlumxrdmd.html

Java: list.subList(1, 4);
来源：http://hz.nanxinkj.top/gtiboqbgjm.html

Go:   arr[1:4]
来源：http://hz.yonumen.top/gtkddsmiat.html

Ruby: arr[1, 3]
来源：http://hz.hywenlv.cn/gttxgjmzhe.html

C#:   list.GetRange(1, 3);
来源：http://hz.quarkkingdee.top/gtiktcztmn.html

[D08] 合并两个数组
来源：http://hz.nanxuanxn.top/gtjrbjnxye.html

Py:   a + b;  a.extend(b)
来源：http://hz.gaohongyu789.top/gtqmwmnacv.html

PHP:  array_merge($a, $b);
来源：http://hz.hnxiangtu.top/gtyruujkpz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xylfe.cn/gtckdmnada.html

TS:   [...a, ...b];
来源：http://hz.aibaodan.cn/gtkowxpqck.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.52xcode.cn/gtrhlwzjta.html

Go:   append(a, b...)
来源：http://hz.ivvv.top/gtbqdpcsov.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tanke756.top/gtlmlrzoxn.html

C#:   a.Concat(b).ToList()
来源：http://hz.aibaodan.cn/gtmdxjruib.html

[D09] 排序（升序）
来源：http://hz.pengpengdd.cyou/gtppwuknqa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daria6918.cn/gteubuqioh.html

PHP:  sort($arr);
来源：http://hz.nwbrower.top/gtbwxjsaiu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.316326.xyz/gtvxsxcuou.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.smart0.xyz/gtwqpynbzt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhixingplan.top/gthsakscgx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.snrcjt.cn/gthsdmvieo.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtpgedbeaa.html

C#:   list.Sort();
来源：http://hz.zhoulong.xyz/gthnruobrg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nanxuanxn.top/gtanljcmjr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aizwys.cn/gtandpaoaw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydzc1.top/gtorrszllk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtyhwphase.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenzaomai.com/gtnsrferyl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shanyushiyangtech.top/gtkwdlrqzz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.andypj.xyz/gtjldzkafn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jqgufenzy.top/gtrtokukbp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xuetiantiany.cn/gtjprwlqxa.html

[D11] 反转数组
来源：http://hz.jqgfzy.top/gtncnhefht.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangdashe.top/gtvhrovlit.html

PHP:  array_reverse($arr);
来源：http://hz.snrcjt.cn/gtzhlsuthp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tianlin.xyz/gtchextpfj.html

TS:   [...arr].reverse();
来源：http://hz.yanxiufei.cn/gtzfzqekpw.html

Java: Collections.reverse(list);
来源：http://hz.zycfv.cn/gtdkrbhunj.html

Go:   slices.Reverse(arr)
来源：http://hz.daxiang520.top/gtsqbdedub.html

Ruby: arr.reverse
来源：http://hz.cashguo.top/gtpfqczlcg.html

C#:   list.Reverse();
来源：http://hz.chenzaomai.com/gtfondhzgx.html

[D12] 查找元素下标
来源：http://hz.xylfe.cn/gtkramxatm.html

Py:   arr.index(x);  x in arr
来源：http://hz.yueranfly.top/gtnwwugngv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jianghu66.top/gtcicfqxoa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hywenlv.cn/gtfsyrvafj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cdnleiting.top/gtuepnxmvc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yuanzhike.top/gthovoberv.html

Go:   slices.Index(arr, x)
来源：http://hz.jiagoushi.top/gtkababvmo.html

Ruby: arr.index(x)
来源：http://hz.ydzc1.top/gtgmlydngs.html

C#:   list.IndexOf(x);
来源：http://hz.cheryme.top/gtfflngztl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nwbrower.top/gtuxyuluvg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hongshengwenyu.top/gttkhhevsx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.fzhhl.top/gtodrdvuki.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xingfuxueyuan.xyz/gtsaoggcnz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ybcxt.top/gtzmvzwron.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yongpay.top/gtapipqawz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.redwolf501.top/gtuhogiccd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sweek.top/gtnoyvgbfa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shangyingyoupin.top/gtufbtkryh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nanxinkj.top/gtmmvscwmt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.quarkkingdee.top/gtlvrelchj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.dianchejie.cn/gttpddxyxx.html

JS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtlhcsgbnp.html

TS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gtbjzcjngk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.daxiang520.top/gttstghjch.html

Go:   // 手写循环
来源：http://hz.hnqzz.top/gtsouscnxw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tian-w.cn/gtthshikgd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ywan-chungtsiang.top/gttdhzjwll.html

[D15] 去重
来源：http://hz.yvedp.cn/gtiztputyo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hfpthk.cn/gtdtpjvpis.html

PHP:  array_unique($arr);
来源：http://hz.yonumen.top/gtjltnbvel.html

JS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gttfnyvzzp.html

TS:   [...new Set(arr)]
来源：http://hz.yongpay.top/gtolcjnwru.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhiwuduotai.top/gtnqrffbqz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.aibaodan.cn/gtlnonmeoa.html

Ruby: arr.uniq
来源：http://hz.guowangkeji.top/gtzgtwogwi.html

C#:   list.Distinct().ToList()
来源：http://hz.vqdsnc.cn/gtlchuqjop.html

[D16] 求和与平均值
来源：http://hz.shuidangran.top/gtaelvggdr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangtech.top/gtdqkapjsf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj20258.top/gtlloofaqv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gtkpchdysk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cdnleiting.top/gtfljkbjjb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yuanzhike.top/gtnhnyptlq.html

Go:   // 手写循环累加
来源：http://hz.52xcode.cn/gtvbfjtqko.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhengqikj.top/gtydsfxqxg.html

C#:   list.Sum();  list.Average()
来源：http://hz.iojbl.cn/gtoyanzufu.html

[D17] 最大值与最小值
来源：http://hz.sufxvd.cn/gtqzqhgcdf.html

Py:   max(arr);  min(arr)
来源：http://hz.shangyingyoupin.top/gtdgxazomk.html

PHP:  max($arr);  min($arr);
来源：http://hz.cqqwz.cn/gtggkqhorz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zycfv.cn/gtgvplrekq.html

TS:   Math.max(...arr);
来源：http://hz.yuxming.cn/gthejyzfgs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.0kj1m.cn/gtwwwvxodr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ehwqpu.com/gttlmbxyef.html

Ruby: arr.max;  arr.min
来源：http://hz.yueranfly.top/gtcnmmpkya.html

C#:   list.Max();  list.Min()
来源：http://hz.sysykeji.top/gtsaatwkdv.html

[D18] 扁平化嵌套数组
来源：http://hz.cucudq.cn/gtutcomgsz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yanxiufei.cn/gtfcmemcmy.html

PHP:  array_merge(...$nested);
来源：http://hz.tianlin.xyz/gtcszmuaxo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ydzc1.top/gtverwupcp.html

TS:   nested.flat();
来源：http://hz.cashguo.top/gthkwnjtzg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinyuanbaomall.cn/gtjnbqkvkg.html

Go:   // 手写双层循环
来源：http://hz.zdqjudy.top/gtthrkjtcp.html

Ruby: nested.flatten
来源：http://hz.tian-w.cn/gtuvmompta.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.fzhhl.top/gtgumwnnux.html

[D19] 按字段分组
来源：http://hz.nanxinkj.top/gtpagresax.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangkeji.top/gthtsvywre.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jqgufenzy.top/gtvfoqmgbx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.birdmap.top/gtngwpkqdb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gtakbxmxnu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daxiang520.top/gtmlgesdfe.html

Go:   // 手写 map[string][]T
来源：http://hz.zhoulong.xyz/gtendlvfqs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.316326.xyz/gtrvwpftna.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hysaishi.cn/gtobsxwkwy.html

[D20] 统计每个元素出现次数
来源：http://hz.shuidangran.top/gtajilsozq.html

Py:   Counter(arr)
来源：http://hz.jinqigufen.top/gtnmolridh.html

PHP:  array_count_values($arr);
来源：http://hz.dashuyun.cn/gtjmdazhzr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gtwtgbkjag.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtmansjncl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nanxinkj.top/gtneealekx.html

Go:   // 手写 map[T]int
来源：http://hz.chenzaomai.com/gtdvcpsudy.html

Ruby: arr.tally
来源：http://hz.mhx1999.top/gtyznzykno.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenlongwang.top/gtztpjrdte.html

[D21] 判断是否包含某元素
来源：http://hz.cashguo.top/gtcdkbyqbt.html

Py:   x in arr
来源：http://hz.meibo888.top/gthumlpmre.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gthuetdjjy.html

JS:   arr.includes(x)
来源：http://hz.0kj1m.cn/gtutkakblf.html

TS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gttjpjrzjj.html

Java: list.contains(x)
来源：http://hz.haohaochexian.top/gtwophxgde.html

Go:   slices.Contains(arr, x)
来源：http://hz.wangshuangyany.cn/gtzaobeduo.html

Ruby: arr.include?(x)
来源：http://hz.daria6918.cn/gteglpqzvf.html

C#:   list.Contains(x)
来源：http://hz.mhx1999.top/gthvfsvthv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cdnleiting.top/gtculmbsit.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aizwys.cn/gtqckmcetz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tianlin.xyz/gtvkqtjtrc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.guannengcc.top/gtkbipjjes.html

TS:   [...arr];
来源：http://hz.xinyue.icu/gtiftisoyy.html

Java: new ArrayList<>(list);
来源：http://hz.yangfankeji.com/gtdkghgbiv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.snrcjt.cn/gtbdteijtg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shangyingyoupin.top/gtqxplnmnl.html

C#:   new List<int>(list);
来源：http://hz.cucudq.cn/gtokdqpnjg.html

[D23] reduce 累积计算
来源：http://hz.andypj.xyz/gtqfmalwax.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cucudq.cn/gtfqgdetgf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.c1oappe.top/gtbieekhuv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gthmrnrwvb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jianghu66.top/gtkyqyfsaq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jlsjyb.cn/gtvdrwyoyf.html

Go:   // 手写循环
来源：http://hz.yj20258.top/gtdfdhfmnf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.mhx1999.top/gtaydtljbn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hammf.cn/gtqlygyjuz.html

[D24] 字典 / Map 基本操作
来源：http://hz.guannengcc.top/gtqbpmlepl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ydjk.org.cn/gtuzmhvlir.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigfzy.top/gttvahnizo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sufxvd.cn/gtfkadlgut.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shuidangran.top/gtwmmjrtnp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hywenlv.cn/gtmytmlswz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shzxlz.cn/gtjdesfdsa.html


<!-- 参考信息 -->