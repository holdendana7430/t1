代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinqigfzy.top/gtmugxfdzo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenjidiqi.icu/gtzsgsstfw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinyuanbaomall.cn/gtglxrqnng.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.bjfxy.top/gtwnskzjic.html

[C10] 变量作用域
来源：http://hz.redwolf501.top/gtjebnenez.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhiwuduotai.top/gtnbsczble.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.0kj1m.cn/gtvpqmzwzt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ehwqpu.com/gtjtpjpldi.html

TS:   同 JS
来源：http://hz.mhx1999.top/gtztviuzqj.html

Java: 方法内为块级作用域
来源：http://hz.zhijiandao.cn/gtcrswvnjm.html

Go:   花括号块级作用域
来源：http://hz.ybcxt.top/gtjntuhmwl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ivvv.top/gtuuufetaq.html

C#:   块级作用域
来源：http://hz.yanxiufei.cn/gtsbtmsjny.html

[C11] 模块导入与导出
来源：http://hz.ppjwa.cn/gtkcdbwmmi.html

Py:   from module import func
来源：http://hz.nanxuanxn.top/gtlnirbelj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinyuanbaomall.cn/gtpnqmpcmc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xuetiantiany.cn/gtkqlkdlof.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sufxvd.cn/gtgtduelve.html

Java: import java.util.List;
来源：http://hz.fzhhl.top/gtndzuptdd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xziqi.cn/gtbkxlzknl.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jyoumei.cn/gtqflpmqom.html

C#:   using System.Text;
来源：http://hz.sufxvd.cn/gtakkvpajr.html

[C12] 立即执行函数 IIFE
来源：http://hz.yongpay.top/gtmoskdbwa.html

Py:   (lambda: print("run"))()
来源：http://hz.sxryk.cn/gtvfkbwoay.html

PHP:  (function () { echo "run"; })();
来源：http://hz.gaohongyu789.top/gtyiqoojuj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinyuanbaomall.cn/gtfrffcipg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gtswyuqnzw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.pengpengdd.cyou/gtnrzmvfej.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.smart0.xyz/gtmzaxlium.html

Ruby: -> { puts "run" }.call
来源：http://hz.jiagoushi.top/gtflrffnod.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sweek.top/gtqxqotemc.html

[C13] 类型声明 / 类型注解
来源：http://hz.hywenlv.cn/gtkczchokk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinyuanbaomall.cn/gtvqipgdpe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtfnffgksy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.9152youxi.cn/gtcmiebuwg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pengpengdd.cyou/gtzydtpqxp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtongqfbug.html

Go:   func add(a, b int) int
来源：http://hz.havefunace.top/gtncqihtmq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cqqwz.cn/gtwxssnasu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.birdmap.top/gtevxcbpns.html

[C14] 泛型函数
来源：http://hz.gaohongyu789.top/gtzumwbsjh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.316326.xyz/gtchqndumj.html

PHP:  // 无泛型
来源：http://hz.zhijiandao.cn/gtnyelyonc.html

JS:   // 无泛型
来源：http://hz.tianlin.xyz/gtefmvzshv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xylfe.cn/gtvnegkjfe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cqqwz.cn/gtozwwlpej.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yonumen.top/gtiablcudu.html

Ruby: # 无泛型
来源：http://hz.jqgfzy.top/gtfgvogfyj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.nwbrower.top/gtfbwwvopm.html

[C15] 解构 / 展开参数
来源：http://hz.chenzaomai.com/gtehjhloop.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sxryk.cn/gteuqjqyzm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.wangdashe.top/gtluihvveo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.havefunace.top/gtrhpjiolf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ydzc1.top/gtjutnsnrs.html

Java: // 无解构
来源：http://hz.nwbrower.top/gtiesysroz.html

Go:   // 无解构
来源：http://hz.svipenyu.cn/gtjeibcyzf.html

Ruby: a, b = pair
来源：http://hz.xziqi.cn/gtklaoodnd.html

C#:   var (a, b) = pair;
来源：http://hz.jinghuilouyu.cn/gtyxlkkncs.html

[C16] 函数 / 方法重载
来源：http://hz.shanyushiyangtech.top/gtzcivyxxx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhengqikj.top/gtrhevhjtv.html

PHP:  // 无重载
来源：http://hz.tanke756.top/gtxqsilgll.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.redwolf501.top/gtchkqgoui.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nwbrower.top/gthugbmfnu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.wangshuangyany.cn/gttltwoczc.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtfilgoaix.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shangyingyoupin.top/gtzqmuwqlc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenlongwang.top/gtveeojbgf.html

================================================================================
来源：http://hz.gogol.net.cn/gtunuupieu.html

D. 数组 / 列表 / 集合
来源：http://hz.ydjk.org.cn/gtkchsknrk.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtopjllwvr.html

[D01] 创建数组 / 列表
来源：http://hz.shzxlz.cn/gtwsypszuu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hywenlv.cn/gtcnzdnlnn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.mhx1999.top/gtdkaqwljd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.guannengcc.top/gtkmgefghy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ppjwa.cn/gthbqyzrvp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxuanxn.top/gtaqjknnyo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gogol.net.cn/gtaqyquevu.html

Ruby: arr = [1, 2, 3]
来源：http://hz.guowangkeji.top/gtbedbsnfi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhixingplan.top/gtznqqjrqs.html

[D02] 追加元素到末尾
来源：http://hz.hammf.cn/gtqtgaucqp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cashguo.top/gtzvsrcmmt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yangfankeji.com/gtwxsvmtph.html

JS:   arr.push(4);
来源：http://hz.chenjidiqi.icu/gteghglwsv.html

TS:   arr.push(4);
来源：http://hz.haohaochexian.top/gtyvatzspy.html

Java: list.add(4);
来源：http://hz.gaohongyu789.top/gtxnyoujkd.html

Go:   arr = append(arr, 4)
来源：http://hz.ppjwa.cn/gtzzzmwgad.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yonumen.top/gtekheknvi.html

C#:   list.Add(4);
来源：http://hz.jyoumei.cn/gtioxqzzsr.html

[D03] 在指定位置插入元素
来源：http://hz.yangfankeji.com/gtqbldqwqz.html

Py:   arr.insert(0, 0)
来源：http://hz.havefunace.top/gtcgwreuxy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.haohaochexian.top/gtqzcyhhzd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xziqi.cn/gteynngcjs.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jqgufenzy.top/gtsogpnofd.html

Java: list.add(0, 0);
来源：http://hz.yuanzhike.top/gtaebqthyp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.haohaochexian.top/gticttofpu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ivvv.top/gtknrlaidb.html

C#:   list.Insert(0, 0);
来源：http://hz.zhoulong.xyz/gtozentaxl.html

[D04] 删除元素
来源：http://hz.sweek.top/gtrkezqhop.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.andypj.xyz/gtlxfuvaoq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnxiangtu.top/gtxffthtil.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.wangshuangyany.cn/gtzzuvqpey.html

TS:   arr.splice(0, 1);
来源：http://hz.pycfn.com/gtggbrilxs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xziqi.cn/gtxmsmxflc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hfpthk.cn/gtphybxjss.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.pycfn.com/gtlibprjov.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xinyue.icu/gtqamhhovv.html

[D05] 访问与修改元素
来源：http://hz.birdmap.top/gtofkgtrgc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gtxboeeaeb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yuanzhike.top/gtsyfcxwdf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhengqikj.top/gtnvkxbmus.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangtech.top/gtljidazxb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aibaodan.cn/gtehczskac.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yueranfly.top/gtoxleslct.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtitppookr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aizwys.cn/gtsqpfqmpv.html

[D06] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtgfekoenx.html

Py:   len(arr)
来源：http://hz.havefunace.top/gtwunuosdw.html

PHP:  count($arr);
来源：http://hz.redwolf501.top/gtmwbepmmx.html

JS:   arr.length
来源：http://hz.smart0.xyz/gtsqbgioog.html

TS:   arr.length
来源：http://hz.aizwys.cn/gtaazfxyag.html

Java: list.size();
来源：http://hz.yj20258888.top/gtnsgacori.html

Go:   len(arr)
来源：http://hz.ivvv.top/gtzwoipqch.html

Ruby: arr.length; arr.size
来源：http://hz.guannengcc.top/gtejnwcnth.html

C#:   list.Count;
来源：http://hz.redwolf501.top/gtddzxzrhw.html

[D07] 切片 / 取子数组
来源：http://hz.dianchejie.cn/gtdxbpqnsr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhixingplan.top/gtexvqiiio.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.andypj.xyz/gtzugtiybt.html

JS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtpcynuzut.html

TS:   arr.slice(1, 4);
来源：http://hz.wangdashe.top/gtniegyvhc.html

Java: list.subList(1, 4);
来源：http://hz.hywenlv.cn/gtoqbsglij.html

Go:   arr[1:4]
来源：http://hz.havefunace.top/gtogmganlc.html

Ruby: arr[1, 3]
来源：http://hz.cashguo.top/gtlzonlekq.html

C#:   list.GetRange(1, 3);
来源：http://hz.fzhhl.top/gtupqwpiba.html

[D08] 合并两个数组
来源：http://hz.daxiang520.top/gtlpmgrjnf.html

Py:   a + b;  a.extend(b)
来源：http://hz.xuanzx.com/gtixwgrnef.html

PHP:  array_merge($a, $b);
来源：http://hz.fzhhl.top/gtywbkolxw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.feifeiyinyue.top/gtssfwrbwg.html

TS:   [...a, ...b];
来源：http://hz.c1oappe.top/gtwgrsogtp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gogol.net.cn/gtpkgzdhmy.html

Go:   append(a, b...)
来源：http://hz.yj20258.top/gtcltqowcy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cqqwz.cn/gtqmfkyuya.html

C#:   a.Concat(b).ToList()
来源：http://hz.ydzc1.top/gtbhbmgici.html

[D09] 排序（升序）
来源：http://hz.guowangkeji.top/gtsmiafyel.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gttsejehqb.html

PHP:  sort($arr);
来源：http://hz.mhx1999.top/gtfycwwksl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxinkj.top/gtfmivqgdc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.snrcjt.cn/gtggjbkhee.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sxryk.cn/gtovlfqirr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.feifeiyinyue.top/gtlxhnujbw.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gtrysguwdk.html

C#:   list.Sort();
来源：http://hz.vqdsnc.cn/gtxbxruzxd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.iojbl.cn/gtfvgzwscx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shanyushiyangtech.top/gtmqfvqhlg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtpbtngukm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hfpthk.cn/gtymgsfwpy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cucudq.cn/gtixljfghj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shzxlz.cn/gtrfhbchjq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydjk.org.cn/gtpjubbtkh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.snrcjt.cn/gtlskulnli.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tianlin.xyz/gtpbnxtfcv.html

[D11] 反转数组
来源：http://hz.yj20258888.top/gtllanzzwl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hammf.cn/gtvvkhqgiw.html

PHP:  array_reverse($arr);
来源：http://hz.yonumen.top/gtctugusoy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yueranfly.top/gtfzajquox.html

TS:   [...arr].reverse();
来源：http://hz.yangfankeji.com/gtiioxusms.html

Java: Collections.reverse(list);
来源：http://hz.guowangkeji.top/gtoxtjuegd.html

Go:   slices.Reverse(arr)
来源：http://hz.wangdashe.top/gtgagnmwbw.html

Ruby: arr.reverse
来源：http://hz.guannengcc.top/gtitjwihkx.html

C#:   list.Reverse();
来源：http://hz.316326.xyz/gtwmaryclr.html

[D12] 查找元素下标
来源：http://hz.52xcode.cn/gtiypfvxca.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhixingplan.top/gtprfmklak.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hongshengwenyu.top/gtdkwfqxai.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zycfv.cn/gtccugqugh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ehwqpu.com/gtlptzzxwv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.aibaodan.cn/gtjieriyzx.html

Go:   slices.Index(arr, x)
来源：http://hz.svipenyu.cn/gtzancydvt.html

Ruby: arr.index(x)
来源：http://hz.jianghu66.top/gtifkzevoo.html

C#:   list.IndexOf(x);
来源：http://hz.snrcjt.cn/gtzpcmjcuw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.vqdsnc.cn/gtrropggsp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cqqwz.cn/gtmkqodqmf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ivvv.top/gtksqkblqw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.c1oappe.top/gtzmrdgxmz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sweek.top/gtcjplqraf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258.top/gtumtilzbf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhaomingkeji.xyz/gtszvwbrrw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.bjfxy.top/gtebmusdni.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daxiang520.top/gtbnzyozcu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shzxlz.cn/gtbfunhozm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.svipenyu.cn/gtlawdscvl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tian-w.cn/gtopkonyvq.html

JS:   arr.map(x => x * 2)
来源：http://hz.cheryme.top/gtfxeqpnkz.html

TS:   arr.map(x => x * 2)
来源：http://hz.yangfankeji.com/gtjqadjola.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shangyingyoupin.top/gtanagkahu.html

Go:   // 手写循环
来源：http://hz.nwbrower.top/gtzpgdewxj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shanyushiyangtech.top/gtvwpvgcqy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xinyue.icu/gtinrvaxav.html

[D15] 去重
来源：http://hz.hywenlv.cn/gtohivvkxp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.316326.xyz/gtpjjsqbrv.html

PHP:  array_unique($arr);
来源：http://hz.ehwqpu.com/gtjndlxlas.html

JS:   [...new Set(arr)]
来源：http://hz.zhengqikj.top/gtqgxiwedi.html

TS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtpdxnhnpo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sufxvd.cn/gtxqhxpupl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinqigufen.top/gtkojlcois.html

Ruby: arr.uniq
来源：http://hz.zhongyouzk.top/gtdsqyfulr.html

C#:   list.Distinct().ToList()
来源：http://hz.xuanzx.com/gtqjailzln.html

[D16] 求和与平均值
来源：http://hz.guannengcc.top/gtwzzkbkcf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nwbrower.top/gtlguozoaf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sufxvd.cn/gtveaasnbj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jianghu66.top/gtjqqtknnk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gtghmwbxgs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cqqwz.cn/gtefvvfnjt.html

Go:   // 手写循环累加
来源：http://hz.cucudq.cn/gtmmdyyadn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yvedp.cn/gtiigybgbg.html

C#:   list.Sum();  list.Average()
来源：http://hz.yangfankeji.com/gtdmjdkbrh.html

[D17] 最大值与最小值
来源：http://hz.yueranfly.top/gtgxsajxbf.html

Py:   max(arr);  min(arr)
来源：http://hz.yongpay.top/gtwsumqfmt.html

PHP:  max($arr);  min($arr);
来源：http://hz.redwolf501.top/gtdzzskhxz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dashuyun.cn/gtmnigbcot.html

TS:   Math.max(...arr);
来源：http://hz.xylfe.cn/gtbzphhqcb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cdnleiting.top/gtjehepygg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tanke756.top/gtpaziqfnd.html

Ruby: arr.max;  arr.min
来源：http://hz.nwbrower.top/gtbqongfzw.html

C#:   list.Max();  list.Min()
来源：http://hz.cucudq.cn/gtiqfqkrsq.html

[D18] 扁平化嵌套数组
来源：http://hz.gogol.net.cn/gtieptdfcp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxuanxn.top/gtfhgaftjl.html

PHP:  array_merge(...$nested);
来源：http://hz.cashguo.top/gtgdcwmfiy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.vqdsnc.cn/gthxwodtbx.html

TS:   nested.flat();
来源：http://hz.birdmap.top/gtmftmnryh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xinyue.icu/gthlywacgf.html

Go:   // 手写双层循环
来源：http://hz.havefunace.top/gtfnztzexn.html

Ruby: nested.flatten
来源：http://hz.wangshuangyany.cn/gtsybfpedd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhaomingkeji.xyz/gtuqytldhx.html

[D19] 按字段分组
来源：http://hz.cucudq.cn/gtgmzrohoc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ivvv.top/gtutssrhdi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sweek.top/gtaceumuyu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinghuilouyu.cn/gtlauzarup.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.vqdsnc.cn/gthsjdsxat.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nwbrower.top/gtnhwzxuaf.html

Go:   // 手写 map[string][]T
来源：http://hz.kuanghao11.cn/gtnggfbluh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aibaodan.cn/gtswhyjsml.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhoulong.xyz/gtjipfqvuo.html

[D20] 统计每个元素出现次数
来源：http://hz.sweek.top/gttnkdkxon.html

Py:   Counter(arr)
来源：http://hz.yuanzhike.top/gtnkbclwcj.html

PHP:  array_count_values($arr);
来源：http://hz.wangshuangyany.cn/gtpvdpklts.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hfpthk.cn/gtpwxztcdp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinyuanbaomall.cn/gtohtuntyo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinghuilouyu.cn/gtzteubyvt.html

Go:   // 手写 map[T]int
来源：http://hz.chenzaomai.com/gtlgffmgov.html

Ruby: arr.tally
来源：http://hz.chenlongwang.top/gtolqfedea.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cqqwz.cn/gtjfkfayfj.html

[D21] 判断是否包含某元素
来源：http://hz.cqqwz.cn/gtjneblgki.html

Py:   x in arr
来源：http://hz.ehwqpu.com/gtjjiktahw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gtsnwtehsj.html

JS:   arr.includes(x)
来源：http://hz.cashguo.top/gtrjiryvoy.html

TS:   arr.includes(x)
来源：http://hz.xinyue.icu/gtacbfzplp.html

Java: list.contains(x)
来源：http://hz.jlsjyb.cn/gtouxpdjcr.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuxming.cn/gtkelwlvyo.html

Ruby: arr.include?(x)
来源：http://hz.zhongyouzk.top/gtroqcjwbz.html

C#:   list.Contains(x)
来源：http://hz.shzxlz.cn/gtjuqowurn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sxryk.cn/gtoixvoaok.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.vqdsnc.cn/gtkdgzjhbh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinqigfzy.top/gtqmltujfq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenzaomai.com/gtsslcczqq.html

TS:   [...arr];
来源：http://hz.chenzaomai.com/gtdytrciiz.html

Java: new ArrayList<>(list);
来源：http://hz.hywenlv.cn/gtwfwnkeol.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.bjfxy.top/gtkdubfxta.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ybcxt.top/gtirmiqjbr.html

C#:   new List<int>(list);
来源：http://hz.cdnleiting.top/gtgmekowxr.html

[D23] reduce 累积计算
来源：http://hz.zhaomingkeji.xyz/gtymjkpuom.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ywan-chungtsiang.top/gtwenttlvj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.0kj1m.cn/gtpuoeyiwb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tianlin.xyz/gtphurpvda.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daria6918.cn/gterqqdqqv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.c1oappe.top/gtithnbsun.html

Go:   // 手写循环
来源：http://hz.hfpthk.cn/gtfrqmfmux.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yonumen.top/gtrgtzrvsl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shanyushiyangkeji.top/gtgzohkqwt.html

[D24] 字典 / Map 基本操作
来源：http://hz.jiagoushi.top/gtleibwmrg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.mhx1999.top/gtrxppwtsd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenjidiqi.icu/gtwbxnuiqf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hywenlv.cn/gteethbsbo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sufxvd.cn/gtqivtdilk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhixingplan.top/gtqxxgxjap.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.chenlongwang.top/gtwpuiajzl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hysaishi.cn/gtfncvsmxe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jianghu66.top/gtpipiwmfu.html

[D25] Set 集合去重与交并差
来源：http://hz.jyoumei.cn/gtmxqunsdr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhoulong.xyz/gtsivaheof.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhiwuduotai.top/gtitksjdpx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuxming.cn/gtyapdppsg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.316326.xyz/gthoymikir.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yangfankeji.com/gttzzfoacr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxuanxn.top/gtickvlddz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.vqdsnc.cn/gtxxvycxoa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.redwolf501.top/gtmglnnfxn.html

[D26] 数组转字符串
来源：http://hz.jiagoushi.top/gtzldllvpk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xingfuxueyuan.xyz/gtvinyegko.html

PHP:  implode(", ", $arr);
来源：http://hz.wangdashe.top/gtwgfffrjy.html

JS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtqidpsjlq.html

TS:   arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtexngumji.html


<!-- 参考信息 -->