代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hz.havefunace.top/gtcxaictmx.html

C#:   using System.Text;
来源：http://hz.chenjidiqi.icu/gtlothiayb.html

[C12] 立即执行函数 IIFE
来源：http://hz.jlsjyb.cn/gtmfzmhxaj.html

Py:   (lambda: print("run"))()
来源：http://hz.tianlin.xyz/gtdovwgqkh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhiwuduotai.top/gtgkwdqoni.html

JS:   (() => { console.log("run"); })();
来源：http://hz.vqdsnc.cn/gttznuczir.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hfpthk.cn/gtkfiokldv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhiwuduotai.top/gtgzgbjbio.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hongshengwenyu.top/gtmvdgbsjn.html

Ruby: -> { puts "run" }.call
来源：http://hz.jqgufenzy.top/gtckncbzss.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shanyushiyangkeji.top/gtdfdqabbj.html

[C13] 类型声明 / 类型注解
来源：http://hz.daria6918.cn/gtogiiziwl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sweek.top/gtizydagiw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtgophijzj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gturahndyj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sxryk.cn/gtyhubgkpv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gtzthnqpso.html

Go:   func add(a, b int) int
来源：http://hz.jyoumei.cn/gtfvjkjpuy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.havefunace.top/gtgipazebn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydzc1.top/gtmvypeenb.html

[C14] 泛型函数
来源：http://hz.zhengqikj.top/gtmbhzuann.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj20258.top/gtrphqusqc.html

PHP:  // 无泛型
来源：http://hz.aizwys.cn/gtkmsavlrp.html

JS:   // 无泛型
来源：http://hz.ivvv.top/gtxpiymhip.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zdqjudy.top/gtlfqjurkc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.nanxinkj.top/gtzwpkjstk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj20258888.top/gtrheipomc.html

Ruby: # 无泛型
来源：http://hz.sysykeji.top/gtqhfedcli.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shanyushiyangtech.top/gtfnghfhnx.html

[C15] 解构 / 展开参数
来源：http://hz.jlsjyb.cn/gtnjpjsowz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hywenlv.cn/gtvdvxkveu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenlongwang.top/gtbbptikas.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gotoacloud.top/gthhxcnjif.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.havefunace.top/gtsrygjkwq.html

Java: // 无解构
来源：http://hz.hysaishi.cn/gtvzkpxkwn.html

Go:   // 无解构
来源：http://hz.mhx1999.top/gtyptdjmdv.html

Ruby: a, b = pair
来源：http://hz.sxryk.cn/gtncavynpl.html

C#:   var (a, b) = pair;
来源：http://hz.fzhhl.top/gtmuthqzxk.html

[C16] 函数 / 方法重载
来源：http://hz.guowangkeji.top/gtvrhsahgq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dianchejie.cn/gtgifujurq.html

PHP:  // 无重载
来源：http://hz.gotoacloud.top/gtdzmkdbpk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigufen.top/gtsbxuzstv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.52xcode.cn/gtqxjtcqgh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tanke756.top/gthgisybep.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhengqikj.top/gtpiwidhzp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ybcxt.top/gtlnogiogl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yongpay.top/gtrcxpizne.html

================================================================================
来源：http://hz.snrcjt.cn/gtmwgizgpr.html

D. 数组 / 列表 / 集合
来源：http://hz.redwolf501.top/gtlujfpqbc.html

================================================================================
来源：http://hz.tanke756.top/gtpiwuvtqo.html

[D01] 创建数组 / 列表
来源：http://hz.fengsongda.top/gtggegwidq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenlongwang.top/gtqqaukxcp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuanzhike.top/gtjqjzdeke.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daxiang520.top/gtiakhqlzh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.svipenyu.cn/gtfebjnxmp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhaomingkeji.xyz/gtcvbmevpf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tanke756.top/gtunbozmhb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.dianchejie.cn/gtgrhmqxjg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.mhx1999.top/gtlvjsagmo.html

[D02] 追加元素到末尾
来源：http://hz.aizwys.cn/gtarzumhbv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.svipenyu.cn/gthujicdgw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cucudq.cn/gthrirhsdp.html

JS:   arr.push(4);
来源：http://hz.yvedp.cn/gtdbicdkwe.html

TS:   arr.push(4);
来源：http://hz.nanxinkj.top/gtjfegumif.html

Java: list.add(4);
来源：http://hz.xylfe.cn/gtjdpepaff.html

Go:   arr = append(arr, 4)
来源：http://hz.smart0.xyz/gtobrdrsmq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ybcxt.top/gtcowcascf.html

C#:   list.Add(4);
来源：http://hz.ywan-chungtsiang.top/gtlucqrrcp.html

[D03] 在指定位置插入元素
来源：http://hz.jqgufenzy.top/gtqkippewy.html

Py:   arr.insert(0, 0)
来源：http://hz.yvedp.cn/gtgfwbufca.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jianghu66.top/gtislvbxbp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.gogol.net.cn/gttltitllg.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yanxiufei.cn/gtjjcgermn.html

Java: list.add(0, 0);
来源：http://hz.vqdsnc.cn/gtpmrxfyek.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cucudq.cn/gtvqqskfeu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tian-w.cn/gtmxquwjbu.html

C#:   list.Insert(0, 0);
来源：http://hz.cheryme.top/gtmoghaagr.html

[D04] 删除元素
来源：http://hz.c1oappe.top/gthcsvhnij.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ybcxt.top/gtbxosnish.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.redwolf501.top/gtcrffiuyg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ivvv.top/gtwjjstwwn.html

TS:   arr.splice(0, 1);
来源：http://hz.ehwqpu.com/gticlqkwlz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.iojbl.cn/gtmedrdacg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.bjfxy.top/gtndtrmmqh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cheryme.top/gtruvqwjzj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zdqjudy.top/gtwbqgoynm.html

[D05] 访问与修改元素
来源：http://hz.zhaomingkeji.xyz/gtpremfage.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtraqtmfzn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gotoacloud.top/gteztyvujp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.pycfn.com/gtvovyfgxe.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.kuanghao11.cn/gthewfkjfw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jyoumei.cn/gtwznxphly.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shangyingyoupin.top/gtkkmbzunb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtbppvxpnh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj202588.top/gtdpppykgs.html

[D06] 数组长度
来源：http://hz.zhengqikj.top/gtfhuzopxg.html

Py:   len(arr)
来源：http://hz.ydjk.org.cn/gtbctukubl.html

PHP:  count($arr);
来源：http://hz.xinyue.icu/gtouipmybh.html

JS:   arr.length
来源：http://hz.birdmap.top/gtdwcpamjt.html

TS:   arr.length
来源：http://hz.jqgufenzy.top/gtqjowsibx.html

Java: list.size();
来源：http://hz.nwbrower.top/gteudfxjrw.html

Go:   len(arr)
来源：http://hz.cqqwz.cn/gtjelqkynv.html

Ruby: arr.length; arr.size
来源：http://hz.fengsongda.top/gtlcumyewr.html

C#:   list.Count;
来源：http://hz.zhaomingkeji.xyz/gtlbiunffz.html

[D07] 切片 / 取子数组
来源：http://hz.52xcode.cn/gtxmchenyo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yueranfly.top/gtptndsums.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhixingplan.top/gtytikauga.html

JS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtbcekyjca.html

TS:   arr.slice(1, 4);
来源：http://hz.jinqigufen.top/gtyhevfwqv.html

Java: list.subList(1, 4);
来源：http://hz.meibo888.top/gtttnsrptj.html

Go:   arr[1:4]
来源：http://hz.chenjidiqi.icu/gtpgptkkev.html

Ruby: arr[1, 3]
来源：http://hz.birdmap.top/gtkjomwpiu.html

C#:   list.GetRange(1, 3);
来源：http://hz.shuidangran.top/gtcptfpocj.html

[D08] 合并两个数组
来源：http://hz.yj20258.top/gtyhubvxlt.html

Py:   a + b;  a.extend(b)
来源：http://hz.quarkkingdee.top/gtafglhkty.html

PHP:  array_merge($a, $b);
来源：http://hz.pycfn.com/gtuabmbhfy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jqgfzy.top/gtbcdiqgns.html

TS:   [...a, ...b];
来源：http://hz.sxryk.cn/gtwghymzzx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.fzhhl.top/gthefawhgm.html

Go:   append(a, b...)
来源：http://hz.mhx1999.top/gtqcviecjc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hnxiangtu.top/gtxmdqoirz.html

C#:   a.Concat(b).ToList()
来源：http://hz.jianghu66.top/gtoyxoaxtv.html

[D09] 排序（升序）
来源：http://hz.zdqjudy.top/gtvpigdnrc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxinkj.top/gthadhimlc.html

PHP:  sort($arr);
来源：http://hz.c1oappe.top/gtcflapwoa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xuanzx.com/gtwmhdeksg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ppjwa.cn/gtchajdiqy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.316326.xyz/gtsmxsnhzc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daria6918.cn/gtibatgcxq.html

Ruby: arr.sort
来源：http://hz.zdqjudy.top/gtexlgicaa.html

C#:   list.Sort();
来源：http://hz.shzxlz.cn/gtzmpsowpp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xuanzx.com/gtrtbovupf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.redwolf501.top/gtfykozwnv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.haohaochexian.top/gtkqzricsm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gtlkgylopy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtkdaxumcx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.wangdashe.top/gtpztophvu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cqqwz.cn/gtbsjjaoux.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ivvv.top/gtngzensir.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.redwolf501.top/gtzlghtcrr.html

[D11] 反转数组
来源：http://hz.jlsjyb.cn/gtxgaakdta.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ydjk.org.cn/gtfxjlyjhq.html

PHP:  array_reverse($arr);
来源：http://hz.chenlongwang.top/gtobbmkndk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jlsjyb.cn/gthitmvbbi.html

TS:   [...arr].reverse();
来源：http://hz.yj20258888.top/gtzlypioou.html

Java: Collections.reverse(list);
来源：http://hz.wangshuangyany.cn/gtzgwkbmjr.html

Go:   slices.Reverse(arr)
来源：http://hz.cucudq.cn/gtiuecawat.html

Ruby: arr.reverse
来源：http://hz.jianghu66.top/gtieyofxxw.html

C#:   list.Reverse();
来源：http://hz.jianghu66.top/gtmprctqox.html

[D12] 查找元素下标
来源：http://hz.feifeiyinyue.top/gtgjrqdjpm.html

Py:   arr.index(x);  x in arr
来源：http://hz.pengpengdd.cyou/gtlzglwuvf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yj202588.top/gtfimpuyrr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cdnleiting.top/gtykqntdiv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtnovvbjzy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gaohongyu789.top/gtzzwdbwqw.html

Go:   slices.Index(arr, x)
来源：http://hz.cqqwz.cn/gtovgzljxj.html

Ruby: arr.index(x)
来源：http://hz.xuanzx.com/gtjjwdpmca.html

C#:   list.IndexOf(x);
来源：http://hz.jinqigufen.top/gtqstndcxx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tanke756.top/gtcxrqqmbt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.c1oappe.top/gtorzvgqmb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.aizwys.cn/gtdtppnysi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gtezrbtats.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nanxinkj.top/gtnnsjhhhy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hongshengwenyu.top/gtugzvsjpe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cdnleiting.top/gtagrauaso.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nwbrower.top/gtopowcmja.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.316326.xyz/gtnheoixto.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jqgfzy.top/gtqoejujuy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gtmgxcghdu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yueranfly.top/gtvpfquehg.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhengqikj.top/gtskledpqy.html

TS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtpkexslui.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zdqjudy.top/gtlaiadhis.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtlrjnzpvu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.9152youxi.cn/gtivbhktae.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yonumen.top/gtoligrlcc.html

[D15] 去重
来源：http://hz.yanxiufei.cn/gtbygpdlby.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hysaishi.cn/gtytecyvau.html

PHP:  array_unique($arr);
来源：http://hz.cashguo.top/gtjpcrwrnb.html

JS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gtxsyppulb.html

TS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gtjxfereap.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sweek.top/gttacyoxzf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cashguo.top/gtxwqpiswk.html

Ruby: arr.uniq
来源：http://hz.dianchejie.cn/gtkiysutxi.html

C#:   list.Distinct().ToList()
来源：http://hz.ywan-chungtsiang.top/gtsbfmfbir.html

[D16] 求和与平均值
来源：http://hz.hnqzz.top/gtzjxjuthb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jianghu66.top/gtuskiaokj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.aibaodan.cn/gtdlwcmfsp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gtdxolkemy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.snrcjt.cn/gttljcydlv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sxryk.cn/gtnstolwxw.html

Go:   // 手写循环累加
来源：http://hz.316326.xyz/gtlgzloyrf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daxiang520.top/gtebdgjobj.html

C#:   list.Sum();  list.Average()
来源：http://hz.andypj.xyz/gtfprgbvbm.html

[D17] 最大值与最小值
来源：http://hz.zycfv.cn/gtpcqyvvwn.html

Py:   max(arr);  min(arr)
来源：http://hz.hywenlv.cn/gtccpxzifd.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhengqikj.top/gtqmvjjlib.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinyuanbaomall.cn/gtfhvlpauk.html

TS:   Math.max(...arr);
来源：http://hz.cashguo.top/gtdkaglimq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.fzhhl.top/gtbqhzhnpm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yvedp.cn/gtvdsxiarh.html

Ruby: arr.max;  arr.min
来源：http://hz.xingfuxueyuan.xyz/gtqaeaqmof.html

C#:   list.Max();  list.Min()
来源：http://hz.zhengqikj.top/gtmcoaujgb.html

[D18] 扁平化嵌套数组
来源：http://hz.sweek.top/gtzteborzm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shuidangran.top/gtjvzahoug.html

PHP:  array_merge(...$nested);
来源：http://hz.yuanzhike.top/gtggajsllv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.9152youxi.cn/gternifikw.html

TS:   nested.flat();
来源：http://hz.chenjidiqi.icu/gtkvicnwlg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj20258.top/gtnxzayzeb.html

Go:   // 手写双层循环
来源：http://hz.c1oappe.top/gtrtzinswu.html

Ruby: nested.flatten
来源：http://hz.dashuyun.cn/gtalgzlvxk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hfpthk.cn/gtporfcemn.html

[D19] 按字段分组
来源：http://hz.zdqjudy.top/gtqrulbhnx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinyuanbaomall.cn/gtxlllqvnv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gtqsbrrnuv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daxiang520.top/gtndulbbyn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhengqikj.top/gtwdgpndzk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.svipenyu.cn/gtlaoocadm.html

Go:   // 手写 map[string][]T
来源：http://hz.xuetiantiany.cn/gtcghhvwuz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.wangshuangyany.cn/gtfhatqkyz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhiwuduotai.top/gtmmgmakhc.html

[D20] 统计每个元素出现次数
来源：http://hz.yuxming.cn/gtaqfckbqo.html

Py:   Counter(arr)
来源：http://hz.c1oappe.top/gtwaqheyye.html

PHP:  array_count_values($arr);
来源：http://hz.sufxvd.cn/gtdhixykhk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtaxkwlcwc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.bjfxy.top/gtdcgibuco.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuxming.cn/gtyudrinmy.html

Go:   // 手写 map[T]int
来源：http://hz.smart0.xyz/gtzdshycvp.html

Ruby: arr.tally
来源：http://hz.aibaodan.cn/gtzapgxogg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fzhhl.top/gtwdhcxwhy.html

[D21] 判断是否包含某元素
来源：http://hz.dashuyun.cn/gtrzdrinhz.html

Py:   x in arr
来源：http://hz.jinyuanbaomall.cn/gtpfpqewmh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gaohongyu789.top/gtsnwwmcsy.html

JS:   arr.includes(x)
来源：http://hz.jqgufenzy.top/gtkipmcvzk.html

TS:   arr.includes(x)
来源：http://hz.gogol.net.cn/gtloarsjzc.html

Java: list.contains(x)
来源：http://hz.mhx1999.top/gtsxdcmuzk.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxinkj.top/gtkdcwzmvo.html

Ruby: arr.include?(x)
来源：http://hz.svipenyu.cn/gtimmtwyxt.html

C#:   list.Contains(x)
来源：http://hz.yueranfly.top/gtvnmlhwqe.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhaomingkeji.xyz/gtostevjmk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhiwuduotai.top/gtxoqjcqea.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.andypj.xyz/gtgonhbrod.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.andypj.xyz/gttquiwevl.html

TS:   [...arr];
来源：http://hz.ydzc1.top/gtkwhrtygu.html

Java: new ArrayList<>(list);
来源：http://hz.daxiang520.top/gtnvndauzp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gotoacloud.top/gtutndlbma.html

Ruby: arr.dup;  arr.clone
来源：http://hz.9152youxi.cn/gtzwxlsfuz.html

C#:   new List<int>(list);
来源：http://hz.wangshuangyany.cn/gtyckneqgl.html

[D23] reduce 累积计算
来源：http://hz.hnxiangtu.top/gtiqsysivr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.guannengcc.top/gtfypjxpcc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hysaishi.cn/gtnxxitumd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dashuyun.cn/gtblvkenee.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gthqtzyfcp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jlsjyb.cn/gtoksqnipx.html

Go:   // 手写循环
来源：http://hz.nanxuanxn.top/gthfwmbwsh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sweek.top/gtudeqexhu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj202588.top/gtlvdjdnsg.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhongyouzk.top/gtekhpgyba.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gotoacloud.top/gtlmcfwllh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shzxlz.cn/gtopvdeemq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cqqwz.cn/gtwsjvcjwj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cucudq.cn/gtfkvmfsrh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hongshengwenyu.top/gttcebuauu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.smart0.xyz/gtmqjwckgd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.fzhhl.top/gtlmpvchaw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgfzy.top/gtdzbochii.html

[D25] Set 集合去重与交并差
来源：http://hz.sufxvd.cn/gtxvthyivq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sufxvd.cn/gtgfxpfolp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnqzz.top/gtuqdrwfzx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hongshengwenyu.top/gtbyqcoboe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.wangdashe.top/gtlqbppubv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shanyushiyangkeji.top/gttgjzcszy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ehwqpu.com/gtlkvhiczi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.guowangkeji.top/gtoqgjbkxz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhengqikj.top/gtffgtkvfw.html

[D26] 数组转字符串
来源：http://hz.zhengqikj.top/gtrynnhchu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jianghu66.top/gttglasphu.html

PHP:  implode(", ", $arr);
来源：http://hz.feifeiyinyue.top/gtdlnpdcsh.html

JS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gttxsveaaf.html

TS:   arr.join(", ")
来源：http://hz.xinyue.icu/gtungidwdi.html

Java: String.join(", ", list)
来源：http://hz.aibaodan.cn/gtkkbcsyqc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhoulong.xyz/gtasnugqih.html

Ruby: arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtgdkbqqtl.html

C#:   string.Join(", ", list)
来源：http://hz.wangdashe.top/gtfmwktfsk.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtpkzhnlpu.html

E. 字符串处理
来源：http://hz.smart0.xyz/gtzzqxwmeg.html

================================================================================
来源：http://hz.gogol.net.cn/gticquwmoh.html

[E01] 拼接字符串
来源：http://hz.xinyue.icu/gtihsjfyiz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.guannengcc.top/gtaixcgmaf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shangyingyoupin.top/gteioqrmfm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtrarrktpr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinyuanbaomall.cn/gtngwfebzn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.guannengcc.top/gtokhgscbm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.mhx1999.top/gtkmujochw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.redwolf501.top/gtrjuqcnai.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.meibo888.top/gtkwkfmcyt.html

[E02] 重复字符串
来源：http://hz.tian-w.cn/gtuxawgelj.html

Py:   "ab" * 3
来源：http://hz.bjfxy.top/gtxfbtxxiy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.nanxinkj.top/gtsrsnfsjm.html

JS:   "ab".repeat(3)
来源：http://hz.ybcxt.top/gtgqlwzcwz.html


<!-- 参考信息 -->