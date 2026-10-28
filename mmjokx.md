代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sxryk.cn/gtdfgblewx.html

[C07] 把函数作为参数传入
来源：http://hz.yj20258.top/gtyywvchsw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.vqdsnc.cn/gtgazpitzu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenjidiqi.icu/gtxyjgtgjk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.wangshuangyany.cn/gtjacwylir.html

TS:   arr.map(String)
来源：http://hz.guowangkeji.top/gthnlfjscg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dianchejie.cn/gtleclkvbr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cashguo.top/gtoprwtrpb.html

Ruby: arr.map(&:upcase)
来源：http://hz.shuidangran.top/gttzbhyfow.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.aizwys.cn/gtvsvdgoyo.html

[C08] 闭包
来源：http://hz.zhijiandao.cn/gtremuqmkc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.feifeiyinyue.top/gtafpjfoqa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinghuilouyu.cn/gtgdvdqzdo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ehwqpu.com/gtmejhsfqn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtgcrhjffn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ybcxt.top/gtrnpimajp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cdnleiting.top/gtcmiwmzzu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj20258.top/gtiqmtubhg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtqvmwpoyg.html

[C09] 递归
来源：http://hz.gotoacloud.top/gtziubnihu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.9152youxi.cn/gtsyecucmx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yvedp.cn/gtokcmmwee.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtigoiblrk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xingfuxueyuan.xyz/gtarqjanld.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenjidiqi.icu/gtfbohijwz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xinyue.icu/gtqcdnhxyq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yongpay.top/gtusbyrows.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jyoumei.cn/gtjuoxigie.html

[C10] 变量作用域
来源：http://hz.hnxiangtu.top/gtxcgdgxog.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xylfe.cn/gtyoqywulq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yuxming.cn/gtmaqqxxtn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangdashe.top/gtpbfvgsrh.html

TS:   同 JS
来源：http://hz.smart0.xyz/gtshesqdhs.html

Java: 方法内为块级作用域
来源：http://hz.cdnleiting.top/gtrhzhxutl.html

Go:   花括号块级作用域
来源：http://hz.svipenyu.cn/gtuhrxpvqe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yongpay.top/gtagycujei.html

C#:   块级作用域
来源：http://hz.dianchejie.cn/gtrslfsekg.html

[C11] 模块导入与导出
来源：http://hz.ywan-chungtsiang.top/gtuqgybnwk.html

Py:   from module import func
来源：http://hz.meibo888.top/gthjbdfoay.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xingfuxueyuan.xyz/gtkwrqsotf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yvedp.cn/gtvvdlmcis.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhijiandao.cn/gtzzoewyqm.html

Java: import java.util.List;
来源：http://hz.daria6918.cn/gtiekuojhq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hysaishi.cn/gthaqzdjwk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yanxiufei.cn/gtzlffqzjo.html

C#:   using System.Text;
来源：http://hz.birdmap.top/gtyahgdapz.html

[C12] 立即执行函数 IIFE
来源：http://hz.jlsjyb.cn/gtxlazvmiy.html

Py:   (lambda: print("run"))()
来源：http://hz.kuanghao11.cn/gtvenlezka.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxuanxn.top/gtpytqeyua.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangkeji.top/gturxtgtmn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigfzy.top/gtflrwpkhr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.fengsongda.top/gtpptjgbog.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hammf.cn/gtfrreohxu.html

Ruby: -> { puts "run" }.call
来源：http://hz.hammf.cn/gtxozowgve.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ivvv.top/gtiqkodtho.html

[C13] 类型声明 / 类型注解
来源：http://hz.shanyushiyangtech.top/gtfxaitytj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gaohongyu789.top/gtvkjnzbhp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtcwdmmxga.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sweek.top/gtvywbotub.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgufenzy.top/gtbcwxezqo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtepccjkwv.html

Go:   func add(a, b int) int
来源：http://hz.yvedp.cn/gtmudbbhkl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.tanke756.top/gtfzuqxmdj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gzhubu.top/gtrxrfevnc.html

[C14] 泛型函数
来源：http://hz.zhoulong.xyz/gtochhcond.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ivvv.top/gthgksiusf.html

PHP:  // 无泛型
来源：http://hz.mhx1999.top/gtzdthqeuu.html

JS:   // 无泛型
来源：http://hz.yuanzhike.top/gtxjoymnkb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.feifeiyinyue.top/gtdpjvfpsk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jianghu66.top/gtwmbpcqdf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangdashe.top/gtcvrqzwli.html

Ruby: # 无泛型
来源：http://hz.ydjk.org.cn/gtjjzqitwu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhaomingkeji.xyz/gtmtnlijyv.html

[C15] 解构 / 展开参数
来源：http://hz.yanxiufei.cn/gtkmgwlvfw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ivvv.top/gtwzlsuiqq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.fengsongda.top/gtnnqidwol.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhoulong.xyz/gtwhsgpvux.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xinyue.icu/gtsichxzud.html

Java: // 无解构
来源：http://hz.shanyushiyangtech.top/gtulotdbgf.html

Go:   // 无解构
来源：http://hz.0kj1m.cn/gtvgrztsbd.html

Ruby: a, b = pair
来源：http://hz.vqdsnc.cn/gtayrocbhm.html

C#:   var (a, b) = pair;
来源：http://hz.zhaomingkeji.xyz/gttxrikivz.html

[C16] 函数 / 方法重载
来源：http://hz.yuanzhike.top/gtjcmystim.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jqgfzy.top/gtqpbnozui.html

PHP:  // 无重载
来源：http://hz.guannengcc.top/gtjoqhbsen.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hysaishi.cn/gtbxxokkys.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhixingplan.top/gtbtjfxgba.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.vqdsnc.cn/gtsigbumxw.html

Go:   // 无重载：用不同函数名
来源：http://hz.shuidangran.top/gtzewgheuk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.tian-w.cn/gtklecyyft.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shangyingyoupin.top/gthjvwvgnu.html

================================================================================
来源：http://hz.ivvv.top/gtyiaxygkg.html

D. 数组 / 列表 / 集合
来源：http://hz.cucudq.cn/gtjcpxgcyd.html

================================================================================
来源：http://hz.cucudq.cn/gtdtvdjjdm.html

[D01] 创建数组 / 列表
来源：http://hz.shangyingyoupin.top/gtowuiykcv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sxryk.cn/gtnhixvjvv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xziqi.cn/gtbsxtztfk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.c1oappe.top/gthpqmsocl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shzxlz.cn/gtqleyhlpt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.iojbl.cn/gtjethnlas.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.guannengcc.top/gttbvzputl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ehwqpu.com/gtiiohramv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.daria6918.cn/gtatsfjugz.html

[D02] 追加元素到末尾
来源：http://hz.hammf.cn/gtynkkrkfs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daria6918.cn/gtbctblitw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yuxming.cn/gtzrwojbaj.html

JS:   arr.push(4);
来源：http://hz.gotoacloud.top/gtvdpdpnkg.html

TS:   arr.push(4);
来源：http://hz.daria6918.cn/gtolfamoeo.html

Java: list.add(4);
来源：http://hz.dianchejie.cn/gtuqmwjenw.html

Go:   arr = append(arr, 4)
来源：http://hz.xingfuxueyuan.xyz/gtrzzvavsg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.haohaochexian.top/gtooeqztue.html

C#:   list.Add(4);
来源：http://hz.yuanzhike.top/gtysoyitkq.html

[D03] 在指定位置插入元素
来源：http://hz.haohaochexian.top/gtknnbmbbz.html

Py:   arr.insert(0, 0)
来源：http://hz.quarkkingdee.top/gtbtwalxsf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenjidiqi.icu/gtqvqltmcq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hnqzz.top/gtqcmlvutn.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258.top/gtfrhxkmgt.html

Java: list.add(0, 0);
来源：http://hz.yueranfly.top/gtjrrcjaqs.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.c1oappe.top/gtqiqshtla.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tian-w.cn/gtjyjznxxj.html

C#:   list.Insert(0, 0);
来源：http://hz.ehwqpu.com/gtypidlqkk.html

[D04] 删除元素
来源：http://hz.zdqjudy.top/gtgsgzvyox.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.0kj1m.cn/gtbmhnvmqs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jiagoushi.top/gtyljswfwk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.havefunace.top/gtgndsxhah.html

TS:   arr.splice(0, 1);
来源：http://hz.shanyushiyangkeji.top/gtpctlrmts.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yj20258.top/gtjdzmvnlh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhixingplan.top/gtptcuqxxj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.daxiang520.top/gtarwhohrg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.svipenyu.cn/gtzguwkltq.html

[D05] 访问与修改元素
来源：http://hz.hammf.cn/gtisbnavoc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gttsadqwfp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.meibo888.top/gtojtwoamn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigfzy.top/gtchpdiusx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jiagoushi.top/gtcpmkclfa.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuanzhike.top/gtubkfiunm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.havefunace.top/gtwetgocwx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtuwpbzwck.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.smart0.xyz/gtoexknlgv.html

[D06] 数组长度
来源：http://hz.sweek.top/gtencywykd.html

Py:   len(arr)
来源：http://hz.iojbl.cn/gtxyhobvor.html

PHP:  count($arr);
来源：http://hz.wangshuangyany.cn/gtnrvhxjzp.html

JS:   arr.length
来源：http://hz.fengsongda.top/gtbaiegslc.html

TS:   arr.length
来源：http://hz.shzxlz.cn/gtxthtqrzq.html

Java: list.size();
来源：http://hz.yuxming.cn/gtgrwmbjnp.html

Go:   len(arr)
来源：http://hz.yvedp.cn/gtxkfvoqyn.html

Ruby: arr.length; arr.size
来源：http://hz.kuanghao11.cn/gtnqcwehqp.html

C#:   list.Count;
来源：http://hz.aizwys.cn/gtyujscnmc.html

[D07] 切片 / 取子数组
来源：http://hz.yuanzhike.top/gtanaufkue.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jqgfzy.top/gtqwoomsjd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tianlin.xyz/gttchwapmk.html

JS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtclebngrx.html

TS:   arr.slice(1, 4);
来源：http://hz.ydzc1.top/gtpigqcfzf.html

Java: list.subList(1, 4);
来源：http://hz.fengsongda.top/gthhmmsahh.html

Go:   arr[1:4]
来源：http://hz.haohaochexian.top/gtudphvlgt.html

Ruby: arr[1, 3]
来源：http://hz.0kj1m.cn/gtjfqebjkm.html

C#:   list.GetRange(1, 3);
来源：http://hz.yonumen.top/gtjfxipoxd.html

[D08] 合并两个数组
来源：http://hz.sufxvd.cn/gtqbjnczab.html

Py:   a + b;  a.extend(b)
来源：http://hz.dashuyun.cn/gttjawpgbh.html

PHP:  array_merge($a, $b);
来源：http://hz.sysykeji.top/gtkodcumwx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.feifeiyinyue.top/gtgngisqqr.html

TS:   [...a, ...b];
来源：http://hz.daria6918.cn/gtmbvwwzsn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daxiang520.top/gtuflldcqs.html

Go:   append(a, b...)
来源：http://hz.ppjwa.cn/gtmjnqfsoo.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xingfuxueyuan.xyz/gtihrvehtt.html

C#:   a.Concat(b).ToList()
来源：http://hz.gogol.net.cn/gtvgtfsppv.html

[D09] 排序（升序）
来源：http://hz.chenlongwang.top/gtaitfjfdb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangdashe.top/gtbwqjnfpk.html

PHP:  sort($arr);
来源：http://hz.shangyingyoupin.top/gtefbgnuyo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xuanzx.com/gthmaqsnpk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ywan-chungtsiang.top/gtbslqygas.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tianlin.xyz/gtgypcuaxe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cheryme.top/gtulgaizro.html

Ruby: arr.sort
来源：http://hz.9152youxi.cn/gtteojrsdw.html

C#:   list.Sort();
来源：http://hz.shanyushiyangtech.top/gtmtvojxco.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zycfv.cn/gtbvsqpubo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj20258.top/gtinnyevki.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ehwqpu.com/gtjulnbjvb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yvedp.cn/gtmszlmhwi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gthvomuisy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhijiandao.cn/gtsczrasrs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yonumen.top/gtbhizxenu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.birdmap.top/gtrescukjq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.smart0.xyz/gtjrdyelmc.html

[D11] 反转数组
来源：http://hz.chenzaomai.com/gtatgbtjxd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nanxuanxn.top/gtdaaesais.html

PHP:  array_reverse($arr);
来源：http://hz.hongshengwenyu.top/gtzfghhloj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xingfuxueyuan.xyz/gtsyhlmqhl.html

TS:   [...arr].reverse();
来源：http://hz.shangyingyoupin.top/gtxsulefuw.html

Java: Collections.reverse(list);
来源：http://hz.yonumen.top/gtaldlmsoh.html

Go:   slices.Reverse(arr)
来源：http://hz.hnxiangtu.top/gtejvgfrnp.html

Ruby: arr.reverse
来源：http://hz.zhixingplan.top/gtxdijigri.html

C#:   list.Reverse();
来源：http://hz.tianlin.xyz/gttqocgnbo.html

[D12] 查找元素下标
来源：http://hz.jinqigufen.top/gtgtshedbd.html

Py:   arr.index(x);  x in arr
来源：http://hz.wangshuangyany.cn/gtczfrbvfa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhixingplan.top/gttfyuwrxj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.birdmap.top/gtmwdkqktl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hammf.cn/gtukvximor.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shuidangran.top/gthclsyibn.html

Go:   slices.Index(arr, x)
来源：http://hz.jinqigfzy.top/gtuyroghxh.html

Ruby: arr.index(x)
来源：http://hz.pengpengdd.cyou/gtxhjmrrgq.html

C#:   list.IndexOf(x);
来源：http://hz.sysykeji.top/gtguxbgwkr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yangfankeji.com/gtbhjvqsnt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jiagoushi.top/gtevdwbliv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shanyushiyangtech.top/gtqtsswodr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ybcxt.top/gtsyjiztoy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtfiixtcsy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ywan-chungtsiang.top/gtlrinthrq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhixingplan.top/gtavshyhgq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgfzy.top/gtqqnqmrbg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jianghu66.top/gtnfqsgtje.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinghuilouyu.cn/gtludsiqnn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.bjfxy.top/gtxmakwipu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fengsongda.top/gtrentssqe.html

JS:   arr.map(x => x * 2)
来源：http://hz.hnqzz.top/gteboykayl.html

TS:   arr.map(x => x * 2)
来源：http://hz.yonumen.top/gtwptchxpd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jyoumei.cn/gtwyjwkmkm.html

Go:   // 手写循环
来源：http://hz.yuxming.cn/gthtbbdanh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jianghu66.top/gtpodeuzmj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sufxvd.cn/gtzrjpfpcn.html

[D15] 去重
来源：http://hz.hnqzz.top/gtnrflexbk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.fzhhl.top/gttuevvwie.html

PHP:  array_unique($arr);
来源：http://hz.birdmap.top/gtmuweontw.html

JS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gthylqnnzs.html

TS:   [...new Set(arr)]
来源：http://hz.dianchejie.cn/gtorgpqnze.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sysykeji.top/gthrcgzhgx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.bjfxy.top/gtrrfqqbsy.html

Ruby: arr.uniq
来源：http://hz.dianchejie.cn/gtotfpdtkd.html

C#:   list.Distinct().ToList()
来源：http://hz.ydzc1.top/gtbzvimxzj.html

[D16] 求和与平均值
来源：http://hz.pycfn.com/gttbgxqjoh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinyuanbaomall.cn/gtuhwezbvx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gaohongyu789.top/gtwmljacym.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tanke756.top/gtygklpehu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zdqjudy.top/gtsxumrbav.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hysaishi.cn/gtjqfqvcwh.html

Go:   // 手写循环累加
来源：http://hz.yvedp.cn/gttwpqadro.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.tanke756.top/gtxldwadse.html

C#:   list.Sum();  list.Average()
来源：http://hz.hfpthk.cn/gtgazhlyrp.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gturdithnp.html

Py:   max(arr);  min(arr)
来源：http://hz.fzhhl.top/gtkioixwuo.html

PHP:  max($arr);  min($arr);
来源：http://hz.sweek.top/gtzvtvqshe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nanxinkj.top/gtooynglzn.html

TS:   Math.max(...arr);
来源：http://hz.daria6918.cn/gtxfrbwhrp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.c1oappe.top/gtxuqgalhb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuxming.cn/gtjkuaekqc.html

Ruby: arr.max;  arr.min
来源：http://hz.shanyushiyangtech.top/gtprpreddz.html

C#:   list.Max();  list.Min()
来源：http://hz.shzxlz.cn/gtzppbjfyz.html

[D18] 扁平化嵌套数组
来源：http://hz.aizwys.cn/gtqsupwhby.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ywan-chungtsiang.top/gtvzarsggy.html

PHP:  array_merge(...$nested);
来源：http://hz.cdnleiting.top/gtepqsrrbl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zycfv.cn/gtmwmlndou.html

TS:   nested.flat();
来源：http://hz.hfpthk.cn/gtpbfewmyi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.fengsongda.top/gtfbywways.html

Go:   // 手写双层循环
来源：http://hz.shzxlz.cn/gtbowudeqa.html

Ruby: nested.flatten
来源：http://hz.snrcjt.cn/gtdeeotxqs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhengqikj.top/gtktoqydkd.html

[D19] 按字段分组
来源：http://hz.dianchejie.cn/gtisoiyhiq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aibaodan.cn/gtxapkfarh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jyoumei.cn/gthjbvscpc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.pengpengdd.cyou/gtijykktmw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cashguo.top/gtchgbcqhb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhongyouzk.top/gtumwqmrpz.html

Go:   // 手写 map[string][]T
来源：http://hz.sweek.top/gtvwqjayoh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jiagoushi.top/gthqkmnlnj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxinkj.top/gtttxrgiwb.html

[D20] 统计每个元素出现次数
来源：http://hz.zhixingplan.top/gthvvpnuwk.html

Py:   Counter(arr)
来源：http://hz.aibaodan.cn/gtzjgxjiji.html

PHP:  array_count_values($arr);
来源：http://hz.shangyingyoupin.top/gtsbdtzrvr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtxjqidsdd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hywenlv.cn/gtinopgmca.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dashuyun.cn/gtvvjzbser.html

Go:   // 手写 map[T]int
来源：http://hz.shangyingyoupin.top/gtzwmukzvq.html

Ruby: arr.tally
来源：http://hz.ybcxt.top/gtwzqzfaot.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shuidangran.top/gtmfeelhfd.html

[D21] 判断是否包含某元素
来源：http://hz.c1oappe.top/gtuszgdiqz.html

Py:   x in arr
来源：http://hz.cdnleiting.top/gthtxzabwj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ehwqpu.com/gttozbddvg.html

JS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtwbfsgezy.html

TS:   arr.includes(x)
来源：http://hz.yj20258888.top/gtmeptlrzn.html

Java: list.contains(x)
来源：http://hz.yueranfly.top/gttuotnvvf.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258888.top/gtfwdfclsq.html

Ruby: arr.include?(x)
来源：http://hz.bjfxy.top/gtawiigdak.html

C#:   list.Contains(x)
来源：http://hz.ppjwa.cn/gttmvtdwts.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aizwys.cn/gtbehiobnh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yvedp.cn/gtpoztocjw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.andypj.xyz/gtvfjpgnsy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.havefunace.top/gttxcgexdy.html

TS:   [...arr];
来源：http://hz.kuanghao11.cn/gteypaxmim.html

Java: new ArrayList<>(list);
来源：http://hz.dashuyun.cn/gtwlxtbryp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgfzy.top/gtaqbemxsz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pycfn.com/gthnzicrzn.html

C#:   new List<int>(list);
来源：http://hz.chenzaomai.com/gtescvldra.html

[D23] reduce 累积计算
来源：http://hz.zhongyouzk.top/gtnjcwsrgp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nanxinkj.top/gtcyditezm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenlongwang.top/gtwazhtbfl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gtnqmvlszd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtzpllmviy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.meibo888.top/gtsyfyfhpz.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtaqmyghod.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yj20258888.top/gtwvedfjhc.html


<!-- 参考信息 -->