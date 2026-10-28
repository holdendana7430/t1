代发 wailian999

C#:   块级作用域
来源：http://hz.vqdsnc.cn/gtmwosaisn.html

[C11] 模块导入与导出
来源：http://hz.yj202588.top/gtzlgzmvbk.html

Py:   from module import func
来源：http://hz.yongpay.top/gtjhpbpdzj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.vqdsnc.cn/gtdoinurzd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hywenlv.cn/gtslofayuq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.mhx1999.top/gtfgmhugrd.html

Java: import java.util.List;
来源：http://hz.pycfn.com/gtjmmjvzbe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cheryme.top/gtfarcmikj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jlsjyb.cn/gthgyivyaq.html

C#:   using System.Text;
来源：http://hz.zycfv.cn/gtegenbupj.html

[C12] 立即执行函数 IIFE
来源：http://hz.redwolf501.top/gtyefmdpgy.html

Py:   (lambda: print("run"))()
来源：http://hz.havefunace.top/gtcxrnobsa.html

PHP:  (function () { echo "run"; })();
来源：http://hz.gogol.net.cn/gtwzeyyxyf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cheryme.top/gtrnltutcg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.iojbl.cn/gtojepwwxq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.mhx1999.top/gteseziwne.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shanyushiyangkeji.top/gtxmqnvimh.html

Ruby: -> { puts "run" }.call
来源：http://hz.nanxuanxn.top/gtnjdezgpn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xylfe.cn/gtxyqlvvfd.html

[C13] 类型声明 / 类型注解
来源：http://hz.redwolf501.top/gtnimsbzsr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.mhx1999.top/gtbnrllsbx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtsupixfuq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenlongwang.top/gtjqsrlsvj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fengsongda.top/gtnnfhlgnc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtwelsxyqh.html

Go:   func add(a, b int) int
来源：http://hz.shangyingyoupin.top/gtbpfstemp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sysykeji.top/gtbucdvdmy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxuanxn.top/gtvvteamzw.html

[C14] 泛型函数
来源：http://hz.kuanghao11.cn/gtohjjrkfc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gteikkmmwb.html

PHP:  // 无泛型
来源：http://hz.daxiang520.top/gtcktpiami.html

JS:   // 无泛型
来源：http://hz.nwbrower.top/gtyonowwij.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.c1oappe.top/gtnhrgxnbu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cheryme.top/gtiwdexeui.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gotoacloud.top/gtazccltfm.html

Ruby: # 无泛型
来源：http://hz.shangyingyoupin.top/gttlqukjkf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cqqwz.cn/gtpcnsmcbx.html

[C15] 解构 / 展开参数
来源：http://hz.daria6918.cn/gtvgtrqbnp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.9152youxi.cn/gtkrdjodjw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tanke756.top/gtsriqxjxk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daxiang520.top/gtpyyenwnl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aizwys.cn/gtxajdmoff.html

Java: // 无解构
来源：http://hz.zdqjudy.top/gtuixehtfn.html

Go:   // 无解构
来源：http://hz.zycfv.cn/gtbztzfbbp.html

Ruby: a, b = pair
来源：http://hz.mhx1999.top/gtaxrqhidt.html

C#:   var (a, b) = pair;
来源：http://hz.cucudq.cn/gttbgugykw.html

[C16] 函数 / 方法重载
来源：http://hz.jyoumei.cn/gtrznncwjm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nanxinkj.top/gtelruzugo.html

PHP:  // 无重载
来源：http://hz.dianchejie.cn/gtgpeccpyi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.snrcjt.cn/gtqjdvridv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xziqi.cn/gtyyxxwxiy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gotoacloud.top/gtnqyxtoue.html

Go:   // 无重载：用不同函数名
来源：http://hz.chenlongwang.top/gtglcrlxgj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gogol.net.cn/gtmzwdphav.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shangyingyoupin.top/gtygbwpbjd.html

================================================================================
来源：http://hz.jinqigfzy.top/gteaizdbad.html

D. 数组 / 列表 / 集合
来源：http://hz.zycfv.cn/gtqjvyorrz.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gthiigwpdg.html

[D01] 创建数组 / 列表
来源：http://hz.ydjk.org.cn/gtcqtxmyzg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.haohaochexian.top/gtarldypzb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.dianchejie.cn/gtsotxfjsc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ybcxt.top/gtzauqltqf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ywan-chungtsiang.top/gthmukbjde.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cashguo.top/gtzdtnmyeg.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ywan-chungtsiang.top/gtjxooypef.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daria6918.cn/gtrwlugiaj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenzaomai.com/gtmzozwdbp.html

[D02] 追加元素到末尾
来源：http://hz.svipenyu.cn/gtuxqyywbv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.c1oappe.top/gtryqfbfuc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hammf.cn/gtkqbouunn.html

JS:   arr.push(4);
来源：http://hz.jinyuanbaomall.cn/gtcanjscay.html

TS:   arr.push(4);
来源：http://hz.birdmap.top/gthtamarqz.html

Java: list.add(4);
来源：http://hz.andypj.xyz/gtnrkwqgce.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxinkj.top/gtclctqmgi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinyuanbaomall.cn/gtizokwmgc.html

C#:   list.Add(4);
来源：http://hz.hongshengwenyu.top/gtrqlzfcon.html

[D03] 在指定位置插入元素
来源：http://hz.c1oappe.top/gtwbplnrps.html

Py:   arr.insert(0, 0)
来源：http://hz.hysaishi.cn/gteumsyzdz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.redwolf501.top/gtfwaplsbc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.daria6918.cn/gtbiusxqaw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.bjfxy.top/gtthstfqal.html

Java: list.add(0, 0);
来源：http://hz.jinqigfzy.top/gtcgnyjyft.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yuanzhike.top/gtklfsgkih.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xingfuxueyuan.xyz/gtmidmanrp.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgufenzy.top/gtsuwavrnz.html

[D04] 删除元素
来源：http://hz.guannengcc.top/gthmkdmncv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.tanke756.top/gtmuwxnibv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangshuangyany.cn/gtqwmkhrhf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zycfv.cn/gtoddpgqkf.html

TS:   arr.splice(0, 1);
来源：http://hz.gzhubu.top/gtavufyovd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.snrcjt.cn/gtibqshtdf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jinyuanbaomall.cn/gtkoczkaeg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.dianchejie.cn/gtndnfdhob.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnqzz.top/gtsqmumjxi.html

[D05] 访问与修改元素
来源：http://hz.meibo888.top/gtwqlxxxfd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtyvgxubrc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.haohaochexian.top/gttousuflm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.svipenyu.cn/gthkqpvjgw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yangfankeji.com/gtxmkuzhir.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tian-w.cn/gtlvwnuese.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtcifqbbrb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtrrmrndaj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hywenlv.cn/gtfrhnuods.html

[D06] 数组长度
来源：http://hz.nwbrower.top/gtfnlnalzn.html

Py:   len(arr)
来源：http://hz.yj20258888.top/gtggukrcrf.html

PHP:  count($arr);
来源：http://hz.zhixingplan.top/gtfnwgmnfx.html

JS:   arr.length
来源：http://hz.havefunace.top/gtrmhdbrqd.html

TS:   arr.length
来源：http://hz.ivvv.top/gtphgbiktf.html

Java: list.size();
来源：http://hz.yuanzhike.top/gtxjeprgsn.html

Go:   len(arr)
来源：http://hz.chenzaomai.com/gtgdmnhfrc.html

Ruby: arr.length; arr.size
来源：http://hz.9152youxi.cn/gtrbbhwepa.html

C#:   list.Count;
来源：http://hz.pycfn.com/gtcfqjtscx.html

[D07] 切片 / 取子数组
来源：http://hz.smart0.xyz/gtrqsdesax.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hnqzz.top/gtgcjgakab.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yonumen.top/gtzytdvuqj.html

JS:   arr.slice(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtpuqgcima.html

TS:   arr.slice(1, 4);
来源：http://hz.zhijiandao.cn/gtimfusxtz.html

Java: list.subList(1, 4);
来源：http://hz.sysykeji.top/gtvcortxhx.html

Go:   arr[1:4]
来源：http://hz.dianchejie.cn/gtygcvlrbm.html

Ruby: arr[1, 3]
来源：http://hz.xziqi.cn/gtuohtcnee.html

C#:   list.GetRange(1, 3);
来源：http://hz.gaohongyu789.top/gtjxeqeljw.html

[D08] 合并两个数组
来源：http://hz.hysaishi.cn/gtyqdldxhb.html

Py:   a + b;  a.extend(b)
来源：http://hz.xingfuxueyuan.xyz/gthccgshrb.html

PHP:  array_merge($a, $b);
来源：http://hz.zhaomingkeji.xyz/gtlfbmdwcv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gzhubu.top/gtdrskhfhx.html

TS:   [...a, ...b];
来源：http://hz.guowangkeji.top/gtvnlphkxw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pengpengdd.cyou/gtcltnzjgz.html

Go:   append(a, b...)
来源：http://hz.cqqwz.cn/gtkavpsbwj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cqqwz.cn/gtrksbyjji.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenlongwang.top/gtbgwazzkp.html

[D09] 排序（升序）
来源：http://hz.chenzaomai.com/gtactkovyi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.9152youxi.cn/gtwfdgccak.html

PHP:  sort($arr);
来源：http://hz.yangfankeji.com/gtybxrtjbv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhijiandao.cn/gtngjzbmwh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zdqjudy.top/gteyxdohdl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.bjfxy.top/gtrywniona.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sweek.top/gtpwxoiplx.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gtjhmbflkh.html

C#:   list.Sort();
来源：http://hz.chenjidiqi.icu/gtxalvqhcr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.andypj.xyz/gtqgvglvbn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gzhubu.top/gtbqxjpsvc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.svipenyu.cn/gtjqzactdi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj202588.top/gtsanvhojd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenlongwang.top/gtbmddhdxw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tanke756.top/gtvdiownhy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shanyushiyangtech.top/gtfihvqhpb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.daria6918.cn/gteajiajuz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.52xcode.cn/gtdltjkqtu.html

[D11] 反转数组
来源：http://hz.tian-w.cn/gtcgkqoncl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.smart0.xyz/gtgalkxgdd.html

PHP:  array_reverse($arr);
来源：http://hz.hnqzz.top/gtjdmexrjy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258888.top/gtpcxclfpx.html

TS:   [...arr].reverse();
来源：http://hz.smart0.xyz/gtfcylyycy.html

Java: Collections.reverse(list);
来源：http://hz.chenjidiqi.icu/gttrmijwxa.html

Go:   slices.Reverse(arr)
来源：http://hz.shanyushiyangtech.top/gtlmzrfqau.html

Ruby: arr.reverse
来源：http://hz.jinqigfzy.top/gthjylcoxg.html

C#:   list.Reverse();
来源：http://hz.redwolf501.top/gtvjlasyol.html

[D12] 查找元素下标
来源：http://hz.cheryme.top/gtenettrqk.html

Py:   arr.index(x);  x in arr
来源：http://hz.smart0.xyz/gtyorhrdvf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuanzhike.top/gtsdusethu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gtbyshpmwp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.redwolf501.top/gtrzijzras.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.kuanghao11.cn/gtljgydcze.html

Go:   slices.Index(arr, x)
来源：http://hz.andypj.xyz/gtyymqsokq.html

Ruby: arr.index(x)
来源：http://hz.hysaishi.cn/gtbsiaapwh.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangtech.top/gtaekmqjah.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yuanzhike.top/gtizdzynqh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sxryk.cn/gtkpwjswjz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jiagoushi.top/gtthzfdfnl.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtbnutrejr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gtgxjyrfvf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.redwolf501.top/gtyvdhhdmq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ppjwa.cn/gtdtxnuqwk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zdqjudy.top/gttcikrplc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yvedp.cn/gtestwldsl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xingfuxueyuan.xyz/gtbckxdpgo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhijiandao.cn/gtehqvieqb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tian-w.cn/gtrlvzetyy.html

JS:   arr.map(x => x * 2)
来源：http://hz.sufxvd.cn/gtwthkpjhg.html

TS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtcuxzqetx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.redwolf501.top/gtdpdrjcjf.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gtgrashctq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj20258888.top/gtnlayeiql.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jianghu66.top/gtppnmgmff.html

[D15] 去重
来源：http://hz.yuanzhike.top/gtftnjppdv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ppjwa.cn/gtpcqvuati.html

PHP:  array_unique($arr);
来源：http://hz.pycfn.com/gtblmwyolo.html

JS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gtgskeqnzb.html

TS:   [...new Set(arr)]
来源：http://hz.jinqigfzy.top/gtajfuccut.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ywan-chungtsiang.top/gtzloxvuyv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.chenjidiqi.icu/gtufiforkv.html

Ruby: arr.uniq
来源：http://hz.gogol.net.cn/gtxokdfafp.html

C#:   list.Distinct().ToList()
来源：http://hz.xuetiantiany.cn/gthzqbhddk.html

[D16] 求和与平均值
来源：http://hz.jlsjyb.cn/gtokpesiup.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.316326.xyz/gtrzwtuwmg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ydzc1.top/gtvppygmew.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zdqjudy.top/gtuyzwwrxp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnxiangtu.top/gtdpddimjc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.wangdashe.top/gtzoputvue.html

Go:   // 手写循环累加
来源：http://hz.yj20258888.top/gtxnhbihrx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinghuilouyu.cn/gtpfsvmxjs.html

C#:   list.Sum();  list.Average()
来源：http://hz.shangyingyoupin.top/gtrdwlkvqt.html

[D17] 最大值与最小值
来源：http://hz.sweek.top/gtnkzrpoha.html

Py:   max(arr);  min(arr)
来源：http://hz.yongpay.top/gtpvcrxwgu.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhoulong.xyz/gttztyjbwn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ybcxt.top/gtcwnmumxy.html

TS:   Math.max(...arr);
来源：http://hz.zhaomingkeji.xyz/gtnkkfidgb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangshuangyany.cn/gtbuqvhwhd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.daria6918.cn/gttrauziot.html

Ruby: arr.max;  arr.min
来源：http://hz.guowangkeji.top/gtzbasaujv.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxinkj.top/gtacfdwyvh.html

[D18] 扁平化嵌套数组
来源：http://hz.zhongyouzk.top/gtzhiewihl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hywenlv.cn/gtzpfsmxwt.html

PHP:  array_merge(...$nested);
来源：http://hz.nwbrower.top/gtkuffliux.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yvedp.cn/gturvhbekn.html

TS:   nested.flat();
来源：http://hz.fengsongda.top/gtupgwraow.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jyoumei.cn/gtzeiphasn.html

Go:   // 手写双层循环
来源：http://hz.fengsongda.top/gtjjkaqjob.html

Ruby: nested.flatten
来源：http://hz.zhixingplan.top/gtuieahbrk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hnxiangtu.top/gtanhrabep.html

[D19] 按字段分组
来源：http://hz.birdmap.top/gthimrbssk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.nanxinkj.top/gtliapjhxf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.haohaochexian.top/gtdaoqmcsg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.andypj.xyz/gtoszlhwym.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.redwolf501.top/gtaiysiqpe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinghuilouyu.cn/gtfuzpjnji.html

Go:   // 手写 map[string][]T
来源：http://hz.kuanghao11.cn/gtvzbawwas.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yuxming.cn/gtnbxzvysb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sweek.top/gtrpmagjlz.html

[D20] 统计每个元素出现次数
来源：http://hz.gzhubu.top/gtubkmbyhl.html

Py:   Counter(arr)
来源：http://hz.hongshengwenyu.top/gtqamaauwt.html

PHP:  array_count_values($arr);
来源：http://hz.hammf.cn/gtxyjhshzr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guowangkeji.top/gtgaafofyh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuanzx.com/gtevhhqnsm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shzxlz.cn/gtvidployc.html

Go:   // 手写 map[T]int
来源：http://hz.birdmap.top/gtkklpoyie.html

Ruby: arr.tally
来源：http://hz.jlsjyb.cn/gthtytflgf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangdashe.top/gtkoaotoaf.html

[D21] 判断是否包含某元素
来源：http://hz.nanxuanxn.top/gtbncfcemx.html

Py:   x in arr
来源：http://hz.sxryk.cn/gtrlrrnakh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nwbrower.top/gtwxkcmmhn.html

JS:   arr.includes(x)
来源：http://hz.guowangkeji.top/gttwzmsofi.html

TS:   arr.includes(x)
来源：http://hz.shuidangran.top/gthhilnoiu.html

Java: list.contains(x)
来源：http://hz.cdnleiting.top/gtagbwlrvr.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnxiangtu.top/gtqgaexgpr.html

Ruby: arr.include?(x)
来源：http://hz.chenzaomai.com/gtamlhpdaq.html

C#:   list.Contains(x)
来源：http://hz.ivvv.top/gtrlyuttyl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.redwolf501.top/gtwpydihbi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xylfe.cn/gtvoxfrhnz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.nanxuanxn.top/gtgerbxinz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zdqjudy.top/gtavrfbbmy.html

TS:   [...arr];
来源：http://hz.zhiwuduotai.top/gtjlatxmez.html

Java: new ArrayList<>(list);
来源：http://hz.jqgufenzy.top/gtxgarevgc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenzaomai.com/gtexydgfoy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinyuanbaomall.cn/gtpukrjffa.html

C#:   new List<int>(list);
来源：http://hz.shanyushiyangkeji.top/gtoidlpycl.html

[D23] reduce 累积计算
来源：http://hz.jlsjyb.cn/gtrwfhwpdv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.aibaodan.cn/gtrznzijst.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ywan-chungtsiang.top/gtmbpbvmik.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtdprpmdgt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgfzy.top/gtqemcarka.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.pengpengdd.cyou/gtgkzmbjbx.html

Go:   // 手写循环
来源：http://hz.xinyue.icu/gtesvrglyc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenlongwang.top/gtytevndhn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.andypj.xyz/gtpiriiatb.html

[D24] 字典 / Map 基本操作
来源：http://hz.ivvv.top/gtjprxojcb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hongshengwenyu.top/gtgrhyypzu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhaomingkeji.xyz/gtavzotbfx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.dianchejie.cn/gttvhirbcp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yvedp.cn/gtnxkkomar.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxuanxn.top/gtprhsqiij.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj20258888.top/gtfirflwxu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yj202588.top/gtzcaxtpub.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.svipenyu.cn/gtosmslmnq.html

[D25] Set 集合去重与交并差
来源：http://hz.mhx1999.top/gthrnexxxc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jiagoushi.top/gtmljktzue.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ehwqpu.com/gtbjveqbxj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jqgufenzy.top/gtbsipxsds.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cqqwz.cn/gtgtjgwqsg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hfpthk.cn/gtogqaswii.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sxryk.cn/gtwsspzndo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinyuanbaomall.cn/gtegdeftev.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cheryme.top/gtyuqycmyy.html

[D26] 数组转字符串
来源：http://hz.52xcode.cn/gtozzgbsql.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cashguo.top/gtrhftpqhp.html

PHP:  implode(", ", $arr);
来源：http://hz.redwolf501.top/gtepcsfcfz.html

JS:   arr.join(", ")
来源：http://hz.jiagoushi.top/gtngseisei.html

TS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtmdequsvh.html

Java: String.join(", ", list)
来源：http://hz.sxryk.cn/gtbwhgjvbr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.guowangkeji.top/gtlmihlnig.html

Ruby: arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtcwcwbxpa.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigfzy.top/gtpmndqnia.html

================================================================================
来源：http://hz.iojbl.cn/gttzvmdtua.html

E. 字符串处理
来源：http://hz.hfpthk.cn/gtcioexlmw.html

================================================================================
来源：http://hz.hfpthk.cn/gtpmjgodzb.html

[E01] 拼接字符串
来源：http://hz.vqdsnc.cn/gtlbksahqb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gzhubu.top/gtazvkrezv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.tianlin.xyz/gtfmbldmqi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cdnleiting.top/gtneiqrdgz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtbmxitxyq.html


<!-- 参考信息 -->