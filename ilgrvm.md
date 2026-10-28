代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://hz.jlsjyb.cn/gtqdmydudo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.wangshuangyany.cn/gtvhtfmpvo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sufxvd.cn/gtvlvkzdwd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ppjwa.cn/gtgtkghirh.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenlongwang.top/gtqozppdjd.html

Ruby: -> { puts "run" }.call
来源：http://hz.daria6918.cn/gtbfgimovf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yuxming.cn/gtuxopfkwr.html

[C13] 类型声明 / 类型注解
来源：http://hz.ppjwa.cn/gthyqsaqxb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jqgfzy.top/gtldlenstp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtzdniepjp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ydjk.org.cn/gttkgzoacl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zdqjudy.top/gtxgybainf.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtdpvheooc.html

Go:   func add(a, b int) int
来源：http://hz.xuetiantiany.cn/gturnkwerm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yueranfly.top/gtikttsqmm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.tianlin.xyz/gtmlgmbshs.html

[C14] 泛型函数
来源：http://hz.xuetiantiany.cn/gtxxmvjson.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.dianchejie.cn/gtdvxieeke.html

PHP:  // 无泛型
来源：http://hz.gzhubu.top/gtsecgxdmu.html

JS:   // 无泛型
来源：http://hz.xylfe.cn/gtbkqaskvq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tanke756.top/gthdzvkvxv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinghuilouyu.cn/gtymisazpm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.guowangkeji.top/gttkavnxde.html

Ruby: # 无泛型
来源：http://hz.52xcode.cn/gtwzrhfzra.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.iojbl.cn/gtllcdrpjv.html

[C15] 解构 / 展开参数
来源：http://hz.xuanzx.com/gtlblgdhmg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.wangshuangyany.cn/gtrnqcjapq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.haohaochexian.top/gtlwjjycen.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hysaishi.cn/gtloddahbb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhongyouzk.top/gtpgjfhgme.html

Java: // 无解构
来源：http://hz.chenlongwang.top/gtdmdxcoki.html

Go:   // 无解构
来源：http://hz.yangfankeji.com/gtmcuoasnz.html

Ruby: a, b = pair
来源：http://hz.iojbl.cn/gtxtwyyvkk.html

C#:   var (a, b) = pair;
来源：http://hz.jinqigufen.top/gtljsqkfly.html

[C16] 函数 / 方法重载
来源：http://hz.9152youxi.cn/gtygezvoov.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hongshengwenyu.top/gtwjdnncnv.html

PHP:  // 无重载
来源：http://hz.xylfe.cn/gtsonpwbyb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yj202588.top/gtxiqkdivi.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinqigfzy.top/gtzovbrklr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jlsjyb.cn/gtmlhcmccw.html

Go:   // 无重载：用不同函数名
来源：http://hz.cheryme.top/gttiwuwlxk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shuidangran.top/gtugpgyhfw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.c1oappe.top/gtzzvddpdz.html

================================================================================
来源：http://hz.ppjwa.cn/gtayzymcsz.html

D. 数组 / 列表 / 集合
来源：http://hz.yuxming.cn/gtvlghkeav.html

================================================================================
来源：http://hz.snrcjt.cn/gtbfxtpuqe.html

[D01] 创建数组 / 列表
来源：http://hz.ivvv.top/gtlxjmwblf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.sweek.top/gtwwtpclwr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shanyushiyangkeji.top/gtajxdrtzc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.kuanghao11.cn/gtygankquq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yongpay.top/gtmknhowrd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinyuanbaomall.cn/gtbkaajiyb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shangyingyoupin.top/gtybpigqin.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cqqwz.cn/gtdxnftfqp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhaomingkeji.xyz/gtcgzmgymy.html

[D02] 追加元素到末尾
来源：http://hz.c1oappe.top/gtnvflztit.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xziqi.cn/gtpzhsqeme.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.bjfxy.top/gtmhtccjew.html

JS:   arr.push(4);
来源：http://hz.nanxinkj.top/gtybomzeta.html

TS:   arr.push(4);
来源：http://hz.gzhubu.top/gtetrxwvvw.html

Java: list.add(4);
来源：http://hz.fzhhl.top/gtezcwjpmh.html

Go:   arr = append(arr, 4)
来源：http://hz.shzxlz.cn/gtsuzwrdnx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ppjwa.cn/gtabiipybs.html

C#:   list.Add(4);
来源：http://hz.guowangkeji.top/gtduviuftk.html

[D03] 在指定位置插入元素
来源：http://hz.iojbl.cn/gtxaonlmmp.html

Py:   arr.insert(0, 0)
来源：http://hz.smart0.xyz/gtxoxjxjvm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yanxiufei.cn/gtifgttupc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hnxiangtu.top/gtuytqtgjy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xuetiantiany.cn/gtphnnrvwp.html

Java: list.add(0, 0);
来源：http://hz.birdmap.top/gticpqqybn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shanyushiyangtech.top/gtvaxhjvgg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenlongwang.top/gtyslwsbpy.html

C#:   list.Insert(0, 0);
来源：http://hz.smart0.xyz/gthrswusbx.html

[D04] 删除元素
来源：http://hz.yj202588.top/gttsbxcsre.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nwbrower.top/gtynxaappr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xziqi.cn/gtacknzjgi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinqigfzy.top/gtsiropbty.html

TS:   arr.splice(0, 1);
来源：http://hz.jyoumei.cn/gtdgrrikde.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fzhhl.top/gtaoeooctf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cucudq.cn/gtvtbhxxnb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.dashuyun.cn/gtshwbklii.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.316326.xyz/gttksqgncj.html

[D05] 访问与修改元素
来源：http://hz.svipenyu.cn/gtlvkrtlsa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtssvwrnih.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.pycfn.com/gtzzzvwasc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shzxlz.cn/gtkfbdkqsv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.haohaochexian.top/gtoceabnqq.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhongyouzk.top/gtxwpcnmkq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xziqi.cn/gtgmuluxgb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guannengcc.top/gtnafstypq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuetiantiany.cn/gtfozhamfp.html

[D06] 数组长度
来源：http://hz.cashguo.top/gtmecqctjc.html

Py:   len(arr)
来源：http://hz.quarkkingdee.top/gttretbwkf.html

PHP:  count($arr);
来源：http://hz.xinyue.icu/gtjhbuigju.html

JS:   arr.length
来源：http://hz.ehwqpu.com/gtxuxterib.html

TS:   arr.length
来源：http://hz.0kj1m.cn/gttxzasowb.html

Java: list.size();
来源：http://hz.dianchejie.cn/gtfpqdqcaq.html

Go:   len(arr)
来源：http://hz.snrcjt.cn/gtcgxrnhkk.html

Ruby: arr.length; arr.size
来源：http://hz.sufxvd.cn/gtltlynkhu.html

C#:   list.Count;
来源：http://hz.shangyingyoupin.top/gtjjcdrzgn.html

[D07] 切片 / 取子数组
来源：http://hz.quarkkingdee.top/gthoywdigy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.fengsongda.top/gtrgfwjbtt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ehwqpu.com/gtsvdygqhx.html

JS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtscpmuxpp.html

TS:   arr.slice(1, 4);
来源：http://hz.hnxiangtu.top/gtyzpaydgb.html

Java: list.subList(1, 4);
来源：http://hz.tian-w.cn/gtyjoqkynl.html

Go:   arr[1:4]
来源：http://hz.haohaochexian.top/gtulwbwgyc.html

Ruby: arr[1, 3]
来源：http://hz.52xcode.cn/gtqujrxeor.html

C#:   list.GetRange(1, 3);
来源：http://hz.yongpay.top/gtxpsxpqtz.html

[D08] 合并两个数组
来源：http://hz.hywenlv.cn/gtlbjadduy.html

Py:   a + b;  a.extend(b)
来源：http://hz.shzxlz.cn/gtiznoacsi.html

PHP:  array_merge($a, $b);
来源：http://hz.andypj.xyz/gtgzmllkhy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yuanzhike.top/gturcmchsk.html

TS:   [...a, ...b];
来源：http://hz.ydjk.org.cn/gtybqdwzpc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxinkj.top/gtyjouitrb.html

Go:   append(a, b...)
来源：http://hz.cucudq.cn/gtpxnleluq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj20258.top/gtabdhfrat.html

C#:   a.Concat(b).ToList()
来源：http://hz.shuidangran.top/gtjclrkhhg.html

[D09] 排序（升序）
来源：http://hz.xylfe.cn/gtohqmugly.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenzaomai.com/gtmnkpfshk.html

PHP:  sort($arr);
来源：http://hz.redwolf501.top/gtjwmyeegh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jyoumei.cn/gtprzzgejv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.snrcjt.cn/gtvicekbij.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.smart0.xyz/gtsiezlxds.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yvedp.cn/gtryrvjmfv.html

Ruby: arr.sort
来源：http://hz.ppjwa.cn/gttatjkrkf.html

C#:   list.Sort();
来源：http://hz.cheryme.top/gtfmlhzwir.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.tian-w.cn/gtndsktppm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhaomingkeji.xyz/gtwvpwxada.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jiagoushi.top/gtmphwvdbe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gttfypcmbj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sxryk.cn/gtazibsvzy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zdqjudy.top/gtnuztafoh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xinyue.icu/gtksfvfsas.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.iojbl.cn/gtergtgaon.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.mhx1999.top/gtpckqmmhp.html

[D11] 反转数组
来源：http://hz.yuanzhike.top/gtnhpslyuy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.svipenyu.cn/gtmmahfpug.html

PHP:  array_reverse($arr);
来源：http://hz.birdmap.top/gtedevshcv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hywenlv.cn/gtqqpnljwj.html

TS:   [...arr].reverse();
来源：http://hz.jqgufenzy.top/gtcojpmhlp.html

Java: Collections.reverse(list);
来源：http://hz.smart0.xyz/gtlihoymgk.html

Go:   slices.Reverse(arr)
来源：http://hz.wangdashe.top/gtvojzonzh.html

Ruby: arr.reverse
来源：http://hz.cdnleiting.top/gtyniihxwl.html

C#:   list.Reverse();
来源：http://hz.andypj.xyz/gtnnmiswin.html

[D12] 查找元素下标
来源：http://hz.daxiang520.top/gtacaiskts.html

Py:   arr.index(x);  x in arr
来源：http://hz.0kj1m.cn/gtzmwbrfah.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.fzhhl.top/gtsddewmtd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydjk.org.cn/gtektsqnuq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shzxlz.cn/gtkazrppov.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sweek.top/gtwaypozsq.html

Go:   slices.Index(arr, x)
来源：http://hz.birdmap.top/gttqeknovx.html

Ruby: arr.index(x)
来源：http://hz.xingfuxueyuan.xyz/gtrotmjrnm.html

C#:   list.IndexOf(x);
来源：http://hz.jiagoushi.top/gtyltcgviq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nanxuanxn.top/gtsftspklc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jqgfzy.top/gtimqpjyiv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhengqikj.top/gtksynjxec.html

JS:   arr.filter(x => x > 3)
来源：http://hz.nwbrower.top/gturjdpnml.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gtfsdqenuk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ivvv.top/gtrdhedhcs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.quarkkingdee.top/gtjbjzjknd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ybcxt.top/gtkxvpjlzm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sysykeji.top/gtmhyzzzdw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ywan-chungtsiang.top/gtynpdfznq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tianlin.xyz/gtiwwhdzuw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xziqi.cn/gtrvucqsut.html

JS:   arr.map(x => x * 2)
来源：http://hz.quarkkingdee.top/gtidalzlno.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gtueotloek.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.snrcjt.cn/gtoljmnvdy.html

Go:   // 手写循环
来源：http://hz.snrcjt.cn/gthctogeaw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinghuilouyu.cn/gtvswpakjn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhengqikj.top/gtiuyimanx.html

[D15] 去重
来源：http://hz.cheryme.top/gtliyageca.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenzaomai.com/gtjqpvakkg.html

PHP:  array_unique($arr);
来源：http://hz.0kj1m.cn/gtusrypxsx.html

JS:   [...new Set(arr)]
来源：http://hz.wangshuangyany.cn/gtzbanvoef.html

TS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtboasvlcj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258888.top/gtbvlttokz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.andypj.xyz/gtmyvdbvfm.html

Ruby: arr.uniq
来源：http://hz.birdmap.top/gtjmcffxtx.html

C#:   list.Distinct().ToList()
来源：http://hz.cashguo.top/gtxpotjoya.html

[D16] 求和与平均值
来源：http://hz.havefunace.top/gtltkimusy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xinyue.icu/gtvhwfapcr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj20258.top/gtfkfurmod.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.haohaochexian.top/gtcpwlztiu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtuozfksju.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tianlin.xyz/gtajiymrzz.html

Go:   // 手写循环累加
来源：http://hz.jqgfzy.top/gtbxetnwwo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xuetiantiany.cn/gtfxnhdpft.html

C#:   list.Sum();  list.Average()
来源：http://hz.yueranfly.top/gtdsnemslx.html

[D17] 最大值与最小值
来源：http://hz.jqgfzy.top/gtdrxmgzbg.html

Py:   max(arr);  min(arr)
来源：http://hz.hywenlv.cn/gtfhvugkff.html

PHP:  max($arr);  min($arr);
来源：http://hz.svipenyu.cn/gtusjfqxhi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhengqikj.top/gtlkuvsgxc.html

TS:   Math.max(...arr);
来源：http://hz.hywenlv.cn/gtzrvezpyp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinghuilouyu.cn/gtoowqquzk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.tanke756.top/gtvonsxzqr.html

Ruby: arr.max;  arr.min
来源：http://hz.chenzaomai.com/gttbpunpvr.html

C#:   list.Max();  list.Min()
来源：http://hz.wangshuangyany.cn/gtwyiiaetq.html

[D18] 扁平化嵌套数组
来源：http://hz.xinyue.icu/gtfhdlibjh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ppjwa.cn/gtesjqmkqn.html

PHP:  array_merge(...$nested);
来源：http://hz.0kj1m.cn/gtbpzqatwj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ehwqpu.com/gtgsrrxjmg.html

TS:   nested.flat();
来源：http://hz.snrcjt.cn/gtypfpmxfq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zycfv.cn/gtlwxflykf.html

Go:   // 手写双层循环
来源：http://hz.jinqigfzy.top/gtnfyyfhzo.html

Ruby: nested.flatten
来源：http://hz.hywenlv.cn/gtucsjhrpq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gtxunrztap.html

[D19] 按字段分组
来源：http://hz.vqdsnc.cn/gtdvcpowwa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.quarkkingdee.top/gtlmdxscvb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.9152youxi.cn/gtrnrwslmi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yongpay.top/gtxqsotxwb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shzxlz.cn/gtffadebsd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhixingplan.top/gtozqbuzyc.html

Go:   // 手写 map[string][]T
来源：http://hz.hfpthk.cn/gtsbdoscpp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yangfankeji.com/gthfbjfebs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hywenlv.cn/gtkxspkkbq.html

[D20] 统计每个元素出现次数
来源：http://hz.andypj.xyz/gtnfcovenc.html

Py:   Counter(arr)
来源：http://hz.vqdsnc.cn/gtarplprlg.html

PHP:  array_count_values($arr);
来源：http://hz.tian-w.cn/gtvrvikkie.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtvbxowbsh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.316326.xyz/gtrkswythq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hfpthk.cn/gtfmieqlvz.html

Go:   // 手写 map[T]int
来源：http://hz.hfpthk.cn/gtrquwlbry.html

Ruby: arr.tally
来源：http://hz.sxryk.cn/gtbekiragc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhijiandao.cn/gtuzaklzqs.html

[D21] 判断是否包含某元素
来源：http://hz.zhijiandao.cn/gtdgudgzyr.html

Py:   x in arr
来源：http://hz.sweek.top/gtndohkzii.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xziqi.cn/gthcsxlncp.html

JS:   arr.includes(x)
来源：http://hz.gogol.net.cn/gtbjtovcgk.html

TS:   arr.includes(x)
来源：http://hz.yangfankeji.com/gtuhrxwenz.html

Java: list.contains(x)
来源：http://hz.xuetiantiany.cn/gtphmmbayu.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuanzhike.top/gtvzwouuuo.html

Ruby: arr.include?(x)
来源：http://hz.jyoumei.cn/gtrwvsvkpr.html

C#:   list.Contains(x)
来源：http://hz.xylfe.cn/gtzqqekoep.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cdnleiting.top/gtfluislhp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gaohongyu789.top/gtbagninje.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhoulong.xyz/gtjngwvcix.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gogol.net.cn/gtsdiawznn.html

TS:   [...arr];
来源：http://hz.ivvv.top/gtmzvguruq.html

Java: new ArrayList<>(list);
来源：http://hz.hywenlv.cn/gtqfcahmcb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yvedp.cn/gtbcgiatrv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gzhubu.top/gtbzysjhmz.html

C#:   new List<int>(list);
来源：http://hz.gogol.net.cn/gtfafnrhcf.html

[D23] reduce 累积计算
来源：http://hz.jqgfzy.top/gtckpfjaev.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jlsjyb.cn/gtsekxbwgc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zycfv.cn/gtokduovbs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtrzglxkvp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gtgvaeyrlc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.aizwys.cn/gtxawhyxvh.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtlhbexobs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.havefunace.top/gtqetpqzju.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangdashe.top/gtnliejovk.html

[D24] 字典 / Map 基本操作
来源：http://hz.xuanzx.com/gtxcagzzfm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.svipenyu.cn/gtbjtezkrk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.wangdashe.top/gtkjuxowej.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cucudq.cn/gtyvnbjbxh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.snrcjt.cn/gtsfibguzv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zdqjudy.top/gtrfetcqgn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhongyouzk.top/gtzntdmuld.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hywenlv.cn/gtcknjankm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yvedp.cn/gtuzivipmd.html

[D25] Set 集合去重与交并差
来源：http://hz.dianchejie.cn/gtvgyudtaw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.chenjidiqi.icu/gtwsljdqkv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenjidiqi.icu/gtnyfpedgt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hysaishi.cn/gtijgmwqhq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinyuanbaomall.cn/gtepfubnlq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.guannengcc.top/gthxphswwh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xinyue.icu/gtzpgyrfyu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.52xcode.cn/gtghpazlmc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj20258888.top/gtvqikfkfp.html

[D26] 数组转字符串
来源：http://hz.kuanghao11.cn/gtfwudpgpo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yueranfly.top/gtptvnsyfx.html

PHP:  implode(", ", $arr);
来源：http://hz.sxryk.cn/gthzkasbnw.html

JS:   arr.join(", ")
来源：http://hz.cashguo.top/gtyvjzrtwo.html

TS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gtsmbqymmu.html

Java: String.join(", ", list)
来源：http://hz.yuanzhike.top/gtiekukdyb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.bjfxy.top/gtgxjcbnrl.html

Ruby: arr.join(", ")
来源：http://hz.sysykeji.top/gtwepxtwku.html

C#:   string.Join(", ", list)
来源：http://hz.andypj.xyz/gtquvlxsub.html

================================================================================
来源：http://hz.fengsongda.top/gtwivqqqip.html

E. 字符串处理
来源：http://hz.0kj1m.cn/gtzikmvxha.html

================================================================================
来源：http://hz.svipenyu.cn/gtatqydnbk.html

[E01] 拼接字符串
来源：http://hz.cheryme.top/gtsiexxgde.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hysaishi.cn/gtjtzkkcji.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj202588.top/gthbiexbrb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hfpthk.cn/gtzuqexywr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tianlin.xyz/gtlgngjdoz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenjidiqi.icu/gtkplmaamf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gotoacloud.top/gthfgglurh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ydjk.org.cn/gtvqemucbl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangshuangyany.cn/gtducfnnaf.html

[E02] 重复字符串
来源：http://hz.sysykeji.top/gtuqvvmrtn.html

Py:   "ab" * 3
来源：http://hz.iojbl.cn/gtlrcdgywm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aizwys.cn/gtsmszwkeu.html

JS:   "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gtyygfreby.html

TS:   "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gttlvpadmv.html

Java: "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtwhcetwxa.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jianghu66.top/gtgmkwdivf.html

Ruby: "ab" * 3
来源：http://hz.chenlongwang.top/gtihbvisuh.html


<!-- 参考信息 -->