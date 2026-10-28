代发 wailian999

C#:   块级作用域
来源：http://hz.jyoumei.cn/gtqnskvxbx.html

[C11] 模块导入与导出
来源：http://hz.redwolf501.top/gtcthgnuqn.html

Py:   from module import func
来源：http://hz.0kj1m.cn/gtcaigcebe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.9152youxi.cn/gtiaxaodph.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ybcxt.top/gtyowbibkm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.andypj.xyz/gtgzvurntw.html

Java: import java.util.List;
来源：http://hz.feifeiyinyue.top/gtmiraibcu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ybcxt.top/gtepbsogyw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xuanzx.com/gtarweesai.html

C#:   using System.Text;
来源：http://hz.sufxvd.cn/gthrbrazey.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhoulong.xyz/gtbfnmiwhh.html

Py:   (lambda: print("run"))()
来源：http://hz.xylfe.cn/gtbxhiysdg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.aibaodan.cn/gtuzpylpqb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hysaishi.cn/gtonuzfnwd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtkkmgwxee.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cucudq.cn/gtqrrcuspc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydjk.org.cn/gtflmkctts.html

Ruby: -> { puts "run" }.call
来源：http://hz.mhx1999.top/gtttwwxqjw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hnxiangtu.top/gtvsbknpry.html

[C13] 类型声明 / 类型注解
来源：http://hz.guannengcc.top/gtfgbrtipe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shanyushiyangkeji.top/gtzsvqyuaj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtrczvdgla.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cashguo.top/gtcbfgghxv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxinkj.top/gtmcikgppe.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yvedp.cn/gtwxitsioo.html

Go:   func add(a, b int) int
来源：http://hz.zhoulong.xyz/gtouafdacg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinyuanbaomall.cn/gtxybmmkzi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhengqikj.top/gtvasnyipi.html

[C14] 泛型函数
来源：http://hz.xinyue.icu/gtbpqsotbm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cashguo.top/gtfxlemivg.html

PHP:  // 无泛型
来源：http://hz.sysykeji.top/gtukgirkno.html

JS:   // 无泛型
来源：http://hz.nanxinkj.top/gtfrnplxrz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.quarkkingdee.top/gtjwvejook.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shuidangran.top/gteulvcrcw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhoulong.xyz/gtlvksoued.html

Ruby: # 无泛型
来源：http://hz.yongpay.top/gtpjrptkio.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinqigfzy.top/gtvlvktkyg.html

[C15] 解构 / 展开参数
来源：http://hz.ybcxt.top/gtcxerowxg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jlsjyb.cn/gtsclxjdfg.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258888.top/gtvkmwumif.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zdqjudy.top/gtflicggdk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ppjwa.cn/gtjlqnpyis.html

Java: // 无解构
来源：http://hz.nanxinkj.top/gtywuqqqmd.html

Go:   // 无解构
来源：http://hz.kuanghao11.cn/gtsbfzyzuv.html

Ruby: a, b = pair
来源：http://hz.nanxinkj.top/gtbyupvzic.html

C#:   var (a, b) = pair;
来源：http://hz.yonumen.top/gtnzqiupbl.html

[C16] 函数 / 方法重载
来源：http://hz.yj20258888.top/gtmpytangv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cashguo.top/gtmtfdijzp.html

PHP:  // 无重载
来源：http://hz.guowangkeji.top/gtwdgopopx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tanke756.top/gthjrxvmrn.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jiagoushi.top/gtstngjeri.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.fengsongda.top/gtgbgkoqda.html

Go:   // 无重载：用不同函数名
来源：http://hz.svipenyu.cn/gtdooiqarc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.svipenyu.cn/gtcekvbkyz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhongyouzk.top/gtijvypqbh.html

================================================================================
来源：http://hz.fengsongda.top/gtubcxmwvw.html

D. 数组 / 列表 / 集合
来源：http://hz.yuanzhike.top/gtympdbdnr.html

================================================================================
来源：http://hz.zhijiandao.cn/gtcknfwkkm.html

[D01] 创建数组 / 列表
来源：http://hz.jqgfzy.top/gtlwvwleca.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sufxvd.cn/gtyfrjoifc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hywenlv.cn/gttchiiqmw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.chenlongwang.top/gtpthjaibt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yuanzhike.top/gtichlufmp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hywenlv.cn/gtvjdlmiek.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.iojbl.cn/gtzvsgxzrh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.316326.xyz/gtvltsgvcc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj202588.top/gtoztywivp.html

[D02] 追加元素到末尾
来源：http://hz.jqgfzy.top/gtvqcoqqez.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hfpthk.cn/gtnhhrufjx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hysaishi.cn/gtcwjgnnnh.html

JS:   arr.push(4);
来源：http://hz.mhx1999.top/gtmxspxapi.html

TS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtwlpcfuel.html

Java: list.add(4);
来源：http://hz.zdqjudy.top/gthcsvknss.html

Go:   arr = append(arr, 4)
来源：http://hz.tian-w.cn/gtoitidicz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nanxinkj.top/gtrlpoghle.html

C#:   list.Add(4);
来源：http://hz.jinghuilouyu.cn/gtiubrsgak.html

[D03] 在指定位置插入元素
来源：http://hz.meibo888.top/gtnlyhfvpo.html

Py:   arr.insert(0, 0)
来源：http://hz.hongshengwenyu.top/gtudjggdyr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ydjk.org.cn/gtwmwlamml.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.bjfxy.top/gtfwzmlrwg.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258888.top/gtecrvogvh.html

Java: list.add(0, 0);
来源：http://hz.c1oappe.top/gtcqtpeyfr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shuidangran.top/gtizhgxdzy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sweek.top/gtudvsygma.html

C#:   list.Insert(0, 0);
来源：http://hz.xziqi.cn/gthyulzqlc.html

[D04] 删除元素
来源：http://hz.xuetiantiany.cn/gtjwvdbqsu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yj20258888.top/gtzppxqxif.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.smart0.xyz/gtzchezyzt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ybcxt.top/gtnranvrfq.html

TS:   arr.splice(0, 1);
来源：http://hz.hywenlv.cn/gtdgslmuzy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydjk.org.cn/gtiypmmnka.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgufenzy.top/gtzxgjcfqs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.bjfxy.top/gtqtyeggnj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhixingplan.top/gthekvfijs.html

[D05] 访问与修改元素
来源：http://hz.cheryme.top/gtjkvuoojh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cucudq.cn/gthqogtibc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.redwolf501.top/gtknvaohow.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.nanxuanxn.top/gtmiyxcooz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhongyouzk.top/gtkgtlgsqt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hfpthk.cn/gtrcfcymjg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtsyeqjpiz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtiobdaqbj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gogol.net.cn/gtguugwyep.html

[D06] 数组长度
来源：http://hz.zhixingplan.top/gtfjpmigii.html

Py:   len(arr)
来源：http://hz.xylfe.cn/gtdsnfcqaw.html

PHP:  count($arr);
来源：http://hz.sxryk.cn/gtnahchtyx.html

JS:   arr.length
来源：http://hz.jianghu66.top/gtbszbhung.html

TS:   arr.length
来源：http://hz.hysaishi.cn/gtmidalyts.html

Java: list.size();
来源：http://hz.jlsjyb.cn/gtopeohixn.html

Go:   len(arr)
来源：http://hz.ybcxt.top/gtechvkojz.html

Ruby: arr.length; arr.size
来源：http://hz.hammf.cn/gtaageyduw.html

C#:   list.Count;
来源：http://hz.gogol.net.cn/gtunhikrqy.html

[D07] 切片 / 取子数组
来源：http://hz.guowangkeji.top/gtztrxuxom.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sysykeji.top/gttchqfsiv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.andypj.xyz/gtjibhozqw.html

JS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtvsumvkgz.html

TS:   arr.slice(1, 4);
来源：http://hz.zhengqikj.top/gtgubhqyab.html

Java: list.subList(1, 4);
来源：http://hz.shzxlz.cn/gttjtnqzmw.html

Go:   arr[1:4]
来源：http://hz.gotoacloud.top/gthtiugcxw.html

Ruby: arr[1, 3]
来源：http://hz.xingfuxueyuan.xyz/gtdrjteqnx.html

C#:   list.GetRange(1, 3);
来源：http://hz.0kj1m.cn/gtrzktfrgu.html

[D08] 合并两个数组
来源：http://hz.xziqi.cn/gtthzgbesp.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenjidiqi.icu/gtjelomyfh.html

PHP:  array_merge($a, $b);
来源：http://hz.hammf.cn/gttuzgfzvs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.guowangkeji.top/gtjbpwbngg.html

TS:   [...a, ...b];
来源：http://hz.meibo888.top/gtwbstiftn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.0kj1m.cn/gtvppiwogt.html

Go:   append(a, b...)
来源：http://hz.hongshengwenyu.top/gtrdveuxvw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shuidangran.top/gtzxjfoxpb.html

C#:   a.Concat(b).ToList()
来源：http://hz.shangyingyoupin.top/gtihgpwmxh.html

[D09] 排序（升序）
来源：http://hz.cashguo.top/gtmaggbpna.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtuvokvmkn.html

PHP:  sort($arr);
来源：http://hz.pengpengdd.cyou/gtmqviqcov.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yj202588.top/gtzefaiowx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhongyouzk.top/gtmvsgagmb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.0kj1m.cn/gtiawfyefe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydzc1.top/gtfynuypfp.html

Ruby: arr.sort
来源：http://hz.sxryk.cn/gtmylbtfvl.html

C#:   list.Sort();
来源：http://hz.jianghu66.top/gtlrmunipd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sxryk.cn/gtucimnmri.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhaomingkeji.xyz/gtkmegxlyh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cheryme.top/gtwuuwrhev.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ywan-chungtsiang.top/gtskysvryx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.feifeiyinyue.top/gtzlvsedzj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ybcxt.top/gtfktdhkoq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenzaomai.com/gtxnuqfqmg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenzaomai.com/gtzueaaiyd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yuanzhike.top/gtkiwozsku.html

[D11] 反转数组
来源：http://hz.fzhhl.top/gtuylzzgoy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jqgfzy.top/gtdsrremfu.html

PHP:  array_reverse($arr);
来源：http://hz.xuanzx.com/gtnoiicbfv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hammf.cn/gttmvqdawa.html

TS:   [...arr].reverse();
来源：http://hz.zycfv.cn/gtlmxtgggl.html

Java: Collections.reverse(list);
来源：http://hz.cheryme.top/gtgemyvitv.html

Go:   slices.Reverse(arr)
来源：http://hz.iojbl.cn/gtfkenhpcf.html

Ruby: arr.reverse
来源：http://hz.hammf.cn/gteieauvlg.html

C#:   list.Reverse();
来源：http://hz.zdqjudy.top/gttyswsmqk.html

[D12] 查找元素下标
来源：http://hz.feifeiyinyue.top/gtafdbzbrz.html

Py:   arr.index(x);  x in arr
来源：http://hz.sysykeji.top/gtumcceaqi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gaohongyu789.top/gtmqebssuf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxuanxn.top/gttyfmzloz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gtfewtkynz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cucudq.cn/gtekzbzses.html

Go:   slices.Index(arr, x)
来源：http://hz.hongshengwenyu.top/gtegtjzdfw.html

Ruby: arr.index(x)
来源：http://hz.jqgufenzy.top/gtkpplejre.html

C#:   list.IndexOf(x);
来源：http://hz.sxryk.cn/gtuoyguicd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gotoacloud.top/gtxofnrfdf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.9152youxi.cn/gtiyimgabc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ywan-chungtsiang.top/gthdsynjtj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cqqwz.cn/gtnaeorxyw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xziqi.cn/gtbrakrols.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sweek.top/gteqgigcgz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258888.top/gtqkwejtdf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jiagoushi.top/gtlqkjsdrh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tianlin.xyz/gtndfkrhxp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tianlin.xyz/gtfdzoajkw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhaomingkeji.xyz/gtwggscwrq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gzhubu.top/gtpczcplfv.html

JS:   arr.map(x => x * 2)
来源：http://hz.yongpay.top/gtvdgebbsu.html

TS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gtnzvydtff.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.nanxinkj.top/gtxjribetd.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtzwbzwadi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.birdmap.top/gtbumcoptc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dianchejie.cn/gtbhvjyzgo.html

[D15] 去重
来源：http://hz.zycfv.cn/gtjkvbikdh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtshetxtok.html

PHP:  array_unique($arr);
来源：http://hz.jinqigufen.top/gtcsayqkno.html

JS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtvymiiqlt.html

TS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtqmzcvopv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yvedp.cn/gtowdebuej.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hnqzz.top/gtgdrtipwq.html

Ruby: arr.uniq
来源：http://hz.feifeiyinyue.top/gtlpmjvblv.html

C#:   list.Distinct().ToList()
来源：http://hz.sxryk.cn/gtjuiqtugl.html

[D16] 求和与平均值
来源：http://hz.sweek.top/gtkccylnzp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aibaodan.cn/gttajjofii.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cheryme.top/gtlyjxafye.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigfzy.top/gtbyhoojjc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gtueaqtbgt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.quarkkingdee.top/gtqqpzyhui.html

Go:   // 手写循环累加
来源：http://hz.sweek.top/gtccwotfhn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cucudq.cn/gtoegomkml.html

C#:   list.Sum();  list.Average()
来源：http://hz.ehwqpu.com/gtvyhxhebz.html

[D17] 最大值与最小值
来源：http://hz.hywenlv.cn/gtrwgyzavo.html

Py:   max(arr);  min(arr)
来源：http://hz.haohaochexian.top/gtvqeiouau.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxuanxn.top/gtvoqdbsdy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ivvv.top/gtxzxzkovg.html

TS:   Math.max(...arr);
来源：http://hz.zhijiandao.cn/gtpwpwsglc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hysaishi.cn/gtvulnnkjb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guannengcc.top/gtwwedperx.html

Ruby: arr.max;  arr.min
来源：http://hz.mhx1999.top/gtgfgwzjww.html

C#:   list.Max();  list.Min()
来源：http://hz.xinyue.icu/gtfazoqmmi.html

[D18] 扁平化嵌套数组
来源：http://hz.tian-w.cn/gtemaezqhh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhixingplan.top/gtnyuevhyl.html

PHP:  array_merge(...$nested);
来源：http://hz.shuidangran.top/gtkbqeuhrk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gaohongyu789.top/gtlodaqmkt.html

TS:   nested.flat();
来源：http://hz.jinyuanbaomall.cn/gtayaydtgz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinyuanbaomall.cn/gtjitoexry.html

Go:   // 手写双层循环
来源：http://hz.xingfuxueyuan.xyz/gtgjvkytna.html

Ruby: nested.flatten
来源：http://hz.tian-w.cn/gtedvnyxfs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.fzhhl.top/gthfgmcaxe.html

[D19] 按字段分组
来源：http://hz.9152youxi.cn/gtdamtjeqc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gzhubu.top/gtwonpzaqx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.birdmap.top/gtjhyjwbcj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hammf.cn/gtyrkmelpw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtsqxcwpap.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jianghu66.top/gtcdxomynw.html

Go:   // 手写 map[string][]T
来源：http://hz.52xcode.cn/gtjqklnvcr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aizwys.cn/gtqyjeuqqz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhijiandao.cn/gtjletcgzc.html

[D20] 统计每个元素出现次数
来源：http://hz.svipenyu.cn/gtafgxxnmj.html

Py:   Counter(arr)
来源：http://hz.yvedp.cn/gtgciairyn.html

PHP:  array_count_values($arr);
来源：http://hz.yj20258888.top/gtmqxbrjkw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gtkcpyxyrr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhiwuduotai.top/gtqgvvjjjs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.andypj.xyz/gtmxcwpghx.html

Go:   // 手写 map[T]int
来源：http://hz.jinyuanbaomall.cn/gtglqcftre.html

Ruby: arr.tally
来源：http://hz.sxryk.cn/gtidrhiskk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yuxming.cn/gtlpwhhhjp.html

[D21] 判断是否包含某元素
来源：http://hz.smart0.xyz/gtftecmkqy.html

Py:   x in arr
来源：http://hz.yvedp.cn/gtrpvejsas.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yongpay.top/gtbhpmvwll.html

JS:   arr.includes(x)
来源：http://hz.feifeiyinyue.top/gtksepenhn.html

TS:   arr.includes(x)
来源：http://hz.cheryme.top/gtcknqmelp.html

Java: list.contains(x)
来源：http://hz.zycfv.cn/gthyaqfkyn.html

Go:   slices.Contains(arr, x)
来源：http://hz.xuanzx.com/gtbyvaybvj.html

Ruby: arr.include?(x)
来源：http://hz.smart0.xyz/gthwpscmcx.html

C#:   list.Contains(x)
来源：http://hz.sweek.top/gtetysfduw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daria6918.cn/gtqcysvaid.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigfzy.top/gtgzuarblo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.52xcode.cn/gtsamuldqb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tian-w.cn/gtcejinacm.html

TS:   [...arr];
来源：http://hz.daria6918.cn/gtjrvqjsjg.html

Java: new ArrayList<>(list);
来源：http://hz.jqgufenzy.top/gtwcijreye.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dashuyun.cn/gthlzpfdso.html

Ruby: arr.dup;  arr.clone
来源：http://hz.vqdsnc.cn/gttodvoiut.html

C#:   new List<int>(list);
来源：http://hz.jiagoushi.top/gticqeupbb.html

[D23] reduce 累积计算
来源：http://hz.sysykeji.top/gtmefxzjwl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydjk.org.cn/gtfydmuwue.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.c1oappe.top/gtoiavjika.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ybcxt.top/gtrhdetlhg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gzhubu.top/gtcjxvwzop.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jqgfzy.top/gtehbojswl.html

Go:   // 手写循环
来源：http://hz.jianghu66.top/gtlfsmoaeu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhixingplan.top/gtfnalopui.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj202588.top/gtbpvkonrl.html

[D24] 字典 / Map 基本操作
来源：http://hz.shanyushiyangtech.top/gtxmhspwux.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gzhubu.top/gtlaiojgnk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tanke756.top/gtazrhrtwr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.snrcjt.cn/gtljfqkzvk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sweek.top/gtrbuyfrfk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fengsongda.top/gtbxzynmhi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.iojbl.cn/gtsisfwwrw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zycfv.cn/gtvwxmkkih.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ydjk.org.cn/gtyrrxwgoo.html

[D25] Set 集合去重与交并差
来源：http://hz.ybcxt.top/gtydkwuzgq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhiwuduotai.top/gtmaqbmhqw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cucudq.cn/gtcdfcefut.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dashuyun.cn/gtyvvauucr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gaohongyu789.top/gtpoolekij.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gogol.net.cn/gtfedymccf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhongyouzk.top/gttyhjguqa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.meibo888.top/gtcuuvugox.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jlsjyb.cn/gtqhktbygs.html

[D26] 数组转字符串
来源：http://hz.yvedp.cn/gtwqjxzfxf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xylfe.cn/gtwejjwhko.html

PHP:  implode(", ", $arr);
来源：http://hz.guannengcc.top/gtwvrjddqt.html

JS:   arr.join(", ")
来源：http://hz.mhx1999.top/gtcegixtel.html

TS:   arr.join(", ")
来源：http://hz.jqgufenzy.top/gtewedtpvp.html

Java: String.join(", ", list)
来源：http://hz.9152youxi.cn/gtgwffrtoh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgfzy.top/gttfnwmugj.html

Ruby: arr.join(", ")
来源：http://hz.cashguo.top/gtnjbxpbdf.html

C#:   string.Join(", ", list)
来源：http://hz.0kj1m.cn/gtocsmgqzc.html

================================================================================
来源：http://hz.hysaishi.cn/gtktplekix.html

E. 字符串处理
来源：http://hz.zycfv.cn/gthqsyqdih.html

================================================================================
来源：http://hz.yj20258.top/gtbquuefoy.html

[E01] 拼接字符串
来源：http://hz.xuetiantiany.cn/gtndovlvsb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.vqdsnc.cn/gtkoauvwpt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.iojbl.cn/gtjkevniir.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gtfugiyion.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gtigiumrod.html


<!-- 参考信息 -->