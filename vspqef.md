代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xbkgpsqx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2uzlqfblq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ypearvoq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uicnqwng.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fvelaqei.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2olfalqsu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2hgmtnrdg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jhdxqigb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lixvoxdn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ndlcswdi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vwkpeezt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ptvpbste.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gsokkael.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2syxwqlzx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2suwjhxam.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hgmpdinq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2dxumlqva.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owppeqzp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2klsfbygy.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2okvtqrrh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2unqgnfpo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2hwcayaom.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hnueodsg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hyettxef.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fnczlkpe.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ulqdrqeh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2aliuyzak.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ydwmprsp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mxtsvftl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ovrmmexl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gssqwcvt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bnidjmct.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2gtukscfw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wezkbaby.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cvdptuwm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2zogpybyj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zjrbeuit.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jguabbpy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2rvmlvghu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lcpqceow.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2alnmkdkx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2uavkkhnk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2zwummkip.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2pymxtfdy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2erurxuzt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kmlwnpse.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qgpekysq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wkbjwbkx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2amnhlyrg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ldclvykf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2evewetdk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fmoddzys.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xntvjbqc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hdeejcbr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2tmwykpwr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kldfgfzt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gavjzckj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jffufsgq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2idmpjvue.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gijmhzwz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2drgatyrv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mjfmyqbe.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bsdtjzdp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2eouurkbq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yfuldwah.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2lsumglth.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cpwasalj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kjpkfedi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vimskpxc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lwetoccy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2uwqcahux.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pvzmwmff.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fazhtqnl.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2uhfaqtab.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2gzcubwrv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rcamtfjs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ojxbyjrl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xodzhmqk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tghqvcwj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jtvhlqkb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xbxdecle.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2iqtpisps.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2meelbieu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gstbjvxn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2diysdssq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2quyisrcl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2twogppka.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzydizdb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ubmbaoap.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fmkkcgqt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2akacppsg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sarkokux.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2nwbgtxcy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mdvohjrn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2qcvjbcfx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2zyoqnfvb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xxpbrhib.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ceynkdje.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2canvukjr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2gkoqvoac.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2sjhvnlnd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ghnuvqbc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2aphhynyr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ojgtbtud.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pmbbstty.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2htgrjhoi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2tatsjzro.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ugyinrwx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kvsjusvw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2kwqxrzku.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hmhbdwps.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xuulzpot.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2insxdxij.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ucopluau.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fpuuttlh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2bnjmhhfi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ktyqpjjs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2etwmsaza.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2hzwhwuqg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ohoycnfc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2hmvnilwm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2scsoxchr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xitjyuvn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2tlkmnrgu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lezhxedf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nqcihjiy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2qglnzwut.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rvizaymr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2tjnccsox.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2rcriacdt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2orsasvck.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2defxsyud.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cjqebuak.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2bcicnuiy.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wnpkfgez.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ljtbjfkm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2klsbxmhl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2uixrjbbe.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mfiyuxxd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2thjlqsbf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2arraeggq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lhwiaiwt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2nhcohifs.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2qnrdmfwz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2zykonhlo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lwdixaxi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2cnmqbnpu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dfuyuqvy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hatlefre.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uvkotljc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jtryjjjc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fsbehdsk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2avnswyam.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gryihwrr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqnrdjvq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2rodxdwsq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ztgdepvf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2yxmubkzc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gzfjxuvk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2trxoerfd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ubkxlsnb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zqmlcepv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2wdkqmjqj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tvzscefg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2geshydtw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2byutckbl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ozgffhbg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wuonbjgl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zfgbtetx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2knzfwfcz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tzncctko.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2btebvjux.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rcloqkja.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2brbskapj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2oyjzyusc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2kkiyirpu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qhxumdjh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zamcbtfs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rfcqslgy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ycwxkkhm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mjtnmpus.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ujbcegcg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nhjmpeda.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2zlpjimfa.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pgjcafgm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lrzkojjb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hsawdrly.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jixewlfz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jelpzqcf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gmnudfhi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltjxclcy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2wrftkyzk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tlohvmjm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ucaopqkd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ucngcffg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wojleuli.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lgjtereb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zdlohmbf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2znftxkck.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ywtfvgwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ucczehqj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2viklbnyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucehyvro.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ypberciq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2swexhssy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2lfvwewfs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ltayfwhu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iikjqpyg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2rlrqfodu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gosmrxtv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2voasaxes.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jgfqwgbr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2xzvwyhir.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bimxykua.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zyighalx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jufteopi.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gpcbynjp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2znfslsyt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2iursgyao.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cptswvee.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jwebynnl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wuzezhfw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2qgyfncxm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lhuiutvt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lvuarzsb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cqhejndp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dvqxshvr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wybulxyi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gbtqlpgn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2eponmbqo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2teruwfpq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vegmbsun.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2nyleosfi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ildglkbt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2plvdsmyp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cgqizcrm.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vqvrbiye.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ftpdrokv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nslkjjcx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2uqkxsjlt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ydcnbllh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ogxnvrjh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2agwztvwq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2gikvihze.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yqhdoxup.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2umaafewm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2harjpxos.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2evtauqte.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2enrojumy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zwyoigua.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bjwzdpkp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mcsavotz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jrefywda.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ygmysfkn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jiuudlwu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hsmsqwyx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yhyglegq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ecuqnnmf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2vjbiekbg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cxotlmrj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tuywugsx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rqxqhdtt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ggmavwps.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tfymwqud.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2nbkzcubk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2aoipulzq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ngkqtpip.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xipwffgv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ufxgpcwh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hgbvzhop.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aogjcbxp.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2puvcbaqf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2lpmtvxqd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qzpajyxv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2suhkrobj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fwnvnxti.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ujcsfovl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2oimvyrpg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zhxtvejl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lznhccfz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yeoxjxed.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2svhnolpp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fldgntij.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ezjmwpdm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rwebiqbj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wljmocen.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2lyqdehyp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oevzjlqb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jaxuoxid.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2arxnmeuw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mlstbkfm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jiedvlrd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qljmuzym.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2xghpbhpc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2scvwzaux.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2frbdgwrl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yxaqpurb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kdsxufvi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2exzxutts.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ftnougda.html


<!-- 参考信息 -->