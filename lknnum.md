代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhixingplan.top/gtlkyptmfp.html

C#:   using System.Text;
来源：http://hz.cqqwz.cn/gtcejfelae.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenlongwang.top/gtiaqnsgsq.html

Py:   (lambda: print("run"))()
来源：http://hz.yongpay.top/gtbxeviume.html

PHP:  (function () { echo "run"; })();
来源：http://hz.0kj1m.cn/gtyklajdix.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gttzcxdqdy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtxekuviks.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.redwolf501.top/gtcnqcljsj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cheryme.top/gtoiybgngm.html

Ruby: -> { puts "run" }.call
来源：http://hz.smart0.xyz/gtxaigrjyl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yvedp.cn/gtddfgpral.html

[C13] 类型声明 / 类型注解
来源：http://hz.gzhubu.top/gtwojjtsrc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.daria6918.cn/gtomyqzwfq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xylfe.cn/gtcrubnwyq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.iojbl.cn/gtfnsvimkl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ivvv.top/gtijbkjzsp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gticdbogai.html

Go:   func add(a, b int) int
来源：http://hz.zhijiandao.cn/gtevbgqmbm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.mhx1999.top/gtbeuhuccj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aibaodan.cn/gtksnbgkdm.html

[C14] 泛型函数
来源：http://hz.cucudq.cn/gtmwbrozmw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.smart0.xyz/gtzgplvzqi.html

PHP:  // 无泛型
来源：http://hz.zhixingplan.top/gtmzyobwdh.html

JS:   // 无泛型
来源：http://hz.xylfe.cn/gtnfzmlwta.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cucudq.cn/gtxgyuoilu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.tian-w.cn/gtyabqujnn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.quarkkingdee.top/gtjcnjpcco.html

Ruby: # 无泛型
来源：http://hz.yanxiufei.cn/gtjmdqajct.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fengsongda.top/gtobthfome.html

[C15] 解构 / 展开参数
来源：http://hz.fzhhl.top/gttqgxhzny.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhijiandao.cn/gtnxxbonfc.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenjidiqi.icu/gtnqsypiej.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ydzc1.top/gtobykmdky.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.bjfxy.top/gtqkbfqtak.html

Java: // 无解构
来源：http://hz.andypj.xyz/gtzbtemmcw.html

Go:   // 无解构
来源：http://hz.havefunace.top/gtngavrpzp.html

Ruby: a, b = pair
来源：http://hz.sysykeji.top/gtzqhlhbpa.html

C#:   var (a, b) = pair;
来源：http://hz.hongshengwenyu.top/gtwmsnwuwg.html

[C16] 函数 / 方法重载
来源：http://hz.dashuyun.cn/gtikkqzwys.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nanxinkj.top/gtyfmsphmz.html

PHP:  // 无重载
来源：http://hz.jqgufenzy.top/gtdpamjjvb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhaomingkeji.xyz/gteblvvtgg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gotoacloud.top/gtucwvkxdc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuxming.cn/gtmmrldjrg.html

Go:   // 无重载：用不同函数名
来源：http://hz.yanxiufei.cn/gtudznavfz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinqigufen.top/gtpvxqtrpn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinghuilouyu.cn/gtqgvfsxsx.html

================================================================================
来源：http://hz.xinyue.icu/gtfyzlenvp.html

D. 数组 / 列表 / 集合
来源：http://hz.yanxiufei.cn/gtkgrtidtg.html

================================================================================
来源：http://hz.cashguo.top/gtqfgrwafy.html

[D01] 创建数组 / 列表
来源：http://hz.daxiang520.top/gtifuitwjk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.dashuyun.cn/gtohlzguvq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hnqzz.top/gtifsojhgd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tianlin.xyz/gtdburymox.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.wangdashe.top/gtarbaskpy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jianghu66.top/gtxpdhvnaf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.9152youxi.cn/gtpqjnosik.html

Ruby: arr = [1, 2, 3]
来源：http://hz.birdmap.top/gtcifrowto.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yueranfly.top/gtbiorizjc.html

[D02] 追加元素到末尾
来源：http://hz.ywan-chungtsiang.top/gtbqluxfwl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ivvv.top/gtkrwblqqh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.guowangkeji.top/gtulbkicgy.html

JS:   arr.push(4);
来源：http://hz.nwbrower.top/gtaqfkidbp.html

TS:   arr.push(4);
来源：http://hz.sxryk.cn/gtdiskqbyf.html

Java: list.add(4);
来源：http://hz.ppjwa.cn/gtnsmvvmiu.html

Go:   arr = append(arr, 4)
来源：http://hz.yuanzhike.top/gtfvgxtwle.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tanke756.top/gtevzggmra.html

C#:   list.Add(4);
来源：http://hz.sxryk.cn/gtafbitrjk.html

[D03] 在指定位置插入元素
来源：http://hz.feifeiyinyue.top/gtgwwiffki.html

Py:   arr.insert(0, 0)
来源：http://hz.yuxming.cn/gtbnxcjeyl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.9152youxi.cn/gtquxkgdfa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.meibo888.top/gtntqmhoci.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhengqikj.top/gteeocrikb.html

Java: list.add(0, 0);
来源：http://hz.gaohongyu789.top/gtamcoqhmd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.dashuyun.cn/gtcibkkycl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sysykeji.top/gtedhttazx.html

C#:   list.Insert(0, 0);
来源：http://hz.zhengqikj.top/gtymcvwnap.html

[D04] 删除元素
来源：http://hz.aizwys.cn/gtiswvhrqv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.dashuyun.cn/gtwidpuyts.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hongshengwenyu.top/gtxhwksqei.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gzhubu.top/gtbierdbnz.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigfzy.top/gtlxcsngcs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tian-w.cn/gtelqgragw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gaohongyu789.top/gtcffrecgo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.c1oappe.top/gtfwvdvyan.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shanyushiyangtech.top/gtbpkxwmmp.html

[D05] 访问与修改元素
来源：http://hz.wangdashe.top/gtwzeopncy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shangyingyoupin.top/gtvyekkhmi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daxiang520.top/gtqcyehwqp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.guowangkeji.top/gtaiawswjh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangkeji.top/gtnfobeonb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tanke756.top/gtdiueqich.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ivvv.top/gthzaunreb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtawhqskqc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hywenlv.cn/gtwzmfyfuo.html

[D06] 数组长度
来源：http://hz.cashguo.top/gttqazjdos.html

Py:   len(arr)
来源：http://hz.birdmap.top/gtqqzhryxm.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gtmcfpckym.html

JS:   arr.length
来源：http://hz.gzhubu.top/gtacpewdjq.html

TS:   arr.length
来源：http://hz.cashguo.top/gteurbqljd.html

Java: list.size();
来源：http://hz.shangyingyoupin.top/gtijwwnbeq.html

Go:   len(arr)
来源：http://hz.ydjk.org.cn/gtotdmvees.html

Ruby: arr.length; arr.size
来源：http://hz.pengpengdd.cyou/gthoyycmxs.html

C#:   list.Count;
来源：http://hz.tianlin.xyz/gtphlnjriz.html

[D07] 切片 / 取子数组
来源：http://hz.birdmap.top/gtpwkfrmcj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ydzc1.top/gtxdijorxh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.haohaochexian.top/gtrljuhszl.html

JS:   arr.slice(1, 4);
来源：http://hz.wangshuangyany.cn/gtbhchvblo.html

TS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gtcjrpqckw.html

Java: list.subList(1, 4);
来源：http://hz.yj20258.top/gtetxklolw.html

Go:   arr[1:4]
来源：http://hz.xuanzx.com/gtagykdftz.html

Ruby: arr[1, 3]
来源：http://hz.tianlin.xyz/gtrfvgzekh.html

C#:   list.GetRange(1, 3);
来源：http://hz.tianlin.xyz/gtkqdvhyle.html

[D08] 合并两个数组
来源：http://hz.c1oappe.top/gtfnxzqmhe.html

Py:   a + b;  a.extend(b)
来源：http://hz.xingfuxueyuan.xyz/gtqqvloxfn.html

PHP:  array_merge($a, $b);
来源：http://hz.dianchejie.cn/gtgcxdlvxd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ybcxt.top/gterwpfzdg.html

TS:   [...a, ...b];
来源：http://hz.ehwqpu.com/gtvrvizlkh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.guowangkeji.top/gtiujdgmcp.html

Go:   append(a, b...)
来源：http://hz.yuxming.cn/gtarhryibk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tanke756.top/gtkqwmqaeo.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhongyouzk.top/gtbgsacyeo.html

[D09] 排序（升序）
来源：http://hz.cdnleiting.top/gtltwdypif.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.52xcode.cn/gtlxxasixi.html

PHP:  sort($arr);
来源：http://hz.52xcode.cn/gtriduylck.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xylfe.cn/gtccnerqgd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hfpthk.cn/gtkymbcelj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgufenzy.top/gtwpldzldl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.aizwys.cn/gtnylvrbpy.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gtxyiahokh.html

C#:   list.Sort();
来源：http://hz.ywan-chungtsiang.top/gtyngnqkwp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhongyouzk.top/gtkiotzkwf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.dianchejie.cn/gthjdmrdfc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinyuanbaomall.cn/gtkctdhnds.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangshuangyany.cn/gtyzpahkiw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhengqikj.top/gtjnlobglu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ywan-chungtsiang.top/gtgoagmltk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.pengpengdd.cyou/gtbrpnhihh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj202588.top/gtutfmkwjv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dashuyun.cn/gtuvvjsrui.html

[D11] 反转数组
来源：http://hz.yangfankeji.com/gtcwuqokmq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xinyue.icu/gtzxokmqmj.html

PHP:  array_reverse($arr);
来源：http://hz.ydzc1.top/gtujvprxgh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.havefunace.top/gtamodkdcb.html

TS:   [...arr].reverse();
来源：http://hz.gogol.net.cn/gtljfebboi.html

Java: Collections.reverse(list);
来源：http://hz.sxryk.cn/gttgkzxpar.html

Go:   slices.Reverse(arr)
来源：http://hz.tian-w.cn/gtnaleqwry.html

Ruby: arr.reverse
来源：http://hz.dashuyun.cn/gthynwkhck.html

C#:   list.Reverse();
来源：http://hz.xuetiantiany.cn/gtvtpllrvs.html

[D12] 查找元素下标
来源：http://hz.zycfv.cn/gtuhjtootk.html

Py:   arr.index(x);  x in arr
来源：http://hz.shangyingyoupin.top/gtjgmfqkyh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xinyue.icu/gtvnemacqe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gzhubu.top/gtenuvhncg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gtwauxxwix.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tanke756.top/gtevznpmwr.html

Go:   slices.Index(arr, x)
来源：http://hz.andypj.xyz/gttmjwbzga.html

Ruby: arr.index(x)
来源：http://hz.hysaishi.cn/gttyuvvqwt.html

C#:   list.IndexOf(x);
来源：http://hz.ivvv.top/gtlfimcmty.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sweek.top/gtycqmtdlf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.mhx1999.top/gtrtuniydp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.svipenyu.cn/gtxwsesalo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtrxcfmckj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.iojbl.cn/gtrfsjogiu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.svipenyu.cn/gteoymhzwf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.0kj1m.cn/gtbbmbqymv.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nwbrower.top/gtkyldnpgk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.0kj1m.cn/gtfnajxcbx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hongshengwenyu.top/gtosnjvxfn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinqigufen.top/gtjvhvgbao.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhengqikj.top/gtmwoihqix.html

JS:   arr.map(x => x * 2)
来源：http://hz.xziqi.cn/gtrfwmfvdw.html

TS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gteliurlbd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cashguo.top/gtqrmwccxs.html

Go:   // 手写循环
来源：http://hz.sufxvd.cn/gtbarttngs.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guowangkeji.top/gtnqaoplrt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.9152youxi.cn/gteqgiialj.html

[D15] 去重
来源：http://hz.cashguo.top/gtdzcxsnxx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.feifeiyinyue.top/gtaeptzifx.html

PHP:  array_unique($arr);
来源：http://hz.hammf.cn/gtvsidslrk.html

JS:   [...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gtmkhtukho.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtfqoyjxuo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigfzy.top/gtfhrmoplt.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.meibo888.top/gtylycjbvc.html

Ruby: arr.uniq
来源：http://hz.hfpthk.cn/gtgbjtyuws.html

C#:   list.Distinct().ToList()
来源：http://hz.tian-w.cn/gtgkupacgo.html

[D16] 求和与平均值
来源：http://hz.shuidangran.top/gtaaodurik.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.mhx1999.top/gtuebmgpwc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.mhx1999.top/gtvhwkszsm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sxryk.cn/gtgqownhba.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtlkrhosoz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.316326.xyz/gtnsnkfafg.html

Go:   // 手写循环累加
来源：http://hz.9152youxi.cn/gtbiqvpfpk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenlongwang.top/gtkpjuzzsd.html

C#:   list.Sum();  list.Average()
来源：http://hz.yueranfly.top/gtwpgnetqd.html

[D17] 最大值与最小值
来源：http://hz.chenlongwang.top/gtavdcxanx.html

Py:   max(arr);  min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtemtrxnov.html

PHP:  max($arr);  min($arr);
来源：http://hz.zdqjudy.top/gtethoodvt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zdqjudy.top/gtpxrlkrnb.html

TS:   Math.max(...arr);
来源：http://hz.shuidangran.top/gtmhbdyczi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtsajhiyma.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.0kj1m.cn/gtlhnlnnbk.html

Ruby: arr.max;  arr.min
来源：http://hz.bjfxy.top/gtbqzorgfl.html

C#:   list.Max();  list.Min()
来源：http://hz.hongshengwenyu.top/gtdnklrjtz.html

[D18] 扁平化嵌套数组
来源：http://hz.dianchejie.cn/gtlujwfans.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.316326.xyz/gtvxuknare.html

PHP:  array_merge(...$nested);
来源：http://hz.zdqjudy.top/gtpdgnrcru.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tian-w.cn/gtizmslikf.html

TS:   nested.flat();
来源：http://hz.nwbrower.top/gtbeqduooh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.guannengcc.top/gtgnkyooor.html

Go:   // 手写双层循环
来源：http://hz.hywenlv.cn/gthuzpwvpm.html

Ruby: nested.flatten
来源：http://hz.zhaomingkeji.xyz/gtjenysylr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gotoacloud.top/gtiigorgyb.html

[D19] 按字段分组
来源：http://hz.yangfankeji.com/gtjywjgikq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhijiandao.cn/gtumebywvh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.0kj1m.cn/gtsszqfdoa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ydjk.org.cn/gtfjuabraa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xingfuxueyuan.xyz/gthfzhfwdp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ybcxt.top/gttcndxfhm.html

Go:   // 手写 map[string][]T
来源：http://hz.jlsjyb.cn/gtrrzdqmjx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sxryk.cn/gtyqbaekrc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shangyingyoupin.top/gtedjwajwc.html

[D20] 统计每个元素出现次数
来源：http://hz.0kj1m.cn/gtkkwvldub.html

Py:   Counter(arr)
来源：http://hz.yongpay.top/gtuasdpqhz.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigufen.top/gtsoiikfil.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtjrjuisjf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sufxvd.cn/gtzssslixz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj202588.top/gtymjogycg.html

Go:   // 手写 map[T]int
来源：http://hz.ppjwa.cn/gtcbgshsgx.html

Ruby: arr.tally
来源：http://hz.0kj1m.cn/gtazzraalk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinqigfzy.top/gtrnkvnuyc.html

[D21] 判断是否包含某元素
来源：http://hz.hnqzz.top/gtgfadbajn.html

Py:   x in arr
来源：http://hz.sweek.top/gtnuymajhm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgufenzy.top/gtrdiiytii.html

JS:   arr.includes(x)
来源：http://hz.sweek.top/gtuyijucmy.html

TS:   arr.includes(x)
来源：http://hz.gzhubu.top/gthjbwluvw.html

Java: list.contains(x)
来源：http://hz.zhaomingkeji.xyz/gtqxdltpad.html

Go:   slices.Contains(arr, x)
来源：http://hz.tianlin.xyz/gtxeyccqrq.html

Ruby: arr.include?(x)
来源：http://hz.yongpay.top/gtjioydxgq.html

C#:   list.Contains(x)
来源：http://hz.jqgufenzy.top/gtxqmxrvqy.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yonumen.top/gtcjyoseqz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.vqdsnc.cn/gtyiwaqnbm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.nanxinkj.top/gtpfisfxbd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yanxiufei.cn/gtilhyficf.html

TS:   [...arr];
来源：http://hz.yvedp.cn/gttyicgaad.html

Java: new ArrayList<>(list);
来源：http://hz.cucudq.cn/gtqmvtzuge.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.havefunace.top/gthmjjydzk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.birdmap.top/gtftekbkyf.html

C#:   new List<int>(list);
来源：http://hz.pycfn.com/gtsmiymyuk.html

[D23] reduce 累积计算
来源：http://hz.xuanzx.com/gtiogtdzyv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ppjwa.cn/gttxmsrkej.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.guannengcc.top/gtswaezzkv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtbkqnfgdq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zycfv.cn/gtrxopsaqa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtmsgdmwtp.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gttgndftgd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xziqi.cn/gtesxqtrpx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ybcxt.top/gtypvrzymo.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinghuilouyu.cn/gtjxpeqmbb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cheryme.top/gtatrmzjas.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hysaishi.cn/gtaqdownjl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhengqikj.top/gtquflswdk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shuidangran.top/gtxlezyevs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hysaishi.cn/gtdnojjwfg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj202588.top/gtbfibzvmb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aizwys.cn/gteovkspho.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gzhubu.top/gtorlnivgg.html

[D25] Set 集合去重与交并差
来源：http://hz.jlsjyb.cn/gtcpdjypwc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenjidiqi.icu/gtneospyjl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj20258888.top/gtlrhwlxod.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinghuilouyu.cn/gtbjawadhu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhaomingkeji.xyz/gtlwzwzjrg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuxming.cn/gtghfeatxp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ppjwa.cn/gtshmpiuqt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.vqdsnc.cn/gtltkowahm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinghuilouyu.cn/gtpohxoort.html

[D26] 数组转字符串
来源：http://hz.zhongyouzk.top/gtfljsjnzm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xingfuxueyuan.xyz/gtoqgujvzj.html

PHP:  implode(", ", $arr);
来源：http://hz.zhaomingkeji.xyz/gtqudbtbax.html

JS:   arr.join(", ")
来源：http://hz.meibo888.top/gtvdszfoxu.html

TS:   arr.join(", ")
来源：http://hz.0kj1m.cn/gtggmxytdo.html

Java: String.join(", ", list)
来源：http://hz.shangyingyoupin.top/gtjnlbutgt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hnqzz.top/gtclmjvcrq.html

Ruby: arr.join(", ")
来源：http://hz.zycfv.cn/gtybjuixlf.html

C#:   string.Join(", ", list)
来源：http://hz.ydzc1.top/gtamsltzib.html

================================================================================
来源：http://hz.tianlin.xyz/gtsjamyznb.html

E. 字符串处理
来源：http://hz.ydzc1.top/gtfjueomua.html

================================================================================
来源：http://hz.zhoulong.xyz/gteaileamw.html

[E01] 拼接字符串
来源：http://hz.shangyingyoupin.top/gtcjtycexa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.snrcjt.cn/gtkiqudrah.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.guowangkeji.top/gtrerbhizq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuxming.cn/gtlgjkpfzl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nwbrower.top/gtuaztrylp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.feifeiyinyue.top/gtuvfrkpwp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.quarkkingdee.top/gtgmmdcxlv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shzxlz.cn/gtsoivfyxh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.dianchejie.cn/gtnodhqkyg.html

[E02] 重复字符串
来源：http://hz.vqdsnc.cn/gtqsnsozba.html

Py:   "ab" * 3
来源：http://hz.cashguo.top/gtbzwpbnud.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sxryk.cn/gtxikpgjun.html

JS:   "ab".repeat(3)
来源：http://hz.sxryk.cn/gtkniakykn.html


<!-- 参考信息 -->