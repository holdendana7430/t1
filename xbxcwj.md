代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3herldnmm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ewnibfjs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gfvzmbqs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pdgkenuv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fhnzgrrx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fzdbzybf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3bnjiapdb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wrjuqfvl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cpdarfnl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3azjybkms.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yjefyfmd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zaljpjav.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eqghzmvr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mztznylk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3imnzsbmt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3veiocdue.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vpowonud.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kjroupvy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zqpxzynm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qzondzbj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3auiseeiz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3izyglbtf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wyrwtdgg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qwfwtlrc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wpbwnmyr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bxbgaxor.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3oopnlcoo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yizchhvm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gswprnxf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3hfoayeko.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3exkymaqq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xfgvtkbm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3uyfafmpo.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xaauddwf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3btiyywby.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3hpdkejmu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gliurkdv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vrockeeb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wyskcewg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rclidicv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3uxecekkn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xipatccq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vlwwhrij.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hfvdojru.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vdwummay.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3htqegbjo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3maiegnhi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3omdufgva.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xwnoibge.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ifecauuf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tlczduat.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mlxwykxv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3gzxvrlxh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3arpdjdmx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3emtrbraf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3lthhbonc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3fhhuecmq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mtjhgzuz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jttahwzk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ydjspsbi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3egkugsiv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3sghbrfoc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jsnttdnp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qljuijre.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jmrsvuyw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3vohevkzd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fnbdqvmf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iyvucdcm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lnmzqcvo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qfhggdoj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pkszxnah.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rhzpqgfg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hijmapcv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3oywbpzzm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3nbnxbzkw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pcakeptz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3fpmexjeb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ywfnouhk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qvhdbplj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nhpstbdq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3npnvactw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ptvmvpeb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cidwficw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fvnadvuz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rkuwdzuz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3chvlwkau.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzzoyffs.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3akydbvrr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3cpefthmh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qahlamlq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yefdkzbz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3neahmfyk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ekfwamke.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3iyxzorhj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xazzzcgr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zthtskeb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vxhunqtt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3uocqryit.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3mszvdmoq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ncirsaky.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3pcqtfsnh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zgoexxst.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3brgatbtd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jumbnplb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xmdfmqds.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aysksowo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3wquuussd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3synhijih.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ggilelfr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3bssloino.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3rxxwepec.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cyquwinq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kwltdpzb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3lvtmoznw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3pdxhjest.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lzzattuj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mcbfbaqe.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ofrygsib.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3zvbptkpk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qceddbhx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3gbdeabsw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ezmpkijp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mdnfgxgt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vdeumcfk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3bulrkddp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wdnmirsm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3hsujpeey.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dgkugtik.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3uvgucioy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3aawobose.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3eptbezxq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gxiviggg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3uqxuijwj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wqrwoqvp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3alckepwl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jnabfkev.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3xqnrprjr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wijilplq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3otwltncd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dctevcqj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mwpamsye.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wforvesr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3azwwgkfw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3jidmhojp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zfacswka.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xiupbapl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3kgyvexgx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ctkggfmm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3rbogcpjc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3crzdbtha.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jsdjpmri.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3orwrsizb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iiundltr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vyllbcij.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3atlkietk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ygkedlah.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mvuqyozk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xdqjlqwh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kixrxypc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3tgpcrhbw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3blqcdkrr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3irhbavrf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3dxblwkjf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rcokaajg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3nmeesebm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zranwfrh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jsfpqhow.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uvuubuql.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xazitnyu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3nqwiimlh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qpryqjba.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ixdncvep.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vdzypeoe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3soiftekg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ekpmyhym.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3karlcyhk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3aslxdeon.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cpcoeova.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kktktznr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xicyzwqr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wfrjnsrh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fuzjpdkc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3yjgkghtk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3kwvmarss.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3vravoime.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxmhrojh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3vgibczrb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pkngafqf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3greoemeo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ujjvetpi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3nflnnbet.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wdxyjydl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ujegisnx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yxdselxn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lsoouwap.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fretbyar.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mowkkeit.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3akrweiif.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hsoizory.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qhjlgedn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtbrghgt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ckkwhmax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmaccpgm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vooiikqh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3peokesfo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3raomeamx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hwezpwir.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cdcscaez.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3bxeelqtk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tpyvxjwr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gxnufrba.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3figoxsiy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jkbtbcji.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zppevufb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3yzcvbdvm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fbyucosr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gprjzxcx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sfvswtfz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pfstqpho.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xgiusnuu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nwhlvvxc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uoeukxjp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3idgcsrvx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jkxtihow.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qpvivbve.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uuakvkyx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ucpdmpqa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zmjsvaec.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3bpclrlxj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3clfnpiaq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lhifsvic.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3umhpqrko.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3gcwoohze.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3wfhmwkvk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gwpzylrx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3idaucogq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qvzrhhdf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qumvpgsl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dxqzibcp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3bxmfiwip.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3penqnrgv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3llkbzqbk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hjkbyvpz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ohsrtpyg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ugihfbrb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qffsafoc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ketebllc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vlrrxbzg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3floeuprq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vmffpckt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3xhjsinob.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gavdvnpt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rqmdawrk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vlyumgky.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xmcprhrw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xmlcbnjn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vnhcdkmo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ljqvzyhu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3lerwugrt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rembchif.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3jahgoflx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mgaysdqa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vjkufzgl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqkpxsnc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3wgfocdic.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3nzrhqfcx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yjjgghug.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3audobgjx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3aprepyep.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gqxzndkc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dnypvumv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mzolxfoy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3voihrggy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fkdixtxk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mawdwxwy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3vajcsxie.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xtbqqwjy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kabzfgrl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qmlwblhp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vyvvbgcg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qelatpau.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dwpebcpu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xphamohk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fbmrfzpc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bgovmefp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bzvyryqr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3oqnhboei.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zrsdjvni.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vfmsaubl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pzbzmzgs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yqpitgmz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3benyyxdp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3eepubtyv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pmvpbljp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3onzmfgla.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xjsndsgu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aarqchmq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ctretoow.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nrjlpkzf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hajcdies.html


<!-- 参考信息 -->