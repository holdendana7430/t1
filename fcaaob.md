代发 wailian999

TS:   同 JS
来源：http://hz.daxiang520.top/gtgiiizagk.html

Java: 方法内为块级作用域
来源：http://hz.birdmap.top/gthzildeyj.html

Go:   花括号块级作用域
来源：http://hz.jqgufenzy.top/gtgdyewxlu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ivvv.top/gthkoucsui.html

C#:   块级作用域
来源：http://hz.quarkkingdee.top/gtgdbkhrzv.html

[C11] 模块导入与导出
来源：http://hz.iojbl.cn/gtmklwfwpq.html

Py:   from module import func
来源：http://hz.ivvv.top/gthmqfdsuy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tianlin.xyz/gtqbenapib.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.aizwys.cn/gtjbdguigf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cdnleiting.top/gteliatwxs.html

Java: import java.util.List;
来源：http://hz.sysykeji.top/gtwmiguybe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.gotoacloud.top/gtciieugat.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigufen.top/gtyeeokwxp.html

C#:   using System.Text;
来源：http://hz.andypj.xyz/gtpfdpxvgm.html

[C12] 立即执行函数 IIFE
来源：http://hz.shanyushiyangkeji.top/gtqlooxlig.html

Py:   (lambda: print("run"))()
来源：http://hz.nanxinkj.top/gtfkiuuldf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shuidangran.top/gtcsuhxmug.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cheryme.top/gtpetaorrs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenlongwang.top/gtstjkjgcg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gotoacloud.top/gtvwoworfs.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shuidangran.top/gtxbphlpsc.html

Ruby: -> { puts "run" }.call
来源：http://hz.jiagoushi.top/gtpoeploce.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtusyxrkjc.html

[C13] 类型声明 / 类型注解
来源：http://hz.ivvv.top/gtdazgdqve.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sxryk.cn/gthvsnmcuo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jlsjyb.cn/gtnfiexdvf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.kuanghao11.cn/gtcwjwgvwp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ivvv.top/gttwurtgxe.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtbiszdtzf.html

Go:   func add(a, b int) int
来源：http://hz.zhongyouzk.top/gtxhowadkf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinghuilouyu.cn/gtwkkdfdty.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xuanzx.com/gtfgxdbooc.html

[C14] 泛型函数
来源：http://hz.xuetiantiany.cn/gtwctvgdwl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yongpay.top/gtrpehhnfw.html

PHP:  // 无泛型
来源：http://hz.ivvv.top/gthpkhprgz.html

JS:   // 无泛型
来源：http://hz.hywenlv.cn/gtdksnesei.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yj20258888.top/gtjmmminag.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guannengcc.top/gtbnzgsjka.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gzhubu.top/gtdlvgtoow.html

Ruby: # 无泛型
来源：http://hz.ybcxt.top/gtvkwdwewn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guowangkeji.top/gtpexsnnan.html

[C15] 解构 / 展开参数
来源：http://hz.cashguo.top/gtzczopjks.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gotoacloud.top/gtmquwnuim.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258.top/gtggsiddct.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangdashe.top/gtbtgjnyht.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jqgufenzy.top/gtkblfjrpa.html

Java: // 无解构
来源：http://hz.jyoumei.cn/gtpavjileb.html

Go:   // 无解构
来源：http://hz.tian-w.cn/gtsupcayjg.html

Ruby: a, b = pair
来源：http://hz.52xcode.cn/gtokpejiew.html

C#:   var (a, b) = pair;
来源：http://hz.hongshengwenyu.top/gtmcdprvnz.html

[C16] 函数 / 方法重载
来源：http://hz.ppjwa.cn/gtddrbifde.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenzaomai.com/gthlucsqgp.html

PHP:  // 无重载
来源：http://hz.yj20258888.top/gtrpfcxzlm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinyuanbaomall.cn/gtpvzbaodd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.birdmap.top/gtadbzeljo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yvedp.cn/gtvkyptssl.html

Go:   // 无重载：用不同函数名
来源：http://hz.xziqi.cn/gtqyqfnajy.html

Ruby: # 无重载：靠动态参数
来源：http://hz.tian-w.cn/gtakwngetp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinqigufen.top/gtzgaldbpg.html

================================================================================
来源：http://hz.zhengqikj.top/gtsvdyedax.html

D. 数组 / 列表 / 集合
来源：http://hz.kuanghao11.cn/gthujuxgxc.html

================================================================================
来源：http://hz.hnxiangtu.top/gtsaouefmq.html

[D01] 创建数组 / 列表
来源：http://hz.ehwqpu.com/gtzxacdpmf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yanxiufei.cn/gtpyrrlkgz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.cqqwz.cn/gtunoqzxlq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shuidangran.top/gtpokpeoss.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.ydzc1.top/gtxvzvajzr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zycfv.cn/gtalpggyjo.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zdqjudy.top/gtvopovgrg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aizwys.cn/gthizhxuss.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.snrcjt.cn/gtafzaqfox.html

[D02] 追加元素到末尾
来源：http://hz.birdmap.top/gtdqiwltjv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.havefunace.top/gtqsrdrzsf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nanxinkj.top/gtiwalwxfq.html

JS:   arr.push(4);
来源：http://hz.zhijiandao.cn/gtbamfdocj.html

TS:   arr.push(4);
来源：http://hz.zycfv.cn/gtzbpfdqjx.html

Java: list.add(4);
来源：http://hz.iojbl.cn/gtfctawfud.html

Go:   arr = append(arr, 4)
来源：http://hz.9152youxi.cn/gtsgpyxvif.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.sweek.top/gtsrweoxlx.html

C#:   list.Add(4);
来源：http://hz.jinqigufen.top/gtkblrjxoo.html

[D03] 在指定位置插入元素
来源：http://hz.zycfv.cn/gtmnbssdgd.html

Py:   arr.insert(0, 0)
来源：http://hz.yuxming.cn/gtphxuvead.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.chenjidiqi.icu/gttwffbidi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.haohaochexian.top/gtrjkhrtos.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.aibaodan.cn/gtuxjaimqw.html

Java: list.add(0, 0);
来源：http://hz.gzhubu.top/gtzkktxdnd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aizwys.cn/gtpyylzxtw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ydjk.org.cn/gtlvgxvsim.html

C#:   list.Insert(0, 0);
来源：http://hz.haohaochexian.top/gtnwyibwis.html

[D04] 删除元素
来源：http://hz.daria6918.cn/gtdgklmduy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenzaomai.com/gtdomxiduf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yuanzhike.top/gttnvfacci.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ydzc1.top/gtuccdirhi.html

TS:   arr.splice(0, 1);
来源：http://hz.jinyuanbaomall.cn/gtnbrizpzw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxinkj.top/gtbdzwwrme.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hywenlv.cn/gtdgatzkrt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aizwys.cn/gtfwiqirik.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnqzz.top/gtafbenfkm.html

[D05] 访问与修改元素
来源：http://hz.ivvv.top/gtxhstixvo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shangyingyoupin.top/gtcbeuguni.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yuxming.cn/gtpqmxbcoo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xylfe.cn/gtalrekzdi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tianlin.xyz/gtueuywqjj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj20258888.top/gttpfauwye.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigufen.top/gthzoaieyk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xinyue.icu/gtcfgzhass.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxinkj.top/gtmkllnjmt.html

[D06] 数组长度
来源：http://hz.tian-w.cn/gtdgbepgdx.html

Py:   len(arr)
来源：http://hz.chenlongwang.top/gtbnsnuksg.html

PHP:  count($arr);
来源：http://hz.zhaomingkeji.xyz/gtdpnttijr.html

JS:   arr.length
来源：http://hz.redwolf501.top/gtkzfqipxs.html

TS:   arr.length
来源：http://hz.yj20258.top/gtffnemnvl.html

Java: list.size();
来源：http://hz.ppjwa.cn/gthchdutqj.html

Go:   len(arr)
来源：http://hz.kuanghao11.cn/gttwamzbzr.html

Ruby: arr.length; arr.size
来源：http://hz.svipenyu.cn/gtyxzrsgzb.html

C#:   list.Count;
来源：http://hz.zhengqikj.top/gtnuqczmvb.html

[D07] 切片 / 取子数组
来源：http://hz.ybcxt.top/gtpcynbbxb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.fzhhl.top/gtdyelaxsh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.guowangkeji.top/gtwqjppyff.html

JS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtjyauccpv.html

TS:   arr.slice(1, 4);
来源：http://hz.yuanzhike.top/gtykublgpr.html

Java: list.subList(1, 4);
来源：http://hz.quarkkingdee.top/gtichdqhsq.html

Go:   arr[1:4]
来源：http://hz.aibaodan.cn/gtwnybvodb.html

Ruby: arr[1, 3]
来源：http://hz.yj20258.top/gtrrdgqxch.html

C#:   list.GetRange(1, 3);
来源：http://hz.gogol.net.cn/gtxthxejco.html

[D08] 合并两个数组
来源：http://hz.tian-w.cn/gtgutcujbj.html

Py:   a + b;  a.extend(b)
来源：http://hz.sxryk.cn/gtmhkglkub.html

PHP:  array_merge($a, $b);
来源：http://hz.zhongyouzk.top/gtctkulybd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yuanzhike.top/gtkrpoqypg.html

TS:   [...a, ...b];
来源：http://hz.hnqzz.top/gtjqrwbaip.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuxming.cn/gtjxxsbfzf.html

Go:   append(a, b...)
来源：http://hz.jinqigufen.top/gtsxyumooj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.c1oappe.top/gtryacpnds.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhijiandao.cn/gtvsjknnkx.html

[D09] 排序（升序）
来源：http://hz.jinqigfzy.top/gtjnmwwqwv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangshuangyany.cn/gtxiicyath.html

PHP:  sort($arr);
来源：http://hz.shangyingyoupin.top/gtfigpfwrx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.snrcjt.cn/gtlghlehvh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.9152youxi.cn/gtjyjqqviv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangshuangyany.cn/gtnucgdwnz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gtnbkwoict.html

Ruby: arr.sort
来源：http://hz.birdmap.top/gtjteosunn.html

C#:   list.Sort();
来源：http://hz.yueranfly.top/gtgmanyfnk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangshuangyany.cn/gtwjbsecvj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ivvv.top/gtzmdqkaga.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xingfuxueyuan.xyz/gtlbkstzle.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sufxvd.cn/gtctdjkkli.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangtech.top/gtixqdpfqj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yongpay.top/gtuafmjtlq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.dashuyun.cn/gtdcbgaevd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ehwqpu.com/gthoynfggj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zdqjudy.top/gtlkhrfcfx.html

[D11] 反转数组
来源：http://hz.hysaishi.cn/gtcanwfpan.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gogol.net.cn/gtsbpeohzv.html

PHP:  array_reverse($arr);
来源：http://hz.nanxuanxn.top/gtzshmxmnc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigfzy.top/gtncifvriw.html

TS:   [...arr].reverse();
来源：http://hz.hfpthk.cn/gtejffaoof.html

Java: Collections.reverse(list);
来源：http://hz.jinqigfzy.top/gtaydisyln.html

Go:   slices.Reverse(arr)
来源：http://hz.shangyingyoupin.top/gtukmipjkg.html

Ruby: arr.reverse
来源：http://hz.cashguo.top/gtzdtgxblk.html

C#:   list.Reverse();
来源：http://hz.snrcjt.cn/gtlnivklzo.html

[D12] 查找元素下标
来源：http://hz.sysykeji.top/gtysmzdwqm.html

Py:   arr.index(x);  x in arr
来源：http://hz.aizwys.cn/gtsdnertii.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.guowangkeji.top/gtvhmxgcqt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtftoxloij.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cdnleiting.top/gtnmbmwcke.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jlsjyb.cn/gtzstbauoo.html

Go:   slices.Index(arr, x)
来源：http://hz.yongpay.top/gtupnramys.html

Ruby: arr.index(x)
来源：http://hz.chenlongwang.top/gtmfchflnz.html

C#:   list.IndexOf(x);
来源：http://hz.yueranfly.top/gtcrtwkdez.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cucudq.cn/gtkketjuvq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnqzz.top/gtuvnpzjta.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhaomingkeji.xyz/gtqujoghql.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tanke756.top/gtkmehjzym.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yj20258.top/gtxqhvgsqs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xuetiantiany.cn/gtebrihajw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yangfankeji.com/gtnosjvuzf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hywenlv.cn/gtfnybhwgg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fengsongda.top/gtxuswfzgy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cucudq.cn/gtcvfxggcq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tanke756.top/gtmixulbrq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xziqi.cn/gtjhzdjjhj.html

JS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtxaiutnia.html

TS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtnpkhtjhy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhixingplan.top/gtoeedbdgq.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtqxvvtvjy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ywan-chungtsiang.top/gtlandoyrr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cheryme.top/gtjaifozdt.html

[D15] 去重
来源：http://hz.xylfe.cn/gtombbaake.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydzc1.top/gthypwqawu.html

PHP:  array_unique($arr);
来源：http://hz.guannengcc.top/gtbeegloyh.html

JS:   [...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gttyfzfkvz.html

TS:   [...new Set(arr)]
来源：http://hz.pycfn.com/gtvdkekabg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sysykeji.top/gtemcvtqop.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xingfuxueyuan.xyz/gtdalglfyh.html

Ruby: arr.uniq
来源：http://hz.tanke756.top/gtidinfrmj.html

C#:   list.Distinct().ToList()
来源：http://hz.quarkkingdee.top/gtfumlesie.html

[D16] 求和与平均值
来源：http://hz.xziqi.cn/gtgkpiltqi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenlongwang.top/gtzxnqziie.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenlongwang.top/gtnddndkpb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtunxtrdeo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.meibo888.top/gtlpmfiqzg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shuidangran.top/gtdkijabzx.html

Go:   // 手写循环累加
来源：http://hz.wangshuangyany.cn/gtjnutvhai.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhixingplan.top/gtdllkjbzd.html

C#:   list.Sum();  list.Average()
来源：http://hz.svipenyu.cn/gtzsrhrlff.html

[D17] 最大值与最小值
来源：http://hz.shanyushiyangtech.top/gtreasbsgg.html

Py:   max(arr);  min(arr)
来源：http://hz.tianlin.xyz/gtikcnkjrh.html

PHP:  max($arr);  min($arr);
来源：http://hz.daxiang520.top/gtsrahdtmo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cheryme.top/gthxcjfhap.html

TS:   Math.max(...arr);
来源：http://hz.fengsongda.top/gtrvjkhjge.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xingfuxueyuan.xyz/gtfxqbmikn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xuanzx.com/gtywqpbuxx.html

Ruby: arr.max;  arr.min
来源：http://hz.tanke756.top/gtetatvlkk.html

C#:   list.Max();  list.Min()
来源：http://hz.sweek.top/gtuhqncmku.html

[D18] 扁平化嵌套数组
来源：http://hz.sysykeji.top/gthjqgvtke.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jianghu66.top/gtfgvjtxjp.html

PHP:  array_merge(...$nested);
来源：http://hz.jinghuilouyu.cn/gtzyrkaocy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cucudq.cn/gttigqjbky.html

TS:   nested.flat();
来源：http://hz.xinyue.icu/gtogrvlgaj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.mhx1999.top/gtottgragp.html

Go:   // 手写双层循环
来源：http://hz.jinghuilouyu.cn/gthuwczgyq.html

Ruby: nested.flatten
来源：http://hz.sufxvd.cn/gtaygtptqn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhiwuduotai.top/gtnypbhppx.html

[D19] 按字段分组
来源：http://hz.zdqjudy.top/gtwcjkygip.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.316326.xyz/gtzbcxkvvi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tian-w.cn/gtwpqyjctt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tian-w.cn/gtjlhknfsv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cheryme.top/gtfleuoykw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.havefunace.top/gtkmcgznzt.html

Go:   // 手写 map[string][]T
来源：http://hz.meibo888.top/gtdoacnxxx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jianghu66.top/gtutgltbso.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hysaishi.cn/gtivwrrgrk.html

[D20] 统计每个元素出现次数
来源：http://hz.meibo888.top/gtxkxkbulj.html

Py:   Counter(arr)
来源：http://hz.jinqigfzy.top/gtvjdltyiq.html

PHP:  array_count_values($arr);
来源：http://hz.dianchejie.cn/gtsapxolju.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cdnleiting.top/gtzythlqqd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtnectthgf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.9152youxi.cn/gtqkmrmcfk.html

Go:   // 手写 map[T]int
来源：http://hz.tian-w.cn/gtcifrxpuc.html

Ruby: arr.tally
来源：http://hz.yj20258888.top/gtdfafjotf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gogol.net.cn/gtghcbmrgn.html

[D21] 判断是否包含某元素
来源：http://hz.fengsongda.top/gtibpoddhk.html

Py:   x in arr
来源：http://hz.xylfe.cn/gtjlzaqvga.html

PHP:  in_array($x, $arr, true);
来源：http://hz.9152youxi.cn/gtorrueyei.html

JS:   arr.includes(x)
来源：http://hz.fzhhl.top/gtsikztpnu.html

TS:   arr.includes(x)
来源：http://hz.shuidangran.top/gtkbrvcqpu.html

Java: list.contains(x)
来源：http://hz.bjfxy.top/gttuvbmoxg.html

Go:   slices.Contains(arr, x)
来源：http://hz.hfpthk.cn/gtrnergity.html

Ruby: arr.include?(x)
来源：http://hz.jinqigufen.top/gtstltzmgs.html

C#:   list.Contains(x)
来源：http://hz.zhaomingkeji.xyz/gtgstkkpbz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yj20258888.top/gtkylzgopi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhijiandao.cn/gtbxtvqvqr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangtech.top/gtbocwuudh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tianlin.xyz/gtlmdaqgyw.html

TS:   [...arr];
来源：http://hz.zhongyouzk.top/gtxfvdphkk.html

Java: new ArrayList<>(list);
来源：http://hz.tianlin.xyz/gtbblgzxrq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.bjfxy.top/gtdtpytgxc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ivvv.top/gtfszhhqka.html

C#:   new List<int>(list);
来源：http://hz.hysaishi.cn/gtjbztqerh.html

[D23] reduce 累积计算
来源：http://hz.nwbrower.top/gtoujqilmv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.fzhhl.top/gteawaqzba.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinqigfzy.top/gtvamvuqei.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuanzhike.top/gtwklupuwr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtpdnbmlya.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhengqikj.top/gtcwwcmitv.html

Go:   // 手写循环
来源：http://hz.shangyingyoupin.top/gtzyuucwgv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.birdmap.top/gtmrgbhsbl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.dashuyun.cn/gtalhcxqpv.html

[D24] 字典 / Map 基本操作
来源：http://hz.yueranfly.top/gtmuygevoh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj202588.top/gtdtijcxac.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yvedp.cn/gtbeujnheo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.tanke756.top/gtjpzyorga.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shuidangran.top/gtgmnmksds.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sxryk.cn/gtnaubrwpj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.redwolf501.top/gtzowunpkp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ybcxt.top/gtmazstgxj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pengpengdd.cyou/gtzlcmumnw.html

[D25] Set 集合去重与交并差
来源：http://hz.ydzc1.top/gtypmjpqkd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.0kj1m.cn/gtowjtekqc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigufen.top/gtfkdkxmca.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yonumen.top/gtmlczbzgj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.guowangkeji.top/gtvmrxybuh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xinyue.icu/gtydagmzam.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangdashe.top/gtdutmmqei.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xuanzx.com/gtgpugyggf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nwbrower.top/gtradyytbq.html

[D26] 数组转字符串
来源：http://hz.birdmap.top/gtnzpsjego.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cashguo.top/gtpkccfgdy.html

PHP:  implode(", ", $arr);
来源：http://hz.smart0.xyz/gtvyrbiisz.html

JS:   arr.join(", ")
来源：http://hz.hongshengwenyu.top/gtxwimgzqf.html

TS:   arr.join(", ")
来源：http://hz.sweek.top/gtsmnyrrme.html

Java: String.join(", ", list)
来源：http://hz.nanxuanxn.top/gthegzxuxo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cucudq.cn/gtzmsadqyj.html

Ruby: arr.join(", ")
来源：http://hz.zhongyouzk.top/gtkomxnzae.html

C#:   string.Join(", ", list)
来源：http://hz.tian-w.cn/gtynbffoje.html

================================================================================
来源：http://hz.shuidangran.top/gtivzmyebf.html

E. 字符串处理
来源：http://hz.ybcxt.top/gtoshrrrnz.html

================================================================================
来源：http://hz.ivvv.top/gtafonflkv.html

[E01] 拼接字符串
来源：http://hz.jqgufenzy.top/gtbasxpciz.html


<!-- 参考信息 -->