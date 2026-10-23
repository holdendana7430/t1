代发 wailian999

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3whzjosai.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oqnavmhr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lnrmqlaf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ailaqnmu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dxiwmqwe.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmgzbhz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wulraapt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fsedlagq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ldpnvwgi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fesgfhtz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3yvcdtmxz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3uyjuarxz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3efpirbdw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3baavlwrw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3kmykeavt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fruznuzj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3mmtkyrxg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3modrqwxd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ipogipar.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kdcbqttk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hyjybkrw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3xchmpema.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3aanxffrs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gjgsoljg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pmjdbzkw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ljeoddhn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3wmpvgjyn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3yefhfbxt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vhptukjd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hphkcyla.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qkbcoswt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3cwylbaup.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hlqjivyg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fikuubqx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xruxhmux.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pckypeld.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3fgkkmyxc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfgbakqa.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3evxoknah.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3siwgefid.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bbaymise.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3tvprmqzp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ojwiughe.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3aijunuxk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3coplywse.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xhraakis.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kditwmmd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3liqvvnwr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yyaxcmae.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nvbdhmze.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3llhbyihx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ojculgtj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3pavlujts.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ynkxrbsx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uetpsmkz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3rymdyubm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ltwjckfk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dakaflor.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zdaijdpu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gxunafqm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nwvyonei.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3radzgvkd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3lvehuyrw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3bvestjut.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wrhpdiee.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kifiaoxc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xrcxvvct.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xvcsqyop.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rrxndfhh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aevxilme.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fxnejlqy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3imtfrcrj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jahkbukn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3tzsgmhnh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rbbrdkib.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zswwjzse.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3lrwgjbkr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3njbqvxmm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ktkzytxt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3mckknezf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hzikzhwf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3bqysrrkr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gdwovgfp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3souckbir.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3pausyktd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fzdankvi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ltwefqwj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vcmfzgqs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vmewrwzy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sdunoiec.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3dafymjlr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hiuiyfsi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pnjwvghv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fwrrjyhu.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3isumxwcz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3gycbgeeg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hkudyarv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lsdcgbrz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vcdwgnno.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gjjwexoc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3wlpznkew.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qufyqzaq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3olnlrtik.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3yuafyglp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bxpxcobm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yewppmtm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vigsjakf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgufnqek.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3jpjkrfhv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lhydbiwe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cdcsbnoo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pbuqbpnw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tfwbudye.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hppxmltv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jxuvxxrb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zctdiurd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ttswbfzl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3kzfmmeet.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bvqanvzw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3diedtsdh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ngkpbghg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ridawtve.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hrxiqanr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nqcdddkq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uozffabn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hzlwkrla.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ezhkgxhd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qhdrdqhf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ncgbadfi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3nhfenvoz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gimkrial.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jubfvcar.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3wksbbviu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3blpjnddh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3gkcymcsf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3xmisofge.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gabrjrki.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mfnrqngv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3boorwvba.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3tspqjmii.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vnelevut.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pdzczgqw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3xocabzdb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3rmiagqpm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ocoqkbgb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3dyllksuf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3aqzsnhot.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uazhgsvp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ltmxpzph.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3crbrbzhn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3cfsmgloh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3okdflkng.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3avssgufy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3aqxazzhw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3uzbrjavs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hkddkfuy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3qqixllru.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bfqxknmc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3clsleavx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3bmtshleq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bcfqrtrt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3srwptchm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yuinytzy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3msspfwny.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ekjnquec.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3brmkzqax.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3rrcambnz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3erhushyf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3yftvwjfk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bkdwkcgl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hwucxlza.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwmxemow.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fgxzkncm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eklxgnpo.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwicuegk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3onbciyuu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3grtxxdeo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3cvqdbmot.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lpjnmpke.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mjuaxboq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3azmhvsio.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fyzhzeie.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3aoiizfip.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dirkrwes.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3exebmmjl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dpttawan.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fawhxoyu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lxuceyag.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xzehobpl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3lqwymqvq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xvpsleei.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dfvetuzt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3wlpxzqjr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3hwgxsilh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kuqpzcch.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vdjvwolb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ecgbrnos.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rudljtzf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3yfrfiipx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3zbsukkhj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vedvpdbe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ttferqmq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3phabmcnx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3nhzkdylw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3etaengek.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3syqkodwh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tzmnixck.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nosnjmhi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3gpzjklab.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbmcljok.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wgfmugmu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pdwkzgch.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3lipfiekn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ckdvbgro.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dcecupxe.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eovounpp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jmrcjezc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qkobhhsg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vgixhekn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3egyytosg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofzrctni.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3yluplghb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3biaktrap.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fpblawtf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ngwrmrbi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3sykvrlvx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3bdjksbzb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lrqstqpw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ofypjirg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3uwirtusd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3vgqineai.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ucmykmkw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nykdkprv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wnxxkept.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3czuttcst.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rmjpyqwe.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ymekafzv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hshbelud.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hloueceb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3chbqyakk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3birycklt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dytytkii.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3soyvdfef.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ylmpjopj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kkerycif.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bmdqdiiw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3evdaadma.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nlakwjcc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zwkhoems.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wapcpoio.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3rrbvdbhg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lruugxcz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xztaapvc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3lvvlloup.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ghcfhypc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mmlphehq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qvdptbpw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rxyyyyvz.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gtfjhyrz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3gmnledom.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qrpxsjsg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rhnwctpd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3alugchgy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hnhexjzt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3meylffhc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3fzjsjokb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yjkiehgh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3azfpfqoq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3aslzrhvm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tifzlvux.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mnsizdkh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bzrxtesq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qbwvmurw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rluyanel.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zavwrdxz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mglydebi.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oebbzaes.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xljdwaaq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3swxxaber.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3adyckbjr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hsjmrery.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3euzcsvya.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3eubhisuo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3knxacadr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ytkythne.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xxbndyoh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3mncztvdq.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3mhbnsaxb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hnylcdiv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nobcdeno.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3krzsobjd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jsqtkdbn.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jynikeql.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3psydmnfm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3twjfxoee.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fuyjmwfv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dborcvky.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjpkuyom.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uclwgwxq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vyirmtez.html


<!-- 参考信息 -->