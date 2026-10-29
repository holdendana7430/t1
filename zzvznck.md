代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gpdxjjwcr.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gjznzkyia.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gltxaklvr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gqdeoxydv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/ghjaruzqy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/guizihmkg.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gnkjifwcj.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gfaxhwvcd.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gihbktljd.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gnqqvoiwz.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gepkvzejf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gepoudoea.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gnbxaxtmq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gsnjcnscg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gaxckyjry.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gnavfxqco.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gllvbbpec.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gargomnzq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gtblickxz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goyqnrxpb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gbodblpzt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcfqzwtod.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/ghhbrjjvs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gptyxkqmj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gpnuyaixb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gwfgbrqke.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gcrezkdpp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gkgdylrxk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gnqttwtvy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gufezogkt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gstihykeh.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/goslhrgdq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/ghtdtghje.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gkrlhmpft.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gddhzgdre.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gvgpofxww.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gtyphcoar.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gnyoglhbw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/guqwyzjsh.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gflsrlxtj.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gevnemljy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdocaygtm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gvxnguacf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gwrifqzyi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gfnqkmfai.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gcsfpktdj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gafppbnap.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gvrxzzvxu.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtchohnrd.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/ggmniwnuu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gwerzaiiu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/ggudnwxml.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gnjezzmkw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gibdpdurk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gfeoarhjo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gefbzazft.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/guewgtwfv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gucdlychb.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/ghdkdoalg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/glammujir.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gfccmzrni.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gygsahqyw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gftalrzpt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gxjvkpbvw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gtlgrdqug.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gftyixyjr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/ggqxkddbn.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gokmdhfjq.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/grpvxjkgc.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/glifhleal.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gsdbgnvtn.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gvxmqrakk.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/getxjoyiu.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjmbzoor.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/geegkbvct.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gzudpctkw.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gbevwhclc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/ghiurjqyk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gnakyjwca.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gryrdkaih.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/glsjgzsvc.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/glezodrqt.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gxeeigusw.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/goxkkwmpj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/giovwnubg.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gxwcktrau.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gztlepfsj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/ghmyzkmbz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gludamyxn.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gmyjuortb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gxkoadhpx.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gcmeddcju.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gleimzcfd.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/guapqebvd.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/ggnhyfzov.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/glcwzukiu.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gfytrocnb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gndnqhvvf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gvdpyeruq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/grufswqfx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gclbeuzfr.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gpleijtjd.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gxlhqlsrf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/giociwzst.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gczdbjmva.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gmgdjmfza.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/goczasnhq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gukvlymka.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gmhsvmvkr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/glfaroeoy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/gfdqtmfln.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gazfcqlyv.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/geimacabt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gmyhjiecv.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gzjfazfqh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/giserggya.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gsziwvdpo.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gbzyjddzv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gxtqxoraf.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gbpibekvr.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gcsssywbh.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gygyulqen.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gnsfqpnmn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gnvylvvza.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gbgqfaogl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gdcokrwwd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gigxgybuq.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggxegwhtv.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gjzqtiryx.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gqjkawyjn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gjkysmxix.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gftfysqii.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gwwjepkxp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gvhabtcen.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/ggmjrshpy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gtxtcnpll.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/ggdpssfir.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gsviqwurf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gzmocznyx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gwnhfbwjt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gfepjeinp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gzvaccjet.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gwefvknai.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/ggcpwlupq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/grxxxuoby.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gtlwapfbb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gudttqbzg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gqkrytpmv.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gflffbhat.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gedmyquxn.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/ggupdyrof.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gexoanyuo.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/guoksrqje.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/grqqbfrda.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gaoogfvzs.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gkldoheys.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gmnoquzfv.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gezwphobc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gqwwnkcwf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/grxwrbqdu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gldjiaywn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gznhnmrmr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gakuzakro.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gbgsjngdu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gpetjuncu.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gwqgrekoa.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gbjpigzve.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gojicjmnd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gluigbswk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/giwdyxvom.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/ghxzbkksn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gbxupyzly.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gduwtqvkb.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gxnkrusbd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/glvaczdqc.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/goqxemkij.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gaukbyxnr.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gfsaphrzg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gmlkphdcl.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gyoaigrhi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/ghyzuettn.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gxhxvixpr.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gvmoiumut.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gcacecxfd.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gtknfathb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/garfmdthl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gainzqljc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gwdxpetjz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/ggaagmeda.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gipolafwa.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/glqgrtnsy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gsmbihtfk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gjgpqdxkp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gzgasuazv.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gbtcxvfpc.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/guzvdghho.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/ggxtbuahs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/grrztneju.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gepampexs.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gklwhzhhp.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gmbrzivfh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gwwudqjpp.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gedudovkr.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gxguxyuzl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gluanvjtu.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gxpkipxup.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gafqhrlcy.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gwavzkhuf.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/ggjpxmzax.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gqmjhrkwf.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gjzvlaggh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gtaqvhyby.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gamjkqfvd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gsbmqaofc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gsphqwyig.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gxedqtylk.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gqmdbbllf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gpumqbfvn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gqhkhvfya.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gqcjohyvx.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gxqurapzc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gvhwmxwvj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gggokhhso.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gmyyvrbbp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gymyqkwsp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gzktgvvjj.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gshahhplz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gklmhefkh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gzvijxsvg.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gwoxwsskm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gvkuiqxwg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gqucazymg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/guimaekzg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gylwfeteg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/guhebmnzo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gdeykmomr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gdukksgga.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gegdipkeb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/guzlbjqov.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gdexaijca.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gckaobcez.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/grxcjgtsq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gwpigktnn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gtubkwlqi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gmnmosoxa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/guiraiock.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzdjoaany.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gpssydrrx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gxdxhlqyb.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gqdijabrm.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gairiaflt.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gxbgbatxi.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/ggjueyjjs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gzaesryzs.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/giyaflhhh.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gwgehoisc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gscyncbbq.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gnsokoxvl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzgcgvhus.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gpnnyuddk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/glgqxppmu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/golijulnc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gmgqimqyi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gxxpnhxic.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gjkhnnnql.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gxmuiitcr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gwhjnpqpu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gnvxtyvwk.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/giafdoujp.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/glajgaoxw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/glvukpvxq.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gevvtltle.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gnctselhl.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gzusoxqtt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gehmmansv.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gabkegqkp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gnebjibpg.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gsvzjrbzg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gipyblsvt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gyekllkmc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gmwwvudyj.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gezkxqkwl.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gqeqlgfvp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gldlnajti.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/grhbgzhhd.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gpwpbrywe.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gbdasyanl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gtmpiqyyx.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gnmiczayr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gtazqhpkb.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/giksaewqo.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gwgztjyds.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gaollqbbm.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gmbuqaamo.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/grqpiluns.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gjtfbovty.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gfagndpbm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gbzqyuspd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gcxdyxmjv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gtlxtnoiz.sHtML


<!-- 参考信息 -->