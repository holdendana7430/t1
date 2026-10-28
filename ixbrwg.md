代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.birdmap.top/gtlfovfmsw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.iojbl.cn/gtzufmwkxs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yonumen.top/gtobodkrna.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.feifeiyinyue.top/gtiecgccai.html

[C10] 变量作用域
来源：http://hz.jqgfzy.top/gtzlrbfhyi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinyuanbaomall.cn/gtncdpounz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinghuilouyu.cn/gtxcrefedj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.svipenyu.cn/gtwsqvwicd.html

TS:   同 JS
来源：http://hz.andypj.xyz/gtdcrgsphr.html

Java: 方法内为块级作用域
来源：http://hz.guannengcc.top/gtysiqwwrh.html

Go:   花括号块级作用域
来源：http://hz.iojbl.cn/gtvnbwgmri.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dianchejie.cn/gtzuounwgi.html

C#:   块级作用域
来源：http://hz.cheryme.top/gtjsxprpdi.html

[C11] 模块导入与导出
来源：http://hz.jqgufenzy.top/gteiigszws.html

Py:   from module import func
来源：http://hz.gogol.net.cn/gtozqwsyfs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ybcxt.top/gtzwqwvena.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhixingplan.top/gtoyaprjny.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.feifeiyinyue.top/gthdailmlz.html

Java: import java.util.List;
来源：http://hz.ehwqpu.com/gteucpeizm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhongyouzk.top/gtiqhdkvde.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhiwuduotai.top/gtghhhrpws.html

C#:   using System.Text;
来源：http://hz.jinqigufen.top/gtbwnpwilh.html

[C12] 立即执行函数 IIFE
来源：http://hz.bjfxy.top/gtgbprbkzm.html

Py:   (lambda: print("run"))()
来源：http://hz.jinyuanbaomall.cn/gtddufalla.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhixingplan.top/gtuoywmgol.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hongshengwenyu.top/gtmvcrxbso.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtrjwyvavb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ydzc1.top/gtcehsptow.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.aizwys.cn/gtrdldfbzg.html

Ruby: -> { puts "run" }.call
来源：http://hz.gaohongyu789.top/gtzdutlprr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.smart0.xyz/gtllnnzzgb.html

[C13] 类型声明 / 类型注解
来源：http://hz.yuxming.cn/gtgegqqpdc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guannengcc.top/gtjyszhckt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtduktnzij.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnxiangtu.top/gtkhievcvt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yangfankeji.com/gtwbijmeam.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gtwekxflle.html

Go:   func add(a, b int) int
来源：http://hz.birdmap.top/gtisprzdxy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.guowangkeji.top/gtmuqdpvqh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj20258.top/gthtgigwcr.html

[C14] 泛型函数
来源：http://hz.cdnleiting.top/gtrpbsuhqe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.birdmap.top/gtuluvudce.html

PHP:  // 无泛型
来源：http://hz.dianchejie.cn/gtcijewuzc.html

JS:   // 无泛型
来源：http://hz.yuanzhike.top/gthjfzlccu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sysykeji.top/gtvxorpifm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shangyingyoupin.top/gtsjhykgei.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hongshengwenyu.top/gtxlhuzywd.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangtech.top/gtbfkmpbjy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yueranfly.top/gtsmiipvoq.html

[C15] 解构 / 展开参数
来源：http://hz.52xcode.cn/gtxcjrbxxa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tian-w.cn/gtwiwykffe.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jinyuanbaomall.cn/gtttvjolfg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtcytsknri.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.haohaochexian.top/gtyqtrxzgf.html

Java: // 无解构
来源：http://hz.xingfuxueyuan.xyz/gtxemsxlez.html

Go:   // 无解构
来源：http://hz.sysykeji.top/gtofslqzqv.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtxcousyyl.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtrcvveskg.html

[C16] 函数 / 方法重载
来源：http://hz.gzhubu.top/gthtrckhgu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nwbrower.top/gtpctnoyjw.html

PHP:  // 无重载
来源：http://hz.guannengcc.top/gtexecgdwu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ppjwa.cn/gtpoqnzszn.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.chenlongwang.top/gtxrokmgad.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hywenlv.cn/gtimdsqggx.html

Go:   // 无重载：用不同函数名
来源：http://hz.yj202588.top/gttzgqfajj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gotoacloud.top/gtouxmjxzx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinqigfzy.top/gtrtwsilek.html

================================================================================
来源：http://hz.andypj.xyz/gtjjqojsou.html

D. 数组 / 列表 / 集合
来源：http://hz.daxiang520.top/gtwdwtxike.html

================================================================================
来源：http://hz.9152youxi.cn/gtamodzsff.html

[D01] 创建数组 / 列表
来源：http://hz.0kj1m.cn/gtjzjjknkx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuanzx.com/gtwwdsdcar.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xziqi.cn/gtdtszfwfi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hammf.cn/gtibpynosn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhongyouzk.top/gtimbkpyck.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuanzhike.top/gtahxocxmk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yonumen.top/gtqhpdswvc.html

Ruby: arr = [1, 2, 3]
来源：http://hz.redwolf501.top/gtfeomsldi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xziqi.cn/gtvancnsst.html

[D02] 追加元素到末尾
来源：http://hz.yj202588.top/gtdgevnyfx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhaomingkeji.xyz/gtohomzoqy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shanyushiyangtech.top/gtfkbhzdbd.html

JS:   arr.push(4);
来源：http://hz.gaohongyu789.top/gtycimofbs.html

TS:   arr.push(4);
来源：http://hz.hywenlv.cn/gtabbdontk.html

Java: list.add(4);
来源：http://hz.9152youxi.cn/gtpwgtxldc.html

Go:   arr = append(arr, 4)
来源：http://hz.yuxming.cn/gtglaugzun.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.316326.xyz/gtsueyzhkl.html

C#:   list.Add(4);
来源：http://hz.chenjidiqi.icu/gtlidhuloq.html

[D03] 在指定位置插入元素
来源：http://hz.dashuyun.cn/gtvmqqlmgn.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangkeji.top/gtbjxfsoyu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgfzy.top/gtgvbzcfow.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jianghu66.top/gtncdvrpot.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.aibaodan.cn/gtferozwpu.html

Java: list.add(0, 0);
来源：http://hz.nanxinkj.top/gtzzwnbtnk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.nanxuanxn.top/gtdmhhxmep.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jianghu66.top/gttjbpcysu.html

C#:   list.Insert(0, 0);
来源：http://hz.zycfv.cn/gtxhqylsjk.html

[D04] 删除元素
来源：http://hz.zhijiandao.cn/gtkbgmtvuf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenlongwang.top/gtggvidadh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yanxiufei.cn/gtpabjkzds.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gzhubu.top/gthtynbres.html

TS:   arr.splice(0, 1);
来源：http://hz.meibo888.top/gtidtmkdbk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sxryk.cn/gtuakesikr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xinyue.icu/gtwsgsadon.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xuetiantiany.cn/gtrkwnrlkh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ivvv.top/gtzriyhewf.html

[D05] 访问与修改元素
来源：http://hz.zhiwuduotai.top/gtmbqovkzu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.c1oappe.top/gturikkkpm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.haohaochexian.top/gtmxoxysfh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.meibo888.top/gtzafdbikd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.dashuyun.cn/gtylmnihhl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fengsongda.top/gtlnbkifuf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtaptsupje.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtprvkrigp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.c1oappe.top/gtvfozpnox.html

[D06] 数组长度
来源：http://hz.chenlongwang.top/gtvfzfbgbz.html

Py:   len(arr)
来源：http://hz.sysykeji.top/gtagbfsrgc.html

PHP:  count($arr);
来源：http://hz.fzhhl.top/gtgdpndthj.html

JS:   arr.length
来源：http://hz.dianchejie.cn/gtyjonmgeo.html

TS:   arr.length
来源：http://hz.wangshuangyany.cn/gttfffdozo.html

Java: list.size();
来源：http://hz.cheryme.top/gtgowcofqj.html

Go:   len(arr)
来源：http://hz.ppjwa.cn/gtrpjoynhw.html

Ruby: arr.length; arr.size
来源：http://hz.aibaodan.cn/gtzxrbgddx.html

C#:   list.Count;
来源：http://hz.yanxiufei.cn/gtvlpwfhwx.html

[D07] 切片 / 取子数组
来源：http://hz.fzhhl.top/gtadcveijx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yonumen.top/gtlwzvpesl.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yueranfly.top/gtpixrshmw.html

JS:   arr.slice(1, 4);
来源：http://hz.andypj.xyz/gtdyrswghh.html

TS:   arr.slice(1, 4);
来源：http://hz.ydzc1.top/gtoswrtfbq.html

Java: list.subList(1, 4);
来源：http://hz.nwbrower.top/gtvnebxqoo.html

Go:   arr[1:4]
来源：http://hz.yuxming.cn/gtblfgzsnx.html

Ruby: arr[1, 3]
来源：http://hz.yj20258.top/gtwinfatdw.html

C#:   list.GetRange(1, 3);
来源：http://hz.gaohongyu789.top/gthpqgemiv.html

[D08] 合并两个数组
来源：http://hz.hongshengwenyu.top/gtehvylbrm.html

Py:   a + b;  a.extend(b)
来源：http://hz.ybcxt.top/gtqbbydzjm.html

PHP:  array_merge($a, $b);
来源：http://hz.zhaomingkeji.xyz/gtucbbcpgg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dashuyun.cn/gtsjnrdjmz.html

TS:   [...a, ...b];
来源：http://hz.sweek.top/gtseunfeuv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ppjwa.cn/gtswqnvmnl.html

Go:   append(a, b...)
来源：http://hz.kuanghao11.cn/gtqnweiytf.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ydzc1.top/gtxjvaltut.html

C#:   a.Concat(b).ToList()
来源：http://hz.yvedp.cn/gtwiksnfke.html

[D09] 排序（升序）
来源：http://hz.gzhubu.top/gtrufrblwy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenzaomai.com/gtcdfnckcj.html

PHP:  sort($arr);
来源：http://hz.xinyue.icu/gtzxrnvlzi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aizwys.cn/gtswdmedwi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hfpthk.cn/gtrrmskkir.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cheryme.top/gtwbaaalfm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gzhubu.top/gtomstqtvs.html

Ruby: arr.sort
来源：http://hz.jinqigufen.top/gtsteoiimi.html

C#:   list.Sort();
来源：http://hz.ivvv.top/gtovumuotg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shuidangran.top/gtfmwmsrzw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangdashe.top/gtecxjrqic.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yangfankeji.com/gthggixdgs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtxscufszx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.andypj.xyz/gtoyxlvqst.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zdqjudy.top/gtvvxyeado.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sxryk.cn/gtpfkuflgu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydjk.org.cn/gtasjwjtvn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.mhx1999.top/gtphiaqzbi.html

[D11] 反转数组
来源：http://hz.chenlongwang.top/gtsnjhdocj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nanxinkj.top/gtsnejcvzg.html

PHP:  array_reverse($arr);
来源：http://hz.fzhhl.top/gtpjcqdbog.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fengsongda.top/gtaghnoguu.html

TS:   [...arr].reverse();
来源：http://hz.smart0.xyz/gtpyyplssh.html

Java: Collections.reverse(list);
来源：http://hz.ywan-chungtsiang.top/gtwqcywkoq.html

Go:   slices.Reverse(arr)
来源：http://hz.c1oappe.top/gtgsxmtqgr.html

Ruby: arr.reverse
来源：http://hz.9152youxi.cn/gttxqwpfuw.html

C#:   list.Reverse();
来源：http://hz.ydzc1.top/gtbyfymguj.html

[D12] 查找元素下标
来源：http://hz.tanke756.top/gthbsdkboy.html

Py:   arr.index(x);  x in arr
来源：http://hz.ppjwa.cn/gtvooaziet.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.316326.xyz/gtnhetilaq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hywenlv.cn/gtjanxisuy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangtech.top/gthbtytafm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.svipenyu.cn/gtnsyukbsp.html

Go:   slices.Index(arr, x)
来源：http://hz.feifeiyinyue.top/gtqtdvcvrr.html

Ruby: arr.index(x)
来源：http://hz.yueranfly.top/gtthicvqtx.html

C#:   list.IndexOf(x);
来源：http://hz.xziqi.cn/gtuiavydal.html

[D13] 过滤（保留满足条件的）
来源：http://hz.0kj1m.cn/gtajpesrzq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sweek.top/gtpauindzz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhijiandao.cn/gtivdjewxi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtcqbqyfsf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ybcxt.top/gtdpvcvqdw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.andypj.xyz/gtqkzooiev.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pengpengdd.cyou/gtxvrbjkim.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.snrcjt.cn/gtrbohbyqx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fzhhl.top/gtgvghqhta.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj202588.top/gtpjwkfjdw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.9152youxi.cn/gtcymfikbj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fzhhl.top/gtopelrgwa.html

JS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtzuygmors.html

TS:   arr.map(x => x * 2)
来源：http://hz.ybcxt.top/gtitowbrqt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.vqdsnc.cn/gtwkwbxded.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gtexvqdimu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.daria6918.cn/gtkemqipfx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jyoumei.cn/gtrvzixkpg.html

[D15] 去重
来源：http://hz.chenlongwang.top/gtsjekahqv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gtlzmpfrva.html

PHP:  array_unique($arr);
来源：http://hz.ppjwa.cn/gtofwwsqbe.html

JS:   [...new Set(arr)]
来源：http://hz.shuidangran.top/gtczjmyvwv.html

TS:   [...new Set(arr)]
来源：http://hz.dianchejie.cn/gtwuvzzbhu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.havefunace.top/gtkwsnjgyx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangshuangyany.cn/gtfypjvxcc.html

Ruby: arr.uniq
来源：http://hz.yj20258.top/gtgwzwltht.html

C#:   list.Distinct().ToList()
来源：http://hz.iojbl.cn/gticauwxoi.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangkeji.top/gtpdfkuzdj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ehwqpu.com/gtmkaixtzo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenlongwang.top/gtkxpckuqq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gogol.net.cn/gtjpktaaxx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dianchejie.cn/gthbblwzby.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.haohaochexian.top/gtvzcydope.html

Go:   // 手写循环累加
来源：http://hz.snrcjt.cn/gtkuaeukep.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.dashuyun.cn/gtpydvotkm.html

C#:   list.Sum();  list.Average()
来源：http://hz.dashuyun.cn/gtrxckxwcv.html

[D17] 最大值与最小值
来源：http://hz.zdqjudy.top/gtjwaqjymc.html

Py:   max(arr);  min(arr)
来源：http://hz.havefunace.top/gtjdmncunz.html

PHP:  max($arr);  min($arr);
来源：http://hz.svipenyu.cn/gtwauyfioe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tianlin.xyz/gtqisbovke.html

TS:   Math.max(...arr);
来源：http://hz.shuidangran.top/gtszqraebb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhijiandao.cn/gtmivnypmn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhoulong.xyz/gtsgrhdyzc.html

Ruby: arr.max;  arr.min
来源：http://hz.shuidangran.top/gtdnhqljee.html

C#:   list.Max();  list.Min()
来源：http://hz.316326.xyz/gtejnwabaj.html

[D18] 扁平化嵌套数组
来源：http://hz.cqqwz.cn/gtpeljdltn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zdqjudy.top/gtzpgzkfjp.html

PHP:  array_merge(...$nested);
来源：http://hz.tianlin.xyz/gtqgdwufnq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhengqikj.top/gthscleanw.html

TS:   nested.flat();
来源：http://hz.jqgfzy.top/gtyrdpprrf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xylfe.cn/gtugqnvdai.html

Go:   // 手写双层循环
来源：http://hz.ydzc1.top/gtzmqxmdod.html

Ruby: nested.flatten
来源：http://hz.xuanzx.com/gtmqgghavk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gzhubu.top/gtlnxepdlp.html

[D19] 按字段分组
来源：http://hz.0kj1m.cn/gtzkzoaain.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.9152youxi.cn/gtjxfohmez.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hfpthk.cn/gtlbzcbbwe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nanxinkj.top/gtlukcdscv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jqgufenzy.top/gtlycdwkgz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yonumen.top/gtoowhzamg.html

Go:   // 手写 map[string][]T
来源：http://hz.ywan-chungtsiang.top/gtlwuthlld.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jlsjyb.cn/gtongueuoz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhijiandao.cn/gtynpnbymr.html

[D20] 统计每个元素出现次数
来源：http://hz.mhx1999.top/gtqjwjnhai.html

Py:   Counter(arr)
来源：http://hz.zhixingplan.top/gtchmpvdch.html

PHP:  array_count_values($arr);
来源：http://hz.9152youxi.cn/gtlrblbajg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tian-w.cn/gtwpbtednd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gtuuqcyakb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj20258888.top/gtifsflmvj.html

Go:   // 手写 map[T]int
来源：http://hz.yvedp.cn/gtedsnxbai.html

Ruby: arr.tally
来源：http://hz.chenlongwang.top/gttxezeryn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cucudq.cn/gtchgogntg.html

[D21] 判断是否包含某元素
来源：http://hz.dianchejie.cn/gtxsajannd.html

Py:   x in arr
来源：http://hz.nwbrower.top/gtdutrvxsa.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nwbrower.top/gtcjfrynva.html

JS:   arr.includes(x)
来源：http://hz.daxiang520.top/gtmhxfwxav.html

TS:   arr.includes(x)
来源：http://hz.meibo888.top/gtgieulpud.html

Java: list.contains(x)
来源：http://hz.svipenyu.cn/gttawsqcha.html

Go:   slices.Contains(arr, x)
来源：http://hz.yongpay.top/gtyxsbiohk.html

Ruby: arr.include?(x)
来源：http://hz.jinyuanbaomall.cn/gtfulxlgid.html

C#:   list.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtbdqrioav.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnxiangtu.top/gtoebtwfug.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gzhubu.top/gtzhpitehe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnxiangtu.top/gtiyubnvkw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hammf.cn/gtzmvcagvz.html

TS:   [...arr];
来源：http://hz.tianlin.xyz/gtciqrmgxi.html

Java: new ArrayList<>(list);
来源：http://hz.dashuyun.cn/gtjduqlnrt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.fzhhl.top/gtfaipdonn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxinkj.top/gtjwlkjgwj.html

C#:   new List<int>(list);
来源：http://hz.tian-w.cn/gtzcwffgfk.html

[D23] reduce 累积计算
来源：http://hz.jyoumei.cn/gtcurgtkin.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yanxiufei.cn/gtovfyjsfy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258888.top/gtbigsemlj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zycfv.cn/gtjtakbjhy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gtbuhlukwq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shzxlz.cn/gtvnaziwwk.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gtsklhmwtf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.pengpengdd.cyou/gtirlucxpq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.mhx1999.top/gtifzabdcm.html

[D24] 字典 / Map 基本操作
来源：http://hz.ydzc1.top/gtuzgvbnzg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.9152youxi.cn/gtgjiajzhx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hongshengwenyu.top/gtgffixzjf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sxryk.cn/gtxofrthap.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtspijwybx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yvedp.cn/gtxacqwwmh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhixingplan.top/gtpvhujjga.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shzxlz.cn/gtbwfvosjl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yuxming.cn/gtgaktemmb.html

[D25] Set 集合去重与交并差
来源：http://hz.cdnleiting.top/gtgoxioqwe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnqzz.top/gtrurxpvwr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.quarkkingdee.top/gtdvwkumac.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yonumen.top/gtdptaahrm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xylfe.cn/gtaayssysp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhongyouzk.top/gtcodkrryi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hywenlv.cn/gtpiwczvwu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhijiandao.cn/gtzqayhofi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.guannengcc.top/gtakhdzebe.html

[D26] 数组转字符串
来源：http://hz.yuxming.cn/gtccsdavrg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhoulong.xyz/gtceokbbvn.html

PHP:  implode(", ", $arr);
来源：http://hz.feifeiyinyue.top/gtqnlbsmtg.html

JS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtbqnyvisb.html

TS:   arr.join(", ")
来源：http://hz.chenzaomai.com/gtyouagvfw.html


<!-- 参考信息 -->