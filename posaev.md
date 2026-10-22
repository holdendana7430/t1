代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mkquiycd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2adnmbije.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ynmasybs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bejvxvqc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2akvhinyx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vwbuifuz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tcbfkcuw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dakrvthd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2swhfdjfq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2beaysxtu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yoivkwvj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2atmrymkc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sircntrg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrnwgaze.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lohjuyju.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2whtmlpve.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2bfdhwuwp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ypnwcsms.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2hyascabp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2obgctblq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2jkujinba.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tepfpxpv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yclctbyv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gacneqqz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wokyujug.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2omouqlhn.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ihpyswfg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jmobrtnv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kqjdycew.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rrrlmrxu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2leqbfcwx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2wzlyydzb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dwfpvwya.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jkbdgarg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tenzwifl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2eahnrsye.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wequvray.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sbtowrvw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2qzfjkmvz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2oojhwlvc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kvqrkkne.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2oiesbnby.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2japweoof.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2bpvlljam.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qdxrauyr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2shbizmwr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2osyfhiwp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2goqcdafq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2trzutufu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ttthvryk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qdxjzmmp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cickkcak.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cydxhqkl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vgipcacw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pvmcotnh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ynsduiba.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qmybejim.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fbfoqkua.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yqqhvxel.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xtvghxlk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hcxmvoby.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xhslwqvh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fkqsahlu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tvwqkhbk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aswaqghp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gaordnjf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2yscyvwfs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lsavcjko.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ofnnqfio.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zwoahnog.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2pbzzkyho.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zawnesxi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rszytvsz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2uwnrwfry.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hkeodsyc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2thxtponf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2dfpmuowr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cuejiekr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xmzpvbsm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qopwvamu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xuubdela.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2uiidokht.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zgfbzcei.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2htcicyhk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2rtfmjstv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2igsrsyug.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wdtscddm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2exyzkucp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xvqmtnba.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2onmygkqa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hlreesrj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bxhdzmrp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nkdnqczo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2infsekxa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fewwcvgv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ghwlumbi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ohpowigl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2vffoxekm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rcraefrg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2onqdfdzb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2jozecstt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2qzszosai.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oemyqull.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qjfcyxdt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aytvnuwh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ngtpjlpq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gaxyzcmy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2vawhdjzy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2wefdefbm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2wljrrkbk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2eszqtyfh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gdjzltil.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2puhrorvc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2neuzmztm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xjqlvkdw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ebqqohxz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qnsbqiei.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ehwokore.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2kinjfrsb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2yjcmearo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fnvnnlcj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fzicsjhx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ufmltgid.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qqssmixa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wwwtqmwg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wnlecaet.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2unvqiudg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yplirvda.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qhkusuay.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qowmdtab.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2rlpnsstc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2mbdjqutv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2osmnfgga.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dqcgzotg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bkmwxcfj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2mziqpkha.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2upjvogyc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2cbanxdbf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2oleccdoi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2iuovuyxs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dgpacfqx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mvbelbau.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2hdgbuvcy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yybgrxze.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cgngurun.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vgerltao.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hurtzuhd.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2zgmboxww.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mxtedzto.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yklnhgco.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dnexwexn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsocfjus.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zmmxnudk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pkilnscs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sumsgbbb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2chmrokvn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2obtrqplt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2wurydrui.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vtzdyfiw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2oxidvksk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uamoibvc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2fbyvmqja.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2yuwqggvn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gvmcpwsr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2fcvklqqy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ucnvsfvk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sksutcua.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2duaudxwv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zfcascgc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2cuzijvpp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dnsjbgia.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2icuebfzr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2frueiaix.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2yuzcwijd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2fnbyjvkx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2dfwslkoj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qqytzhpv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2azdqmocj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wubxcdtn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pinexots.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2kbdnqwns.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2tlekagsc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bkklnaqn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2eenyijcl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mvgeynwa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rqjqsida.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bcxeasiw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2egohhbgd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jasvrkfw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2chmiisah.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2chojysgt.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jgbqfkjf.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xyjprxiy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ypgolkup.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dmkkrrgo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rqthqxhq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bhndmfok.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mrlahqgp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kmnbpnrt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yyzhlfdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbcmrpwn.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2boyjiuzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtuwqndi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tsbaolwc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2dprkqvfd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zplbgmfj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2imgvlbem.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sqgguhbk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2rqygendp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2hztpxisz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ixnjjcwg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rhnqswgg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rqkmmnbr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2imfpzdbj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2saqntfjm.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cumcseac.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fscawswt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wdzsmzxw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2galglxdf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rakxjqjp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pirwcckl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qnbggpfr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2zzhlemhx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zzbighji.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oxqkrszn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xmszapvr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dvedjrys.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gydplpsu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qekzfbzf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hagzntpv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2knkpnqwg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cdhceheb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2upqgjgkz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2jikbkroi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2masvzysw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oyuawloi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2wdgwrzzm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jxlktons.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ncowvwqu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2eqyvzvdu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hcexviyk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xovmzycn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qpbjnzlr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ycxhkpeu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gqnxdlxt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xekckglz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ffyhhvjk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mjprvjzl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mplcrstp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2nepoofgk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2iwtxqdsb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2enebvhyu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2paypmavo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yykmaobs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ldfhiaqq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kxqrhxxa.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cagcvkun.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rjswmlpp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ohrrydsw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lhqgkvxs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vgfwvbpb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2xtyzjyib.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2hikzytrw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2kujjptkq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jldswljy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2nfwchras.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pwmfecrc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vegwywqa.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2phgglltj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2owhrhzzt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lthogkie.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fvgxkhav.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2zoyozdhf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pshvaajb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ubcmpxue.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lrddvvqq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2aghzdmua.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qfuxxoqy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jhusdlww.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kkypykko.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2morntmnm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2mhpqbvmg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xhepowfh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ufbgaeoy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2libsjfqa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2smjosytj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2berxeyns.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ibbhucyq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dkjjnqxz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lbitrkso.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gxfyajes.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vlgmcndf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2frebhmje.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xvzwdcpw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qbklzwan.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nzlujvgr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vrzbygpm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rmzonpbe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2msibojqv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lkcrsitt.html


<!-- 参考信息 -->