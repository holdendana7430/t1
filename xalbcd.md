代发 wailian999

C#:   块级作用域
来源：http://hz.zhoulong.xyz/gtcllkblbo.html

[C11] 模块导入与导出
来源：http://hz.quarkkingdee.top/gtbafyrglf.html

Py:   from module import func
来源：http://hz.haohaochexian.top/gtygvralzl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yongpay.top/gtcnlvbkzg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuanzhike.top/gtoxxxacjy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.kuanghao11.cn/gtevzlncqq.html

Java: import java.util.List;
来源：http://hz.hysaishi.cn/gtlbyovgkk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.guowangkeji.top/gticzllkhd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.pycfn.com/gtvhnqqvrg.html

C#:   using System.Text;
来源：http://hz.zhongyouzk.top/gtqpunglfc.html

[C12] 立即执行函数 IIFE
来源：http://hz.xingfuxueyuan.xyz/gtijvlivbe.html

Py:   (lambda: print("run"))()
来源：http://hz.ppjwa.cn/gtnxwqcokh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hnqzz.top/gtikemnfsh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gtaesvydog.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cucudq.cn/gtvmptiboc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.meibo888.top/gtxmyuzjyr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.c1oappe.top/gtpivqmyte.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj20258888.top/gtlxzjgxii.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jiagoushi.top/gtnhztvskj.html

[C13] 类型声明 / 类型注解
来源：http://hz.iojbl.cn/gtdnnelhoc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.tanke756.top/gtsguyoahs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ppjwa.cn/gtumrdgpex.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jlsjyb.cn/gtgejebond.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gtljqqaoqw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtwfrtchaq.html

Go:   func add(a, b int) int
来源：http://hz.jinqigfzy.top/gthapfhfuw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.9152youxi.cn/gtwtnnscys.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.dianchejie.cn/gtqdiqkuui.html

[C14] 泛型函数
来源：http://hz.ydzc1.top/gtpkwpityc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zycfv.cn/gtkuimivbh.html

PHP:  // 无泛型
来源：http://hz.yj20258.top/gtlfyuyjyb.html

JS:   // 无泛型
来源：http://hz.ehwqpu.com/gtoylnnedu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cdnleiting.top/gtlccjolpj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigufen.top/gtazdfchhl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cucudq.cn/gtorlnlifu.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gtfolopwti.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj20258888.top/gttufwtpbt.html

[C15] 解构 / 展开参数
来源：http://hz.cdnleiting.top/gtcpkgkidx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ehwqpu.com/gtdhfblnfz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.tian-w.cn/gtrwnniple.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jqgfzy.top/gtueyrhvpn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj20258888.top/gtwatikhyh.html

Java: // 无解构
来源：http://hz.nwbrower.top/gtamnrrojg.html

Go:   // 无解构
来源：http://hz.52xcode.cn/gtkmjqvabm.html

Ruby: a, b = pair
来源：http://hz.pengpengdd.cyou/gtfzdwtwav.html

C#:   var (a, b) = pair;
来源：http://hz.xuanzx.com/gtjggwkyho.html

[C16] 函数 / 方法重载
来源：http://hz.zycfv.cn/gtnqkxfcid.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.daria6918.cn/gtgyyaxbmc.html

PHP:  // 无重载
来源：http://hz.wangshuangyany.cn/gtxztmotjs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.52xcode.cn/gttllzudbt.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ydzc1.top/gtqezjehpr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ydjk.org.cn/gtvgloqxhp.html

Go:   // 无重载：用不同函数名
来源：http://hz.chenlongwang.top/gteutcggqe.html

Ruby: # 无重载：靠动态参数
来源：http://hz.guowangkeji.top/gtrnvntdzv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhixingplan.top/gtvunigzlk.html

================================================================================
来源：http://hz.gzhubu.top/gtfmmtmjkj.html

D. 数组 / 列表 / 集合
来源：http://hz.sxryk.cn/gtlquuxbih.html

================================================================================
来源：http://hz.ppjwa.cn/gtoxhupuij.html

[D01] 创建数组 / 列表
来源：http://hz.fengsongda.top/gtwnlsthlc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yvedp.cn/gtgnxaykdc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shzxlz.cn/gtociarbth.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.nanxinkj.top/gtjlilxnxp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cashguo.top/gtwfrfcgsh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.quarkkingdee.top/gtswuqhfzk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.dianchejie.cn/gtszpvcaov.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhongyouzk.top/gtuhbmcgex.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.316326.xyz/gtsoazzbml.html

[D02] 追加元素到末尾
来源：http://hz.cashguo.top/gtvezjbxhm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenjidiqi.icu/gtoigeqllc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xinyue.icu/gtvxsnfwhk.html

JS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtuqhjdcqx.html

TS:   arr.push(4);
来源：http://hz.jyoumei.cn/gtrfnasqdb.html

Java: list.add(4);
来源：http://hz.chenlongwang.top/gtzmmatvyi.html

Go:   arr = append(arr, 4)
来源：http://hz.yanxiufei.cn/gtwfwakvye.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hnqzz.top/gtugghgrxz.html

C#:   list.Add(4);
来源：http://hz.jinqigufen.top/gtbnctbtca.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangkeji.top/gtwuxhcxka.html

Py:   arr.insert(0, 0)
来源：http://hz.yuxming.cn/gtxwzzgfrn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenjidiqi.icu/gteswxvzqv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shzxlz.cn/gtpkwvlqpc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.quarkkingdee.top/gtkpupoocr.html

Java: list.add(0, 0);
来源：http://hz.hnqzz.top/gtwxpvmecy.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cdnleiting.top/gtrakwsyms.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hywenlv.cn/gtrhksvrzn.html

C#:   list.Insert(0, 0);
来源：http://hz.yj202588.top/gtubuixfvc.html

[D04] 删除元素
来源：http://hz.ppjwa.cn/gtdtgeakdy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhixingplan.top/gtmrzgaiys.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yangfankeji.com/gtgcvwulhf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cqqwz.cn/gtgnragrxb.html

TS:   arr.splice(0, 1);
来源：http://hz.ydzc1.top/gtzhblvahp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.smart0.xyz/gtccahbuon.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zdqjudy.top/gtdyemlrts.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuanzx.com/gtnsxznbbl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangshuangyany.cn/gtuhccguay.html

[D05] 访问与修改元素
来源：http://hz.xziqi.cn/gtwnrifxdb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtwbejonai.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ivvv.top/gtbpombpqb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hnxiangtu.top/gtjsvduzft.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hfpthk.cn/gtceneoygb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhixingplan.top/gtsjusuzns.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jianghu66.top/gtoalnnmfp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xziqi.cn/gthrxlvfpn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.0kj1m.cn/gtbrqvezqi.html

[D06] 数组长度
来源：http://hz.daria6918.cn/gtrxejthsj.html

Py:   len(arr)
来源：http://hz.zhixingplan.top/gtmqpmhdch.html

PHP:  count($arr);
来源：http://hz.hnxiangtu.top/gthvmcwiim.html

JS:   arr.length
来源：http://hz.ydzc1.top/gtmdgubimp.html

TS:   arr.length
来源：http://hz.hnxiangtu.top/gtcqsnnljz.html

Java: list.size();
来源：http://hz.gogol.net.cn/gtrfiphbtm.html

Go:   len(arr)
来源：http://hz.yj20258.top/gtnxqdqtrw.html

Ruby: arr.length; arr.size
来源：http://hz.redwolf501.top/gttabgqmdm.html

C#:   list.Count;
来源：http://hz.gogol.net.cn/gtapbgwlcw.html

[D07] 切片 / 取子数组
来源：http://hz.gogol.net.cn/gtxarkrjea.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.birdmap.top/gtraahzoyc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yueranfly.top/gtqscfsvwv.html

JS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gtnrljoljo.html

TS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gtysajwwph.html

Java: list.subList(1, 4);
来源：http://hz.ydzc1.top/gtjlydjzjy.html

Go:   arr[1:4]
来源：http://hz.jinqigfzy.top/gtfgposoaq.html

Ruby: arr[1, 3]
来源：http://hz.daxiang520.top/gtvfclrsxv.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258888.top/gteqjcvvlv.html

[D08] 合并两个数组
来源：http://hz.tianlin.xyz/gtdjgsawnv.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxuanxn.top/gtxgzsrhre.html

PHP:  array_merge($a, $b);
来源：http://hz.gogol.net.cn/gtagioqqal.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cdnleiting.top/gtxtmnvbfq.html

TS:   [...a, ...b];
来源：http://hz.hywenlv.cn/gtuhvaroch.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.9152youxi.cn/gtyrfekogh.html

Go:   append(a, b...)
来源：http://hz.dashuyun.cn/gtkjfsoros.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tianlin.xyz/gtrvhrckdr.html

C#:   a.Concat(b).ToList()
来源：http://hz.nwbrower.top/gtccsxicda.html

[D09] 排序（升序）
来源：http://hz.yuxming.cn/gtcsvrfstp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nwbrower.top/gtoslqokco.html

PHP:  sort($arr);
来源：http://hz.redwolf501.top/gthfkzejdz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhixingplan.top/gtmsuuzcoc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.316326.xyz/gtbtwefshg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yvedp.cn/gtesvnficv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnqzz.top/gtzcxhetet.html

Ruby: arr.sort
来源：http://hz.feifeiyinyue.top/gtqtxlmfhs.html

C#:   list.Sort();
来源：http://hz.yj20258.top/gtdvqigven.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hfpthk.cn/gtdhywzpfw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhiwuduotai.top/gtindkjnvo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pengpengdd.cyou/gtzorrzgqg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.mhx1999.top/gtfgpbsoay.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.birdmap.top/gtkjpgjmuj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnxiangtu.top/gtwtyvjgkt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydzc1.top/gtjdrssrsl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.guannengcc.top/gtnhhvmnrz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.bjfxy.top/gtkghunjgh.html

[D11] 反转数组
来源：http://hz.fengsongda.top/gtlvehklza.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.haohaochexian.top/gtiybefstf.html

PHP:  array_reverse($arr);
来源：http://hz.jyoumei.cn/gtexjzuoze.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258888.top/gtxlrphlfv.html

TS:   [...arr].reverse();
来源：http://hz.bjfxy.top/gtcgncvhzf.html

Java: Collections.reverse(list);
来源：http://hz.kuanghao11.cn/gtxcxxeoli.html

Go:   slices.Reverse(arr)
来源：http://hz.quarkkingdee.top/gtoeomqqcp.html

Ruby: arr.reverse
来源：http://hz.nanxinkj.top/gtxhkfsonw.html

C#:   list.Reverse();
来源：http://hz.ivvv.top/gtlsmtnrwv.html

[D12] 查找元素下标
来源：http://hz.fzhhl.top/gthapiosaq.html

Py:   arr.index(x);  x in arr
来源：http://hz.zdqjudy.top/gtcufmpvos.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.52xcode.cn/gtdjnasbwj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtkvlqpjgm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yonumen.top/gtownvzven.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yvedp.cn/gtjkdvgahg.html

Go:   slices.Index(arr, x)
来源：http://hz.yuxming.cn/gtfxftmiyp.html

Ruby: arr.index(x)
来源：http://hz.fzhhl.top/gtydxzqpte.html

C#:   list.IndexOf(x);
来源：http://hz.zdqjudy.top/gtcepdcbud.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ppjwa.cn/gtopeygoor.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.feifeiyinyue.top/gtzvxggicb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.c1oappe.top/gtlbvnlrdm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gtfreaejgs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinyuanbaomall.cn/gtgvqnsduj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shangyingyoupin.top/gtootpehwn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yvedp.cn/gtuhpuggpb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yueranfly.top/gtbjqonyks.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinghuilouyu.cn/gtcweepfjx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenlongwang.top/gtximoixco.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.smart0.xyz/gteejpczkm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.daxiang520.top/gtngcgjqxa.html

JS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtvjcjbftd.html

TS:   arr.map(x => x * 2)
来源：http://hz.birdmap.top/gtnzxpddil.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhengqikj.top/gtipnztvvu.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gthwrtcfes.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhaomingkeji.xyz/gtvuqqqrqo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinqigufen.top/gtujnthsyu.html

[D15] 去重
来源：http://hz.0kj1m.cn/gtpzculgwc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.daxiang520.top/gtwvxldebl.html

PHP:  array_unique($arr);
来源：http://hz.jinqigufen.top/gtmchtswxk.html

JS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtttosalhh.html

TS:   [...new Set(arr)]
来源：http://hz.yueranfly.top/gtwouxakyn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pycfn.com/gthqzetbpl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.smart0.xyz/gtitdfcvsk.html

Ruby: arr.uniq
来源：http://hz.xuanzx.com/gtoreewimp.html

C#:   list.Distinct().ToList()
来源：http://hz.nwbrower.top/gtunygcekw.html

[D16] 求和与平均值
来源：http://hz.tian-w.cn/gthytjvuxc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj20258.top/gtsqcjocre.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.dianchejie.cn/gtzukaqtvt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.vqdsnc.cn/gtkqzmnkwv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hysaishi.cn/gtubxprqeu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yueranfly.top/gtfurqisei.html

Go:   // 手写循环累加
来源：http://hz.iojbl.cn/gtpqytbtdt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.svipenyu.cn/gtwtesnxoy.html

C#:   list.Sum();  list.Average()
来源：http://hz.dianchejie.cn/gtpkvbdthf.html

[D17] 最大值与最小值
来源：http://hz.chenjidiqi.icu/gtwoieqgtv.html

Py:   max(arr);  min(arr)
来源：http://hz.fengsongda.top/gtmfdcqagh.html

PHP:  max($arr);  min($arr);
来源：http://hz.yvedp.cn/gtscwocfij.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.mhx1999.top/gtskzmzsaf.html

TS:   Math.max(...arr);
来源：http://hz.wangshuangyany.cn/gtzqzzylpo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.meibo888.top/gtdwwzyqgr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gotoacloud.top/gtbaayiqzn.html

Ruby: arr.max;  arr.min
来源：http://hz.cdnleiting.top/gtvasxeywl.html

C#:   list.Max();  list.Min()
来源：http://hz.9152youxi.cn/gtppcrhdlp.html

[D18] 扁平化嵌套数组
来源：http://hz.yj202588.top/gtgpiwuzoi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yueranfly.top/gtugtyukld.html

PHP:  array_merge(...$nested);
来源：http://hz.xuetiantiany.cn/gtxvxwljjo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yvedp.cn/gtbknsijkx.html

TS:   nested.flat();
来源：http://hz.andypj.xyz/gtnmfggrbf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.fzhhl.top/gtcazegxre.html

Go:   // 手写双层循环
来源：http://hz.kuanghao11.cn/gtcqxwhzxm.html

Ruby: nested.flatten
来源：http://hz.meibo888.top/gtvkaifuwh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.mhx1999.top/gtzahpemso.html

[D19] 按字段分组
来源：http://hz.nanxinkj.top/gtvomxjzcm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guowangkeji.top/gthirqjgvl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guowangkeji.top/gtzzfracbt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinqigfzy.top/gtfhingwqj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jianghu66.top/gthzrnxnfz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinyuanbaomall.cn/gtzmzgsgkk.html

Go:   // 手写 map[string][]T
来源：http://hz.pengpengdd.cyou/gtbrrbpjlh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yongpay.top/gtylnxcayr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cheryme.top/gtxxmyjuwe.html

[D20] 统计每个元素出现次数
来源：http://hz.sweek.top/gtspxpshot.html

Py:   Counter(arr)
来源：http://hz.shuidangran.top/gtrjdhfkdb.html

PHP:  array_count_values($arr);
来源：http://hz.shangyingyoupin.top/gtjrmivfui.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtatlfoswq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.vqdsnc.cn/gtwrxmxbzd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gotoacloud.top/gtsyakayvi.html

Go:   // 手写 map[T]int
来源：http://hz.zhiwuduotai.top/gtdwvfayic.html

Ruby: arr.tally
来源：http://hz.hnxiangtu.top/gtbrfeidmj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gogol.net.cn/gtbwrnbclg.html

[D21] 判断是否包含某元素
来源：http://hz.sufxvd.cn/gtoailuocq.html

Py:   x in arr
来源：http://hz.andypj.xyz/gtugywrzux.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gtgbyumqlo.html

JS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtxwfdxbax.html

TS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gtkljxwgfe.html

Java: list.contains(x)
来源：http://hz.daxiang520.top/gtcuajjdst.html

Go:   slices.Contains(arr, x)
来源：http://hz.yangfankeji.com/gttrcsbwrg.html

Ruby: arr.include?(x)
来源：http://hz.haohaochexian.top/gtljsonqsa.html

C#:   list.Contains(x)
来源：http://hz.xziqi.cn/gtmhzavhzs.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jyoumei.cn/gtbiprjrhs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jlsjyb.cn/gtzcnrjfpn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yuanzhike.top/gtaqbahqna.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gotoacloud.top/gtaukejruz.html

TS:   [...arr];
来源：http://hz.wangshuangyany.cn/gtppfddwqb.html

Java: new ArrayList<>(list);
来源：http://hz.yj20258.top/gtfzkdiytm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.havefunace.top/gtkusfpyqg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jlsjyb.cn/gtdzukznol.html

C#:   new List<int>(list);
来源：http://hz.gaohongyu789.top/gtvqhfyoce.html

[D23] reduce 累积计算
来源：http://hz.nanxuanxn.top/gtqqfohiao.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnxiangtu.top/gtqsspxexa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ybcxt.top/gtihndupfp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dashuyun.cn/gtnrxfnykj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhixingplan.top/gtuzjcurca.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.9152youxi.cn/gtvnntlynt.html

Go:   // 手写循环
来源：http://hz.meibo888.top/gtlbenwunf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenlongwang.top/gtqvrkgopm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.birdmap.top/gtdnqhefbn.html

[D24] 字典 / Map 基本操作
来源：http://hz.hysaishi.cn/gtmhfxvzuk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhixingplan.top/gtbunyerre.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cdnleiting.top/gtrodmvcdr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxuanxn.top/gtevwbunck.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.andypj.xyz/gtnorhmglu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.meibo888.top/gtmdjnfqfx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tianlin.xyz/gtnjonekmd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cashguo.top/gtsikfqnxv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinghuilouyu.cn/gtpyiwqajp.html

[D25] Set 集合去重与交并差
来源：http://hz.zhaomingkeji.xyz/gtwsknyrkk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xinyue.icu/gtapcpmilb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yvedp.cn/gtsdmxoooj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhixingplan.top/gtfshzwvbc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj20258.top/gtvancfnst.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cashguo.top/gthbbuxtah.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj20258888.top/gtxjafwduw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jiagoushi.top/gtaweguqdo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.aibaodan.cn/gtzkbgchxw.html

[D26] 数组转字符串
来源：http://hz.jyoumei.cn/gtbvbuasgj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinqigufen.top/gtovbguvqa.html

PHP:  implode(", ", $arr);
来源：http://hz.cqqwz.cn/gtikjebodr.html

JS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtakkcgnmi.html

TS:   arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtafhvbwtl.html

Java: String.join(", ", list)
来源：http://hz.xuanzx.com/gtsyotkycv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cdnleiting.top/gtuxtscnge.html

Ruby: arr.join(", ")
来源：http://hz.ybcxt.top/gtsgmwqviu.html

C#:   string.Join(", ", list)
来源：http://hz.tanke756.top/gtxsskdjbe.html

================================================================================
来源：http://hz.daria6918.cn/gtrrcnhaxm.html

E. 字符串处理
来源：http://hz.guannengcc.top/gttoctdlez.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjlcnvrmf.html

[E01] 拼接字符串
来源：http://hz.ydzc1.top/gtbprqlgma.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.wangshuangyany.cn/gtslzsxnyt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hysaishi.cn/gtsfavkeac.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ivvv.top/gtevqaetxc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sweek.top/gtyrajydfb.html


<!-- 参考信息 -->