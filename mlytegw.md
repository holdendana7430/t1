代发 wailian999

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gxqbcfydv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdzmzqzvz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/giiefnvjc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gwhvdwcar.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gcbwzwcjr.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gmjqvxnth.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gjwtheiwe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/giufthpmy.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gamduftza.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/grvmusbjo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gvijwtujb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gxppocdxe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gvtgzkaix.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gnhmwikpb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/grqdcvmvv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/givauugvi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gfnwoubbm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gievfsgqe.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gwykstzjm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gvqchfuaj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gfqxzvcgf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gsgjjxiqk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/guilvcgqx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gajnjevtr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gvzjxwect.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gbnfaxkaw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gbbsxgytw.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gaiiqqqtg.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmyesuaik.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gwajtmhuj.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gamzpizds.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gcwtztgvl.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gaooyksqa.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gbriqxahm.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gjydzaajn.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gpstnvpoh.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gyjsokefj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gfyrgqpqm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/ghovnswoz.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gzvixqwli.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gfltwqqjd.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gmhdgnxah.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gdaaercnt.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gkveksnjw.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gxrzyqsoa.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/grxceyuoo.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gnuskyyzo.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gcyxdzisu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gateirqlf.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/guylukxde.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gbcaoohwy.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/ggvdaekwu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gjopkuxqv.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gqciqqflc.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gmjuxktvg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gjzbblrqi.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/grqcaqhli.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gizjvnpyw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/ggxvcxsnh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gwlazravg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gurzelofe.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gemjfjcjf.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gmvwrhqmh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gpebwfdlg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gnnsphduu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gtubvofku.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gxtuwxncz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gpomlexqa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gtoutlpad.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gtpzseqhl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/guuvjgwlk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gbldwekpn.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gnmcohroj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gkmaqtyvp.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gregjlzqz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gqeeyyulw.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gfjmoucqi.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gwdlnnhcn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gtjripmms.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gomemqlvq.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gfxorxpes.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gidyzgpay.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gupesmvor.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/ganldashm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gezqamxai.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gsezjgvpc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gyaiawapk.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gbzqcbxqr.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gztzynong.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gvdgimhmy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gjgbqwopk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gwxqagxwg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gnwmlqitk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gcuxmmpph.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gkqqrhoos.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gkbmcrlgq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gctxdwcup.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gkrjrslgo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/giebskudz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gxtivlaso.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gkxzjewby.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gibemxxge.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gcdjnisqw.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gtfddifek.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/glskbidmm.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gagqlepqe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gjuvnbiqn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/grtraeyfy.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/ghxfpjzdk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gbwetmqia.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gawmjynqi.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gtmbdtrot.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gcyaavohw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/ggcplevww.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/grrdxlwyh.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gsynunjyc.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gzfxqxgcn.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/grvxqcpzj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gycjssvjj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gaddxxgwx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gtwggoubi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gnybpdkhk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/govelwalp.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gxzmbtozx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gbyykappm.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gijwenkne.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gbzxxgurj.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxfbmdzod.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gmlrkrrtd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gwlysgmio.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gppeyrswn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/genqkbcnb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gprmvghgd.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gejyhssvu.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gokxieovq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gyzbzthgh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gczmwawcf.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gcayxnwwm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/ghuuzvuav.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/glauqljhh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gavpaimai.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gkvthyogu.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gypavthwq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gylbdalwh.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gkzuxsejp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gfwltmxeg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gnyzlpivo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gksivcqrr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gltlnxrit.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gfupsrujf.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gbzozawul.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gykwkjabs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gzredkvpn.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gsgscdimp.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gjkkmdggz.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gupfmngyu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/ggmnkdkzp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/grntksdac.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gtvaoukya.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gdrvubjbb.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gdqyeyvlu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gxafndwym.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gvdudjueo.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gpmxawnym.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gozncytua.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gilwtlwyy.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkpkyenq.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/ggmxhkkvd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gsmqtqlpd.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gvvethnic.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gzrrzdops.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/guyqhnerf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gqchaerlh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gzpzlejvo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gqmdeuwtq.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gclekzfvl.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/ggsvusaru.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/glyygbxni.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gweqoxuka.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gjjosmqdp.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/ghmpfwhbi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/giqifjhrh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjqwmxkrg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gatmjfyag.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gprhvoewo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gxttgegfu.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gklamgwzs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gktekwzmv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gvajgnbml.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.hesvh.cn/Article/details/gsdgxelpk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/ghtlklmmi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/ggppizdqz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gkgstnsjq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gfiuuoypd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gqiqlraay.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/guvtyvuxh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gdjftpzif.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/ghxowoghp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gpamktlkl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gqbhaxxpp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/gkltzvoul.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gprbltuxi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gxpmhjtys.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/guzqomoho.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gvczuvkax.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gyiidxcgm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/goblwclhk.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gobdrrnpt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gmxshszxn.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gozqiplwe.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gjatttbtt.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gcrhpdzfk.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gsfidxdzx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gsftigfjm.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gdltlbzrw.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/goesjilvs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guertxgbf.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gphwhopqo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxklqvljt.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjkpthhgb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gezrqyhzu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gcgsdjoyg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gobjybowi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gnfmkrxof.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gipfpywpc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gldntekke.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gkbvfugoe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/ggkgleajn.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gbaowpuew.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gsslwjslw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gdfsjudad.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gppdzaiog.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ghqsxljpf.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/goygjkptv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gbvokoisc.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gceqedrii.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gtookazag.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gzwhnkxue.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/ghdiktnau.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gnprddrqd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gbdhjcnun.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gjwepufah.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxtxhjpph.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gldvvrddf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gkxnjjutz.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gxxoasmxh.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/ggfgztdgq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gpamxybup.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/ggsqmspnz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gxhrwseih.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gktfagxwi.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzkrvvyts.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gmffdvggy.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gfefobxkt.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gtfwcfkkr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/ggqwpeosz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gatyrrlnj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gxelpdwwd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gtdupzzpj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/ghixrmizx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gmyebyydu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gvvlftftq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gdpeuqadx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gdxvugqup.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/ghkwebdwe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gzxdkoaoc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gqqhiniyo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gfytapiuk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ggyrwuuai.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqdbjgsde.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gxpyfqnjn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpuhkjqqs.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gckaucbtz.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gpfnkxofv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gjnbbzbpv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gxxxfjawg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gdkfytqeh.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gwhqzktbm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gjrlqawxs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gnsvklizp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gkqjiruhd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gganjxvhn.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gpsiyslaj.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gpxesgwgn.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gqgjajgnr.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gxmaywpdh.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/guapdzepv.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gakciegoy.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/grlaiqomd.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gcjvgvjdc.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gfltqkjdh.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gwhyjobch.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gsqvbruyt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gbstyzdoq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gizetuxqb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gfqppavpg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gzbmnaoac.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gunzwyvfs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gdvljvqmu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gkqskekce.sHtML


<!-- 参考信息 -->