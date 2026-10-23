代发 wailian999

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3nsgjkhsa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3gxudectx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3aaifrvkb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mofznwgn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ysulhpvf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ztgqaypv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mopuzibi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3asxbpfdi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3yzockfbw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zdmxhkqw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3azhlifzt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gyaorqtl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dzhpwnoy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wbttznkm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ozujasbt.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lmjtktfc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kxtjgftd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jpuqwwha.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3sulerhlv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3swmvbach.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3idftigwi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jashbkog.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dxhtxpsn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yqevxafm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3phvokqeq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3kpegyctq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dhxpgltn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3iakzjmzg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3niseophf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3snocntad.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uizfanlx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qynzwkez.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ohbtngta.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sxifdier.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jzuzreqk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ripkgsqb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3flcwvfmb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ppgbnfvi.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jfxefsjh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vwsmmgtv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lqogvkzv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hxqdaeqs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wmlsqhpi.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jyrwyawy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pinziaze.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ibkkzqxt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gslsdxvi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hiynnvwv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cahvdelw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3asoisnrb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mvsrobwi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3yfqulffg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cfnjyqdg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3jxvjywws.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3tgrprzgs.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xtwxiizg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tekidzuy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xjvbysme.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bkrjehzg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3eluwvrxe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nomomztw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3nfxppaej.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3tvqihylf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ijuecxqe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3jlqumtkr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xkezqnlg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3buwxjnbr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nesdbhgj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xbflnehv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qcwuztlk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3rjouwjwq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3awmaynug.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3peadojoq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3golsjyys.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ezbzwxif.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bkstgshj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3smdfoqyl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3gqxoiqyt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ptleptdn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3caqoolnr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3zcpskcmx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bvxncvzw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gjgljryy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3guajmbuw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yymbgvzs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kktkzmhi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3cxbbckkr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3bsxfplkz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3xgqaoaxg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ybjdsheh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3bbjzvrom.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3cozsykus.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3fkkdswxs.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3otkskrsb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mafyrpic.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ycotcphz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhdigqxv.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yecbiqpn.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iraonqct.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ffstgdxj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cuzghmjg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3muelpvtj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ffhrqpau.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jgjscxjq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rccglsse.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3xlecrhxq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kvdwvxdr.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3vilzpdxu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jyvaeznb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kblpslhy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ngikjika.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pjxzccbg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3curbdynp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ixzsgfiz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wdbjstvr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3vfsdipdu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jjmhbpdh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vlbeukgc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iyjpthot.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ciiaiege.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3aiycbyki.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xssdclkz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3snebvmkf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3rodygmvi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3uvvmdzhs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mhwbfsyd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3eiqvhrpp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ycxijdab.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3jmfiencs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3sdofnkpy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xqmaifmi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wrqsibrv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3plldjdar.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qgdhnxpb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lvjpkeos.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3scvpkmir.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3pdtsdtmq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yadoalcb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ajrikekp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3degqlwls.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zvopgowh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3yzhufwtx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3umpgiqjx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hpknjicj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcmgfszm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3miukzywa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbzsgrot.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3inkvvxlw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3gspjzshb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3acunlrea.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uzzsfzjt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hvutxnby.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3arbriofb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ystcliao.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bjfqvzvb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ebuimfzc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3elluppqv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mnruogpn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3pgxrlerl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aotwgmon.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cciathei.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jddtudsm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gqgucxll.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zplarlqm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3mquqnolb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jypovbsk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3mrjncjbh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dwypkdmp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ofougyob.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qptwnnjd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ifjqmfyh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3iqlxdpgv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ocpdaees.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ezdivdbh.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3xrwzxdwo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hhhmtmbx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kwtqazrn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xxeqrrkt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xbhlucji.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qyidyyhu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3oalropbm.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3lznktffk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wgwxndaf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ukzdlgex.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gnwsbqxz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ehppufqt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ejdfssel.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3itsjtucl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3isczojfh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3rqpkvbtm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3taojsjle.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wlcduepo.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3tlxibdjb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhhtjded.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3llrbxrdv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jtdvmxav.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ybhptdcb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ynwikiqz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcxakgpi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ppjzbpfj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vnhhxdzv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yhxvjdez.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3igxqdfdt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nedmerym.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wuwegvlu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wfdkgdyi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ryvhlfwf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufufjdyl.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3yujdhiqi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3romzslqn.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3swktjpuz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vykxqghh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qaeqzkzf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3czneugom.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kbufquox.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3homivvpf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lxtyzfhx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dnzqmdcp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ytipthjd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3edzwyvmi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3aipuhamb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3iwmhhokl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kmmjcfbz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ngcvknsq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mmicrmxx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3wvoduxov.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ucnhuqpk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bhnzaefj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3bsbcopyi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uaklaata.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3nhoanrib.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cphepfei.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eoxtyrvk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kbctnvwz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lsndsfgt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tdotecqz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3nuxvkxdy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jquguqnh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xxmouhni.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxbfztoa.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ozxpkkvc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vthzicsd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xghmijdk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3huximxwv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ullomadx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rsmwnuvb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vjiomgju.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bjxiecrg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3yfdmrtnz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ezfmhurj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tqdpckfz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ziaynazq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3auypiyaz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3umaixdca.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3osmevnhv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3zgyuulbu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3dptaxeil.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tpzhqxph.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ykdcvrxq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3emuowzzq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3agsfmmif.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ocniriuk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3crbfmjas.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mjpngidc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qlngejcb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3yprnyxqo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jdjiligg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3tksgihjn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ocomaodw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3aypvzmxm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3moorcdqj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tbzulthk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rsloywka.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xfogvtve.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3faubpiic.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3pjgyydwb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kkbhewtt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3njozyjne.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rasxvpcq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3mffruzgn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wszkkjbp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3rtggtbmi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jpgfjumr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jhivocrg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3xfrlrhrr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mljrutyd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jvhbpqkn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xsmialgi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xhiipgaq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nicdseux.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vlxeyqiv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3daynrgwu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hfwcfmya.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jkepoobk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nmpulujh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fogqvphy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzjpkfit.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3enfijfne.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lqwqxqgh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rokvtned.html


<!-- 参考信息 -->