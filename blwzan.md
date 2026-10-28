代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://hz.zhixingplan.top/gtdaiilojx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sxryk.cn/gtakabuete.html

TS:   (() => { console.log("run"); })();
来源：http://hz.nanxinkj.top/gtqyjpmgys.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.ppjwa.cn/gthzjkqhke.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sxryk.cn/gtgtwimngt.html

Ruby: -> { puts "run" }.call
来源：http://hz.birdmap.top/gtfcamoxqt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sysykeji.top/gtfcfgdsjl.html

[C13] 类型声明 / 类型注解
来源：http://hz.birdmap.top/gtczcxobyh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shangyingyoupin.top/gtkhvvdnbw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtzhxsjasv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yvedp.cn/gttzgsuuft.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yonumen.top/gtcgcibsts.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtmybowhdo.html

Go:   func add(a, b int) int
来源：http://hz.sufxvd.cn/gtzpijiakr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.iojbl.cn/gtxdllbxqy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gotoacloud.top/gtpagsgcvf.html

[C14] 泛型函数
来源：http://hz.zycfv.cn/gtzanuyaxp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuanzx.com/gtiicaspfq.html

PHP:  // 无泛型
来源：http://hz.chenlongwang.top/gtcwdwpybk.html

JS:   // 无泛型
来源：http://hz.tanke756.top/gthoejvdzf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuetiantiany.cn/gteouxiycx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.svipenyu.cn/gtwipszmux.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hammf.cn/gtkqaqvxcc.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangtech.top/gtvxrumcxj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.redwolf501.top/gtpnskoiet.html

[C15] 解构 / 展开参数
来源：http://hz.yonumen.top/gtlhennawi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hywenlv.cn/gtgxzwqxtq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhiwuduotai.top/gtheknzxxi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yonumen.top/gtdlafnoxs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gogol.net.cn/gtfrfkdjwu.html

Java: // 无解构
来源：http://hz.xuetiantiany.cn/gtsgoxnjbr.html

Go:   // 无解构
来源：http://hz.vqdsnc.cn/gtncvemddj.html

Ruby: a, b = pair
来源：http://hz.hnqzz.top/gtcrycsyvx.html

C#:   var (a, b) = pair;
来源：http://hz.havefunace.top/gtweupbsyc.html

[C16] 函数 / 方法重载
来源：http://hz.ydjk.org.cn/gtahkolzbp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.shanyushiyangtech.top/gtprrskqma.html

PHP:  // 无重载
来源：http://hz.yuxming.cn/gtqfolcwhn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shzxlz.cn/gtjfycxlda.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuxming.cn/gtomynjikh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxinkj.top/gttqiwqrci.html

Go:   // 无重载：用不同函数名
来源：http://hz.haohaochexian.top/gttchkujap.html

Ruby: # 无重载：靠动态参数
来源：http://hz.iojbl.cn/gtdmuipzue.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhixingplan.top/gtqahjgami.html

================================================================================
来源：http://hz.zhoulong.xyz/gtelvzjnaq.html

D. 数组 / 列表 / 集合
来源：http://hz.xingfuxueyuan.xyz/gtoapdcppz.html

================================================================================
来源：http://hz.cashguo.top/gtsncwbwhs.html

[D01] 创建数组 / 列表
来源：http://hz.smart0.xyz/gtatoagepi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ydzc1.top/gtcvfzwxet.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.c1oappe.top/gtwslsvecs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinyuanbaomall.cn/gtpmuiqyhg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hysaishi.cn/gtnytygnjx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shangyingyoupin.top/gtkgiyiyyw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.c1oappe.top/gtbvvcbcuw.html

Ruby: arr = [1, 2, 3]
来源：http://hz.redwolf501.top/gtaxepoczz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ivvv.top/gthqpkogwm.html

[D02] 追加元素到末尾
来源：http://hz.dashuyun.cn/gtiayfelej.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.c1oappe.top/gttylhwmxd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hysaishi.cn/gtkoumzryq.html

JS:   arr.push(4);
来源：http://hz.aibaodan.cn/gthwckyukj.html

TS:   arr.push(4);
来源：http://hz.yvedp.cn/gtxkaalplz.html

Java: list.add(4);
来源：http://hz.fzhhl.top/gtqrkksmyb.html

Go:   arr = append(arr, 4)
来源：http://hz.ehwqpu.com/gtvsiooiwj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daria6918.cn/gttcswnntc.html

C#:   list.Add(4);
来源：http://hz.guannengcc.top/gtmsggfufg.html

[D03] 在指定位置插入元素
来源：http://hz.chenjidiqi.icu/gtrvhcuxlk.html

Py:   arr.insert(0, 0)
来源：http://hz.zhoulong.xyz/gtqukvuomj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hnqzz.top/gtbsnbgfem.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgufenzy.top/gtbdexodia.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.andypj.xyz/gtqgwfgixf.html

Java: list.add(0, 0);
来源：http://hz.zhongyouzk.top/gtqnvthpam.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.svipenyu.cn/gtraarhqyl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinqigfzy.top/gteghdzcyw.html

C#:   list.Insert(0, 0);
来源：http://hz.yongpay.top/gtobzascdg.html

[D04] 删除元素
来源：http://hz.chenjidiqi.icu/gtuhdulxrg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jqgufenzy.top/gtabbqlcko.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.aibaodan.cn/gtflqpvpwj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cdnleiting.top/gtmnsjkvrz.html

TS:   arr.splice(0, 1);
来源：http://hz.gaohongyu789.top/gtiezlvaun.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.quarkkingdee.top/gtqyntucik.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.redwolf501.top/gtnqfgpvoj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ydjk.org.cn/gtrdsgtzwr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zdqjudy.top/gtldvqsxar.html

[D05] 访问与修改元素
来源：http://hz.ehwqpu.com/gtqnbxkcck.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.svipenyu.cn/gtzatvqyzi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.wangdashe.top/gtdsquoonj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aizwys.cn/gtxtbpiocp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhengqikj.top/gtserydids.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guannengcc.top/gtontpmmoz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yangfankeji.com/gtrayistwg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sufxvd.cn/gthbjcesou.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.snrcjt.cn/gttqpmyjya.html

[D06] 数组长度
来源：http://hz.316326.xyz/gtwdaicnot.html

Py:   len(arr)
来源：http://hz.ydjk.org.cn/gtrmqbhrgf.html

PHP:  count($arr);
来源：http://hz.aizwys.cn/gtpgfgmfev.html

JS:   arr.length
来源：http://hz.hysaishi.cn/gtzksztiyb.html

TS:   arr.length
来源：http://hz.yj20258.top/gtrfuuvyxy.html

Java: list.size();
来源：http://hz.cashguo.top/gtxqicsubj.html

Go:   len(arr)
来源：http://hz.sufxvd.cn/gthpagcugn.html

Ruby: arr.length; arr.size
来源：http://hz.aibaodan.cn/gtqfopxiju.html

C#:   list.Count;
来源：http://hz.andypj.xyz/gtoehqddfn.html

[D07] 切片 / 取子数组
来源：http://hz.cashguo.top/gticbisfeb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.fzhhl.top/gtlqyvvqsa.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenlongwang.top/gtprdkbnac.html

JS:   arr.slice(1, 4);
来源：http://hz.jyoumei.cn/gtefcdosgh.html

TS:   arr.slice(1, 4);
来源：http://hz.dashuyun.cn/gtstngzsvf.html

Java: list.subList(1, 4);
来源：http://hz.sxryk.cn/gtxjpyxtzw.html

Go:   arr[1:4]
来源：http://hz.shangyingyoupin.top/gthgluvwkh.html

Ruby: arr[1, 3]
来源：http://hz.aizwys.cn/gtgzwdqgdx.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuetiantiany.cn/gtbzywfxmb.html

[D08] 合并两个数组
来源：http://hz.cucudq.cn/gtzyvmpohe.html

Py:   a + b;  a.extend(b)
来源：http://hz.gotoacloud.top/gthzhdglic.html

PHP:  array_merge($a, $b);
来源：http://hz.jqgufenzy.top/gtqfqwlkiq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinqigfzy.top/gtgwiyifdr.html

TS:   [...a, ...b];
来源：http://hz.nwbrower.top/gtitadhrpg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ywan-chungtsiang.top/gtypauzzoa.html

Go:   append(a, b...)
来源：http://hz.chenjidiqi.icu/gtorsyshhv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.sysykeji.top/gtprnwbfwp.html

C#:   a.Concat(b).ToList()
来源：http://hz.9152youxi.cn/gtrqrksxgl.html

[D09] 排序（升序）
来源：http://hz.nwbrower.top/gtzwjtzhwr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtqnijbuoi.html

PHP:  sort($arr);
来源：http://hz.xuanzx.com/gtimlqqtvy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgfzy.top/gtyuwxtzbm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.kuanghao11.cn/gtdluxswck.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.quarkkingdee.top/gtgbrhsmej.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.quarkkingdee.top/gtxcimqego.html

Ruby: arr.sort
来源：http://hz.zycfv.cn/gtomyichpq.html

C#:   list.Sort();
来源：http://hz.wangshuangyany.cn/gthfuyhhvs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.smart0.xyz/gtyjpnudyd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sweek.top/gtauhykvhs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtwwouvslq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ehwqpu.com/gtwjfmvfxj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuetiantiany.cn/gtgmrrprnv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yvedp.cn/gtzphgxvvq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xuanzx.com/gtyxzixecy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.snrcjt.cn/gtcqxbjtzx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shzxlz.cn/gtifmpxhat.html

[D11] 反转数组
来源：http://hz.jqgufenzy.top/gtphricuzc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangkeji.top/gtitevjvyq.html

PHP:  array_reverse($arr);
来源：http://hz.hongshengwenyu.top/gtydphsvvr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hnqzz.top/gtvivsbruw.html

TS:   [...arr].reverse();
来源：http://hz.birdmap.top/gtkjafcpbo.html

Java: Collections.reverse(list);
来源：http://hz.zhongyouzk.top/gtuonexbzr.html

Go:   slices.Reverse(arr)
来源：http://hz.svipenyu.cn/gtcvhzksnp.html

Ruby: arr.reverse
来源：http://hz.sweek.top/gtiorbqenq.html

C#:   list.Reverse();
来源：http://hz.zhixingplan.top/gtgbuvmeft.html

[D12] 查找元素下标
来源：http://hz.hammf.cn/gtfkklsoky.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangtech.top/gtnylmkecn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.wangdashe.top/gtzihrxlpw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dashuyun.cn/gtcnfssbjh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.birdmap.top/gteexgqgxh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jlsjyb.cn/gtoqrbizry.html

Go:   slices.Index(arr, x)
来源：http://hz.gogol.net.cn/gtjtjmoaob.html

Ruby: arr.index(x)
来源：http://hz.meibo888.top/gtbrcovgdb.html

C#:   list.IndexOf(x);
来源：http://hz.gotoacloud.top/gtajngqonp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guannengcc.top/gtbefoewby.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ybcxt.top/gtlduwrbwd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yuanzhike.top/gtduhoqdxq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cdnleiting.top/gtjmmlanvf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gotoacloud.top/gtdktelkcz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.vqdsnc.cn/gtgjnxaoyh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.52xcode.cn/gtrbocpalp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinqigfzy.top/gtvcamjhmr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cdnleiting.top/gtfqkzisto.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dashuyun.cn/gtskhbzeda.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.andypj.xyz/gtcdzhbxwi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.mhx1999.top/gtlqlhdtdp.html

JS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtvrufhbbx.html

TS:   arr.map(x => x * 2)
来源：http://hz.tianlin.xyz/gtphyafsfj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shangyingyoupin.top/gtkzleucdp.html

Go:   // 手写循环
来源：http://hz.jinyuanbaomall.cn/gtddajwbvy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.redwolf501.top/gtfnmfavmz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.aibaodan.cn/gthcssfjwl.html

[D15] 去重
来源：http://hz.nanxinkj.top/gtonmqyfnm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtuwcdiufh.html

PHP:  array_unique($arr);
来源：http://hz.cdnleiting.top/gtnozepfmb.html

JS:   [...new Set(arr)]
来源：http://hz.xuetiantiany.cn/gtvudsyeck.html

TS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtllmzqyxf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.smart0.xyz/gtjwmtotku.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cdnleiting.top/gtpviarfvp.html

Ruby: arr.uniq
来源：http://hz.tianlin.xyz/gtacjpsmmm.html

C#:   list.Distinct().ToList()
来源：http://hz.mhx1999.top/gtbjmsqnbw.html

[D16] 求和与平均值
来源：http://hz.meibo888.top/gtlaghxbhq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yonumen.top/gtrtlqeuqg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhijiandao.cn/gtmfefozxr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.andypj.xyz/gtmmvyvfjt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cqqwz.cn/gtxsedjldi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnqzz.top/gtuoztciid.html

Go:   // 手写循环累加
来源：http://hz.guowangkeji.top/gtpbrcbzzk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hysaishi.cn/gtkubhuuzj.html

C#:   list.Sum();  list.Average()
来源：http://hz.pycfn.com/gtzklinsvb.html

[D17] 最大值与最小值
来源：http://hz.c1oappe.top/gttnyekeeg.html

Py:   max(arr);  min(arr)
来源：http://hz.jinqigfzy.top/gtwtlatmzm.html

PHP:  max($arr);  min($arr);
来源：http://hz.gzhubu.top/gtxwwokpwc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tianlin.xyz/gtkhicbrcp.html

TS:   Math.max(...arr);
来源：http://hz.ehwqpu.com/gtodbhlqkf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinghuilouyu.cn/gthqkegthr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.vqdsnc.cn/gtjmvqmosp.html

Ruby: arr.max;  arr.min
来源：http://hz.guannengcc.top/gtvtmstzit.html

C#:   list.Max();  list.Min()
来源：http://hz.yonumen.top/gtrveqxven.html

[D18] 扁平化嵌套数组
来源：http://hz.yuanzhike.top/gtfvxokhau.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.havefunace.top/gtkmgxgxhb.html

PHP:  array_merge(...$nested);
来源：http://hz.pycfn.com/gttywwzjiq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhongyouzk.top/gtrhworldx.html

TS:   nested.flat();
来源：http://hz.nanxinkj.top/gtdreprpoi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhijiandao.cn/gtrnkhvtyr.html

Go:   // 手写双层循环
来源：http://hz.yuxming.cn/gtwnumyopu.html

Ruby: nested.flatten
来源：http://hz.52xcode.cn/gtnevxoajm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.quarkkingdee.top/gtmkugbget.html

[D19] 按字段分组
来源：http://hz.ybcxt.top/gtfqmiaujt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zdqjudy.top/gtvchsrsjs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ppjwa.cn/gtmtuvjmpd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.fengsongda.top/gtpvudbhll.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gogol.net.cn/gtiotnspoh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jyoumei.cn/gtvmcyqugm.html

Go:   // 手写 map[string][]T
来源：http://hz.feifeiyinyue.top/gthcqxirzr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.quarkkingdee.top/gttbajcczf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jyoumei.cn/gtwluybdbh.html

[D20] 统计每个元素出现次数
来源：http://hz.andypj.xyz/gtpaysbcby.html

Py:   Counter(arr)
来源：http://hz.hywenlv.cn/gtewiduotb.html

PHP:  array_count_values($arr);
来源：http://hz.feifeiyinyue.top/gthhyjwlcp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtxcjeqmjl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tanke756.top/gtymlasrio.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigfzy.top/gtxzomjugy.html

Go:   // 手写 map[T]int
来源：http://hz.snrcjt.cn/gtrnxlasyf.html

Ruby: arr.tally
来源：http://hz.zycfv.cn/gtzbppyxgp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.meibo888.top/gtmdwnqhnj.html

[D21] 判断是否包含某元素
来源：http://hz.sweek.top/gtzodmbthx.html

Py:   x in arr
来源：http://hz.wangdashe.top/gtzadikqha.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yonumen.top/gtdbkuryyz.html

JS:   arr.includes(x)
来源：http://hz.zycfv.cn/gtlnpuaxxh.html

TS:   arr.includes(x)
来源：http://hz.jyoumei.cn/gttoukxtzn.html

Java: list.contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtdszjxqvp.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgfzy.top/gtxiihaoln.html

Ruby: arr.include?(x)
来源：http://hz.jinyuanbaomall.cn/gtknmajyop.html

C#:   list.Contains(x)
来源：http://hz.zhongyouzk.top/gttrxdqbzr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenzaomai.com/gtibslwcyw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydzc1.top/gtjpuzemnx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aibaodan.cn/gtzjqirqif.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhixingplan.top/gtfucdgcmw.html

TS:   [...arr];
来源：http://hz.pycfn.com/gtqkxiudee.html

Java: new ArrayList<>(list);
来源：http://hz.jqgufenzy.top/gtzoosdpll.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhoulong.xyz/gthbeworij.html

Ruby: arr.dup;  arr.clone
来源：http://hz.daxiang520.top/gtgrzlaonj.html

C#:   new List<int>(list);
来源：http://hz.sweek.top/gtocgxdguh.html

[D23] reduce 累积计算
来源：http://hz.pycfn.com/gtohpzhgyx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yongpay.top/gtcbgiemll.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj202588.top/gtlplevpeo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtixutrfxs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guannengcc.top/gtmzrudfuo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj202588.top/gtneekhiuk.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gtsokjyokx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shzxlz.cn/gtaemdokyx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xylfe.cn/gtezsoqvvl.html

[D24] 字典 / Map 基本操作
来源：http://hz.guannengcc.top/gtxvftydav.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hnqzz.top/gtifjnyvdg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yonumen.top/gtilxebait.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jqgufenzy.top/gtitybljug.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hammf.cn/gtjxhmtxsd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jyoumei.cn/gtxjxryljy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.birdmap.top/gtvggeyurl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jianghu66.top/gtcwxwsyjz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cheryme.top/gtkwfuemhk.html

[D25] Set 集合去重与交并差
来源：http://hz.xuetiantiany.cn/gtwvrnsoeg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xinyue.icu/gtzjiddzlj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xuanzx.com/gtawarvhns.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.haohaochexian.top/gtmkeczayy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yonumen.top/gtkltpjtyc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jyoumei.cn/gtvucdajcp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gzhubu.top/gtvwlvunbv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tianlin.xyz/gtlfpwdlld.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.redwolf501.top/gtavuisjvq.html

[D26] 数组转字符串
来源：http://hz.smart0.xyz/gtawcqgqbu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sweek.top/gtnpsbeqpi.html

PHP:  implode(", ", $arr);
来源：http://hz.iojbl.cn/gtdihqskuw.html

JS:   arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtawwehxog.html

TS:   arr.join(", ")
来源：http://hz.nanxuanxn.top/gtohyiwykr.html

Java: String.join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtojtgiopp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgfzy.top/gtsaypicax.html

Ruby: arr.join(", ")
来源：http://hz.guowangkeji.top/gtsfkdstpm.html

C#:   string.Join(", ", list)
来源：http://hz.cucudq.cn/gtgvswccyp.html

================================================================================
来源：http://hz.shuidangran.top/gtsauykpyf.html

E. 字符串处理
来源：http://hz.shzxlz.cn/gthjyqjjlc.html

================================================================================
来源：http://hz.dianchejie.cn/gtnuuvdsxi.html

[E01] 拼接字符串
来源：http://hz.shanyushiyangtech.top/gteheuwwtw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhongyouzk.top/gteodlucxz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.vqdsnc.cn/gtlhxlxjuq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtmuepcscp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yvedp.cn/gtdxpbqytx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tanke756.top/gtdgolfwqv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.feifeiyinyue.top/gtruceyyuw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258.top/gttvmuvmjr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sweek.top/gtbokhgmhf.html

[E02] 重复字符串
来源：http://hz.xinyue.icu/gtlbciitqf.html

Py:   "ab" * 3
来源：http://hz.ehwqpu.com/gtwzxzvasc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xziqi.cn/gtrfbkgmdl.html

JS:   "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtzotkzlqg.html

TS:   "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtuzybsbso.html

Java: "ab".repeat(3)
来源：http://hz.yvedp.cn/gtqzoyatis.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.fengsongda.top/gtfddjxkzb.html

Ruby: "ab" * 3
来源：http://hz.shuidangran.top/gtqhaikozl.html


<!-- 参考信息 -->