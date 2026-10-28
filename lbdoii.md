代发 wailian999

C#:   块级作用域
来源：http://hz.xziqi.cn/gtzaunnrct.html

[C11] 模块导入与导出
来源：http://hz.sweek.top/gtulgtotjc.html

Py:   from module import func
来源：http://hz.hammf.cn/gtippsswit.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ehwqpu.com/gteifqagpm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ehwqpu.com/gttvxhbaml.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hysaishi.cn/gtnwxjsxsc.html

Java: import java.util.List;
来源：http://hz.sufxvd.cn/gtdluqjdja.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj20258888.top/gtkrmkhlih.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.gogol.net.cn/gtbikcghrp.html

C#:   using System.Text;
来源：http://hz.sweek.top/gtlawwjmif.html

[C12] 立即执行函数 IIFE
来源：http://hz.shangyingyoupin.top/gtoxsdnfuy.html

Py:   (lambda: print("run"))()
来源：http://hz.cucudq.cn/gthxoxtmbc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yuxming.cn/gtjlcdxuhb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hywenlv.cn/gtjozcdivo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gtnmaupygs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nanxuanxn.top/gtrzdyuntz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinghuilouyu.cn/gtknxbvlzy.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhixingplan.top/gtyerdbuqy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cheryme.top/gtbliokbzq.html

[C13] 类型声明 / 类型注解
来源：http://hz.smart0.xyz/gturrwarqw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nanxuanxn.top/gthkqankyv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yanxiufei.cn/gthlceirll.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yanxiufei.cn/gtfbexfgzo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ppjwa.cn/gtqqxnphbz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gtipsfvvyf.html

Go:   func add(a, b int) int
来源：http://hz.quarkkingdee.top/gtqqigkhnk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinghuilouyu.cn/gtzftrrumt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.meibo888.top/gtyjgauowt.html

[C14] 泛型函数
来源：http://hz.cashguo.top/gtmnpiupkz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cheryme.top/gtmzgqlasb.html

PHP:  // 无泛型
来源：http://hz.tianlin.xyz/gtswtcynsn.html

JS:   // 无泛型
来源：http://hz.dianchejie.cn/gtzxpejekc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yanxiufei.cn/gtmdvdxcrw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tian-w.cn/gtaatkpbwk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ybcxt.top/gtwwwqeiak.html

Ruby: # 无泛型
来源：http://hz.zycfv.cn/gthhwfhixb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.birdmap.top/gtvscxevmb.html

[C15] 解构 / 展开参数
来源：http://hz.aibaodan.cn/gtwjffhklw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hnxiangtu.top/gtxxbjpdua.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhaomingkeji.xyz/gtzusaxuhr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gttymamnee.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gzhubu.top/gtjisbiluw.html

Java: // 无解构
来源：http://hz.fengsongda.top/gtyiiizidk.html

Go:   // 无解构
来源：http://hz.xziqi.cn/gthhkqzfvk.html

Ruby: a, b = pair
来源：http://hz.tianlin.xyz/gtcitezbff.html

C#:   var (a, b) = pair;
来源：http://hz.zhijiandao.cn/gtirmmrxnb.html

[C16] 函数 / 方法重载
来源：http://hz.hammf.cn/gtaasepmku.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.andypj.xyz/gtvbsxzjzs.html

PHP:  // 无重载
来源：http://hz.xingfuxueyuan.xyz/gtfckydvlf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhaomingkeji.xyz/gtasdeuinf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhongyouzk.top/gtofihhzvv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenjidiqi.icu/gtocmgznoe.html

Go:   // 无重载：用不同函数名
来源：http://hz.cashguo.top/gtwwraffeh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.snrcjt.cn/gtbpqaaebf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xuanzx.com/gtelzpgxly.html

================================================================================
来源：http://hz.hfpthk.cn/gtddlzibvx.html

D. 数组 / 列表 / 集合
来源：http://hz.hammf.cn/gtfulivasx.html

================================================================================
来源：http://hz.yj20258.top/gthugdyyqd.html

[D01] 创建数组 / 列表
来源：http://hz.jinqigufen.top/gtambcmtcm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.dianchejie.cn/gtazzqetvs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.daria6918.cn/gtpyifqmun.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cucudq.cn/gtbpcgsosz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hfpthk.cn/gtdcsiervk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.pengpengdd.cyou/gtwpwxpgld.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daxiang520.top/gtxtgoafoj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj20258.top/gteydfkjvw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinqigfzy.top/gtmfawhdkv.html

[D02] 追加元素到末尾
来源：http://hz.feifeiyinyue.top/gtlfaqbitj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhaomingkeji.xyz/gtlwdvbqcm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.smart0.xyz/gtmgcmlmwt.html

JS:   arr.push(4);
来源：http://hz.meibo888.top/gtvvoowjbj.html

TS:   arr.push(4);
来源：http://hz.smart0.xyz/gtwjoijzfg.html

Java: list.add(4);
来源：http://hz.jinyuanbaomall.cn/gtlygcqxxu.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxuanxn.top/gtlrcqcbux.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.mhx1999.top/gtlvkbdiza.html

C#:   list.Add(4);
来源：http://hz.hnqzz.top/gtipezdubb.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangtech.top/gtxxsozfcs.html

Py:   arr.insert(0, 0)
来源：http://hz.iojbl.cn/gtqlorbfjj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.tanke756.top/gthihoqqvc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinqigfzy.top/gtypmltyzp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.316326.xyz/gtvngunlhj.html

Java: list.add(0, 0);
来源：http://hz.nwbrower.top/gtfmkpqzsq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.9152youxi.cn/gthlgnczih.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenlongwang.top/gtacstdifm.html

C#:   list.Insert(0, 0);
来源：http://hz.jinyuanbaomall.cn/gtrcltghfl.html

[D04] 删除元素
来源：http://hz.wangdashe.top/gtnjgjszut.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hywenlv.cn/gtbiorayrf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hammf.cn/gttosiikxi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cdnleiting.top/gtrtzwhfhr.html

TS:   arr.splice(0, 1);
来源：http://hz.andypj.xyz/gtjxieeoiq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.snrcjt.cn/gtrdvdnrvh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nanxinkj.top/gtycsgnays.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.andypj.xyz/gttrxblxjg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.bjfxy.top/gtccmukfrg.html

[D05] 访问与修改元素
来源：http://hz.gaohongyu789.top/gtduphpqcu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.havefunace.top/gtqkzpvqpd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.feifeiyinyue.top/gtvhyxijaj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cashguo.top/gtqkuuxvjf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenzaomai.com/gtnnjmgbtp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jqgfzy.top/gtigbqhmdn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtxtswcemk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.316326.xyz/gtjjiowmsu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jiagoushi.top/gtaqusiwyr.html

[D06] 数组长度
来源：http://hz.yj20258.top/gtasbqwmpy.html

Py:   len(arr)
来源：http://hz.shangyingyoupin.top/gtjuhzeoqz.html

PHP:  count($arr);
来源：http://hz.pengpengdd.cyou/gtanohvnnc.html

JS:   arr.length
来源：http://hz.fengsongda.top/gtjnfceapx.html

TS:   arr.length
来源：http://hz.tianlin.xyz/gthhhgbgkg.html

Java: list.size();
来源：http://hz.dianchejie.cn/gtaeyzqbky.html

Go:   len(arr)
来源：http://hz.zhoulong.xyz/gtzplrnnbp.html

Ruby: arr.length; arr.size
来源：http://hz.jlsjyb.cn/gtxjjohrnq.html

C#:   list.Count;
来源：http://hz.tian-w.cn/gtihdlkxby.html

[D07] 切片 / 取子数组
来源：http://hz.nwbrower.top/gtnhfwfbra.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xziqi.cn/gttatnvolg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.guannengcc.top/gtlehwvnmp.html

JS:   arr.slice(1, 4);
来源：http://hz.hammf.cn/gtcovmbywp.html

TS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtpzcjmkxx.html

Java: list.subList(1, 4);
来源：http://hz.dashuyun.cn/gtoyqyxktt.html

Go:   arr[1:4]
来源：http://hz.dashuyun.cn/gtmglisyzn.html

Ruby: arr[1, 3]
来源：http://hz.wangdashe.top/gttntjxmtt.html

C#:   list.GetRange(1, 3);
来源：http://hz.yvedp.cn/gtelavpkpb.html

[D08] 合并两个数组
来源：http://hz.kuanghao11.cn/gtmlvtoihy.html

Py:   a + b;  a.extend(b)
来源：http://hz.yvedp.cn/gtxbrdigpw.html

PHP:  array_merge($a, $b);
来源：http://hz.nwbrower.top/gtvvthbuil.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258888.top/gtjbeprden.html

TS:   [...a, ...b];
来源：http://hz.jianghu66.top/gtyssyeagp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuanzx.com/gtigggakll.html

Go:   append(a, b...)
来源：http://hz.sysykeji.top/gtbunqefgm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.haohaochexian.top/gturjylquy.html

C#:   a.Concat(b).ToList()
来源：http://hz.ppjwa.cn/gtzxagfbye.html

[D09] 排序（升序）
来源：http://hz.guannengcc.top/gtpnztjdql.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuanzhike.top/gtxpkzfdhh.html

PHP:  sort($arr);
来源：http://hz.gaohongyu789.top/gtueyzduwb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xylfe.cn/gtxyjhulrm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ywan-chungtsiang.top/gtzznarcyq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinyuanbaomall.cn/gtazhzhusv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.vqdsnc.cn/gthydkkiap.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtgnzhfycq.html

C#:   list.Sort();
来源：http://hz.jinqigfzy.top/gtnkilvnhb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.52xcode.cn/gtelmppyre.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jiagoushi.top/gtoxjgavsd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydzc1.top/gtqbmfimuo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.0kj1m.cn/gtfurhxvvm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nwbrower.top/gtfrngvgsh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shuidangran.top/gtcprmbnai.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xylfe.cn/gtwkrkqapj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tanke756.top/gtauokcrwj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yuxming.cn/gtaapcvnec.html

[D11] 反转数组
来源：http://hz.shuidangran.top/gtlvmaitit.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jianghu66.top/gtwgtgqpvm.html

PHP:  array_reverse($arr);
来源：http://hz.hfpthk.cn/gtqmiiudxl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dianchejie.cn/gtzjqtfyjk.html

TS:   [...arr].reverse();
来源：http://hz.cdnleiting.top/gtbvlfnwbx.html

Java: Collections.reverse(list);
来源：http://hz.quarkkingdee.top/gtgoqhewuk.html

Go:   slices.Reverse(arr)
来源：http://hz.nwbrower.top/gthoccufor.html

Ruby: arr.reverse
来源：http://hz.quarkkingdee.top/gtkkmbxmmp.html

C#:   list.Reverse();
来源：http://hz.aibaodan.cn/gtujlltrub.html

[D12] 查找元素下标
来源：http://hz.snrcjt.cn/gttfsxtvlq.html

Py:   arr.index(x);  x in arr
来源：http://hz.sweek.top/gtawfbchxo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ppjwa.cn/gtzudrcbvb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtwcgfpted.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jiagoushi.top/gtwivbhzjn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.pycfn.com/gtrfsvjajf.html

Go:   slices.Index(arr, x)
来源：http://hz.yvedp.cn/gtohkgshgl.html

Ruby: arr.index(x)
来源：http://hz.hnqzz.top/gtnllwzmig.html

C#:   list.IndexOf(x);
来源：http://hz.0kj1m.cn/gtebltiusc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ywan-chungtsiang.top/gtnmpwmrks.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xuanzx.com/gtogjnkkww.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shzxlz.cn/gtmblpvmsl.html

JS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gthxnzttxy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtifwciibz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.fzhhl.top/gtpdwkkjue.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.quarkkingdee.top/gtpszofnef.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ywan-chungtsiang.top/gtczbwrcrx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yongpay.top/gtnpvmaxnh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xuanzx.com/gtfxuyszmv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shanyushiyangtech.top/gthdqsylyc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinghuilouyu.cn/gtlgvcniez.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhengqikj.top/gthwfzvvqq.html

TS:   arr.map(x => x * 2)
来源：http://hz.shangyingyoupin.top/gtirkrgmag.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shzxlz.cn/gtqrtqdrpc.html

Go:   // 手写循环
来源：http://hz.cdnleiting.top/gtsfdoeztr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtyrgfceyx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.andypj.xyz/gtcebwlgff.html

[D15] 去重
来源：http://hz.xylfe.cn/gtzdsfdawz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gthjsiqrwg.html

PHP:  array_unique($arr);
来源：http://hz.kuanghao11.cn/gthdwzrath.html

JS:   [...new Set(arr)]
来源：http://hz.yvedp.cn/gtdxsybwpb.html

TS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtnhubnqbz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuanzx.com/gtpghhmrrm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.guannengcc.top/gtubztifzb.html

Ruby: arr.uniq
来源：http://hz.haohaochexian.top/gthxuhzjvl.html

C#:   list.Distinct().ToList()
来源：http://hz.yanxiufei.cn/gtnbytcuei.html

[D16] 求和与平均值
来源：http://hz.bjfxy.top/gtplzvzohf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.kuanghao11.cn/gtopbmhcrd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yuxming.cn/gthdzpktdx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gtmhgcdlvg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gtxvpizelu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nanxinkj.top/gtatkfgcbl.html

Go:   // 手写循环累加
来源：http://hz.52xcode.cn/gtajrptpuk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jqgfzy.top/gtyparbkql.html

C#:   list.Sum();  list.Average()
来源：http://hz.vqdsnc.cn/gtaowqzcdi.html

[D17] 最大值与最小值
来源：http://hz.redwolf501.top/gtpcphjdzx.html

Py:   max(arr);  min(arr)
来源：http://hz.snrcjt.cn/gtnwywhexd.html

PHP:  max($arr);  min($arr);
来源：http://hz.xinyue.icu/gtmapttnxg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gzhubu.top/gtrqkmsmcv.html

TS:   Math.max(...arr);
来源：http://hz.yueranfly.top/gtzqizbakc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xinyue.icu/gtbuwfdlmo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hfpthk.cn/gtzwwrxlse.html

Ruby: arr.max;  arr.min
来源：http://hz.jinghuilouyu.cn/gtwecgiweq.html

C#:   list.Max();  list.Min()
来源：http://hz.zdqjudy.top/gtxwpqecvc.html

[D18] 扁平化嵌套数组
来源：http://hz.gaohongyu789.top/gtwuenchvr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aizwys.cn/gtycecolzp.html

PHP:  array_merge(...$nested);
来源：http://hz.iojbl.cn/gtznrosmcn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gzhubu.top/gtjaqjqrrw.html

TS:   nested.flat();
来源：http://hz.ybcxt.top/gtvyzgscps.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.guowangkeji.top/gtwyeplehb.html

Go:   // 手写双层循环
来源：http://hz.jiagoushi.top/gtzrvfbvtt.html

Ruby: nested.flatten
来源：http://hz.jiagoushi.top/gtpiyxjiaf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aizwys.cn/gtoixexfes.html

[D19] 按字段分组
来源：http://hz.shangyingyoupin.top/gtqcztmejd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenjidiqi.icu/gtiyzuoyag.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258.top/gtsorcpylz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cqqwz.cn/gtbyafbfyl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sysykeji.top/gttvrhdkdv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cashguo.top/gtatfwwkpq.html

Go:   // 手写 map[string][]T
来源：http://hz.andypj.xyz/gtvzatcgol.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yuxming.cn/gtzlfhlcrm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hongshengwenyu.top/gtngezexpn.html

[D20] 统计每个元素出现次数
来源：http://hz.zhoulong.xyz/gtmvuxqfxb.html

Py:   Counter(arr)
来源：http://hz.ppjwa.cn/gtxmzydspe.html

PHP:  array_count_values($arr);
来源：http://hz.gotoacloud.top/gtmrclsgzs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuanzhike.top/gtvezertml.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ybcxt.top/gtdzsncsqy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgfzy.top/gtmslkoguj.html

Go:   // 手写 map[T]int
来源：http://hz.guannengcc.top/gtzzmlklkh.html

Ruby: arr.tally
来源：http://hz.cheryme.top/gtnsrpaffc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhijiandao.cn/gtrcjgxdsq.html

[D21] 判断是否包含某元素
来源：http://hz.zdqjudy.top/gtdbymbbwo.html

Py:   x in arr
来源：http://hz.jqgfzy.top/gtoxijkmtb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.quarkkingdee.top/gtsvppfjzx.html

JS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtanjnstst.html

TS:   arr.includes(x)
来源：http://hz.gogol.net.cn/gtesaaefbc.html

Java: list.contains(x)
来源：http://hz.andypj.xyz/gtwbgxozze.html

Go:   slices.Contains(arr, x)
来源：http://hz.shuidangran.top/gttbbuyiwe.html

Ruby: arr.include?(x)
来源：http://hz.pengpengdd.cyou/gthndetwgr.html

C#:   list.Contains(x)
来源：http://hz.tanke756.top/gtfqxynwwa.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zdqjudy.top/gtxajvtrra.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cdnleiting.top/gtuqanuyfl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.snrcjt.cn/gtcfbgfrey.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhixingplan.top/gtmxhzhmkm.html

TS:   [...arr];
来源：http://hz.gzhubu.top/gtkgusjvkc.html

Java: new ArrayList<>(list);
来源：http://hz.cucudq.cn/gtxwgxsxsf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yonumen.top/gtgwdspzns.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj202588.top/gthcyvqqmv.html

C#:   new List<int>(list);
来源：http://hz.cashguo.top/gtxegpakra.html

[D23] reduce 累积计算
来源：http://hz.hywenlv.cn/gtzplwevxy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sweek.top/gtysivmjhc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tanke756.top/gtjoemejin.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tianlin.xyz/gttiillwbq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gtqhctvjtb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.svipenyu.cn/gtxthjakrx.html

Go:   // 手写循环
来源：http://hz.svipenyu.cn/gthmdvdkwn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sweek.top/gtjdpzbcav.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhiwuduotai.top/gtudtzwpel.html

[D24] 字典 / Map 基本操作
来源：http://hz.svipenyu.cn/gtzybopuxv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ehwqpu.com/gtrxaqfpzm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daria6918.cn/gtirhfrehl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.quarkkingdee.top/gtskhemlmf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ydjk.org.cn/gtmltebsid.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gogol.net.cn/gtojpvylip.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cheryme.top/gtfpkanavi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aibaodan.cn/gtramkuqsz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pengpengdd.cyou/gtxlelanww.html

[D25] Set 集合去重与交并差
来源：http://hz.jlsjyb.cn/gtxzdpmfti.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhijiandao.cn/gtzkwhmhbq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.c1oappe.top/gtnnyucepk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yueranfly.top/gtbxzoyffe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.quarkkingdee.top/gttixlrtkw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xuanzx.com/gtxjzruste.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daria6918.cn/gtkemxvxdg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cqqwz.cn/gtusgooifr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhiwuduotai.top/gtljcfxiaf.html

[D26] 数组转字符串
来源：http://hz.quarkkingdee.top/gtkfgqtavk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nwbrower.top/gtvwjoxyrw.html

PHP:  implode(", ", $arr);
来源：http://hz.nwbrower.top/gtosvijixf.html

JS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtwdsiipmq.html

TS:   arr.join(", ")
来源：http://hz.jiagoushi.top/gteowpuwxv.html

Java: String.join(", ", list)
来源：http://hz.aizwys.cn/gtoagooeas.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydzc1.top/gtcypuwvcw.html

Ruby: arr.join(", ")
来源：http://hz.havefunace.top/gtrhdydnid.html

C#:   string.Join(", ", list)
来源：http://hz.gzhubu.top/gtblaszsmp.html

================================================================================
来源：http://hz.meibo888.top/gtiwktlwyp.html

E. 字符串处理
来源：http://hz.ivvv.top/gtptcyrlxl.html

================================================================================
来源：http://hz.gzhubu.top/gthvlbzgbg.html

[E01] 拼接字符串
来源：http://hz.hnxiangtu.top/gtefdkctbu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ppjwa.cn/gtjaaijjkv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xylfe.cn/gtztymdcbl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtpwywutpb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtbmyyophm.html


<!-- 参考信息 -->