代发 wailian999

C#:   块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtdqfnvhnl.html

[C11] 模块导入与导出
来源：http://hz.mhx1999.top/gtgkvajryi.html

Py:   from module import func
来源：http://hz.shzxlz.cn/gtjtssreep.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nanxuanxn.top/gtdcgctikc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.pengpengdd.cyou/gtboevjqbg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ybcxt.top/gtotgcmlmb.html

Java: import java.util.List;
来源：http://hz.ywan-chungtsiang.top/gtelyyzcjt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shzxlz.cn/gtanskhosk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sxryk.cn/gtrewripqj.html

C#:   using System.Text;
来源：http://hz.svipenyu.cn/gtggemjfnm.html

[C12] 立即执行函数 IIFE
来源：http://hz.jianghu66.top/gtsnbirxvq.html

Py:   (lambda: print("run"))()
来源：http://hz.52xcode.cn/gtftwemfrg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxuanxn.top/gtaejolgmp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtlvafdgit.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cqqwz.cn/gtcsbzynjy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xinyue.icu/gtcrciedvb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hongshengwenyu.top/gtnlcwaenj.html

Ruby: -> { puts "run" }.call
来源：http://hz.pengpengdd.cyou/gtzhrpxptd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.gogol.net.cn/gtluzezjdk.html

[C13] 类型声明 / 类型注解
来源：http://hz.jianghu66.top/gtinajsaog.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jianghu66.top/gtuyrfhzzk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.svipenyu.cn/gtkenlamgq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tian-w.cn/gtndvbplto.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgufenzy.top/gtuxbgdjkj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gthjzwkjch.html

Go:   func add(a, b int) int
来源：http://hz.feifeiyinyue.top/gtdjeexezh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.havefunace.top/gtlpijhbfk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yvedp.cn/gtmdydnzuf.html

[C14] 泛型函数
来源：http://hz.birdmap.top/gtgsbbecfg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258888.top/gtlomthhzr.html

PHP:  // 无泛型
来源：http://hz.zhongyouzk.top/gtxibvvdxp.html

JS:   // 无泛型
来源：http://hz.jianghu66.top/gtqzcahaoe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.wangdashe.top/gtgapymnjc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cashguo.top/gtrewkzcfx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.redwolf501.top/gtwxatrzlv.html

Ruby: # 无泛型
来源：http://hz.yvedp.cn/gtleetvosd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guowangkeji.top/gtvrjmojzr.html

[C15] 解构 / 展开参数
来源：http://hz.quarkkingdee.top/gtxyekutxe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hammf.cn/gtgtdojtwb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gotoacloud.top/gtuutqcfrm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhoulong.xyz/gtttodvvbe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.shangyingyoupin.top/gtkzzmxoza.html

Java: // 无解构
来源：http://hz.sxryk.cn/gtchstyfzd.html

Go:   // 无解构
来源：http://hz.tian-w.cn/gtntapndmv.html

Ruby: a, b = pair
来源：http://hz.svipenyu.cn/gtwwrdzowe.html

C#:   var (a, b) = pair;
来源：http://hz.zhengqikj.top/gtxytjihba.html

[C16] 函数 / 方法重载
来源：http://hz.yuxming.cn/gtjbnljbys.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xuetiantiany.cn/gtmohhacod.html

PHP:  // 无重载
来源：http://hz.aibaodan.cn/gtjavltazr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gzhubu.top/gtiyipjkhr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daxiang520.top/gtbdcvqqhy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jqgufenzy.top/gtmidnzpkt.html

Go:   // 无重载：用不同函数名
来源：http://hz.andypj.xyz/gtponvrbqv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.snrcjt.cn/gtowrjlvlx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnqzz.top/gtkclrjvni.html

================================================================================
来源：http://hz.cashguo.top/gtmtypbubl.html

D. 数组 / 列表 / 集合
来源：http://hz.jinghuilouyu.cn/gtupaqtuur.html

================================================================================
来源：http://hz.gaohongyu789.top/gtsjmdezyv.html

[D01] 创建数组 / 列表
来源：http://hz.nwbrower.top/gtthbssbgn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jyoumei.cn/gthtmdtzrn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.havefunace.top/gtejundewh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ppjwa.cn/gtshuaeohs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sxryk.cn/gtngonwksi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtieymltcr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.c1oappe.top/gtrezcmlen.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ydjk.org.cn/gthsrgclny.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xylfe.cn/gthkjrnusi.html

[D02] 追加元素到末尾
来源：http://hz.yanxiufei.cn/gtpiftlbdz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.meibo888.top/gtipbuiacg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhaomingkeji.xyz/gtzgjlbtkc.html

JS:   arr.push(4);
来源：http://hz.xuetiantiany.cn/gtvmcjhpmj.html

TS:   arr.push(4);
来源：http://hz.yanxiufei.cn/gtraaweaop.html

Java: list.add(4);
来源：http://hz.ybcxt.top/gtockxsuqk.html

Go:   arr = append(arr, 4)
来源：http://hz.ydzc1.top/gtjkgwobnv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xziqi.cn/gthgxiisxx.html

C#:   list.Add(4);
来源：http://hz.bjfxy.top/gtvqdeckml.html

[D03] 在指定位置插入元素
来源：http://hz.xziqi.cn/gtxkpfzqkx.html

Py:   arr.insert(0, 0)
来源：http://hz.ehwqpu.com/gtvjujeyds.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ydjk.org.cn/gtiyrmxzav.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.daxiang520.top/gtguoicjsh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ydjk.org.cn/gtkasplqrm.html

Java: list.add(0, 0);
来源：http://hz.zhaomingkeji.xyz/gtgbbutunx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.0kj1m.cn/gtuojtkqim.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shzxlz.cn/gtelihilus.html

C#:   list.Insert(0, 0);
来源：http://hz.xinyue.icu/gtoihoxnpu.html

[D04] 删除元素
来源：http://hz.nanxinkj.top/gtngbyzekx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.pycfn.com/gtjqeqhcwq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.gogol.net.cn/gtcwqavsbr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.tanke756.top/gtoesjvloi.html

TS:   arr.splice(0, 1);
来源：http://hz.nanxinkj.top/gtgqiudyoo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.daxiang520.top/gtpjdyycjy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guowangkeji.top/gtupwqaixe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.mhx1999.top/gtvnulelxb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.kuanghao11.cn/gtylwpovel.html

[D05] 访问与修改元素
来源：http://hz.yj20258888.top/gtsysamrkm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jianghu66.top/gtpehftesy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daxiang520.top/gtrdkeolxd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cdnleiting.top/gtalnfanup.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yj20258.top/gtwnfajtle.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shanyushiyangtech.top/gttxfisnry.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtdzbbokta.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gtqactvvjc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sweek.top/gtsygratwx.html

[D06] 数组长度
来源：http://hz.hfpthk.cn/gtixmpjodl.html

Py:   len(arr)
来源：http://hz.ybcxt.top/gtlhjccxfg.html

PHP:  count($arr);
来源：http://hz.ppjwa.cn/gtdhrrojjq.html

JS:   arr.length
来源：http://hz.sweek.top/gtxxcmicct.html

TS:   arr.length
来源：http://hz.0kj1m.cn/gtygmtozuo.html

Java: list.size();
来源：http://hz.sufxvd.cn/gtqjcokeuo.html

Go:   len(arr)
来源：http://hz.chenjidiqi.icu/gtgtkbfdsa.html

Ruby: arr.length; arr.size
来源：http://hz.vqdsnc.cn/gtiqmqlhiz.html

C#:   list.Count;
来源：http://hz.hammf.cn/gtnxlrhiki.html

[D07] 切片 / 取子数组
来源：http://hz.yueranfly.top/gtyddljrcw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.mhx1999.top/gtceuvbtel.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shanyushiyangtech.top/gtlhpqzvag.html

JS:   arr.slice(1, 4);
来源：http://hz.jinghuilouyu.cn/gthlwyzssd.html

TS:   arr.slice(1, 4);
来源：http://hz.tian-w.cn/gtwgcnexhb.html

Java: list.subList(1, 4);
来源：http://hz.pengpengdd.cyou/gtqhlwccqy.html

Go:   arr[1:4]
来源：http://hz.9152youxi.cn/gtnwolkjch.html

Ruby: arr[1, 3]
来源：http://hz.zhongyouzk.top/gtplqubxdm.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangshuangyany.cn/gthwcldely.html

[D08] 合并两个数组
来源：http://hz.hysaishi.cn/gtxkrfxskw.html

Py:   a + b;  a.extend(b)
来源：http://hz.fzhhl.top/gtonbooimx.html

PHP:  array_merge($a, $b);
来源：http://hz.xylfe.cn/gtxftvfqkq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinghuilouyu.cn/gtzwqnovkb.html

TS:   [...a, ...b];
来源：http://hz.xuanzx.com/gtycjtovab.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.kuanghao11.cn/gtyyiwfczn.html

Go:   append(a, b...)
来源：http://hz.aizwys.cn/gtvkpmvidx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yuxming.cn/gtozkigoxi.html

C#:   a.Concat(b).ToList()
来源：http://hz.hammf.cn/gtynimaomy.html

[D09] 排序（升序）
来源：http://hz.xingfuxueyuan.xyz/gtrtbiihat.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtaqgucslt.html

PHP:  sort($arr);
来源：http://hz.fengsongda.top/gtibsdngxy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.daria6918.cn/gtrvlvrfzx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hongshengwenyu.top/gtelfmbknh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.c1oappe.top/gtkhdytchp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtrpljsrte.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtgyimtnot.html

C#:   list.Sort();
来源：http://hz.yanxiufei.cn/gtcjpplcde.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhengqikj.top/gtosbzcheu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yangfankeji.com/gtwhgbgkzc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tianlin.xyz/gtqhddgwvv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangdashe.top/gtoubttavd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gtckwlhdan.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nanxinkj.top/gtnfxbnesc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.316326.xyz/gtwtmbjcru.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shzxlz.cn/gtajfpiraf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ivvv.top/gtvsnqljbj.html

[D11] 反转数组
来源：http://hz.zhixingplan.top/gtvbxhpgmm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shangyingyoupin.top/gtdvhmrrah.html

PHP:  array_reverse($arr);
来源：http://hz.nanxinkj.top/gtjnvmfoyx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sufxvd.cn/gtnacabfcy.html

TS:   [...arr].reverse();
来源：http://hz.hfpthk.cn/gtrfavnvtg.html

Java: Collections.reverse(list);
来源：http://hz.pycfn.com/gtxxjljgfe.html

Go:   slices.Reverse(arr)
来源：http://hz.cheryme.top/gtsotmnpeh.html

Ruby: arr.reverse
来源：http://hz.cashguo.top/gtplrvvijt.html

C#:   list.Reverse();
来源：http://hz.jinqigufen.top/gttvumasuk.html

[D12] 查找元素下标
来源：http://hz.jinyuanbaomall.cn/gtahtwmtcn.html

Py:   arr.index(x);  x in arr
来源：http://hz.haohaochexian.top/gttuexjvlm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhiwuduotai.top/gteekvkqea.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtisiobrbm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.c1oappe.top/gthohssfdc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhoulong.xyz/gtzwfoyzgp.html

Go:   slices.Index(arr, x)
来源：http://hz.quarkkingdee.top/gtzffohwlo.html

Ruby: arr.index(x)
来源：http://hz.yj20258888.top/gtenfsabhm.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangtech.top/gtausyljox.html

[D13] 过滤（保留满足条件的）
来源：http://hz.dashuyun.cn/gtokgzwqjr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ywan-chungtsiang.top/gtdqkeskns.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangdashe.top/gtogcdgkjb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtgneqpwfp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtllowfask.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jlsjyb.cn/gtjhpyhfuj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhongyouzk.top/gtvapclthh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yanxiufei.cn/gtcslvupku.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhijiandao.cn/gtfefhbdyx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aibaodan.cn/gtwsbiamwk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tanke756.top/gtxjpsibpc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuanzx.com/gtewnhqisi.html

JS:   arr.map(x => x * 2)
来源：http://hz.yueranfly.top/gtkdfifyak.html

TS:   arr.map(x => x * 2)
来源：http://hz.yongpay.top/gtktehjltm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangshuangyany.cn/gtksewdmgv.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gtxqrqmrqd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gotoacloud.top/gtfgzzqchw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.daria6918.cn/gtmsadbjxz.html

[D15] 去重
来源：http://hz.yj202588.top/gtfjfagbnq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtblwiojgf.html

PHP:  array_unique($arr);
来源：http://hz.jiagoushi.top/gtvscygkhy.html

JS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtkpwngrfn.html

TS:   [...new Set(arr)]
来源：http://hz.ybcxt.top/gtzmxunkwr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ppjwa.cn/gtovacnrzl.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhiwuduotai.top/gtsbywfvtj.html

Ruby: arr.uniq
来源：http://hz.vqdsnc.cn/gtqhwufamb.html

C#:   list.Distinct().ToList()
来源：http://hz.zdqjudy.top/gtqpgyevvh.html

[D16] 求和与平均值
来源：http://hz.chenzaomai.com/gtfcjbkzcg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhaomingkeji.xyz/gtdcpugjbb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shangyingyoupin.top/gtgopwpmgg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fzhhl.top/gtrczpainm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtyoidbvrj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.wangdashe.top/gthhfmoxol.html

Go:   // 手写循环累加
来源：http://hz.aizwys.cn/gtchupmefb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xingfuxueyuan.xyz/gtaxuqidcc.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinghuilouyu.cn/gtbhnhnmkw.html

[D17] 最大值与最小值
来源：http://hz.zhaomingkeji.xyz/gtnqiywuop.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxinkj.top/gtynlgskuo.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxinkj.top/gttrohdhqx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj202588.top/gtrigdakot.html

TS:   Math.max(...arr);
来源：http://hz.gaohongyu789.top/gtlkiidzto.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258888.top/gttusmbvrn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ehwqpu.com/gtbfszhwmx.html

Ruby: arr.max;  arr.min
来源：http://hz.jianghu66.top/gthaginehp.html

C#:   list.Max();  list.Min()
来源：http://hz.316326.xyz/gthyjmgyqo.html

[D18] 扁平化嵌套数组
来源：http://hz.ivvv.top/gtemwaekap.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhoulong.xyz/gtcwoxofpm.html

PHP:  array_merge(...$nested);
来源：http://hz.zhengqikj.top/gtjmldnpgc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.kuanghao11.cn/gtkulosqek.html

TS:   nested.flat();
来源：http://hz.ivvv.top/gtscdsskcx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xuanzx.com/gtsfospmvv.html

Go:   // 手写双层循环
来源：http://hz.jqgfzy.top/gtohjncdlx.html

Ruby: nested.flatten
来源：http://hz.ehwqpu.com/gtydkitigf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ybcxt.top/gtqjrnrjbm.html

[D19] 按字段分组
来源：http://hz.jyoumei.cn/gtawrxmowi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.andypj.xyz/gtbviabbnj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yangfankeji.com/gtqrcrfkws.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ydzc1.top/gtiwoeklto.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hnxiangtu.top/gtixkoxphq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj202588.top/gtordidbkh.html

Go:   // 手写 map[string][]T
来源：http://hz.cqqwz.cn/gtsckzvbfn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.birdmap.top/gtsqvkzwyb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jqgufenzy.top/gtpbzcehil.html

[D20] 统计每个元素出现次数
来源：http://hz.52xcode.cn/gtpumgtkin.html

Py:   Counter(arr)
来源：http://hz.yanxiufei.cn/gtgztibdwy.html

PHP:  array_count_values($arr);
来源：http://hz.zdqjudy.top/gtpqgvtmnq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtrhsjwljx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtakdlsdaq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.kuanghao11.cn/gtnfjovmip.html

Go:   // 手写 map[T]int
来源：http://hz.yongpay.top/gtzjamtglz.html

Ruby: arr.tally
来源：http://hz.gzhubu.top/gthfakxwnp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.vqdsnc.cn/gtcaodxmjs.html

[D21] 判断是否包含某元素
来源：http://hz.quarkkingdee.top/gtjmtnuwbc.html

Py:   x in arr
来源：http://hz.pycfn.com/gtyipvxpvj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhaomingkeji.xyz/gtyaucmunr.html

JS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gtyelspkvy.html

TS:   arr.includes(x)
来源：http://hz.iojbl.cn/gtperthyde.html

Java: list.contains(x)
来源：http://hz.pengpengdd.cyou/gtziwuzjaa.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258.top/gtmaswybei.html

Ruby: arr.include?(x)
来源：http://hz.nwbrower.top/gtehurgqkx.html

C#:   list.Contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtwsxyrbhp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.kuanghao11.cn/gthgbozbrv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.haohaochexian.top/gthebtuvik.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ywan-chungtsiang.top/gtcoomfqvx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.dianchejie.cn/gtabwwahjw.html

TS:   [...arr];
来源：http://hz.ybcxt.top/gtwxfbanuo.html

Java: new ArrayList<>(list);
来源：http://hz.zhengqikj.top/gtroujfswj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hfpthk.cn/gtwwurfzzq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.redwolf501.top/gtafacchqc.html

C#:   new List<int>(list);
来源：http://hz.shzxlz.cn/gtdorzbkyn.html

[D23] reduce 累积计算
来源：http://hz.zdqjudy.top/gtbkeefmiu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.svipenyu.cn/gtuskestzk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.daria6918.cn/gtvwdxuypk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sysykeji.top/gtaniwyeqj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ehwqpu.com/gtzgbnhzbo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.havefunace.top/gtqetypmgu.html

Go:   // 手写循环
来源：http://hz.jinqigfzy.top/gtjpdzhgzr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.daxiang520.top/gtonvyheip.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yvedp.cn/gtdxvksxqj.html

[D24] 字典 / Map 基本操作
来源：http://hz.birdmap.top/gtohwsyapj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ybcxt.top/gtvumsajnq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hfpthk.cn/gtgrgavogq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jiagoushi.top/gtmocsyfoa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yangfankeji.com/gtfchntxqz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydzc1.top/gtwlyzfrth.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cdnleiting.top/gtzriwzwpr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.guannengcc.top/gtgeckxbfz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.bjfxy.top/gtcnlzyqkd.html

[D25] Set 集合去重与交并差
来源：http://hz.xuanzx.com/gtcicqruzy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.iojbl.cn/gtvlgtoytv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.guannengcc.top/gtcwpjmtpq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sweek.top/gtatlqmzrb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.birdmap.top/gthklehxen.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhiwuduotai.top/gtbiitjbhc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jianghu66.top/gtcpynxdjd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgfzy.top/gtklyeljeg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zycfv.cn/gttzbjcfmd.html

[D26] 数组转字符串
来源：http://hz.yanxiufei.cn/gtbpyudzhj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cucudq.cn/gthvarkgqo.html

PHP:  implode(", ", $arr);
来源：http://hz.sufxvd.cn/gtbjlovbae.html

JS:   arr.join(", ")
来源：http://hz.yvedp.cn/gtzwhfdild.html

TS:   arr.join(", ")
来源：http://hz.cashguo.top/gtiftajbvg.html

Java: String.join(", ", list)
来源：http://hz.chenzaomai.com/gtomewkevn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xylfe.cn/gtmdtcuopf.html

Ruby: arr.join(", ")
来源：http://hz.jinghuilouyu.cn/gtpbttapnz.html

C#:   string.Join(", ", list)
来源：http://hz.smart0.xyz/gtbnghtbqy.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtyphmbxfo.html

E. 字符串处理
来源：http://hz.sufxvd.cn/gtqnntucxi.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtadbhrubm.html

[E01] 拼接字符串
来源：http://hz.0kj1m.cn/gtietplxuc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hfpthk.cn/gtxmbkfivd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhijiandao.cn/gtwvbgvfmt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtoadbucdw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ywan-chungtsiang.top/gtmoiznfgv.html


<!-- 参考信息 -->