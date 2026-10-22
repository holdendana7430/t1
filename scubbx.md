代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2uwaguoor.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2mfkcdfxp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxjqpwhr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2akvchtcu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2erhueejd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nxizeutf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2pxdlspso.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2owaflskz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eijxlzxk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vfcjlzjd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dtorjgoo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xagnvdgt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cquhpgiv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zqbdmruy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2xpfemgul.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2emdbcmeg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ettldcpx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2flmxafbh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2fgbaeloy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2scspbmtu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2weecdnbb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2kxpcvqub.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bvlawluf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2tjncswwd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zoaitdug.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qipmhcxh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2nlsfepyy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gaqiygmx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jeshjqmd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xnmwkxkz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cwryvjus.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2sewpzdja.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mcacqgrt.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2fsichzxl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2notkemdy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ukdyunkv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qotwtafm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ggkwgrji.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2epizdmbv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hdbjjejl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdubntyn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2pxskvyia.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2madrftrl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hiqftzly.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2lcfbzjpo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qgnfyybi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bcaprlcn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2oxiajwfp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cnejonyr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2coafqqdi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dqdjomjg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yenymnpt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jrzjobwq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hchknydd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekvokfqo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yasontyy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ffkurafl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2poienewx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cbdeeszk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yubahgko.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bzshevvk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sgfbuwmz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nkautymn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nuzglhxo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gkzvneky.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2dklkdaay.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2veswedfz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cidzinif.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwocceyz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pssybzlm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tslgatha.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fsntbsba.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wnhbtdvw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bccpyzsg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2tjtvooco.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ccszxbqi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zfrhlfhf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qwdvylut.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mjyufrjy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2npwxrbbk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ieocymda.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wyyjpnqr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dssgykit.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fujmtunl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hiqjxyjf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kyiwylhq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zadkliwe.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ctkbzwyu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2gcughbtm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2kqecnwef.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2llfrsdyu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kutapvxu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ydgsdchd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lbtabokk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2agvikere.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jtjwpmxq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yrxdygwk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mvyxvrjj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2cofjwghi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2dwjoplfk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cmnizohs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2whjttpxp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lprcvuvz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2smvwindj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mpjdxfxi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hxdudvih.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rszfjojn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kfefzqlm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ufnnpdza.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dsjqqbmp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2gjowtffz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jltnxqcp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vtnyrzea.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2fjtqnczu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2eqenwgaj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qktjbvgs.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mkkpvpky.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rqyjetms.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tzdeybrp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dclpnusk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mfyngydw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eowntmbr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojdqwubv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ywkouoqy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2uhivtctn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2isjraway.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jjcszdry.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ttumiwzq.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2kquthbty.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qkffdnxe.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2tuxqwcqg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zbxzgztq.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kjgkfyvs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gpocrcpu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bugzraiu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ebkgjaed.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wqzyufxz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2emdfqknf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2okxdlqrc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mbgljevc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2jyuxdrwu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qraxmfsw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ovzplfit.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fkkezkrd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipqabfsx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kpuerqbk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2sseiyfkv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2uyfxzgus.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2usobaldv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2druxywtj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2cliqhozs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zddjavuq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2adoywvca.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2brlcxtut.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2oohajpxc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tiiwseap.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2nnjcyctr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2foydpbbo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmmfuqhh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hpdvuznz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rdxoohmi.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uvlwvcwl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uhngdoce.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xltwuptz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2akorrwmw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sorxqbex.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wndjpewj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2iqekhmls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmfucytj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2cjtigpxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pphluscq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fpocbufj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2frsjmuhr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xkutvtwl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xtfdoois.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mbvvbzkd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2pvsmtkxa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2iegyspyr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2raiqwqkz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jbcrxpoy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gksdxpfg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2elltzrla.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eldubvpo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zkvogfop.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2swdcwwvg.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xpostvdo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2oqrgezml.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2stqckhmp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dohishpg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ewqadqgy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vkguohgf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dejugtnf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gsfqiwoe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jtjcmyrh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tgvoptvi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vgqgfzhq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xhvgveem.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2smxqcmby.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tpaeziuo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jfuttvpi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2iihmwgah.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2zhterkcg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jtbgdyix.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zvpygpcr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ujgsvxuh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ytbufgsq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2suoixipx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2oogrdnvo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hlwcgqaq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2khhhizfl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wtwvyypa.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hyfqeqfw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qxpdmojf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2yelfpqfw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2swrmmfak.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nzkkpatx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2bthuowmx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zkpxduec.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qlawewly.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ypmjttvx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zyumnfel.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2foodhroh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2usvfzmgx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tolemdjt.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wghngumf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2qngdcbcs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2rkgptkqq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hsxjbbif.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ikdudfmb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qpicojgc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vcflzltv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mmsxtckh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ufpgqgal.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hpuhtjhf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ucablpmq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2zdskwjao.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2opydsxms.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gtgaecsa.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qimpousl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2etptpbdu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vllhcjuz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uypvcchc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ncchxvkl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2enbmhqwf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2abmuzrpb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2xdgkjekh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ajaqrekx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nglhrxzc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bmpowxfy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2twnabnpy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tsbrmpdl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2unnsfekl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ynfbuthe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jwedtcyw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2dcoqssuk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ahtnkkpo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rpvwvhvf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2drwcaxjg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pjervcqv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vryoyhjl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2gbxacqrv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vhwiyhyj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2misxwnnh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lfcvxrhi.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vuwmsymx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cmhbledu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2sswzeyht.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2antwrzfz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ppuwkbte.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vzuudzhn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vtgbcwqk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2obkmyfog.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2iwbsswac.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qvkjvjro.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ckphcqxs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bcnmwsrv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2kmoygqbm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bdwyyzxw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kiilnzlg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ukwofcif.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ftypsore.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gzymagfa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hydzsdpd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2svaghwjl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vijquwji.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jvghzxlv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2enghjaki.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fuhipxvs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2siximjad.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zvujnoey.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dyjxmsrq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xdylxnmo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uurzzqfk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2awmqexkb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2iflajfni.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2cpkzdpxt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kwzwlwgd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2abwzdqaq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aadddivd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zobvgoio.html


<!-- 参考信息 -->