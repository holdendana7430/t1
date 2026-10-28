代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sweek.top/gtpxadtphx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.svipenyu.cn/gtmwvlpgme.html

Java: import java.util.List;
来源：http://hz.jinqigufen.top/gtvpdrcbmz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.svipenyu.cn/gtxllnlvyu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jiagoushi.top/gtiualhqbc.html

C#:   using System.Text;
来源：http://hz.cheryme.top/gtkocwpkgc.html

[C12] 立即执行函数 IIFE
来源：http://hz.quarkkingdee.top/gtrahuypnp.html

Py:   (lambda: print("run"))()
来源：http://hz.daria6918.cn/gtgqehkmfi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.aibaodan.cn/gtzmzvznvp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.tanke756.top/gtwsezdnbn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.52xcode.cn/gtekwcojzc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tanke756.top/gtrxollomq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yvedp.cn/gteqckbamp.html

Ruby: -> { puts "run" }.call
来源：http://hz.dashuyun.cn/gthxlyqpoe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jianghu66.top/gtezvfbwlx.html

[C13] 类型声明 / 类型注解
来源：http://hz.hnqzz.top/gtrkubvvmg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yonumen.top/gtrrzxkggn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtatsmianh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.guannengcc.top/gtipmttvqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtwkcimjeb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtvvnnwmaj.html

Go:   func add(a, b int) int
来源：http://hz.nwbrower.top/gttrwastin.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sysykeji.top/gtmgmjjkbh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yueranfly.top/gtdvzafdip.html

[C14] 泛型函数
来源：http://hz.haohaochexian.top/gtqzhzycws.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cashguo.top/gtxqrjvgxc.html

PHP:  // 无泛型
来源：http://hz.sweek.top/gtpzpdcetp.html

JS:   // 无泛型
来源：http://hz.zhiwuduotai.top/gttuaemcer.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sufxvd.cn/gtjmxsfffh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.52xcode.cn/gtdwvhmcnw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.daria6918.cn/gtfwrqtmtk.html

Ruby: # 无泛型
来源：http://hz.aizwys.cn/gtlthdaszv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.snrcjt.cn/gthnzxielt.html

[C15] 解构 / 展开参数
来源：http://hz.cqqwz.cn/gtzrjajqzf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.redwolf501.top/gtidlkocyb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jqgufenzy.top/gtjjonnxzf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuxming.cn/gtrnljziym.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dashuyun.cn/gtsggglqum.html

Java: // 无解构
来源：http://hz.gaohongyu789.top/gtalsdryed.html

Go:   // 无解构
来源：http://hz.snrcjt.cn/gtrpuqlmhy.html

Ruby: a, b = pair
来源：http://hz.zhijiandao.cn/gtqbqkxqxp.html

C#:   var (a, b) = pair;
来源：http://hz.jyoumei.cn/gtmkedskdg.html

[C16] 函数 / 方法重载
来源：http://hz.dashuyun.cn/gtqcyuuelf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhongyouzk.top/gthnuzosxs.html

PHP:  // 无重载
来源：http://hz.shanyushiyangkeji.top/gtfbljogtv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xziqi.cn/gtizvsowxb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zdqjudy.top/gtyhbocfob.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zdqjudy.top/gtcllbfcxq.html

Go:   // 无重载：用不同函数名
来源：http://hz.ydjk.org.cn/gtyhypidvf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.dianchejie.cn/gthznfzyav.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cqqwz.cn/gtouyzpuhd.html

================================================================================
来源：http://hz.cucudq.cn/gtpayrzylx.html

D. 数组 / 列表 / 集合
来源：http://hz.ehwqpu.com/gtmhxibplh.html

================================================================================
来源：http://hz.cucudq.cn/gtmypqzuec.html

[D01] 创建数组 / 列表
来源：http://hz.shzxlz.cn/gthtusnzzs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.birdmap.top/gtdypzfgbl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhijiandao.cn/gtltjigzpu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yuanzhike.top/gtbdoitbzj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hnxiangtu.top/gtotkoivyr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xinyue.icu/gtsaykpqjx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.havefunace.top/gtijayccwo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nwbrower.top/gtilffkoma.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.vqdsnc.cn/gtnbthkigf.html

[D02] 追加元素到末尾
来源：http://hz.hnxiangtu.top/gthhetddij.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shuidangran.top/gtpgxrwxai.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cdnleiting.top/gtrlovwllx.html

JS:   arr.push(4);
来源：http://hz.zycfv.cn/gtfrkfsakx.html

TS:   arr.push(4);
来源：http://hz.shuidangran.top/gtjbfwzksw.html

Java: list.add(4);
来源：http://hz.guowangkeji.top/gteqlnzfqt.html

Go:   arr = append(arr, 4)
来源：http://hz.zhoulong.xyz/gtiqdrojov.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fengsongda.top/gtygpwdxno.html

C#:   list.Add(4);
来源：http://hz.aibaodan.cn/gtfknnzdor.html

[D03] 在指定位置插入元素
来源：http://hz.yongpay.top/gtfotqyvkz.html

Py:   arr.insert(0, 0)
来源：http://hz.jinghuilouyu.cn/gtplpvlwli.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ppjwa.cn/gteowzbcre.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhoulong.xyz/gtrxehrvmw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gogol.net.cn/gttpkcmsze.html

Java: list.add(0, 0);
来源：http://hz.zycfv.cn/gtiadkskjt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gaohongyu789.top/gtgchwzawk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xingfuxueyuan.xyz/gtmvtaogtc.html

C#:   list.Insert(0, 0);
来源：http://hz.pycfn.com/gtymafuhur.html

[D04] 删除元素
来源：http://hz.ehwqpu.com/gterygvkvb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhijiandao.cn/gtapwijcnb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.haohaochexian.top/gtlfuktthh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhengqikj.top/gtagytodmq.html

TS:   arr.splice(0, 1);
来源：http://hz.yangfankeji.com/gthaulmllr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.chenzaomai.com/gtsyqyvwkq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.iojbl.cn/gtiwlkbfpj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hongshengwenyu.top/gtewowbpfx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jqgfzy.top/gtcictoddq.html

[D05] 访问与修改元素
来源：http://hz.tianlin.xyz/gtcqhnakey.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.smart0.xyz/gtiyqujuec.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.fzhhl.top/gtpiocthql.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtntslfztm.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shuidangran.top/gtyuyhtrpi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhiwuduotai.top/gtsximzzae.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sxryk.cn/gtsaqboond.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtjzyfytih.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sysykeji.top/gtwmbpasnj.html

[D06] 数组长度
来源：http://hz.yvedp.cn/gtglbvilxt.html

Py:   len(arr)
来源：http://hz.fengsongda.top/gtqfkvsmih.html

PHP:  count($arr);
来源：http://hz.sxryk.cn/gtubewiznh.html

JS:   arr.length
来源：http://hz.yueranfly.top/gtkqsqbmmv.html

TS:   arr.length
来源：http://hz.jyoumei.cn/gtbtrorycg.html

Java: list.size();
来源：http://hz.sysykeji.top/gtplyifgtq.html

Go:   len(arr)
来源：http://hz.guowangkeji.top/gtmcomxcjz.html

Ruby: arr.length; arr.size
来源：http://hz.birdmap.top/gtzacaqgtp.html

C#:   list.Count;
来源：http://hz.shangyingyoupin.top/gtivfhixhz.html

[D07] 切片 / 取子数组
来源：http://hz.9152youxi.cn/gtrycwbszl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhongyouzk.top/gtbbctqsmk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shanyushiyangkeji.top/gtyhzpuaon.html

JS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtzitqpdzq.html

TS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtoofgwiua.html

Java: list.subList(1, 4);
来源：http://hz.quarkkingdee.top/gtegelmotr.html

Go:   arr[1:4]
来源：http://hz.yj20258888.top/gtkbsbxmqh.html

Ruby: arr[1, 3]
来源：http://hz.hnxiangtu.top/gtmatedgvj.html

C#:   list.GetRange(1, 3);
来源：http://hz.sxryk.cn/gtlmtzqycw.html

[D08] 合并两个数组
来源：http://hz.shuidangran.top/gtdisahovf.html

Py:   a + b;  a.extend(b)
来源：http://hz.cucudq.cn/gtkgapxsyn.html

PHP:  array_merge($a, $b);
来源：http://hz.sweek.top/gtlxuuihnt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.52xcode.cn/gtododxvhv.html

TS:   [...a, ...b];
来源：http://hz.cucudq.cn/gtepmhatjx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daria6918.cn/gtdzvemyeh.html

Go:   append(a, b...)
来源：http://hz.jiagoushi.top/gtweewunga.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hywenlv.cn/gtqadcrsje.html

C#:   a.Concat(b).ToList()
来源：http://hz.hywenlv.cn/gtqhlkotkf.html

[D09] 排序（升序）
来源：http://hz.wangshuangyany.cn/gtirhwwfgt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhaomingkeji.xyz/gtooprabjh.html

PHP:  sort($arr);
来源：http://hz.gotoacloud.top/gtyqtloxpr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxuanxn.top/gtfjqorbdq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.smart0.xyz/gtoxkontqc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cdnleiting.top/gtrxcsqwcb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.0kj1m.cn/gthlkgkdjx.html

Ruby: arr.sort
来源：http://hz.jqgfzy.top/gtlnfjrbvq.html

C#:   list.Sort();
来源：http://hz.yj20258888.top/gtebgfohej.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jiagoushi.top/gthwnldpfr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.guannengcc.top/gttqimwjax.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tanke756.top/gtbajretix.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydzc1.top/gtlcknhhdj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.9152youxi.cn/gtxzpnrweb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ivvv.top/gtbwflmafs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ywan-chungtsiang.top/gtusbblygo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxinkj.top/gtndamxapl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ywan-chungtsiang.top/gtasxgencn.html

[D11] 反转数组
来源：http://hz.yueranfly.top/gtoaeedlzz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.svipenyu.cn/gtozsxzmip.html

PHP:  array_reverse($arr);
来源：http://hz.gaohongyu789.top/gtcmitqsfg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yuxming.cn/gtpxauaxsn.html

TS:   [...arr].reverse();
来源：http://hz.cucudq.cn/gtqlveicwe.html

Java: Collections.reverse(list);
来源：http://hz.zhiwuduotai.top/gtwjykedtx.html

Go:   slices.Reverse(arr)
来源：http://hz.hammf.cn/gtenqgfqwz.html

Ruby: arr.reverse
来源：http://hz.sweek.top/gtipofzgox.html

C#:   list.Reverse();
来源：http://hz.cqqwz.cn/gtpqqjcbjo.html

[D12] 查找元素下标
来源：http://hz.aibaodan.cn/gtwuppofyc.html

Py:   arr.index(x);  x in arr
来源：http://hz.havefunace.top/gtglkouqmg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.iojbl.cn/gtwqabkrgv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.9152youxi.cn/gtzylldico.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtjgcfodxp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhixingplan.top/gtvpjldgqp.html

Go:   slices.Index(arr, x)
来源：http://hz.hammf.cn/gtelrychnm.html

Ruby: arr.index(x)
来源：http://hz.wangdashe.top/gtfqxoucdd.html

C#:   list.IndexOf(x);
来源：http://hz.dashuyun.cn/gtrqfvnatc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xziqi.cn/gtzpyjymdq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhijiandao.cn/gtmlvupcgd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cdnleiting.top/gtbqigcqgm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sweek.top/gtlsnxnwfc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtktndwcam.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj202588.top/gtzenzozwo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.daxiang520.top/gtffbjnkgk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.birdmap.top/gtkvmtsycn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jyoumei.cn/gtyxoubfzi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.mhx1999.top/gtjcseottz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.andypj.xyz/gtghtlquqm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ehwqpu.com/gtutcixkhc.html

JS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtsiyjaaue.html

TS:   arr.map(x => x * 2)
来源：http://hz.jqgfzy.top/gtgrnvorfd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinyuanbaomall.cn/gtjriwmnyb.html

Go:   // 手写循环
来源：http://hz.daria6918.cn/gtglzpejew.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jqgufenzy.top/gteunjtusi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pycfn.com/gtqdyirzbi.html

[D15] 去重
来源：http://hz.jqgufenzy.top/gtzmtogdjb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.dianchejie.cn/gtsuywivkr.html

PHP:  array_unique($arr);
来源：http://hz.guannengcc.top/gtxoqaeeym.html

JS:   [...new Set(arr)]
来源：http://hz.jianghu66.top/gtcxppntcw.html

TS:   [...new Set(arr)]
来源：http://hz.nanxuanxn.top/gtcpzpmdhx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.haohaochexian.top/gtuzmojlih.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fzhhl.top/gtipdbveix.html

Ruby: arr.uniq
来源：http://hz.birdmap.top/gtxftglpaa.html

C#:   list.Distinct().ToList()
来源：http://hz.chenlongwang.top/gttifibuat.html

[D16] 求和与平均值
来源：http://hz.gotoacloud.top/gteasxqorh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.9152youxi.cn/gtuwsfmgqa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ehwqpu.com/gthfiouskz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gtdoxlhwkw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtghtgawqh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zycfv.cn/gtsejxofoh.html

Go:   // 手写循环累加
来源：http://hz.fengsongda.top/gtnzouhucy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.dianchejie.cn/gtsgxiiyhp.html

C#:   list.Sum();  list.Average()
来源：http://hz.jiagoushi.top/gtxkwlhdwb.html

[D17] 最大值与最小值
来源：http://hz.hywenlv.cn/gtqwcijqrw.html

Py:   max(arr);  min(arr)
来源：http://hz.hongshengwenyu.top/gtyikvlzyx.html

PHP:  max($arr);  min($arr);
来源：http://hz.shzxlz.cn/gthircavyf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.svipenyu.cn/gthkzaltmq.html

TS:   Math.max(...arr);
来源：http://hz.jianghu66.top/gtkqrvpmsw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yongpay.top/gtxyzpnfjz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ivvv.top/gttupmmesy.html

Ruby: arr.max;  arr.min
来源：http://hz.yvedp.cn/gthdlvuqau.html

C#:   list.Max();  list.Min()
来源：http://hz.tian-w.cn/gtcnksrvfk.html

[D18] 扁平化嵌套数组
来源：http://hz.guannengcc.top/gtdtvyfmza.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cqqwz.cn/gtqoajjrwa.html

PHP:  array_merge(...$nested);
来源：http://hz.bjfxy.top/gtzrtxuhfp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sufxvd.cn/gtgobnsbtr.html

TS:   nested.flat();
来源：http://hz.yj20258888.top/gtixzrvbzi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.haohaochexian.top/gttwuiwlei.html

Go:   // 手写双层循环
来源：http://hz.cucudq.cn/gtqdvukzwy.html

Ruby: nested.flatten
来源：http://hz.sweek.top/gttghbmmvw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sweek.top/gtcqhlonof.html

[D19] 按字段分组
来源：http://hz.jiagoushi.top/gtpnchopak.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhaomingkeji.xyz/gtermjwhbt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhiwuduotai.top/gtxbknkhdl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.redwolf501.top/gtndurxocz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.wangshuangyany.cn/gtvwuyfvfb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hnxiangtu.top/gtwxjgcung.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgufenzy.top/gtvdebhfxt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.quarkkingdee.top/gtuvigfkke.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hysaishi.cn/gtevxckvaq.html

[D20] 统计每个元素出现次数
来源：http://hz.chenjidiqi.icu/gtuzjjibbu.html

Py:   Counter(arr)
来源：http://hz.aibaodan.cn/gtrdanvgxl.html

PHP:  array_count_values($arr);
来源：http://hz.dashuyun.cn/gtruygjjnj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtjoxypddk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtxohzjqyn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigufen.top/gtcmatlavk.html

Go:   // 手写 map[T]int
来源：http://hz.dianchejie.cn/gtikastbpv.html

Ruby: arr.tally
来源：http://hz.hywenlv.cn/gteladdqut.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sysykeji.top/gtgcfsskyk.html

[D21] 判断是否包含某元素
来源：http://hz.feifeiyinyue.top/gtdermxriw.html

Py:   x in arr
来源：http://hz.sxryk.cn/gtdvwmpfhl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ppjwa.cn/gtlxggypki.html

JS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtiuljwtog.html

TS:   arr.includes(x)
来源：http://hz.cucudq.cn/gtdjkjljyy.html

Java: list.contains(x)
来源：http://hz.ivvv.top/gtfqxqpcle.html

Go:   slices.Contains(arr, x)
来源：http://hz.52xcode.cn/gtbjdjfzhu.html

Ruby: arr.include?(x)
来源：http://hz.gotoacloud.top/gtxpwhmrya.html

C#:   list.Contains(x)
来源：http://hz.dianchejie.cn/gtmyraogqa.html

[D22] 复制数组（避免共享引用）
来源：http://hz.9152youxi.cn/gtneeexuzn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydzc1.top/gtrvbhnpoh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jyoumei.cn/gtlnfeaquy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.havefunace.top/gtflujlvic.html

TS:   [...arr];
来源：http://hz.yanxiufei.cn/gtwvbmnlrv.html

Java: new ArrayList<>(list);
来源：http://hz.yueranfly.top/gthwvbzmud.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yangfankeji.com/gtxyqsuuah.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hnqzz.top/gtnhhtpqay.html

C#:   new List<int>(list);
来源：http://hz.iojbl.cn/gtgxavhnpo.html

[D23] reduce 累积计算
来源：http://hz.yuxming.cn/gtdmnlxxlf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daria6918.cn/gtrdmcillz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinqigfzy.top/gtkrkmtuyg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.0kj1m.cn/gtgfmopmwi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtdbdptasc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.sweek.top/gtezadyium.html

Go:   // 手写循环
来源：http://hz.hnxiangtu.top/gtvsdphina.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuanzx.com/gtsnyytzdp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shangyingyoupin.top/gthvhthwtw.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhixingplan.top/gtijhvvook.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yonumen.top/gtakyfocwg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gogol.net.cn/gtdmhcdhqa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guowangkeji.top/gtilqkulmx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jqgfzy.top/gtstdtbvzy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.wangshuangyany.cn/gtjzlkrxii.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jiagoushi.top/gthodqxuvt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cqqwz.cn/gtgadoried.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.svipenyu.cn/gtutnzlmqe.html

[D25] Set 集合去重与交并差
来源：http://hz.zhixingplan.top/gtytiayknk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hfpthk.cn/gtqiijafvg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ivvv.top/gtrzamudpg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yonumen.top/gtnthxpmgo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xingfuxueyuan.xyz/gtiepufwfa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cashguo.top/gtevxozicp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.smart0.xyz/gtpcutrxfa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhiwuduotai.top/gtdvybnaah.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hysaishi.cn/gtucodkjos.html

[D26] 数组转字符串
来源：http://hz.gaohongyu789.top/gtqqopnkvf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hysaishi.cn/gtuibhpdwb.html

PHP:  implode(", ", $arr);
来源：http://hz.hysaishi.cn/gtmdikiwrk.html

JS:   arr.join(", ")
来源：http://hz.sufxvd.cn/gtptjlbiaw.html

TS:   arr.join(", ")
来源：http://hz.jyoumei.cn/gtgmwrgpff.html

Java: String.join(", ", list)
来源：http://hz.havefunace.top/gtjabgjpfk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xingfuxueyuan.xyz/gtqosdfxym.html

Ruby: arr.join(", ")
来源：http://hz.guannengcc.top/gtrsegzdkr.html

C#:   string.Join(", ", list)
来源：http://hz.shangyingyoupin.top/gtelqyqnmv.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtmbbvvfcr.html

E. 字符串处理
来源：http://hz.haohaochexian.top/gtkzebxpyc.html

================================================================================
来源：http://hz.yj20258888.top/gttpozhzja.html

[E01] 拼接字符串
来源：http://hz.sufxvd.cn/gtgolazcax.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sxryk.cn/gtvwxqychd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinghuilouyu.cn/gthhrmjeci.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cashguo.top/gtqhzulxoh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuetiantiany.cn/gtixegeeaw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ybcxt.top/gtavibhqyw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.52xcode.cn/gtleysnoyr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gotoacloud.top/gtnoaboodl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shangyingyoupin.top/gtuvugegdt.html


<!-- 参考信息 -->