代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/ggthhygwy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gwxgajtwg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gumzcqqeg.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/grwpycllf.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gynidkqln.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gwfsgnkjy.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gpfcntqxj.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gubtczivb.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gkjugsikf.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmwzrrgjz.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gzlowxpoq.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/glnaqnfcd.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/glufrsjyr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gtnhylqtq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gsbqolvsc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gpwuilavv.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gflhsaxnp.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gdpjpmjxe.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/ghfpteuje.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gnydhyivq.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gmejidhbf.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gwcyndnkc.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gtbgxkbdc.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gcfrkfrsp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gotixvrty.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gguvfmrso.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gbxpwexxu.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/grhuwohim.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gmsuvvwpl.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gyjpesirf.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gpglamyok.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/guohnvaxg.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghgqjnmvs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gjjfxhywz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/godtceudr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gnqidezlg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gmayububt.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gusmlzxvv.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gjkefpuzk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gywsveqiq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gdggwnfqb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gxsaserki.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gmesjhmoo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gwteftwmk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gfszpjulr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gbwflofpv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/ggdcyxykt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/ghavzaauq.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/ginjgbzne.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gtllaadfs.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gibksdufi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gdhfscldr.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/grbfdyghf.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gqjpqrbcz.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gnedanlou.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gdsrxlcin.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gvjmigkvx.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gakvrqxnj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/glneuzdns.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gkpsecuhc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gzaocjfeg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gtgukfoyy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gqbtemyid.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gnljtazaz.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gqxuvftem.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gywfvrprf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gnqeltowg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gpljrojjb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gdbzjnkhv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/govzblvnz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gvrnlsmdx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gzivnhcac.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/giogdwnlm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gwbjfihes.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gpeulegfx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gazdhuncg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gmxejodgx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/ggtngvoey.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gjevcpyge.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gjordfexd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gzweejiqa.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gdkrxiwta.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gomnbchbe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gzufrezrc.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gcfuekmmb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gurhwosuv.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/glsbwuwkh.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gimetfklx.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gtwfwrkcx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gdqrpcudi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gtsvibbtc.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gfvsmvlxa.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/godwmhqqw.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gdszivvtf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gfntpbifz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gbwzqrsxm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gsvuvidip.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gzxkcawoe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gjgvhayhr.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gblsonwza.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gikntrgkp.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gxcsgraph.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gmjadtivf.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvfjcbvjf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/giyfklnum.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gaqgoxigu.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmlmmhvcb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/geuebeaub.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gupmuoagt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gkafkbkas.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gufrbckya.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gxgilffvo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gttygtbxk.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gmqvnrwfp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/glegpjhim.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/ghjwyvedm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gfrspjdav.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gpyopspqc.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gmiqycojw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gwxgognmh.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gqpwflerw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gtasxlogq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gamtlkpex.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gwrwsnxuj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gtpimkqmg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gxehkelga.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gplrkiibz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gxofckocc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gjtosrcqp.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/grzmkloef.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbdjwfqxi.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gotfsmcqe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gjqqgmjnz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gigydpasf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gqdfzkpor.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gwcvdygvy.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gkxqtklcg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/grrhmtcli.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/ggjvzntwo.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gmzqjzrpu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/ggrpmvwjv.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gpimrjzjd.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gsrtvrczb.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/geojounbt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gmboinwbf.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/glufkdeoy.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ggpwnbsta.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gfbvwrane.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gyfvjdshy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gemkunbmv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gqnacrlde.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gkuvfxstg.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gpbmlaewu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gklssoams.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gquhipozx.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/glhljljdd.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/ghoszkxdk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gkukvvbls.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gnddgtchb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gnaatrxsl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gzbqxoubv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/golnosouw.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gzqsdrhgw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gumcizadn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gqvgvqrqh.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gbnipcxrs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gcoihbzvn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gobecowlq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gwyladuqg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gpjiidoxi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gffgtznhk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gkfdtgywu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gxflsbkch.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gzuoxvdlq.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/gtiqhvpmc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gzkzaafra.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/ghxxaitqy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/ggiyqxbnl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gcwjmjgcx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gdavrgimm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/ghrazuahj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gsrgaqtyn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gawwahzfn.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gtwesgqxj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gnnwfwqcv.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gtzritkyx.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gmapdgkrh.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/grnmjhcvw.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/ggfipcihb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gyptcjfba.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gskpioqhe.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gppxkdtgi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcaajberq.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gfbtooqhb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gppekhinr.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gwgbhysws.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gpbdwekqn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gphokkzke.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gfdcryppy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gxvuydgvd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gnnfhllbu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gfmhjkrip.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gvepjixze.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gzntknyfb.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/guosxsqfm.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gsohegopj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gcsngyoye.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gwfmrvppc.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gmvvwshgv.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/giimtuqlb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/goulowqex.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gqvbuwnqz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gsypphrum.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/ghordkrht.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gobhrnxgi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gstiuoiui.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gvcunaytk.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gvionzflt.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gmnwjulod.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gykrjlauc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gczcefwrv.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gobatleqg.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/ghydhsdiw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gkcsqgkcq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gheblofgs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/grcdsgvkg.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gjwlgbkwx.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/ghwpofqbw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlmytfgc.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gfzazdwow.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gixwukset.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gjlsverri.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gpnfxkfuj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gkjgoptka.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gvbsnjnaw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/grvhpaspr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gggbncfdm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gxdnbmcte.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gwconeiwr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gycittxfc.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gopuowpme.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gfuacjvnz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/grotlffeu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdklnikyh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gbtrunpxa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmpbskwis.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gocvplxvd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/goxotitsz.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/grbhlbctr.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gfxbfzwdn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gpdgxwgrl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcbduuoel.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/giapyeimi.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gtmwwkwgb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gdjaqnfvs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gdqmraoqs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gcandmpyu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gswmumvvs.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/grjycnmcu.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gjzaqbqlr.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gufldtnes.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gnetcbhuz.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gxhjqvgmd.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/grztxyqpd.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gewpamujd.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/guhngilbr.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/geupjrpyf.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gnezwzylw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gxyorakae.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gljcgkfqc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gbkrehbya.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gsflizovt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gizsawevh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gaiyfmdpg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gpfmgozyn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/grpqsishm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gtagimctt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gzihmkddl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gbjfyansq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gpargjgdz.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/glkyyaogc.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gfsqogmwl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gxdaaeupg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gbvbuzvpd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gmuidtsfh.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gwcffqchr.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gpztvfpnt.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gkvljeazx.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gcztspxum.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gbypojcxx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gdnmhjcet.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gcpucixaq.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gmbwxsaah.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/genmlhrme.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gkzivjege.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gwxpafvmd.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gyojktlyn.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gfnjppehc.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/grjrdkozv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/guvtqdbbl.sHtML


<!-- 参考信息 -->