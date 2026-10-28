代发 wailian999

C#:   块级作用域
来源：http://hz.redwolf501.top/gtbzasxsom.html

[C11] 模块导入与导出
来源：http://hz.haohaochexian.top/gtqjyphtum.html

Py:   from module import func
来源：http://hz.cqqwz.cn/gtaidfjpgp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shangyingyoupin.top/gtxnnvqwgq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.guowangkeji.top/gtbqddkwrx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.vqdsnc.cn/gtmsgxcjhs.html

Java: import java.util.List;
来源：http://hz.jqgfzy.top/gtpqhewraf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shangyingyoupin.top/gtjgihasxf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sweek.top/gturutzqwh.html

C#:   using System.Text;
来源：http://hz.yuanzhike.top/gtwefkeebt.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258.top/gtvupktxuy.html

Py:   (lambda: print("run"))()
来源：http://hz.xuanzx.com/gtfuztlgno.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sysykeji.top/gtmtflemkl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shuidangran.top/gtxhbjrhvc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yangfankeji.com/gtkknsmhgf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.snrcjt.cn/gtooopxmzn.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sufxvd.cn/gtsfckfchr.html

Ruby: -> { puts "run" }.call
来源：http://hz.yuxming.cn/gtssnoskmy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yvedp.cn/gttpczlwtj.html

[C13] 类型声明 / 类型注解
来源：http://hz.52xcode.cn/gtzucavjte.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yonumen.top/gtarhogkru.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtygnocvdp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ydzc1.top/gtjcdoyhli.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fengsongda.top/gtddomamyj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gtreedamgj.html

Go:   func add(a, b int) int
来源：http://hz.yuanzhike.top/gtulsgchxl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yangfankeji.com/gtyddruefo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.birdmap.top/gtzgagzzum.html

[C14] 泛型函数
来源：http://hz.sufxvd.cn/gtubttdyil.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yueranfly.top/gtgsfuvlbd.html

PHP:  // 无泛型
来源：http://hz.hnxiangtu.top/gtecxurvld.html

JS:   // 无泛型
来源：http://hz.aibaodan.cn/gtvdfmhyxg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shanyushiyangkeji.top/gtwcljrmdh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenlongwang.top/gtxwfnelxc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.tian-w.cn/gtgocwvdbc.html

Ruby: # 无泛型
来源：http://hz.svipenyu.cn/gtzdjafmwr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shangyingyoupin.top/gtqddvrsyh.html

[C15] 解构 / 展开参数
来源：http://hz.ppjwa.cn/gtdtfbttir.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhoulong.xyz/gtnqgtnznk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ywan-chungtsiang.top/gtgygbqjwf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shuidangran.top/gtyhfycvym.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fzhhl.top/gtikpeojis.html

Java: // 无解构
来源：http://hz.svipenyu.cn/gttgexpbnl.html

Go:   // 无解构
来源：http://hz.andypj.xyz/gtepkjtdyx.html

Ruby: a, b = pair
来源：http://hz.shanyushiyangtech.top/gtlburywbr.html

C#:   var (a, b) = pair;
来源：http://hz.zhaomingkeji.xyz/gtlxpcpsat.html

[C16] 函数 / 方法重载
来源：http://hz.svipenyu.cn/gtkjljqovh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hnxiangtu.top/gtlzpvqgkr.html

PHP:  // 无重载
来源：http://hz.mhx1999.top/gtbatyrmva.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yj202588.top/gtjbwevkwb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.dashuyun.cn/gtpeerhida.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.kuanghao11.cn/gtrwyqxout.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgfzy.top/gtpclzmgsw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.daria6918.cn/gtcypzsmrv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.kuanghao11.cn/gtllfcataa.html

================================================================================
来源：http://hz.yuanzhike.top/gthdjxxwkf.html

D. 数组 / 列表 / 集合
来源：http://hz.yvedp.cn/gtvqtvhyfb.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtsqgywikz.html

[D01] 创建数组 / 列表
来源：http://hz.daxiang520.top/gtfbcqgkeo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ivvv.top/gtedaaueyw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.316326.xyz/gtosxrqhow.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sxryk.cn/gtveaxmyrj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sysykeji.top/gtmmmheyyc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.svipenyu.cn/gtmypghzla.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.chenjidiqi.icu/gtgqhkgibw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hnqzz.top/gttwgdtkte.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ivvv.top/gtxfiuysba.html

[D02] 追加元素到末尾
来源：http://hz.nanxinkj.top/gtqqstmauw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cdnleiting.top/gtvpopyael.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.redwolf501.top/gtuajbzbsc.html

JS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gttrpziatu.html

TS:   arr.push(4);
来源：http://hz.guannengcc.top/gtqpoyuhgb.html

Java: list.add(4);
来源：http://hz.yuanzhike.top/gtgtnrgkam.html

Go:   arr = append(arr, 4)
来源：http://hz.wangdashe.top/gtbbozzgvj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xuetiantiany.cn/gtnmkjzmdb.html

C#:   list.Add(4);
来源：http://hz.yj20258888.top/gtlmwgpfjy.html

[D03] 在指定位置插入元素
来源：http://hz.52xcode.cn/gtqsgdwyuw.html

Py:   arr.insert(0, 0)
来源：http://hz.sysykeji.top/gtgfhystcu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ppjwa.cn/gtbapwtpir.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.birdmap.top/gtaivkpfur.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cqqwz.cn/gtawxutxgq.html

Java: list.add(0, 0);
来源：http://hz.0kj1m.cn/gtaymmzfph.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hnxiangtu.top/gtlfkhtazk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinyuanbaomall.cn/gtdaoexfxn.html

C#:   list.Insert(0, 0);
来源：http://hz.xuanzx.com/gtqvzjxdkk.html

[D04] 删除元素
来源：http://hz.gzhubu.top/gtzspzlinc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jlsjyb.cn/gtdyenrmsz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ybcxt.top/gtynvdhgtf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nanxuanxn.top/gttkjfcync.html

TS:   arr.splice(0, 1);
来源：http://hz.shuidangran.top/gtugioyvpx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ywan-chungtsiang.top/gtahpxxrsx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.feifeiyinyue.top/gttfoebdgy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhaomingkeji.xyz/gtbhieqrej.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yongpay.top/gtjcufootb.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gtavoefzxg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gthjksarqw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.aizwys.cn/gtxntdychb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.birdmap.top/gtmvvgnkyx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhixingplan.top/gtcmqwwrjs.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yangfankeji.com/gtcrvdotbc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aizwys.cn/gtudtdwcgw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtatvturfg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cashguo.top/gtrrspvayj.html

[D06] 数组长度
来源：http://hz.cucudq.cn/gtiymqkrws.html

Py:   len(arr)
来源：http://hz.jiagoushi.top/gthagwtzeo.html

PHP:  count($arr);
来源：http://hz.jqgfzy.top/gtklaxcrjb.html

JS:   arr.length
来源：http://hz.hnqzz.top/gtadcfodpf.html

TS:   arr.length
来源：http://hz.andypj.xyz/gtmfuerdlo.html

Java: list.size();
来源：http://hz.pycfn.com/gtuzuudwqe.html

Go:   len(arr)
来源：http://hz.havefunace.top/gtsziqxrah.html

Ruby: arr.length; arr.size
来源：http://hz.smart0.xyz/gtuybttapg.html

C#:   list.Count;
来源：http://hz.birdmap.top/gtkoapkswj.html

[D07] 切片 / 取子数组
来源：http://hz.xuetiantiany.cn/gtgucvddry.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.bjfxy.top/gtrldpssjs.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nanxuanxn.top/gtvflxggjy.html

JS:   arr.slice(1, 4);
来源：http://hz.daria6918.cn/gttqpuaefa.html

TS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gthbfjjapr.html

Java: list.subList(1, 4);
来源：http://hz.gaohongyu789.top/gtqyupirhs.html

Go:   arr[1:4]
来源：http://hz.meibo888.top/gtxeupaqof.html

Ruby: arr[1, 3]
来源：http://hz.hnqzz.top/gtzyqymidv.html

C#:   list.GetRange(1, 3);
来源：http://hz.ehwqpu.com/gtnldtycgr.html

[D08] 合并两个数组
来源：http://hz.gzhubu.top/gtbovletyg.html

Py:   a + b;  a.extend(b)
来源：http://hz.xylfe.cn/gtmfmocqdw.html

PHP:  array_merge($a, $b);
来源：http://hz.andypj.xyz/gtfmxehpvr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hnxiangtu.top/gtcidxtkak.html

TS:   [...a, ...b];
来源：http://hz.jqgfzy.top/gtiehajbes.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yvedp.cn/gtakistiis.html

Go:   append(a, b...)
来源：http://hz.shangyingyoupin.top/gtverlnzog.html

Ruby: a + b;  a.concat(b)
来源：http://hz.52xcode.cn/gtbsvcseuv.html

C#:   a.Concat(b).ToList()
来源：http://hz.meibo888.top/gtpqhdgevl.html

[D09] 排序（升序）
来源：http://hz.daxiang520.top/gtkvfrycaa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.birdmap.top/gtrkpfdpgr.html

PHP:  sort($arr);
来源：http://hz.yangfankeji.com/gtcrdgbuoh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hammf.cn/gtkotomsmt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cqqwz.cn/gtocgvghzk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gogol.net.cn/gtnshycvfl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.c1oappe.top/gtdwlgvyhq.html

Ruby: arr.sort
来源：http://hz.0kj1m.cn/gtvbvovaoh.html

C#:   list.Sort();
来源：http://hz.daxiang520.top/gtflpicbnu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ydzc1.top/gtgqnzpthp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nanxuanxn.top/gtcpqnymws.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigufen.top/gtioywynbs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shuidangran.top/gtjegjlwhn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yanxiufei.cn/gtlnoydvwg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj20258.top/gtnftvmitu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.316326.xyz/gtgoisgrvq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tian-w.cn/gtzddpvief.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gotoacloud.top/gtwrmqfrgi.html

[D11] 反转数组
来源：http://hz.shuidangran.top/gtpgouvpvu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cashguo.top/gtwpspypcj.html

PHP:  array_reverse($arr);
来源：http://hz.yueranfly.top/gtdicpjmab.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.316326.xyz/gtdmvnhfij.html

TS:   [...arr].reverse();
来源：http://hz.havefunace.top/gtadznbxvh.html

Java: Collections.reverse(list);
来源：http://hz.cdnleiting.top/gtwctatkuf.html

Go:   slices.Reverse(arr)
来源：http://hz.chenlongwang.top/gtdeqvixhw.html

Ruby: arr.reverse
来源：http://hz.0kj1m.cn/gtqdsdiwiz.html

C#:   list.Reverse();
来源：http://hz.hnqzz.top/gtzzjchckl.html

[D12] 查找元素下标
来源：http://hz.jinqigufen.top/gtvgbyakhh.html

Py:   arr.index(x);  x in arr
来源：http://hz.smart0.xyz/gtaxgqznqg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cheryme.top/gtaznxxrnt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtlowkkjhs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dianchejie.cn/gtpgzdylco.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shangyingyoupin.top/gtialcwctk.html

Go:   slices.Index(arr, x)
来源：http://hz.chenjidiqi.icu/gtezatmvdf.html

Ruby: arr.index(x)
来源：http://hz.hongshengwenyu.top/gtdnjsayzr.html

C#:   list.IndexOf(x);
来源：http://hz.wangshuangyany.cn/gtawgeqzkw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tian-w.cn/gtfdayhkyb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxinkj.top/gtvvcgtltw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nanxuanxn.top/gtatfpsbuq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.c1oappe.top/gtqjvqvhpp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.guowangkeji.top/gtgxrqkirh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shuidangran.top/gtertvlmar.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jlsjyb.cn/gthedlheiw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.dashuyun.cn/gtvpxqvtfw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.havefunace.top/gthfnqmday.html

[D14] 映射转换（每个元素变形）
来源：http://hz.52xcode.cn/gtmxvgtqne.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gtwbugdoes.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.svipenyu.cn/gtqozvserf.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhengqikj.top/gtrvuwdkjq.html

TS:   arr.map(x => x * 2)
来源：http://hz.havefunace.top/gtwbcxioez.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ydzc1.top/gtbzskksyf.html

Go:   // 手写循环
来源：http://hz.jinqigufen.top/gtiiyaduli.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cheryme.top/gtzhfiefrz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sweek.top/gtkesuetor.html

[D15] 去重
来源：http://hz.ydzc1.top/gtaivusbjf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.daria6918.cn/gtfsrsbhwz.html

PHP:  array_unique($arr);
来源：http://hz.daxiang520.top/gtzeuwohgd.html

JS:   [...new Set(arr)]
来源：http://hz.chenlongwang.top/gtpzphsfhc.html

TS:   [...new Set(arr)]
来源：http://hz.shzxlz.cn/gtoxrrlbxe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.smart0.xyz/gtnirbgplr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yongpay.top/gtwfynwabo.html

Ruby: arr.uniq
来源：http://hz.tanke756.top/gtkfnxesyg.html

C#:   list.Distinct().ToList()
来源：http://hz.shangyingyoupin.top/gtyecinvnh.html

[D16] 求和与平均值
来源：http://hz.xinyue.icu/gtofpeygld.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aibaodan.cn/gtsisjnuyz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.smart0.xyz/gtqxjkdhky.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtkvbsccep.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtfdlpiray.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ywan-chungtsiang.top/gtpbpfqrlq.html

Go:   // 手写循环累加
来源：http://hz.hnqzz.top/gtorkkdnyg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pengpengdd.cyou/gtkbxdvudg.html

C#:   list.Sum();  list.Average()
来源：http://hz.zycfv.cn/gtkktqetjw.html

[D17] 最大值与最小值
来源：http://hz.jqgufenzy.top/gtbuyifixl.html

Py:   max(arr);  min(arr)
来源：http://hz.xziqi.cn/gteggtdlsp.html

PHP:  max($arr);  min($arr);
来源：http://hz.gaohongyu789.top/gtbninshmn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fengsongda.top/gthwkpzbyg.html

TS:   Math.max(...arr);
来源：http://hz.jinqigufen.top/gtcvouvwqu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtzozzqnuz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhijiandao.cn/gtjlvhgjvh.html

Ruby: arr.max;  arr.min
来源：http://hz.cucudq.cn/gtxtxydglk.html

C#:   list.Max();  list.Min()
来源：http://hz.wangshuangyany.cn/gtcxwznvtx.html

[D18] 扁平化嵌套数组
来源：http://hz.shuidangran.top/gtlcyeudcw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhixingplan.top/gtkkscsppr.html

PHP:  array_merge(...$nested);
来源：http://hz.jyoumei.cn/gtwtoyhwkd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnqzz.top/gtaqfswxel.html

TS:   nested.flat();
来源：http://hz.c1oappe.top/gtbxrdtbqb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenjidiqi.icu/gtdcrzuwki.html

Go:   // 手写双层循环
来源：http://hz.ivvv.top/gtmgempdrw.html

Ruby: nested.flatten
来源：http://hz.yj202588.top/gtugvniuby.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pengpengdd.cyou/gtvdtbzlyl.html

[D19] 按字段分组
来源：http://hz.ybcxt.top/gtrhrqdxtk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhengqikj.top/gtarzgvpiy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hfpthk.cn/gtjphaeywt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gogol.net.cn/gtcyfnamiv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtdyuaduir.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhijiandao.cn/gtlgdbagtw.html

Go:   // 手写 map[string][]T
来源：http://hz.quarkkingdee.top/gtawmmgiqd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hysaishi.cn/gtwwfxzggv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenjidiqi.icu/gtiqyztqwm.html

[D20] 统计每个元素出现次数
来源：http://hz.fzhhl.top/gtcoccdsgj.html

Py:   Counter(arr)
来源：http://hz.pycfn.com/gtmdqlfown.html

PHP:  array_count_values($arr);
来源：http://hz.xuanzx.com/gtjmhnzzsu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtzpmzammm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ybcxt.top/gtgswqkgmf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.c1oappe.top/gtlyqvjyeh.html

Go:   // 手写 map[T]int
来源：http://hz.pengpengdd.cyou/gtsopuzjbs.html

Ruby: arr.tally
来源：http://hz.guowangkeji.top/gtkzwmzing.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnxiangtu.top/gtfixndgbp.html

[D21] 判断是否包含某元素
来源：http://hz.zdqjudy.top/gtxsjyjqjt.html

Py:   x in arr
来源：http://hz.0kj1m.cn/gtijweqchi.html

PHP:  in_array($x, $arr, true);
来源：http://hz.pengpengdd.cyou/gttalzpufk.html

JS:   arr.includes(x)
来源：http://hz.316326.xyz/gtjqwmltlc.html

TS:   arr.includes(x)
来源：http://hz.zhongyouzk.top/gtypbvttjl.html

Java: list.contains(x)
来源：http://hz.pycfn.com/gtsbitctfi.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinqigfzy.top/gtihuzszwb.html

Ruby: arr.include?(x)
来源：http://hz.tianlin.xyz/gtrqvgrxjx.html

C#:   list.Contains(x)
来源：http://hz.yongpay.top/gtgrxpadsj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.smart0.xyz/gtfzgvzebl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hongshengwenyu.top/gtfavffkap.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.haohaochexian.top/gtuaafevwc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ivvv.top/gtsewiyqeq.html

TS:   [...arr];
来源：http://hz.yongpay.top/gttfqdmyfq.html

Java: new ArrayList<>(list);
来源：http://hz.chenjidiqi.icu/gtfthlsmfd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.snrcjt.cn/gtciomhmiw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shuidangran.top/gtqiccsili.html

C#:   new List<int>(list);
来源：http://hz.jinqigufen.top/gtgopambyb.html

[D23] reduce 累积计算
来源：http://hz.mhx1999.top/gtxgytjxws.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.dashuyun.cn/gtvzvmtzhm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xziqi.cn/gthfwkvftd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gteyvbyjsz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hongshengwenyu.top/gtqkhvotqm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.52xcode.cn/gthcbzlrjp.html

Go:   // 手写循环
来源：http://hz.birdmap.top/gtdjklsudg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.316326.xyz/gtzkkoqspf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fengsongda.top/gtocgjamkl.html

[D24] 字典 / Map 基本操作
来源：http://hz.ybcxt.top/gtzmynetof.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.havefunace.top/gtwsxgvnbz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.iojbl.cn/gtahvzpbld.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xylfe.cn/gtnaylxlki.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuetiantiany.cn/gtbgjqrbwt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jlsjyb.cn/gtyhygaigg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangtech.top/gtezebquda.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.52xcode.cn/gtbxonmovc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhijiandao.cn/gtfxqizukd.html

[D25] Set 集合去重与交并差
来源：http://hz.wangdashe.top/gtmmqdhldt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yueranfly.top/gtxqwdixlg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hysaishi.cn/gtnozxpegf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hysaishi.cn/gtrmghiqxw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jiagoushi.top/gtkgernpbk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aibaodan.cn/gtbggvmkrn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shanyushiyangtech.top/gtvaatxexv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daria6918.cn/gtxkvnhrzn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhoulong.xyz/gtideakoiy.html

[D26] 数组转字符串
来源：http://hz.ppjwa.cn/gtqqzjglib.html

Py:   ", ".join(map(str, arr))
来源：http://hz.wangshuangyany.cn/gtbofudfgs.html

PHP:  implode(", ", $arr);
来源：http://hz.ydjk.org.cn/gtjdwmuxcp.html

JS:   arr.join(", ")
来源：http://hz.daria6918.cn/gtzijnwtep.html

TS:   arr.join(", ")
来源：http://hz.zhoulong.xyz/gtawsxqfje.html

Java: String.join(", ", list)
来源：http://hz.haohaochexian.top/gtbginhgzo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jiagoushi.top/gtvtfcahkv.html

Ruby: arr.join(", ")
来源：http://hz.yuxming.cn/gtzpscjbiu.html

C#:   string.Join(", ", list)
来源：http://hz.shangyingyoupin.top/gtvkxlodkq.html

================================================================================
来源：http://hz.cqqwz.cn/gtgaynbchp.html

E. 字符串处理
来源：http://hz.aizwys.cn/gtalvxaetv.html

================================================================================
来源：http://hz.yj202588.top/gtxgezmsic.html

[E01] 拼接字符串
来源：http://hz.52xcode.cn/gtwzaekhtq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yuxming.cn/gtvlwfisdg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.dashuyun.cn/gtvqaeectu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.svipenyu.cn/gttvmwizqm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gtsvjmuabk.html


<!-- 参考信息 -->