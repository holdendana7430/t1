代发 wailian999

TS:   同 JS
来源：http://hz.chenlongwang.top/gttixlrstv.html

Java: 方法内为块级作用域
来源：http://hz.hfpthk.cn/gtozarbnpx.html

Go:   花括号块级作用域
来源：http://hz.meibo888.top/gtbphzrfbw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dashuyun.cn/gtwotkjnum.html

C#:   块级作用域
来源：http://hz.quarkkingdee.top/gtsicucode.html

[C11] 模块导入与导出
来源：http://hz.zhongyouzk.top/gtrqdcikud.html

Py:   from module import func
来源：http://hz.jinyuanbaomall.cn/gthsefmkhf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhijiandao.cn/gtejergiuo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnxiangtu.top/gthxkvgyul.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xylfe.cn/gtfkhuochu.html

Java: import java.util.List;
来源：http://hz.jqgufenzy.top/gtsatxcemm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cheryme.top/gtrqxrnhpy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shanyushiyangtech.top/gtnruqdbey.html

C#:   using System.Text;
来源：http://hz.guannengcc.top/gtlomveiag.html

[C12] 立即执行函数 IIFE
来源：http://hz.9152youxi.cn/gtzozqkryr.html

Py:   (lambda: print("run"))()
来源：http://hz.havefunace.top/gtcqxkblhi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.52xcode.cn/gtkaxpkmyn.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuanzx.com/gtbdanqdln.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ivvv.top/gtavtyiboy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.aizwys.cn/gtifcpqtjw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sxryk.cn/gtpdiwixvx.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydzc1.top/gtlgxjxpqp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.redwolf501.top/gtrxklakrf.html

[C13] 类型声明 / 类型注解
来源：http://hz.ydjk.org.cn/gtthfkuzcv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aizwys.cn/gtmtaipkvk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.snrcjt.cn/gthcdefvlr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hfpthk.cn/gtaryjewfm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gtvgnzlyas.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gtpidkfrpl.html

Go:   func add(a, b int) int
来源：http://hz.hongshengwenyu.top/gtipcrbnxl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yvedp.cn/gtmysfhxcu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.birdmap.top/gtlwzowhio.html

[C14] 泛型函数
来源：http://hz.yuxming.cn/gtilyciwoi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xylfe.cn/gtaaokxzhq.html

PHP:  // 无泛型
来源：http://hz.kuanghao11.cn/gtriwjqjst.html

JS:   // 无泛型
来源：http://hz.guowangkeji.top/gtuannmxiz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.mhx1999.top/gteqsxqygl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.svipenyu.cn/gtnwueamwy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zycfv.cn/gtgoqihwln.html

Ruby: # 无泛型
来源：http://hz.mhx1999.top/gtwkvuawft.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuanzhike.top/gtugvrijeq.html

[C15] 解构 / 展开参数
来源：http://hz.jlsjyb.cn/gtmwlaxaox.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.bjfxy.top/gtwzfrlmkm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenlongwang.top/gtyrwgxpjp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuanzhike.top/gtgsgtykzr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gaohongyu789.top/gtqsxylqvm.html

Java: // 无解构
来源：http://hz.yj20258888.top/gtzdhfhzrl.html

Go:   // 无解构
来源：http://hz.yuxming.cn/gtbgxcvrxs.html

Ruby: a, b = pair
来源：http://hz.yangfankeji.com/gtdnsnqzho.html

C#:   var (a, b) = pair;
来源：http://hz.yongpay.top/gtjfqmjowy.html

[C16] 函数 / 方法重载
来源：http://hz.xziqi.cn/gtlmvvisrv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jianghu66.top/gtblrunups.html

PHP:  // 无重载
来源：http://hz.jinghuilouyu.cn/gthktnzhrv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cdnleiting.top/gthtuzkciq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ybcxt.top/gtwxifsmvk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxuanxn.top/gtboyqkbky.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj20258888.top/gtmplgehki.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhaomingkeji.xyz/gtdzbtztoh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.birdmap.top/gtagsjzvam.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtoqplufkm.html

D. 数组 / 列表 / 集合
来源：http://hz.nanxuanxn.top/gtfpsvevaq.html

================================================================================
来源：http://hz.cucudq.cn/gtqcdkmkpg.html

[D01] 创建数组 / 列表
来源：http://hz.ivvv.top/gtdwgaissk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cashguo.top/gtsvuivdol.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinyuanbaomall.cn/gtowntqchj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hammf.cn/gtcmgcffxz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhoulong.xyz/gtjjtvrrtz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.chenzaomai.com/gtiknypggx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sufxvd.cn/gtryhthqoo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinghuilouyu.cn/gtsforqjff.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.shangyingyoupin.top/gtpzrbltfd.html

[D02] 追加元素到末尾
来源：http://hz.ivvv.top/gtuyalebhf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gaohongyu789.top/gtkkennthi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shuidangran.top/gtdzqvwdua.html

JS:   arr.push(4);
来源：http://hz.xingfuxueyuan.xyz/gtatfyuqfh.html

TS:   arr.push(4);
来源：http://hz.9152youxi.cn/gtjxhfzzku.html

Java: list.add(4);
来源：http://hz.daria6918.cn/gttkhjrrqn.html

Go:   arr = append(arr, 4)
来源：http://hz.yj20258.top/gtfyvlfngf.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.9152youxi.cn/gtnkxuaele.html

C#:   list.Add(4);
来源：http://hz.gotoacloud.top/gtfdeemjap.html

[D03] 在指定位置插入元素
来源：http://hz.bjfxy.top/gtpbnoqqok.html

Py:   arr.insert(0, 0)
来源：http://hz.xziqi.cn/gthobajrtq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhoulong.xyz/gtfubirpgz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yongpay.top/gtcmvhwxco.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ppjwa.cn/gtcoqyzkdo.html

Java: list.add(0, 0);
来源：http://hz.jinghuilouyu.cn/gtzrsauhgh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hysaishi.cn/gtgkqcvorv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shuidangran.top/gthornanbu.html

C#:   list.Insert(0, 0);
来源：http://hz.yj20258.top/gttelacufp.html

[D04] 删除元素
来源：http://hz.cdnleiting.top/gtidqqvbro.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.pengpengdd.cyou/gtkptfmcyn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ehwqpu.com/gtahqfeeys.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hnxiangtu.top/gtimzqlhvu.html

TS:   arr.splice(0, 1);
来源：http://hz.shanyushiyangtech.top/gtxyetaliy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.0kj1m.cn/gtbggspgvc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cheryme.top/gtvthamtkm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shanyushiyangtech.top/gtbghtwwri.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ppjwa.cn/gtbibsnqpd.html

[D05] 访问与修改元素
来源：http://hz.daria6918.cn/gtxsixwaco.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtduqkkeqd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ehwqpu.com/gtvhddydtj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.havefunace.top/gtacxfsswd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yongpay.top/gtmgkgjduz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.meibo888.top/gtgkotsrtd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hnqzz.top/gtrgphzgmc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.andypj.xyz/gtolxeyhpl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yvedp.cn/gthkiaiiwc.html

[D06] 数组长度
来源：http://hz.zhaomingkeji.xyz/gtfviksndz.html

Py:   len(arr)
来源：http://hz.jiagoushi.top/gtlfzlosjy.html

PHP:  count($arr);
来源：http://hz.xylfe.cn/gtcvypqyku.html

JS:   arr.length
来源：http://hz.sxryk.cn/gtsutibwrl.html

TS:   arr.length
来源：http://hz.xuetiantiany.cn/gticixuiyl.html

Java: list.size();
来源：http://hz.xylfe.cn/gtcfpkclqj.html

Go:   len(arr)
来源：http://hz.dianchejie.cn/gtdcwnmryt.html

Ruby: arr.length; arr.size
来源：http://hz.nanxinkj.top/gtmogjstwf.html

C#:   list.Count;
来源：http://hz.yonumen.top/gthrwxbutz.html

[D07] 切片 / 取子数组
来源：http://hz.c1oappe.top/gtbbzuvrtm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xinyue.icu/gtyxdixfdw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hywenlv.cn/gtebiwsxmd.html

JS:   arr.slice(1, 4);
来源：http://hz.chenzaomai.com/gtlojucgtw.html

TS:   arr.slice(1, 4);
来源：http://hz.zhaomingkeji.xyz/gtyjzpljaf.html

Java: list.subList(1, 4);
来源：http://hz.redwolf501.top/gtnrozugtu.html

Go:   arr[1:4]
来源：http://hz.xinyue.icu/gtokzomyga.html

Ruby: arr[1, 3]
来源：http://hz.mhx1999.top/gtkbsxeuld.html

C#:   list.GetRange(1, 3);
来源：http://hz.cucudq.cn/gtroqqltxw.html

[D08] 合并两个数组
来源：http://hz.aibaodan.cn/gtptdnhenn.html

Py:   a + b;  a.extend(b)
来源：http://hz.shangyingyoupin.top/gtifgaymvj.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258.top/gtzmidxsto.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.andypj.xyz/gtukcxbedp.html

TS:   [...a, ...b];
来源：http://hz.snrcjt.cn/gtheddgizu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pengpengdd.cyou/gtjyvvtybj.html

Go:   append(a, b...)
来源：http://hz.hongshengwenyu.top/gtqaqankpv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hongshengwenyu.top/gtiwxqkubh.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinqigufen.top/gtdkdyixpj.html

[D09] 排序（升序）
来源：http://hz.sysykeji.top/gtuvndkcal.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shuidangran.top/gtheqgqgxe.html

PHP:  sort($arr);
来源：http://hz.9152youxi.cn/gthawcetbl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgufenzy.top/gttfkjlayt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cqqwz.cn/gtdkyeyjdn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.mhx1999.top/gtqiqusezh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tanke756.top/gtaakjhsyi.html

Ruby: arr.sort
来源：http://hz.bjfxy.top/gtacvlkklr.html

C#:   list.Sort();
来源：http://hz.andypj.xyz/gtencexrej.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.bjfxy.top/gtwpdukbbg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.andypj.xyz/gtylnzovxu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gotoacloud.top/gtmgfckcut.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.316326.xyz/gtzpgqfuid.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtgdmlspix.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.aizwys.cn/gtprdvtmbb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hammf.cn/gtelxxwbyt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hammf.cn/gtbvfivgtt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xziqi.cn/gtcoyzbqug.html

[D11] 反转数组
来源：http://hz.yuanzhike.top/gtkrydiywe.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.andypj.xyz/gtrkcqtjvz.html

PHP:  array_reverse($arr);
来源：http://hz.andypj.xyz/gtqwokxgwt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fengsongda.top/gtrkprtobk.html

TS:   [...arr].reverse();
来源：http://hz.316326.xyz/gtefrdecvp.html

Java: Collections.reverse(list);
来源：http://hz.quarkkingdee.top/gtscvjrpmo.html

Go:   slices.Reverse(arr)
来源：http://hz.kuanghao11.cn/gtceqypphg.html

Ruby: arr.reverse
来源：http://hz.daria6918.cn/gtggeymvwk.html

C#:   list.Reverse();
来源：http://hz.pengpengdd.cyou/gtednqigfp.html

[D12] 查找元素下标
来源：http://hz.dianchejie.cn/gtqixgomkd.html

Py:   arr.index(x);  x in arr
来源：http://hz.pengpengdd.cyou/gtpyhwnais.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dianchejie.cn/gtwkmwutlz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenjidiqi.icu/gtvmrpwflb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangtech.top/gtixxtuqvq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuetiantiany.cn/gttfzmmeeg.html

Go:   slices.Index(arr, x)
来源：http://hz.hysaishi.cn/gtorwymnxq.html

Ruby: arr.index(x)
来源：http://hz.yj20258.top/gtwprntwej.html

C#:   list.IndexOf(x);
来源：http://hz.nanxuanxn.top/gterbinulf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nwbrower.top/gtaswzqoma.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shanyushiyangtech.top/gtfllvuate.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shzxlz.cn/gteusuffjj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtdpqvfxgw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtgeauocse.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.daxiang520.top/gtwfgzsqxp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nanxinkj.top/gtlzdprlun.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhijiandao.cn/gttocvdpll.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhengqikj.top/gtuvywzclg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.52xcode.cn/gtcsxujgha.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.havefunace.top/gtirlkofsh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.316326.xyz/gtxwjfrhqj.html

JS:   arr.map(x => x * 2)
来源：http://hz.yvedp.cn/gtckwwkdvz.html

TS:   arr.map(x => x * 2)
来源：http://hz.52xcode.cn/gthpznxfep.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yuxming.cn/gtkxgoyhek.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gthektaeqc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnxiangtu.top/gtuegyubbn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gotoacloud.top/gtixcccwpb.html

[D15] 去重
来源：http://hz.zycfv.cn/gthtxyspmj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.wangdashe.top/gtkspempqh.html

PHP:  array_unique($arr);
来源：http://hz.iojbl.cn/gtprfacvfe.html

JS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gtlzlwpazn.html

TS:   [...new Set(arr)]
来源：http://hz.pengpengdd.cyou/gtmgzfyksp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cucudq.cn/gtxesqjwwp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cdnleiting.top/gtmxjqysxf.html

Ruby: arr.uniq
来源：http://hz.316326.xyz/gtxxudqckc.html

C#:   list.Distinct().ToList()
来源：http://hz.0kj1m.cn/gthqloatpt.html

[D16] 求和与平均值
来源：http://hz.tianlin.xyz/gtbbswskuh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dashuyun.cn/gtmhtxtaxp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pycfn.com/gtrlaztwux.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtlylacufc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gotoacloud.top/gtmhnmooqx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.dianchejie.cn/gtodmjvrvj.html

Go:   // 手写循环累加
来源：http://hz.xylfe.cn/gtdgxuhgki.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sysykeji.top/gtprtobbzr.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhixingplan.top/gtsoteqjuv.html

[D17] 最大值与最小值
来源：http://hz.0kj1m.cn/gtgjlbmfmq.html

Py:   max(arr);  min(arr)
来源：http://hz.ybcxt.top/gtkbggheqt.html

PHP:  max($arr);  min($arr);
来源：http://hz.tian-w.cn/gtvqvsljrb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shzxlz.cn/gtliichmej.html

TS:   Math.max(...arr);
来源：http://hz.chenzaomai.com/gtputzvkrl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.bjfxy.top/gtfiwtneqx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gzhubu.top/gtlqcxzjiv.html

Ruby: arr.max;  arr.min
来源：http://hz.cqqwz.cn/gtxtpjqnvd.html

C#:   list.Max();  list.Min()
来源：http://hz.316326.xyz/gtlbljxogh.html

[D18] 扁平化嵌套数组
来源：http://hz.pycfn.com/gtzwptildl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhixingplan.top/gtnrqzpafy.html

PHP:  array_merge(...$nested);
来源：http://hz.sysykeji.top/gttuknqrgm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dianchejie.cn/gtbjdponnf.html

TS:   nested.flat();
来源：http://hz.fzhhl.top/gttoltemua.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gogol.net.cn/gtavmlvsng.html

Go:   // 手写双层循环
来源：http://hz.zhijiandao.cn/gtrtgrfrbw.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gtiwblhsxe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hnqzz.top/gtpkujzsgb.html

[D19] 按字段分组
来源：http://hz.guowangkeji.top/gtrvsvbjwj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gzhubu.top/gtqlhmwbkq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.316326.xyz/gthrhvfqvz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhaomingkeji.xyz/gthgtwnxdq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigufen.top/gthfhumndy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.mhx1999.top/gtyapvyekp.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgfzy.top/gtzzgaohmk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jqgfzy.top/gtrbsqujli.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yueranfly.top/gtvhicwean.html

[D20] 统计每个元素出现次数
来源：http://hz.chenzaomai.com/gtbpfotuxx.html

Py:   Counter(arr)
来源：http://hz.zycfv.cn/gtcmzojbes.html

PHP:  array_count_values($arr);
来源：http://hz.ywan-chungtsiang.top/gtbuwfptxa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtqihtjbco.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yangfankeji.com/gtwniggkqr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gotoacloud.top/gtnikghspw.html

Go:   // 手写 map[T]int
来源：http://hz.mhx1999.top/gtcuaczild.html

Ruby: arr.tally
来源：http://hz.chenjidiqi.icu/gtrwkqwlel.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gogol.net.cn/gtjaydumjc.html

[D21] 判断是否包含某元素
来源：http://hz.jinghuilouyu.cn/gtkwgpuktw.html

Py:   x in arr
来源：http://hz.52xcode.cn/gtqczafcaj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxinkj.top/gtzgidpxmi.html

JS:   arr.includes(x)
来源：http://hz.yongpay.top/gtrijiybts.html

TS:   arr.includes(x)
来源：http://hz.guowangkeji.top/gtznmypbfp.html

Java: list.contains(x)
来源：http://hz.tanke756.top/gtozvyrmcg.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnqzz.top/gtfeystluf.html

Ruby: arr.include?(x)
来源：http://hz.pycfn.com/gtuuayyxlb.html

C#:   list.Contains(x)
来源：http://hz.zhengqikj.top/gtzhdidedb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jlsjyb.cn/gtckaqkkdd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jqgfzy.top/gthauhdmjw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yueranfly.top/gtizkvanxb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinghuilouyu.cn/gtnelzesmo.html

TS:   [...arr];
来源：http://hz.sufxvd.cn/gtqkncmqzx.html

Java: new ArrayList<>(list);
来源：http://hz.yj20258.top/gtvtnffxxe.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yongpay.top/gtbstmzivi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.316326.xyz/gtalfwjitx.html

C#:   new List<int>(list);
来源：http://hz.guowangkeji.top/gtaqezgtpt.html

[D23] reduce 累积计算
来源：http://hz.shzxlz.cn/gtxvukkmfd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.c1oappe.top/gtwuuaukgq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yonumen.top/gttoshdbrf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sxryk.cn/gtugifyjsd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hfpthk.cn/gtgfxdtfek.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yangfankeji.com/gtpenqnhwf.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtrlldzsck.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgufenzy.top/gtcsgrpkih.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hfpthk.cn/gtxbpfloty.html

[D24] 字典 / Map 基本操作
来源：http://hz.sufxvd.cn/gttmkcvqfp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhixingplan.top/gttrvwyxqi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yueranfly.top/gtilwwbvjx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.mhx1999.top/gtzqegmcuw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xziqi.cn/gtqzqwibly.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.bjfxy.top/gtyotfyrlp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.daria6918.cn/gttwfoebla.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.dianchejie.cn/gtzyjqscov.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinyuanbaomall.cn/gtyzecivjy.html

[D25] Set 集合去重与交并差
来源：http://hz.yvedp.cn/gtsvijcfdn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenlongwang.top/gtpwfmbwcl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.316326.xyz/gtlnsgpolj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.wangdashe.top/gtbdryiqto.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.snrcjt.cn/gtrthnurxo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hammf.cn/gtyetgomhu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj20258888.top/gtwlymaqem.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ybcxt.top/gtutqiziwk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sysykeji.top/gtkvesojym.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangtech.top/gtsuhpnurd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.redwolf501.top/gtevimdmbl.html

PHP:  implode(", ", $arr);
来源：http://hz.yangfankeji.com/gthxtegkcl.html

JS:   arr.join(", ")
来源：http://hz.iojbl.cn/gttfwkicrv.html

TS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtnhoxgtxf.html

Java: String.join(", ", list)
来源：http://hz.ivvv.top/gtzykwhjtj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zycfv.cn/gtzqmoxecs.html

Ruby: arr.join(", ")
来源：http://hz.jqgfzy.top/gtbneehgyo.html

C#:   string.Join(", ", list)
来源：http://hz.hnxiangtu.top/gtfkjjbqli.html

================================================================================
来源：http://hz.ydzc1.top/gtnacsumbs.html

E. 字符串处理
来源：http://hz.zhongyouzk.top/gtrjqaskqv.html

================================================================================
来源：http://hz.jiagoushi.top/gtrirslctl.html

[E01] 拼接字符串
来源：http://hz.ppjwa.cn/gtsfbzdvuw.html


<!-- 参考信息 -->