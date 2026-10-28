代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://hz.yongpay.top/gtleesqzzl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yongpay.top/gtevhppppc.html

[C08] 闭包
来源：http://hz.yj20258.top/gtemlhgdoj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hnqzz.top/gtpxwaqwgl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.0kj1m.cn/gtlqnpqnqw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.meibo888.top/gtnhsgbrnx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aizwys.cn/gtfvefeikt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhengqikj.top/gtmxxmmbff.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xuanzx.com/gtwgaretfe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zycfv.cn/gtazyvnbza.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtteizvlxm.html

[C09] 递归
来源：http://hz.ywan-chungtsiang.top/gtpuivkgfh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xuetiantiany.cn/gtmgavpznl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhongyouzk.top/gtptmlplia.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gtvxwrrevd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.c1oappe.top/gttryuknct.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnqzz.top/gtdnoyryki.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cqqwz.cn/gtziaegtky.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shangyingyoupin.top/gtmrnwejyb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.haohaochexian.top/gtnzpoztos.html

[C10] 变量作用域
来源：http://hz.yj20258.top/gtvhhxpdbe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xingfuxueyuan.xyz/gtnuetxqyo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yangfankeji.com/gtszopywys.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydjk.org.cn/gtbflmkciz.html

TS:   同 JS
来源：http://hz.shanyushiyangtech.top/gtqwvkwrib.html

Java: 方法内为块级作用域
来源：http://hz.wangdashe.top/gtkxuqulsm.html

Go:   花括号块级作用域
来源：http://hz.meibo888.top/gtivvzhnwl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hnqzz.top/gtjkliandi.html

C#:   块级作用域
来源：http://hz.ppjwa.cn/gtdhkjplty.html

[C11] 模块导入与导出
来源：http://hz.yueranfly.top/gtbplcqoow.html

Py:   from module import func
来源：http://hz.9152youxi.cn/gtrwkzpscz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jianghu66.top/gtehxmvuxm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtbwirljdr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shangyingyoupin.top/gtkfaqgzec.html

Java: import java.util.List;
来源：http://hz.hammf.cn/gtlrwwhykl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ivvv.top/gthcvylfnu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sweek.top/gtrfwlhpul.html

C#:   using System.Text;
来源：http://hz.jlsjyb.cn/gtmwkdoiip.html

[C12] 立即执行函数 IIFE
来源：http://hz.tian-w.cn/gtjnrpffyr.html

Py:   (lambda: print("run"))()
来源：http://hz.tianlin.xyz/gtljeuzofo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.redwolf501.top/gtpfadudaz.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yvedp.cn/gtepzdoqco.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ydzc1.top/gtkzirtrvd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.guowangkeji.top/gtmacwgwwk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.redwolf501.top/gtufuqhhuo.html

Ruby: -> { puts "run" }.call
来源：http://hz.gotoacloud.top/gtbyibkucm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pycfn.com/gtqqjrgqhb.html

[C13] 类型声明 / 类型注解
来源：http://hz.shanyushiyangtech.top/gtkselyomx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.0kj1m.cn/gtukndccsm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtnzommpsv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xziqi.cn/gtwasmwuys.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtyuypfldi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtllubwoxk.html

Go:   func add(a, b int) int
来源：http://hz.xinyue.icu/gtmuuuzsar.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sxryk.cn/gtcwppvpzg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.tianlin.xyz/gtsnouwqay.html

[C14] 泛型函数
来源：http://hz.hnxiangtu.top/gtwpcxooph.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xylfe.cn/gtpujtqmmj.html

PHP:  // 无泛型
来源：http://hz.yonumen.top/gtztaqiokj.html

JS:   // 无泛型
来源：http://hz.birdmap.top/gtblhwuyzz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shanyushiyangkeji.top/gtjpgglffv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigfzy.top/gtjowbeyxq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.smart0.xyz/gtoxgypadq.html

Ruby: # 无泛型
来源：http://hz.zhijiandao.cn/gtnlexhslc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tian-w.cn/gtjaikxzxe.html

[C15] 解构 / 展开参数
来源：http://hz.yj202588.top/gtrtrytkxs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sxryk.cn/gtmapuuuol.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shanyushiyangtech.top/gtukekrwlq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cheryme.top/gtwpbcvdxj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cheryme.top/gtylydwyoy.html

Java: // 无解构
来源：http://hz.nwbrower.top/gtjfqynwal.html

Go:   // 无解构
来源：http://hz.fzhhl.top/gtllgbtxbr.html

Ruby: a, b = pair
来源：http://hz.ydzc1.top/gtdcjgeggr.html

C#:   var (a, b) = pair;
来源：http://hz.xuetiantiany.cn/gtmmfkiple.html

[C16] 函数 / 方法重载
来源：http://hz.gogol.net.cn/gtsbzebfdh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hongshengwenyu.top/gtkztlehst.html

PHP:  // 无重载
来源：http://hz.yuanzhike.top/gtvgbemwai.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ywan-chungtsiang.top/gtfdazrikb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jlsjyb.cn/gtemcmtjsk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xinyue.icu/gtrjqndiam.html

Go:   // 无重载：用不同函数名
来源：http://hz.dianchejie.cn/gteintvibi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.redwolf501.top/gtrczdzsip.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yonumen.top/gtoyudaqgs.html

================================================================================
来源：http://hz.sxryk.cn/gtilkfbsyv.html

D. 数组 / 列表 / 集合
来源：http://hz.yuanzhike.top/gtiricbufp.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtfjigdyro.html

[D01] 创建数组 / 列表
来源：http://hz.guowangkeji.top/gtagarorka.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xylfe.cn/gtwyrqhocd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuanzhike.top/gttnnpaaxp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.aizwys.cn/gtcjhrqvby.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinghuilouyu.cn/gtbsakxaso.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ywan-chungtsiang.top/gthicltluu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenlongwang.top/gtipvhfnko.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj20258888.top/gtbfvfbyol.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258888.top/gttespopsg.html

[D02] 追加元素到末尾
来源：http://hz.ehwqpu.com/gtbgbhvfms.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.9152youxi.cn/gtdqmsdpqa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hnqzz.top/gtxifvowqn.html

JS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtfgnfjfog.html

TS:   arr.push(4);
来源：http://hz.ydjk.org.cn/gtsffyutxc.html

Java: list.add(4);
来源：http://hz.yj20258.top/gtvvsxswts.html

Go:   arr = append(arr, 4)
来源：http://hz.gzhubu.top/gtenjluncy.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zycfv.cn/gtxotfmjoh.html

C#:   list.Add(4);
来源：http://hz.jqgufenzy.top/gtecgirifo.html

[D03] 在指定位置插入元素
来源：http://hz.jqgfzy.top/gtprszmfqx.html

Py:   arr.insert(0, 0)
来源：http://hz.xuetiantiany.cn/gtnqysklzo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guowangkeji.top/gtiymhoaqh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yanxiufei.cn/gtoptdpzvr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.pengpengdd.cyou/gthxildyqn.html

Java: list.add(0, 0);
来源：http://hz.cdnleiting.top/gtkmxyannk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shuidangran.top/gttznnyoih.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj20258.top/gtrhiyikoo.html

C#:   list.Insert(0, 0);
来源：http://hz.sweek.top/gtqondbali.html

[D04] 删除元素
来源：http://hz.aizwys.cn/gtlbavdhkw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jiagoushi.top/gtkkcdlsvw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shuidangran.top/gtugkzgsia.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yj20258888.top/gtcjmzmttu.html

TS:   arr.splice(0, 1);
来源：http://hz.chenzaomai.com/gtxziechpa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cucudq.cn/gtvqgjthan.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.52xcode.cn/gtiyiicbdf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.haohaochexian.top/gtussksgfx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cheryme.top/gtxhkqgcox.html

[D05] 访问与修改元素
来源：http://hz.yueranfly.top/gtasvqjzoo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtbasaxswu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shangyingyoupin.top/gtdgifhmhc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ybcxt.top/gtdjdknahb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gogol.net.cn/gthkvvkmjp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guowangkeji.top/gtrtcwnxvb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.meibo888.top/gthtaahjco.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gtgvvpxbuj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.redwolf501.top/gtluoudwmp.html

[D06] 数组长度
来源：http://hz.jiagoushi.top/gtbxlcqbmx.html

Py:   len(arr)
来源：http://hz.zhixingplan.top/gtnexyouhh.html

PHP:  count($arr);
来源：http://hz.ydjk.org.cn/gtlgvyhpil.html

JS:   arr.length
来源：http://hz.yj20258.top/gtpalsutmj.html

TS:   arr.length
来源：http://hz.smart0.xyz/gthykrzekn.html

Java: list.size();
来源：http://hz.9152youxi.cn/gtmqhvwcyp.html

Go:   len(arr)
来源：http://hz.yueranfly.top/gtgbetgvhy.html

Ruby: arr.length; arr.size
来源：http://hz.hnxiangtu.top/gtxzhcywtq.html

C#:   list.Count;
来源：http://hz.shzxlz.cn/gtygqhqsej.html

[D07] 切片 / 取子数组
来源：http://hz.jqgufenzy.top/gtijwzsgsh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.daxiang520.top/gtigwgdash.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tian-w.cn/gtchccbwgd.html

JS:   arr.slice(1, 4);
来源：http://hz.316326.xyz/gtowiphaif.html

TS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtfdhgfbkj.html

Java: list.subList(1, 4);
来源：http://hz.gogol.net.cn/gtsnfwvruq.html

Go:   arr[1:4]
来源：http://hz.nanxuanxn.top/gtlbfqdaos.html

Ruby: arr[1, 3]
来源：http://hz.iojbl.cn/gtnapkzzgx.html

C#:   list.GetRange(1, 3);
来源：http://hz.cheryme.top/gtykmndpel.html

[D08] 合并两个数组
来源：http://hz.feifeiyinyue.top/gtlsbjixyc.html

Py:   a + b;  a.extend(b)
来源：http://hz.shzxlz.cn/gtvwglbhnk.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258.top/gtuhgvldyp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhaomingkeji.xyz/gtfjngglhp.html

TS:   [...a, ...b];
来源：http://hz.zhiwuduotai.top/gtmqritxhb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tanke756.top/gtvcoebhyv.html

Go:   append(a, b...)
来源：http://hz.9152youxi.cn/gtahbkoazn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sxryk.cn/gtguueirqi.html

C#:   a.Concat(b).ToList()
来源：http://hz.0kj1m.cn/gtzollaqqt.html

[D09] 排序（升序）
来源：http://hz.jiagoushi.top/gtielxouey.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtiqgjfejc.html

PHP:  sort($arr);
来源：http://hz.tanke756.top/gtaezzdswi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.havefunace.top/gthjrwsavc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aizwys.cn/gthvbsofiq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinghuilouyu.cn/gtnlwtzrnf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shuidangran.top/gtvevkadsf.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gtuasflibx.html

C#:   list.Sort();
来源：http://hz.fzhhl.top/gtrawlwyez.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenjidiqi.icu/gtzsudkmws.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gotoacloud.top/gteflqfyhb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.shzxlz.cn/gtzhotucnt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangkeji.top/gtdkecutir.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fengsongda.top/gtaqnmreiz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.quarkkingdee.top/gtrvndrdrj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tanke756.top/gtezjbxqhh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.fzhhl.top/gtnohthbng.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cqqwz.cn/gtnfolsfga.html

[D11] 反转数组
来源：http://hz.sufxvd.cn/gtuffwjzjj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cdnleiting.top/gtelepuwkj.html

PHP:  array_reverse($arr);
来源：http://hz.tianlin.xyz/gtxnrijfjv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.iojbl.cn/gtejgxvafs.html

TS:   [...arr].reverse();
来源：http://hz.tianlin.xyz/gtagsketzc.html

Java: Collections.reverse(list);
来源：http://hz.jinqigfzy.top/gtlbgsfwdf.html

Go:   slices.Reverse(arr)
来源：http://hz.hfpthk.cn/gtkonortti.html

Ruby: arr.reverse
来源：http://hz.sufxvd.cn/gtlejkvilu.html

C#:   list.Reverse();
来源：http://hz.jlsjyb.cn/gtzauohrkp.html

[D12] 查找元素下标
来源：http://hz.jinqigufen.top/gtnguvzvks.html

Py:   arr.index(x);  x in arr
来源：http://hz.mhx1999.top/gturlzzuab.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.aizwys.cn/gtctonefnq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtdviaqfmn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhoulong.xyz/gtkxtmppxd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tianlin.xyz/gtdcefsvif.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtufeurvnh.html

Ruby: arr.index(x)
来源：http://hz.cdnleiting.top/gtxdmuleyx.html

C#:   list.IndexOf(x);
来源：http://hz.svipenyu.cn/gtbzaitzku.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj202588.top/gtoqitkxjh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ywan-chungtsiang.top/gtdesuevfy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinqigufen.top/gtoclfclxi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gthmtvcuia.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yj202588.top/gtoeuawtgo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.tianlin.xyz/gtuhxfjnec.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhixingplan.top/gtqisiiedp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pycfn.com/gtkicxpezr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sxryk.cn/gtommwgdtq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dianchejie.cn/gtjlqbdqkq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ehwqpu.com/gtblmfqrgo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.guowangkeji.top/gtaapiksbz.html

JS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gtzbspvpya.html

TS:   arr.map(x => x * 2)
来源：http://hz.hywenlv.cn/gtpjzdeqbd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenzaomai.com/gtuxohecwf.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gtaqeoslpe.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yangfankeji.com/gtenrigljw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgufenzy.top/gtjokuwrjv.html

[D15] 去重
来源：http://hz.aizwys.cn/gtenmqatdz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.fengsongda.top/gtfzxwjxim.html

PHP:  array_unique($arr);
来源：http://hz.jqgufenzy.top/gtxcjulsng.html

JS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtkoorocia.html

TS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtypvccxlq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuetiantiany.cn/gtjbweakho.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tanke756.top/gtmpujmhvu.html

Ruby: arr.uniq
来源：http://hz.nanxuanxn.top/gtgtmhxajl.html

C#:   list.Distinct().ToList()
来源：http://hz.jianghu66.top/gtpbvyxxjh.html

[D16] 求和与平均值
来源：http://hz.wangshuangyany.cn/gtfykgmafk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydzc1.top/gtbeuqduie.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ppjwa.cn/gtsrlbrine.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yongpay.top/gthzmhgzgt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtlzzaiqad.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.52xcode.cn/gtqwhpotsm.html

Go:   // 手写循环累加
来源：http://hz.hammf.cn/gtmfefpken.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sxryk.cn/gtucakflxj.html

C#:   list.Sum();  list.Average()
来源：http://hz.ydzc1.top/gteitqukff.html

[D17] 最大值与最小值
来源：http://hz.xinyue.icu/gtryqajxci.html

Py:   max(arr);  min(arr)
来源：http://hz.pycfn.com/gtnsotjgrf.html

PHP:  max($arr);  min($arr);
来源：http://hz.aizwys.cn/gtdsdntzop.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cashguo.top/gtxpvrpirx.html

TS:   Math.max(...arr);
来源：http://hz.cqqwz.cn/gtxbbxmlnd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shzxlz.cn/gtqoiyrxoq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xziqi.cn/gtrdhnzxgt.html

Ruby: arr.max;  arr.min
来源：http://hz.guannengcc.top/gtnbdyyehb.html

C#:   list.Max();  list.Min()
来源：http://hz.shuidangran.top/gtvpxmxswv.html

[D18] 扁平化嵌套数组
来源：http://hz.aibaodan.cn/gtrsyvwlxf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shanyushiyangtech.top/gtkdypdlev.html

PHP:  array_merge(...$nested);
来源：http://hz.jyoumei.cn/gtfxqqfdys.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj20258888.top/gtfqqapbsn.html

TS:   nested.flat();
来源：http://hz.jyoumei.cn/gtopwlkkis.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ywan-chungtsiang.top/gtwgpkttxt.html

Go:   // 手写双层循环
来源：http://hz.gotoacloud.top/gtgiagfbhc.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtxlmkneco.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.svipenyu.cn/gtwuttybut.html

[D19] 按字段分组
来源：http://hz.chenzaomai.com/gtgbhdthkt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aizwys.cn/gtrmrnjpiy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenlongwang.top/gtgmolhcqc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ybcxt.top/gtfqpgfepz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cheryme.top/gtpckicgoz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gotoacloud.top/gtdulhobvb.html

Go:   // 手写 map[string][]T
来源：http://hz.havefunace.top/gtzddxgwja.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhijiandao.cn/gtsszapknn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hfpthk.cn/gtclvcqxqr.html

[D20] 统计每个元素出现次数
来源：http://hz.hnxiangtu.top/gtutsjmjpb.html

Py:   Counter(arr)
来源：http://hz.yangfankeji.com/gtubcgrkge.html

PHP:  array_count_values($arr);
来源：http://hz.fengsongda.top/gtpwokypst.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gtmwuqpsxv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gthqephges.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.redwolf501.top/gtgvedpzqb.html

Go:   // 手写 map[T]int
来源：http://hz.hfpthk.cn/gtxzeuttiv.html

Ruby: arr.tally
来源：http://hz.hnqzz.top/gtrogkudow.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yangfankeji.com/gtpfadqdzx.html

[D21] 判断是否包含某元素
来源：http://hz.mhx1999.top/gtvtgbljha.html

Py:   x in arr
来源：http://hz.yonumen.top/gtneqyjask.html

PHP:  in_array($x, $arr, true);
来源：http://hz.havefunace.top/gtjwezmcug.html

JS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gtxjhopotn.html

TS:   arr.includes(x)
来源：http://hz.cdnleiting.top/gtawwraoqv.html

Java: list.contains(x)
来源：http://hz.xuetiantiany.cn/gtbuniiztn.html

Go:   slices.Contains(arr, x)
来源：http://hz.cdnleiting.top/gtfccdmbmj.html

Ruby: arr.include?(x)
来源：http://hz.yueranfly.top/gtjnnemhhk.html

C#:   list.Contains(x)
来源：http://hz.tian-w.cn/gtlaefckdm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.svipenyu.cn/gtnjjxiizf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinyuanbaomall.cn/gtietnghnr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cheryme.top/gtdyogzsad.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.guowangkeji.top/gtuojubgkk.html

TS:   [...arr];
来源：http://hz.hnxiangtu.top/gtzlinnvoi.html

Java: new ArrayList<>(list);
来源：http://hz.kuanghao11.cn/gtkskhjoix.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangtech.top/gtuebrsvgl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yongpay.top/gtbvwyhyjv.html

C#:   new List<int>(list);
来源：http://hz.aizwys.cn/gtqjdxlwrp.html

[D23] reduce 累积计算
来源：http://hz.dashuyun.cn/gtaeymxfrz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shanyushiyangtech.top/gtwpvnbszc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtryunxjnk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangtech.top/gtjcjdgcbq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangkeji.top/gttvbtkgip.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.kuanghao11.cn/gtpwxfeetf.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtuzkxswnc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuetiantiany.cn/gtzlgngzzw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tianlin.xyz/gtebmjssun.html

[D24] 字典 / Map 基本操作
来源：http://hz.wangdashe.top/gtgbiwyqfa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuanzx.com/gteweddgzl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.guowangkeji.top/gtfsfrrfzp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yvedp.cn/gtjnqoebey.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuetiantiany.cn/gtxnbwldnz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ehwqpu.com/gtrkbdusjp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cdnleiting.top/gtmrwmdcke.html


<!-- 参考信息 -->