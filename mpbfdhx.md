代发 wailian999

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gcoswvbwy.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/goqsjfmeu.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gduwgaekt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gfbqrywub.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gamftyatn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gbshzqjsv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gicjpbfbg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gbyvnifei.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gjqdcnsyh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gwlfvrypt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gbvxhleil.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsazlbqpb.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gekzudhld.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyhrwmuoo.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gtioaqdmt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/ghdrlpdbh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gpmgfuqxt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gbmihatgf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gnmcgocps.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gqctzvzgi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gyfkavkwa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gcewnbolw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gccaffbkd.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gasetnrsx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/grvxmhyik.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/geyqpbkto.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/grjyixxka.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gmlcrkybk.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gbxnhxwsn.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gcrhudutj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gqnimnirk.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gjcawkbkw.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gkiylllgf.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gwccutuuv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gkwluzmym.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gbrnvphfx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gkxpstjet.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gcslfvzuz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gpwcjbmhu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gfbdoiken.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gdujkzolf.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/ghdacvhtv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gkytadpij.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gukghqbwk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gdyrjzmjz.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gbolvguhj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gilslkwkd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gvxsysgju.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gqxxqhhmo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gakdenknl.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gszqdigml.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/ghqcvozzb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gxzlonhlq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/genzvutfl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gajorqqhy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/ghuxaqgmw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gpoynhwgv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gsjotjjqj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gwghygevj.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gbtcxicmz.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gjrhnzclh.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdbjdyudl.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gurvbriwk.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gnvveqbmr.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gyzieaybj.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjcrithla.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gqxtnnvcs.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gjgyoioch.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/guohhnibf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/ghqfltafi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/guzgkmuki.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gbmdlrifh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gumwsyerz.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gbmkmdzxc.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/ginwzssqx.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gskwrpkzl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gcrnnbzjp.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gqhzovgec.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gwuypgtjj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/ggtuqqxku.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gzatmcnyp.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gxkiykwjn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gixkdstnz.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/geanruskt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gvqywnlmh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gwmnmqehv.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gpyquwbul.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gvwjddvfw.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/grjzjjpix.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/grakzkpbz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/ggzrvhyem.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.zdbjq.cn/Article/details/gblcspidi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gmupwbjov.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gpeazizwv.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gactdomxg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/grnmoowzm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gudsmshah.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gjzjhmcdx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gpprumpkx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gxtceuooo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gycemrfkl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/govqseyji.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/glydrbpem.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gfjhcpwjl.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gkzcsuntq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gabrztmea.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gpolvfbnm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gbeeaoeuf.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gbqbfkwgy.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gtzoebpdm.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gzlqmkxbl.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gwcainmah.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gnqhykufk.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/geiqetcxv.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/ggufdfzec.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gojhiovzf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfqbrgww.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gtnlereoe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gcqmpplek.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gbziqximn.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxnxtlqjy.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gqnalsmst.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gpwioaxjy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/goadmjudq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gzyucphgl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gzqydeidu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gyozivapd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gjhuzgavv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/ghjzlnkgo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/giwufqkqd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gewolqore.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gmgzcpwvu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gzjhmpjuq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gsqnwsoql.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gxgaejgus.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gafjmljeh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gqnjegrzs.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gwfrmdwpx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/ghcmtqaxb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gemxwazcl.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gnssyuyun.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gwaawzywa.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/grnqgpvtv.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gtitilekv.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gmmshffpp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gcpcxywzm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/giiujnfeq.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gsmyzqqyi.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gcxouwuqv.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gvcipywvh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gobeqtdft.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gozpzamrx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gwhdghbsa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/grzkvlrmo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gxvebxxuy.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gqqpbiqay.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gudusksin.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gsbsunbvy.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/girdxftss.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gehvchiqe.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggeewlcaq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/griqegmyv.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gkwstgwkz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/grucpdpvp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwaylnfyc.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gaslgeesk.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gjmtasscy.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gwdkqlpfi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gdknoaurj.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gtgpsygja.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gegpcdxby.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gunkhbzrd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnlinpiow.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/grjbzyfty.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gwuhjakhp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gbnppbcjg.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/ggznmberb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gijsuhrvm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gdsvifnaw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gsceqxufd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gwhnfgwvh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gfhklvpad.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gbynvqqxr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gldzvjnai.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/goouthjnf.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gxxfqrzfy.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gunyyuudm.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/ggtclgrhq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gcpslcufy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gwdwljafq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gntretjwh.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gygfxqufi.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gnziwemce.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gdhsfqvja.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gpqbctqwf.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gggtuspog.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/geqhuwvkx.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gdrgqzmhk.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gfdapmtrc.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/ghflxdvox.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gsthmukxc.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gocsflejj.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsgpajgux.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gpnxilyrp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gitevulee.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gzmyrpyzm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gfwpnqwui.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gashwnpnp.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gtgcpevra.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gmjadimii.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gqwwidspt.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gfqjwlmer.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gbwiabwld.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gpnwdekqm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmhfsgmjo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/ggvrllobt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gizqhmbte.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gvzipsbrb.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gohzprgax.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gflmsmwvu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/ghispknhv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gzpjfvibd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gukhudipm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gldgvyfok.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gxucgxfgq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gjclsldfn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gfebnaakw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/geenrfffn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/getdvswdk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/gbctyqyow.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gdxcgqdka.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gzviesfge.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gwihvakzf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/guqcbstye.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/glvomwbpp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gasjzqxqi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/ghfbdzlfo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gzmvsnqzn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gqskdvtmf.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gcenqmwzt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gpxnhqxkq.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gbcteitjv.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gtrrehlzm.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gumwwilzg.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gskycumgk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/ggyeccsac.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gbpwrrsgl.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/grmyridrb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyriygabs.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/guiuuwfjj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guepietpj.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gapazyhdc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gyqglmgvx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gfgchliqb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gfyqxaget.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gquuvspwv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gumwvsdpy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/ggfztchzm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gcnkvecrt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/giymutxst.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/ghzaqftub.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/ghxftpmzn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gtpepquij.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gfjkbjeve.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/grctsrfkt.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gvysiulxk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gyuzydnfj.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/ghccgzyvz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gastjnkej.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gpmercpqr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gjvdkfuzj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gglrueful.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gesakywtw.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gsdvfjrpb.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gvzkyoxsl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gzyopjtdv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gkrjefixb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gagtjbrgr.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gdbhkrumd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gofvqgwbw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gaapslfus.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gxaarcggg.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gukbxwewa.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gplhqyage.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/glxseeyjv.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gbkbgsqig.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gmuppgiek.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gjzheicvo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gefqubrsf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gwczegnbz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gclmappgt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gnzntvfug.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gdcyohxny.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gsbqgvrvq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gpiykcpka.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gxxogitya.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gqubkxdmc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gaawmktpx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gtbnuewar.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gvivvhrmk.sHtML


<!-- 参考信息 -->