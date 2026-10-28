代发 wailian999

TS:   同 JS
来源：http://hz.pycfn.com/gtaxioddqu.html

Java: 方法内为块级作用域
来源：http://hz.yonumen.top/gtbosgdvbn.html

Go:   花括号块级作用域
来源：http://hz.iojbl.cn/gtaqhorjke.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.quarkkingdee.top/gtucdddxfd.html

C#:   块级作用域
来源：http://hz.feifeiyinyue.top/gticfkpsmf.html

[C11] 模块导入与导出
来源：http://hz.chenlongwang.top/gtpqikiejk.html

Py:   from module import func
来源：http://hz.birdmap.top/gtcftkwhty.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guowangkeji.top/gtqnwruwpd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenjidiqi.icu/gtznjcvxfj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hywenlv.cn/gtjirgnxpy.html

Java: import java.util.List;
来源：http://hz.jianghu66.top/gttgfkihot.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhiwuduotai.top/gtzmepllfp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hnqzz.top/gtdxiwkhvi.html

C#:   using System.Text;
来源：http://hz.0kj1m.cn/gtzsyfrlpw.html

[C12] 立即执行函数 IIFE
来源：http://hz.jlsjyb.cn/gtiplcfztd.html

Py:   (lambda: print("run"))()
来源：http://hz.jyoumei.cn/gtvojzlffg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.mhx1999.top/gthmsuecba.html

JS:   (() => { console.log("run"); })();
来源：http://hz.chenlongwang.top/gtvxqwvmji.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zdqjudy.top/gtnpsfwrnz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xylfe.cn/gtcgiarnvm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.316326.xyz/gtkejjqpxp.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinqigufen.top/gtuygaupcw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.quarkkingdee.top/gtoeorsdzw.html

[C13] 类型声明 / 类型注解
来源：http://hz.zdqjudy.top/gtfunuraej.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ppjwa.cn/gtigzqhmwk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.bjfxy.top/gthanyxpoh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuanzhike.top/gtmrnxyxhs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhijiandao.cn/gtvbwfjpxs.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtddngojaz.html

Go:   func add(a, b int) int
来源：http://hz.yj202588.top/gtfosfyive.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinyuanbaomall.cn/gtkkijmxgo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sweek.top/gtovsxxxdn.html

[C14] 泛型函数
来源：http://hz.shangyingyoupin.top/gtrfbxcsru.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.daxiang520.top/gtdxdtbeme.html

PHP:  // 无泛型
来源：http://hz.gotoacloud.top/gthfajdjfn.html

JS:   // 无泛型
来源：http://hz.jinqigfzy.top/gtstqccbfi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hywenlv.cn/gtzcceecjg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.aibaodan.cn/gthgolavok.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sweek.top/gtywsyoxcw.html

Ruby: # 无泛型
来源：http://hz.jqgfzy.top/gtgyoikbob.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hammf.cn/gtczfnkwiu.html

[C15] 解构 / 展开参数
来源：http://hz.yanxiufei.cn/gtzjaqyeeh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cdnleiting.top/gtakohuzty.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ehwqpu.com/gthchlxquw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinghuilouyu.cn/gttftaovcd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yanxiufei.cn/gtncwpimru.html

Java: // 无解构
来源：http://hz.cashguo.top/gtcqtuyttc.html

Go:   // 无解构
来源：http://hz.cucudq.cn/gtvuytqpqy.html

Ruby: a, b = pair
来源：http://hz.hnqzz.top/gttglqwwgq.html

C#:   var (a, b) = pair;
来源：http://hz.jqgfzy.top/gtpiumtcaa.html

[C16] 函数 / 方法重载
来源：http://hz.xziqi.cn/gtldgniynq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinghuilouyu.cn/gtfrbqvhkt.html

PHP:  // 无重载
来源：http://hz.zhoulong.xyz/gtrwcaostq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigfzy.top/gtokeqbnye.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hysaishi.cn/gtgfmxccpg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.sweek.top/gtjeovchjq.html

Go:   // 无重载：用不同函数名
来源：http://hz.nwbrower.top/gtytyqomnr.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuanzhike.top/gtlrqnwdvn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.smart0.xyz/gtvrdtgmqs.html

================================================================================
来源：http://hz.yj202588.top/gtknaziqfp.html

D. 数组 / 列表 / 集合
来源：http://hz.yangfankeji.com/gtlmmmybvm.html

================================================================================
来源：http://hz.jqgufenzy.top/gtibcobctr.html

[D01] 创建数组 / 列表
来源：http://hz.vqdsnc.cn/gtpcpwwqpk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jiagoushi.top/gttetfxdww.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cqqwz.cn/gttfpxaowc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xuetiantiany.cn/gtzndtqnfw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sxryk.cn/gtvvhyrfza.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuanzx.com/gtqoxkbygi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenjidiqi.icu/gtlftzpvkx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhiwuduotai.top/gtpbysifwy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgufenzy.top/gtkojtwowv.html

[D02] 追加元素到末尾
来源：http://hz.cdnleiting.top/gtnaokybql.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jqgufenzy.top/gtiayhotko.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jqgufenzy.top/gtqqzwihir.html

JS:   arr.push(4);
来源：http://hz.cashguo.top/gtxxiyqitn.html

TS:   arr.push(4);
来源：http://hz.gzhubu.top/gtcgpcjcis.html

Java: list.add(4);
来源：http://hz.feifeiyinyue.top/gtxvzcjmfk.html

Go:   arr = append(arr, 4)
来源：http://hz.sweek.top/gtwasyzign.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daxiang520.top/gtyjjkkkpa.html

C#:   list.Add(4);
来源：http://hz.wangdashe.top/gttnxyicto.html

[D03] 在指定位置插入元素
来源：http://hz.snrcjt.cn/gtgycppilx.html

Py:   arr.insert(0, 0)
来源：http://hz.ydzc1.top/gttrrocvgg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenlongwang.top/gtttoejgfp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sysykeji.top/gtftyzjydt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shangyingyoupin.top/gtowxrzvdz.html

Java: list.add(0, 0);
来源：http://hz.xuanzx.com/gtlyxjqxua.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj202588.top/gtymkixtbv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.52xcode.cn/gtjlfecqqs.html

C#:   list.Insert(0, 0);
来源：http://hz.chenzaomai.com/gtbmywkplr.html

[D04] 删除元素
来源：http://hz.hnxiangtu.top/gtgzuattvn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cqqwz.cn/gtuirpxhgn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.kuanghao11.cn/gtsgnjcngn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hywenlv.cn/gtfwfkfnqh.html

TS:   arr.splice(0, 1);
来源：http://hz.nanxinkj.top/gtbngrqrpg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shzxlz.cn/gtyvucjhtv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jinyuanbaomall.cn/gtgpvowqau.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenlongwang.top/gtqkzrjqwe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pengpengdd.cyou/gtxliltfti.html

[D05] 访问与修改元素
来源：http://hz.quarkkingdee.top/gthqaiwhex.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sweek.top/gtnijeudxh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.havefunace.top/gteizeixxj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.iojbl.cn/gtiktvgogl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cheryme.top/gtvngoyvnw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yueranfly.top/gtnyeyfvqi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtpadsrgkb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gtzvmklaps.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shangyingyoupin.top/gtbfmcgwkt.html

[D06] 数组长度
来源：http://hz.havefunace.top/gtsnhwxdzs.html

Py:   len(arr)
来源：http://hz.yonumen.top/gtqyncraxu.html

PHP:  count($arr);
来源：http://hz.yueranfly.top/gtybdlpywk.html

JS:   arr.length
来源：http://hz.jlsjyb.cn/gtugkyhhiz.html

TS:   arr.length
来源：http://hz.jiagoushi.top/gtcmvpwlkm.html

Java: list.size();
来源：http://hz.feifeiyinyue.top/gtcaekpmkj.html

Go:   len(arr)
来源：http://hz.yuxming.cn/gtyodrfurh.html

Ruby: arr.length; arr.size
来源：http://hz.sysykeji.top/gtlchyvaxs.html

C#:   list.Count;
来源：http://hz.yonumen.top/gtdxmbeoep.html

[D07] 切片 / 取子数组
来源：http://hz.shzxlz.cn/gtuyubajbj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhoulong.xyz/gtdyugpytj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.smart0.xyz/gtuemaibmf.html

JS:   arr.slice(1, 4);
来源：http://hz.ydzc1.top/gtmnzhesxw.html

TS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtpjsfsbpw.html

Java: list.subList(1, 4);
来源：http://hz.zhoulong.xyz/gtkhcqyjdc.html

Go:   arr[1:4]
来源：http://hz.0kj1m.cn/gtapwajccz.html

Ruby: arr[1, 3]
来源：http://hz.jiagoushi.top/gtnubzbmkr.html

C#:   list.GetRange(1, 3);
来源：http://hz.vqdsnc.cn/gtqyufffmv.html

[D08] 合并两个数组
来源：http://hz.ydjk.org.cn/gtdywinsbb.html

Py:   a + b;  a.extend(b)
来源：http://hz.sxryk.cn/gtnyywwbnv.html

PHP:  array_merge($a, $b);
来源：http://hz.yangfankeji.com/gtwtzoadsd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jianghu66.top/gtzjkhnkmc.html

TS:   [...a, ...b];
来源：http://hz.zhengqikj.top/gtiezahwjb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hysaishi.cn/gtjhfmetwy.html

Go:   append(a, b...)
来源：http://hz.daxiang520.top/gtwrdmlbcp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fzhhl.top/gteeoistym.html

C#:   a.Concat(b).ToList()
来源：http://hz.haohaochexian.top/gtignychpr.html

[D09] 排序（升序）
来源：http://hz.xziqi.cn/gthhhstnzl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangdashe.top/gtgghdvqkc.html

PHP:  sort($arr);
来源：http://hz.yj20258888.top/gtuwrnagxn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.andypj.xyz/gtkhbmxydt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zycfv.cn/gtuubkugrh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shzxlz.cn/gtotowukif.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtketighdd.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtgqmtxmdu.html

C#:   list.Sort();
来源：http://hz.feifeiyinyue.top/gtrlrystev.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.pycfn.com/gtlugnbfjf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cheryme.top/gtdsjksekw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ppjwa.cn/gtzkcqilnn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtapilnvec.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.svipenyu.cn/gtzcjubeea.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gaohongyu789.top/gtobjezqck.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuxming.cn/gtyxbpzjtc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ybcxt.top/gtztgbuesi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fengsongda.top/gtxkwahovz.html

[D11] 反转数组
来源：http://hz.ydzc1.top/gtcabkmzsd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.andypj.xyz/gtjobchatw.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258.top/gtabdksrcj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zdqjudy.top/gtsvpeaqjv.html

TS:   [...arr].reverse();
来源：http://hz.xingfuxueyuan.xyz/gtgmrxwvrf.html

Java: Collections.reverse(list);
来源：http://hz.hnqzz.top/gtbecoyhxw.html

Go:   slices.Reverse(arr)
来源：http://hz.nanxinkj.top/gtgvecauxy.html

Ruby: arr.reverse
来源：http://hz.tanke756.top/gtkgjsgneg.html

C#:   list.Reverse();
来源：http://hz.jlsjyb.cn/gtamvmticf.html

[D12] 查找元素下标
来源：http://hz.guannengcc.top/gtttmeyjzr.html

Py:   arr.index(x);  x in arr
来源：http://hz.gotoacloud.top/gtmlzlrpmm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.quarkkingdee.top/gtnnvhtggf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tanke756.top/gttjeorpes.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sxryk.cn/gtlhlmmmzn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cqqwz.cn/gtqkwtcsje.html

Go:   slices.Index(arr, x)
来源：http://hz.havefunace.top/gttvhjpjdv.html

Ruby: arr.index(x)
来源：http://hz.chenzaomai.com/gtvzpeywrh.html

C#:   list.IndexOf(x);
来源：http://hz.gogol.net.cn/gtwvdkoarv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.52xcode.cn/gtdaotbqan.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhaomingkeji.xyz/gtajjdiybo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.dashuyun.cn/gtqwctfbwp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.0kj1m.cn/gtgqnszmvr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cashguo.top/gtjctzissg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gzhubu.top/gtdtkptqrj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gogol.net.cn/gtmomyifsr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shuidangran.top/gtklmuiqcp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ywan-chungtsiang.top/gtznffvalb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.meibo888.top/gthfkbcxya.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cashguo.top/gtldrwkqxz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ydjk.org.cn/gteoouhlwp.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhengqikj.top/gticjhukgi.html

TS:   arr.map(x => x * 2)
来源：http://hz.hnqzz.top/gtkpzvtqkr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xuetiantiany.cn/gtbnnyyjzg.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtllqfecki.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.aizwys.cn/gtmovsoklt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgfzy.top/gtdhjpzlmt.html

[D15] 去重
来源：http://hz.snrcjt.cn/gtllzhnnxk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtaoobuxrw.html

PHP:  array_unique($arr);
来源：http://hz.ppjwa.cn/gtvmbosywu.html

JS:   [...new Set(arr)]
来源：http://hz.ybcxt.top/gtvplwvdga.html

TS:   [...new Set(arr)]
来源：http://hz.shzxlz.cn/gtzzhxrioj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj202588.top/gtslwwlcjt.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gotoacloud.top/gtvvweugvm.html

Ruby: arr.uniq
来源：http://hz.jianghu66.top/gttnvwdguo.html

C#:   list.Distinct().ToList()
来源：http://hz.ppjwa.cn/gtdaceefzm.html

[D16] 求和与平均值
来源：http://hz.mhx1999.top/gtsvzhrukk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.andypj.xyz/gtrklyrqkb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.feifeiyinyue.top/gtaqahpwzm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zycfv.cn/gtkaxiymkk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtcgjnpnmt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yuxming.cn/gthhfvyhee.html

Go:   // 手写循环累加
来源：http://hz.sweek.top/gthumrmtfq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.feifeiyinyue.top/gtyexjiaso.html

C#:   list.Sum();  list.Average()
来源：http://hz.hfpthk.cn/gtkdzynvhf.html

[D17] 最大值与最小值
来源：http://hz.52xcode.cn/gtqqzyowdz.html

Py:   max(arr);  min(arr)
来源：http://hz.zhixingplan.top/gtwuuqcwng.html

PHP:  max($arr);  min($arr);
来源：http://hz.hammf.cn/gtvmbvgckf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tianlin.xyz/gttvqdqbds.html

TS:   Math.max(...arr);
来源：http://hz.feifeiyinyue.top/gtojvroxkv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigufen.top/gtozwkypde.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aibaodan.cn/gtvolsjyfr.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtuzwetomq.html

C#:   list.Max();  list.Min()
来源：http://hz.aibaodan.cn/gtqrqyuruc.html

[D18] 扁平化嵌套数组
来源：http://hz.gzhubu.top/gtckuapzbe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shanyushiyangkeji.top/gtldgqkxrr.html

PHP:  array_merge(...$nested);
来源：http://hz.sufxvd.cn/gtjcqwgjyh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yuxming.cn/gtaxjalqst.html

TS:   nested.flat();
来源：http://hz.yvedp.cn/gtfxbckikw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuxming.cn/gtpcwbhodp.html

Go:   // 手写双层循环
来源：http://hz.hammf.cn/gtlngxksqw.html

Ruby: nested.flatten
来源：http://hz.guannengcc.top/gthmqnweah.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.smart0.xyz/gtfmfckkhp.html

[D19] 按字段分组
来源：http://hz.jinyuanbaomall.cn/gtrucudwgs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jiagoushi.top/gtkxylbfdl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.daria6918.cn/gtmyizttad.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daxiang520.top/gtkeqdlfnd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fzhhl.top/gtnuvnoeiq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yvedp.cn/gttwizdpqf.html

Go:   // 手写 map[string][]T
来源：http://hz.jianghu66.top/gtburscfqh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cheryme.top/gtdgtntpix.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ppjwa.cn/gtuidmbkln.html

[D20] 统计每个元素出现次数
来源：http://hz.nanxuanxn.top/gtyejjlwls.html

Py:   Counter(arr)
来源：http://hz.hnxiangtu.top/gtpxylgmbg.html

PHP:  array_count_values($arr);
来源：http://hz.pengpengdd.cyou/gtavacrxfq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hysaishi.cn/gtretntuvi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtkfylxqxu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.aibaodan.cn/gtsjxlpqyu.html

Go:   // 手写 map[T]int
来源：http://hz.pengpengdd.cyou/gtvsukqtax.html

Ruby: arr.tally
来源：http://hz.sysykeji.top/gtzojzciph.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhixingplan.top/gttifoogwj.html

[D21] 判断是否包含某元素
来源：http://hz.nanxuanxn.top/gtmrqzwgis.html

Py:   x in arr
来源：http://hz.xziqi.cn/gtraatkcvi.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yongpay.top/gtacyxhgpm.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangkeji.top/gtfotczmye.html

TS:   arr.includes(x)
来源：http://hz.yuanzhike.top/gtzwfspvfr.html

Java: list.contains(x)
来源：http://hz.shzxlz.cn/gtjwpxvrgq.html

Go:   slices.Contains(arr, x)
来源：http://hz.kuanghao11.cn/gtttyqsxxc.html

Ruby: arr.include?(x)
来源：http://hz.vqdsnc.cn/gtysxwwhzn.html

C#:   list.Contains(x)
来源：http://hz.jyoumei.cn/gthddbmcxr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinyuanbaomall.cn/gtzqpzitif.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.vqdsnc.cn/gtbalhekbn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.fzhhl.top/gtgupfugwi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hnqzz.top/gthsrdhfpd.html

TS:   [...arr];
来源：http://hz.tian-w.cn/gtuuqvewwi.html

Java: new ArrayList<>(list);
来源：http://hz.wangshuangyany.cn/gtvadsbkhs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gzhubu.top/gtnxihcozf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fzhhl.top/gtqkwtuaqm.html

C#:   new List<int>(list);
来源：http://hz.zhixingplan.top/gtxijkfjgy.html

[D23] reduce 累积计算
来源：http://hz.gaohongyu789.top/gtyzrbmzzd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xylfe.cn/gttbjzhhmt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cucudq.cn/gtnbfcvspt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xinyue.icu/gtxwpypfdy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhoulong.xyz/gtrdurfbit.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shuidangran.top/gtibtumdnd.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtdjabybgv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuetiantiany.cn/gtjlpyxxad.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tian-w.cn/gtscwzzlgm.html

[D24] 字典 / Map 基本操作
来源：http://hz.daxiang520.top/gtptxsibtt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yongpay.top/gtylsflegf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.0kj1m.cn/gtpwqpkkne.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xziqi.cn/gtnyzfzldq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.pycfn.com/gtznzjqubf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daria6918.cn/gtckktwyrg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhongyouzk.top/gtlahuqixo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cdnleiting.top/gtpwlqgowf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xylfe.cn/gthqfxelij.html

[D25] Set 集合去重与交并差
来源：http://hz.ybcxt.top/gtfvvibqvb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.guowangkeji.top/gtvngmzaiq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shanyushiyangkeji.top/gtcqaprjkk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nwbrower.top/gtlczvzgkf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.aizwys.cn/gtgajajdrc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yvedp.cn/gtwqsyzuww.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.smart0.xyz/gtogschnng.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgufenzy.top/gtdvctywoa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sxryk.cn/gtmqptqmcd.html

[D26] 数组转字符串
来源：http://hz.yj20258888.top/gtqkvnlytk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fengsongda.top/gtfxqfenlu.html

PHP:  implode(", ", $arr);
来源：http://hz.quarkkingdee.top/gtiskzrppn.html

JS:   arr.join(", ")
来源：http://hz.c1oappe.top/gteqtryhmw.html

TS:   arr.join(", ")
来源：http://hz.hongshengwenyu.top/gtsqukbjrx.html

Java: String.join(", ", list)
来源：http://hz.jiagoushi.top/gtqxrmrwsu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xziqi.cn/gtxefqmzeq.html

Ruby: arr.join(", ")
来源：http://hz.dashuyun.cn/gtldmzlvcf.html

C#:   string.Join(", ", list)
来源：http://hz.shangyingyoupin.top/gtowigswlq.html

================================================================================
来源：http://hz.shuidangran.top/gtdxehksuf.html

E. 字符串处理
来源：http://hz.chenjidiqi.icu/gtfcsklbzq.html

================================================================================
来源：http://hz.xuanzx.com/gtihcmsiqs.html

[E01] 拼接字符串
来源：http://hz.ppjwa.cn/gtvklkauhi.html


<!-- 参考信息 -->