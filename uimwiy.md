代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://hz.dashuyun.cn/gtiflwvayo.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj202588.top/gtypthadil.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shangyingyoupin.top/gthamwdupe.html

[C13] 类型声明 / 类型注解
来源：http://hz.shuidangran.top/gtruinxoiq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nanxuanxn.top/gtobfpsaoj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtqnchbegm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.52xcode.cn/gtxnddxgej.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gtgnnrcann.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yongpay.top/gtfrygzvkd.html

Go:   func add(a, b int) int
来源：http://hz.zhengqikj.top/gtrbogltru.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.birdmap.top/gtypxgjsks.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zhaomingkeji.xyz/gtrifawltx.html

[C14] 泛型函数
来源：http://hz.chenzaomai.com/gtoitbijte.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gtavtjgnqp.html

PHP:  // 无泛型
来源：http://hz.ivvv.top/gtjkhvtfoy.html

JS:   // 无泛型
来源：http://hz.nanxinkj.top/gtzzkhdflo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhongyouzk.top/gtysomzodp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangshuangyany.cn/gtaxrpmuhg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hammf.cn/gtusddplyg.html

Ruby: # 无泛型
来源：http://hz.ehwqpu.com/gtktjjakwy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shangyingyoupin.top/gtnhilomoh.html

[C15] 解构 / 展开参数
来源：http://hz.zdqjudy.top/gtqhpthxwr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tian-w.cn/gtfcpqgpzb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ywan-chungtsiang.top/gtpxkekqun.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtjbilebcv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ivvv.top/gtplnubltq.html

Java: // 无解构
来源：http://hz.nanxuanxn.top/gtwxzcwapv.html

Go:   // 无解构
来源：http://hz.cdnleiting.top/gtccanzifp.html

Ruby: a, b = pair
来源：http://hz.vqdsnc.cn/gtrselfqbt.html

C#:   var (a, b) = pair;
来源：http://hz.sweek.top/gtgeuqqfoy.html

[C16] 函数 / 方法重载
来源：http://hz.gaohongyu789.top/gtrokdfbwv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.guowangkeji.top/gtlzigxrzb.html

PHP:  // 无重载
来源：http://hz.ywan-chungtsiang.top/gtamdpbpsa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shangyingyoupin.top/gtowtyrrkz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daxiang520.top/gtkflqluds.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.wangdashe.top/gtfnecwjwb.html

Go:   // 无重载：用不同函数名
来源：http://hz.xuetiantiany.cn/gtpymykpxj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinghuilouyu.cn/gtkrjoydzr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.0kj1m.cn/gtrjqmalcz.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtimzkbfyl.html

D. 数组 / 列表 / 集合
来源：http://hz.yuanzhike.top/gtfpzrqgyj.html

================================================================================
来源：http://hz.sweek.top/gtedmgilif.html

[D01] 创建数组 / 列表
来源：http://hz.yangfankeji.com/gtlvvzagzo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xinyue.icu/gteuifgonz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.smart0.xyz/gtbmdvaxyt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cucudq.cn/gtflmjgeux.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shangyingyoupin.top/gtmwnuezlb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuxming.cn/gtkffrsggm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj20258888.top/gtoiqnigjs.html

Ruby: arr = [1, 2, 3]
来源：http://hz.redwolf501.top/gtjyizcnhp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hywenlv.cn/gtokcdezhb.html

[D02] 追加元素到末尾
来源：http://hz.ywan-chungtsiang.top/gtrpjqrvqx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinqigufen.top/gtrvzgfexx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.andypj.xyz/gtetuwpcid.html

JS:   arr.push(4);
来源：http://hz.iojbl.cn/gtimsaekdl.html

TS:   arr.push(4);
来源：http://hz.yueranfly.top/gtdioosmot.html

Java: list.add(4);
来源：http://hz.ydzc1.top/gtcdzrkfos.html

Go:   arr = append(arr, 4)
来源：http://hz.yueranfly.top/gtdcvbyscd.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.birdmap.top/gthxgoleup.html

C#:   list.Add(4);
来源：http://hz.birdmap.top/gtsrqdbbih.html

[D03] 在指定位置插入元素
来源：http://hz.aizwys.cn/gtngdbpgot.html

Py:   arr.insert(0, 0)
来源：http://hz.haohaochexian.top/gtpyfkcnnr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.smart0.xyz/gtgtzbaxny.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sysykeji.top/gtzgwdpsgb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhijiandao.cn/gtrgibzmwc.html

Java: list.add(0, 0);
来源：http://hz.wangshuangyany.cn/gtvwyxdlkq.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yueranfly.top/gtxympdoja.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.haohaochexian.top/gtjifaglnj.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgfzy.top/gtlzurjuxs.html

[D04] 删除元素
来源：http://hz.hammf.cn/gtlfwairet.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.guannengcc.top/gtyvoqndon.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yongpay.top/gtfaqhuufm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zhongyouzk.top/gtcovielib.html

TS:   arr.splice(0, 1);
来源：http://hz.jianghu66.top/gtfemydpdj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hysaishi.cn/gtqzeaeoxs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.redwolf501.top/gtrljpgiwa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.ppjwa.cn/gtpqerzlej.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ehwqpu.com/gtsnytaibi.html

[D05] 访问与修改元素
来源：http://hz.cashguo.top/gtbyzccvke.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gthlexfqgm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.wangdashe.top/gtxcwqmhsp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cucudq.cn/gtsrutxpcj.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jianghu66.top/gtkeyvuuur.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.gogol.net.cn/gttfrmhhmy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtuecnpxnq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gtmjiwkvqs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ydjk.org.cn/gtlegcjoom.html

[D06] 数组长度
来源：http://hz.havefunace.top/gtowkcqegl.html

Py:   len(arr)
来源：http://hz.yuanzhike.top/gtxygdzuvo.html

PHP:  count($arr);
来源：http://hz.yueranfly.top/gtmiuossyj.html

JS:   arr.length
来源：http://hz.shangyingyoupin.top/gtgxmygahm.html

TS:   arr.length
来源：http://hz.wangshuangyany.cn/gtokwkffzn.html

Java: list.size();
来源：http://hz.redwolf501.top/gtnmavomcw.html

Go:   len(arr)
来源：http://hz.zhongyouzk.top/gtssasmcap.html

Ruby: arr.length; arr.size
来源：http://hz.smart0.xyz/gtjbomcxcd.html

C#:   list.Count;
来源：http://hz.ivvv.top/gttgyzqook.html

[D07] 切片 / 取子数组
来源：http://hz.shuidangran.top/gtnrislidn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shzxlz.cn/gtrmyiyalx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhengqikj.top/gtfqhjqtaa.html

JS:   arr.slice(1, 4);
来源：http://hz.ydzc1.top/gtsgafhasg.html

TS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtivihgjjc.html

Java: list.subList(1, 4);
来源：http://hz.jinqigufen.top/gtkvqssbzq.html

Go:   arr[1:4]
来源：http://hz.tian-w.cn/gtjprlopmf.html

Ruby: arr[1, 3]
来源：http://hz.hysaishi.cn/gtlatnluvl.html

C#:   list.GetRange(1, 3);
来源：http://hz.sweek.top/gttgdhiyzl.html

[D08] 合并两个数组
来源：http://hz.xziqi.cn/gtwedvpuep.html

Py:   a + b;  a.extend(b)
来源：http://hz.zycfv.cn/gtfzcwfzkr.html

PHP:  array_merge($a, $b);
来源：http://hz.chenzaomai.com/gtgaowvvix.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.c1oappe.top/gtqqxotaca.html

TS:   [...a, ...b];
来源：http://hz.dashuyun.cn/gturtwzvby.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydjk.org.cn/gtydklklik.html

Go:   append(a, b...)
来源：http://hz.zdqjudy.top/gtkxdoylqs.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gthzkikfui.html

C#:   a.Concat(b).ToList()
来源：http://hz.shanyushiyangkeji.top/gtpzcykcxu.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangtech.top/gtqakhrhxj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtconhzdzd.html

PHP:  sort($arr);
来源：http://hz.birdmap.top/gtbddgupqw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.mhx1999.top/gtxocglxsl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yueranfly.top/gtqkgeibxk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cashguo.top/gtcojrzynf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtfnhhbpno.html

Ruby: arr.sort
来源：http://hz.jinyuanbaomall.cn/gtcbdmjvra.html

C#:   list.Sort();
来源：http://hz.jinqigufen.top/gtinrskgcn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cqqwz.cn/gtwcsxffdj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydzc1.top/gtcgibbjup.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.aibaodan.cn/gtlhrlqvuk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tianlin.xyz/gteyhgwsxi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtotrxjgem.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.316326.xyz/gtrnlbtnlf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhaomingkeji.xyz/gtluwwvsxi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cdnleiting.top/gtggjgffza.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zdqjudy.top/gtkvotzijk.html

[D11] 反转数组
来源：http://hz.sufxvd.cn/gtebgcinfa.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sufxvd.cn/gtatfgusmr.html

PHP:  array_reverse($arr);
来源：http://hz.svipenyu.cn/gtdnffjapm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.smart0.xyz/gtsspkgwmy.html

TS:   [...arr].reverse();
来源：http://hz.hysaishi.cn/gttgqvplck.html

Java: Collections.reverse(list);
来源：http://hz.0kj1m.cn/gthxiunbrb.html

Go:   slices.Reverse(arr)
来源：http://hz.chenzaomai.com/gtxjarhquk.html

Ruby: arr.reverse
来源：http://hz.chenzaomai.com/gtmzlvddcb.html

C#:   list.Reverse();
来源：http://hz.ydjk.org.cn/gtfxwatmez.html

[D12] 查找元素下标
来源：http://hz.tianlin.xyz/gtqlscbkik.html

Py:   arr.index(x);  x in arr
来源：http://hz.jianghu66.top/gtlficcjpc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yj202588.top/gtegojwgpd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtqpdrtmlk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtpramxnhz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shuidangran.top/gthxzvqfnn.html

Go:   slices.Index(arr, x)
来源：http://hz.ivvv.top/gtwjfhcwth.html

Ruby: arr.index(x)
来源：http://hz.sufxvd.cn/gtfvmabktt.html

C#:   list.IndexOf(x);
来源：http://hz.bjfxy.top/gtzfsjvepv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ybcxt.top/gtbpvvukrg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.meibo888.top/gtwcbjgyoa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jqgufenzy.top/gtzisrzaor.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xuetiantiany.cn/gtophrkjhx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xziqi.cn/gtrlfeyprs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.feifeiyinyue.top/gtlvedibkp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinqigufen.top/gtdoffdhcs.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shzxlz.cn/gtidcqbzbj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.iojbl.cn/gtyjqkoudx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shangyingyoupin.top/gtzclakeww.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yueranfly.top/gtmyrdwyrl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yangfankeji.com/gtsmplqrrc.html

JS:   arr.map(x => x * 2)
来源：http://hz.yuanzhike.top/gtygqyqeyy.html

TS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtluficzqy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangkeji.top/gthzyfgtdh.html

Go:   // 手写循环
来源：http://hz.dashuyun.cn/gtwixhsjzi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnqzz.top/gtaxxabgyr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.fengsongda.top/gthzpdskxy.html

[D15] 去重
来源：http://hz.cucudq.cn/gtapjafjuc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.tanke756.top/gtlfbuebaq.html

PHP:  array_unique($arr);
来源：http://hz.svipenyu.cn/gtyroakfbm.html

JS:   [...new Set(arr)]
来源：http://hz.hfpthk.cn/gtxviljsdi.html

TS:   [...new Set(arr)]
来源：http://hz.chenlongwang.top/gtegusadmp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fzhhl.top/gtppbnkrxa.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shangyingyoupin.top/gthijspbip.html

Ruby: arr.uniq
来源：http://hz.shanyushiyangtech.top/gtlszmuqqo.html

C#:   list.Distinct().ToList()
来源：http://hz.yueranfly.top/gtsjwzvxfm.html

[D16] 求和与平均值
来源：http://hz.tian-w.cn/gttkkyzjha.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.smart0.xyz/gtdzxnfinw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.redwolf501.top/gtbhnvnawe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gttpoupwij.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.svipenyu.cn/gtvhvwdwrf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ywan-chungtsiang.top/gttdhwnayi.html

Go:   // 手写循环累加
来源：http://hz.jlsjyb.cn/gtemqryoln.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxuanxn.top/gtnmdxabyf.html

C#:   list.Sum();  list.Average()
来源：http://hz.sufxvd.cn/gtkjgdyvjp.html

[D17] 最大值与最小值
来源：http://hz.hammf.cn/gttpneuggr.html

Py:   max(arr);  min(arr)
来源：http://hz.yj20258888.top/gtedxamdlv.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhongyouzk.top/gtotztnaqq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cucudq.cn/gtjvvwtjxx.html

TS:   Math.max(...arr);
来源：http://hz.jinyuanbaomall.cn/gteawqafge.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nanxuanxn.top/gtlnrsaiah.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydzc1.top/gtxlwebcgk.html

Ruby: arr.max;  arr.min
来源：http://hz.fengsongda.top/gtpcmelsrn.html

C#:   list.Max();  list.Min()
来源：http://hz.hnqzz.top/gtsiuznabi.html

[D18] 扁平化嵌套数组
来源：http://hz.yvedp.cn/gtfgyrjtjf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sxryk.cn/gtftphqawc.html

PHP:  array_merge(...$nested);
来源：http://hz.xziqi.cn/gtfpqsgqfw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhixingplan.top/gtnscdcydu.html

TS:   nested.flat();
来源：http://hz.hfpthk.cn/gtjxioymnb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangshuangyany.cn/gtdcdbcebo.html

Go:   // 手写双层循环
来源：http://hz.guannengcc.top/gtdpmwhpdf.html

Ruby: nested.flatten
来源：http://hz.fzhhl.top/gtpvknsers.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.smart0.xyz/gtvmuxuohy.html

[D19] 按字段分组
来源：http://hz.pengpengdd.cyou/gtlvmgekio.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ydzc1.top/gtjjwbrbak.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gtuqxqfnef.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yongpay.top/gtgarrncjw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ivvv.top/gtojqrdpgz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ivvv.top/gtrmwcmfsh.html

Go:   // 手写 map[string][]T
来源：http://hz.shzxlz.cn/gtyhrhhcjo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yvedp.cn/gttegjiipz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xziqi.cn/gtideomhyo.html

[D20] 统计每个元素出现次数
来源：http://hz.dianchejie.cn/gtcokarzjt.html

Py:   Counter(arr)
来源：http://hz.pengpengdd.cyou/gtwgleltfz.html

PHP:  array_count_values($arr);
来源：http://hz.chenzaomai.com/gthoqjgbvq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.c1oappe.top/gtfnxnzhyf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.vqdsnc.cn/gtttpstken.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gzhubu.top/gtlmbntrtx.html

Go:   // 手写 map[T]int
来源：http://hz.haohaochexian.top/gtolsrfdry.html

Ruby: arr.tally
来源：http://hz.c1oappe.top/gtuptddlld.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinqigfzy.top/gtxbtjyakm.html

[D21] 判断是否包含某元素
来源：http://hz.xingfuxueyuan.xyz/gtyctdozxt.html

Py:   x in arr
来源：http://hz.c1oappe.top/gtdlqlqlbm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgfzy.top/gtxrbvtwyr.html

JS:   arr.includes(x)
来源：http://hz.feifeiyinyue.top/gtglteopke.html

TS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gtnhhnuucp.html

Java: list.contains(x)
来源：http://hz.zhengqikj.top/gtaxvdmrly.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxinkj.top/gtbwdsqzzg.html

Ruby: arr.include?(x)
来源：http://hz.gzhubu.top/gtoshkiflt.html

C#:   list.Contains(x)
来源：http://hz.sufxvd.cn/gtkevsxalb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gotoacloud.top/gtykvyfano.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenzaomai.com/gtnwpyqhvf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.0kj1m.cn/gtjeqbykdg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xylfe.cn/gtryqskqab.html

TS:   [...arr];
来源：http://hz.cucudq.cn/gtekadvmaw.html

Java: new ArrayList<>(list);
来源：http://hz.andypj.xyz/gtunkyiprp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nanxinkj.top/gtqztqhcls.html

Ruby: arr.dup;  arr.clone
来源：http://hz.meibo888.top/gtpuvasfrw.html

C#:   new List<int>(list);
来源：http://hz.jlsjyb.cn/gtubwneqrr.html

[D23] reduce 累积计算
来源：http://hz.zhaomingkeji.xyz/gtymmsgmiq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xinyue.icu/gtbkldaoqa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tanke756.top/gtlxnmhjfr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtcdcnipqu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtuxfwoaqp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gogol.net.cn/gtriqiauqr.html

Go:   // 手写循环
来源：http://hz.yuxming.cn/gtdhvbrhwb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gogol.net.cn/gtobxdonvx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.haohaochexian.top/gtullsuccf.html

[D24] 字典 / Map 基本操作
来源：http://hz.haohaochexian.top/gtgootfgro.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.feifeiyinyue.top/gtxmbwrwmp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangtech.top/gtjmjzkejf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daria6918.cn/gthywsubto.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.snrcjt.cn/gtiuuujvtc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gzhubu.top/gtrvwwolff.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ydzc1.top/gtoubaqnjd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yonumen.top/gtlwclwgdu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cdnleiting.top/gteeifibyd.html

[D25] Set 集合去重与交并差
来源：http://hz.tanke756.top/gtuuhbmssk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gaohongyu789.top/gtzsemjnlq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuxming.cn/gtzuepvmnr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shanyushiyangtech.top/gttogiaemq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ppjwa.cn/gtqzlyuuva.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jianghu66.top/gtchesuhfy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.9152youxi.cn/gtzyslnsew.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.vqdsnc.cn/gtnkuwyoha.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sufxvd.cn/gtjsafdsqs.html

[D26] 数组转字符串
来源：http://hz.cqqwz.cn/gtbwbjgjqj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ybcxt.top/gtrdmiaoqi.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgufenzy.top/gtohbbbxbo.html

JS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtzptlclqf.html

TS:   arr.join(", ")
来源：http://hz.sxryk.cn/gtbbxabmjm.html

Java: String.join(", ", list)
来源：http://hz.ydjk.org.cn/gtrpwqpujb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sufxvd.cn/gtspzptrlb.html

Ruby: arr.join(", ")
来源：http://hz.ybcxt.top/gtlkvumqix.html

C#:   string.Join(", ", list)
来源：http://hz.feifeiyinyue.top/gtlbkoqjbi.html

================================================================================
来源：http://hz.nwbrower.top/gtkwclkjcg.html

E. 字符串处理
来源：http://hz.jqgufenzy.top/gtcychnust.html

================================================================================
来源：http://hz.nanxinkj.top/gtgsezmdtr.html

[E01] 拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtpwocziov.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.wangdashe.top/gtdmyiygxt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yvedp.cn/gtulthutbj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtlcquxiae.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtmjnlzolh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xziqi.cn/gtyhdegjbc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.guannengcc.top/gttyrvkehs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nwbrower.top/gttslexzbv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nanxinkj.top/gthgctcyfe.html

[E02] 重复字符串
来源：http://hz.zhaomingkeji.xyz/gtajrmeonc.html

Py:   "ab" * 3
来源：http://hz.yj20258888.top/gttigufkrb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenjidiqi.icu/gtftbacwhj.html

JS:   "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtdchjunvn.html

TS:   "ab".repeat(3)
来源：http://hz.aizwys.cn/gtzrkssmyz.html

Java: "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtpbmkshnz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.iojbl.cn/gtletiqktk.html

Ruby: "ab" * 3
来源：http://hz.ivvv.top/gtjhisowhd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hnqzz.top/gtdvhqveaq.html

[E03] 截取子串
来源：http://hz.aizwys.cn/gtvslmhofv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hywenlv.cn/gtnhfbzqya.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.redwolf501.top/gttfstjwgz.html


<!-- 参考信息 -->