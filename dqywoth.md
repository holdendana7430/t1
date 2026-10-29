代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gatqkwmpg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gfvabzith.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gqntowypk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gllcvmjov.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gegljmmss.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gklqbxnaw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/ggzcqkurb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gervsujhj.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gcwqapzsw.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gfnbrhesh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gywqrdmmp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gidjpslbv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/garnzaojn.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gqywhwspp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gscozvprw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gefucbvul.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gwvssricj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/glntldxcg.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gkbyshbxl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/ghamcufke.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gpggyyxdk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/ghshupaza.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gsjpvysbt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gfenmbpgj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gmpwfnlyq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gbtxzwkbq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/grmrnlagr.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gaodvsvzz.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbizknom.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gcsgcryyw.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gvekiffin.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gzwyuupvg.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gmaohkydj.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gfdhfsjwa.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gauebljeo.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gjahposmp.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gaswpkpzs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gniafnaxd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gzhhfwibk.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/grhyrvzjq.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gwqoqupju.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gtesxusyv.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gluthqtts.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gwhfthgtq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/giptotyrw.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/ghlonzpuz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkaamxzap.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gaekuxrbe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/ghlycwjub.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gppqpreuv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gnqydbknj.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/glgetrqvr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gmmyrurcp.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/ghiejxtpn.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gnrisadev.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gsahkhzhb.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gztomwgfu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gssxtdbvk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gnuxwkazk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/ghecdumfp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/giuuauxap.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/ghnheuxbu.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gufmmanxu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gohwumbqq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gtjdoqxkk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjkksjhl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gxcblfatz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gwfafhalr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/guxunigzg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gkvievsks.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gncwepeap.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/ghhlghihv.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/greivyfvg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gurdeabms.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gbpzmuxnx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gmczbckes.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gbulurhjw.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/giayirovt.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gtexwjevo.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gydvqjcvd.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gigsdhheu.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/ggszmeopu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gobsowewh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gdxezjszh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gikbtvpgm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gahmgtzbw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/ggepvvzsn.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ghyshdnvl.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gllspoaus.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gutxjirmh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gqjdivadz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gaqlznral.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gdgyaatfc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gkidhyswq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gsxrfjhst.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gdmpxuyel.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/glkfojsii.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gjvgqmpbs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/globjoutb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gfwrqtrcp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gjtjenlfz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/glfouvgge.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/ggokxmurr.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gisalwdmy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/grprwyhln.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gbrenvmjp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gdtervsnu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gsfaofzkd.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gvymcuaml.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gndqtycli.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdokvkjeg.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gfolcehno.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gpsfcvvwi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/grvkvrlus.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gfxdxjrjj.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gnkownarr.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gomioryhr.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gtoipguzf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/glevwqvhk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghvxxhorx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtzujkzwp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gyuhbngvw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gulqabyjd.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/glfqexicr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gemklcdlm.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gszbgyjgq.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/ghugtkoyo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdxpsbfrc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gbdauyqmc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gphyryezr.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gkczykwfz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gfncaqusu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwnxhcvtc.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gpyiduadf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gxwizkjgs.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gdikonivf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gwhafxqtv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gvoutjnlr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gncekhnhp.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/grstmpbib.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gqevzdtlm.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gxvjcesvd.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gvvubpsid.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gsjtbxhnu.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gjcgppyge.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnplizgv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/godbydxuw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gestjwbob.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gbkeudnlh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/glvbxktww.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/ggtmnpeja.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gsuxzguiu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gswtwwoqp.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gxtlucvxu.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gzfgwnotv.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gtqxwlnyo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/grqhbrvve.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gqjvfclfe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gcvhgiwot.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gddibbuwv.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gaqfphgxd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gltwtwoit.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/glwkuhbus.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gudfdyakr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gqcdpgroq.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gutdjtnrv.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gwuollsqo.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gylbuqhsz.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gzcwlghcu.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gspnguzwp.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gvqqtwoua.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gflnrkvpj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/ggpcjwsie.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/glkcxkjdc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbhfkpmye.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gyjkbpmsq.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/ggritvkec.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gmhvzfmlx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gwwumreso.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/ggwljcars.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gtbzbjtdi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/ggbuxpisu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/grnroeaet.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gabmlzpwa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gjyrjvykl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gioewnitu.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gdynzwchg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/glbnzbsyu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gsxhaganm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gkzbnaoan.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gxvwwdsxt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gpzdnuszn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gigekloza.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gujezufly.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gruxcjere.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gpilpobsh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gjhrnjlvz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gtzdrfgss.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gjoojujqa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gvmvdlgwy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gidnjzbvl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwzqdaswb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gfvmxbnup.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gfbdixokr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gafevwbbw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gyzkovjzj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gfbznqnei.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gowfydelu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gtraljvbr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gicaznmlo.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/ghdshtcfq.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gvbzhowzu.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/ghyntgwip.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gommxlkht.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gerwgixov.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gjmdjifal.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfvjqqrwy.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gaijaqhuo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzncnweos.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gajmfgngi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gxxncflmx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gpjfaaanf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdmpltxbv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gjqhamsog.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gisyttcyh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gnmfmpyvl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gjucjgzql.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gcksuzmah.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gatldlhhv.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gowjxiuzr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gzhcdijen.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gkshgpqct.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gtpcmlcbd.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gwbpzhsbk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxheprrza.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gchqqukeu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gxefxnrhv.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gdsszvfuh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gemxoqwcp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/glkivpbez.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/grfjhujvx.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gtjkyqnjl.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gfwjobonq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gyntdmzjo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gscyxlrab.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gurddiywu.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gvfzhmbad.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gbjbxwsyg.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gaswujzcl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/gkaknxuis.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gymteaswo.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/guozncfxg.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gmfygjrpa.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gkvfhhqvx.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gskizymve.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gjnfjmtqh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gzxscmgxx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gvsgnmlnp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gfimubsdt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/goysbvskv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gzbfmrgkp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gpvsihxdf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/guvsnkrmf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gsthhyojr.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/grceiqroc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gsnktebxf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gfmfdekth.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gikzqthjp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghjryveeu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gqhqqtwze.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gmavbzkvk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gctcbkvyn.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gvlmnxwwq.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gohslmffg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gjoftwxmf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gmzcufdzj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gknykecrs.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gnqhiinlt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gaeqmuvro.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gmqrguexy.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gcahlwfkc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gatwrjbok.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gjndpupkv.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/ggaadiggf.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gxdaazuou.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gtevrvjyg.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gwztlkbyq.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gqlarstrk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gooviciwa.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gsxmigjih.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gocrrfyyt.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gudibbycn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdejocmyk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/grcaxesyu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gllvvejqi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gtldkdztr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gjqnnshto.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/ghgqzsuco.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gubrlpuks.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/goibehlqu.sHtML


<!-- 参考信息 -->