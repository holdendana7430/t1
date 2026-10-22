代发 wailian999

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2uvlvivzu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2qjqwshrs.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2peneahct.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hxfupskc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jiakxsdq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jtyfuomy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2bvrwtcfr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yiimiqoz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbxvnse.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2trlqkggz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ydsjltkm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rvumhnms.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vubzgxhx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ejrujghs.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2skixwtih.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vevhiumd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xcmutjpu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kmmkjsfr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zaywkxhm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zzvnpzur.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xctqlfeo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xlkfmzdy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lvcbafmt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mzxtdleh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2difboruy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nustqsum.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gseurtuh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ekgcgwch.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kcybzuza.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ucjpcobg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ktxpmutt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nkddvvpe.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uarvdren.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2usjkrhyg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2cltwsidc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2tcbiehhs.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxaokmin.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mupzapus.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2weolchgi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mnlvupsf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vqhzhzme.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xsgzntwy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2nlcchdyv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2sucuxnyg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2edfuwlwy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qftxnaxa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vdctlqcl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dpyxndbl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rugajmya.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vnrmvkwj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2eqtzahav.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mehvpbhn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2trrfzjyx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qvyigrcy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yhonlduu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2fshkdtza.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bvygvlyn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jfsgazfx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ndwuhbwo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vmhhzvdk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2chmxiekr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2icrwdjye.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ogtjihdb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dtfznlcd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2obtbpjim.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqtlsfej.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wuazmnvz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2sroptsrc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gtprqwyh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2npapdaxd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2opfatuwe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2aylegtrq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2fkhkbbln.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2osirqefx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rmtngljd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vqbjizxx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mjwbudnx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fidgrrbx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2tskoghgn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dyockvqf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2oizftowz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ifmjqsqx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gexpqdjc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gutxkfpa.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hphyzvrg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xmcsoiex.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aodzrudn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jglgscmt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dtxmqdka.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cokgrkmt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkqkydbv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2xmaongey.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sygoljpl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jilquidp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2anjksktr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2bqkipevy.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tfjiihwy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cjtpgfxo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2yaoawiee.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hfhrfrfp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2udckckkx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2dvehtgob.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2jtrusvev.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yzqlslbt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ptainyfe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2nkycudcj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dzlzavwl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bdbxsyxj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2wkyurygd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ufvrylpa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pbzieapr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2upvpkbph.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2nstbikzx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ltwursuq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rponbjbb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2kqtyuuar.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ozimxjhw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2eduddkug.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2uxpjlvwg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ctvmwzyc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2sdshnuxd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2izppjxau.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ieyfekth.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ibwvllgg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hpaycmic.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hyhunaal.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdmxrnqy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ivivorgi.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kaondcbh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tuqywazi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tiauhzoh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uctnjzsi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jvbxtxif.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qbveuqsv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uplfvome.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nfyilzvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crskjjaq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ickzwzar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oufgungf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2njzasquz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2kvlrtiuo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hwyreijb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wvknadjk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cjzfiwws.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2tyblmhvi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2aqsareig.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2eiictcjy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2csepqaic.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2orwzectx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2usyzovcw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2kthjnwys.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cxypyubc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sbjrjsna.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qegkskbe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bohwfwrz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ctovqkhe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nciolhbx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2byklfyyh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2soxquvbr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ulnzlntf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zaogwfyj.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2urxpbago.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xncvdzjq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tieevupu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pjakcjwj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qrkdqglu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ddlaiiwb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hsvpptye.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2rtzavgwc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2qwfcaoaq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eakloact.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yrlusawe.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rwuhrmjd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zlmdfcjk.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yswdqswc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2upxhduya.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lzxrbqgi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ziwlmfup.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gzlnldqu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wguwdjno.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vtavfikx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qyywcerk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2hlgybhbl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cionpqyv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hhndqjjc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uazgdtyu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kfzsivws.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ozfysqkg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nlpllbgt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2orjpyoqa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qojacgzr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eqylugft.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xbowsabu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2wrowuoid.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2lclykmuq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dwjqprki.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2eikrizox.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2lupmgmcy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rlrgjrcj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2lbmdilzz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kghxwkbt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2uvgepnow.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2njcnlwkp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zakcdxhc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xdxlykoh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2edtebpmt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qivgjmqn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2roupqmmc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2lddiqvpd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yhbwgunt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rzyezequ.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vsdrserc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2akyuckyn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kmvipoud.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ysckuglr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pebyqter.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cqaybmcb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2qnhygzks.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ohetobdw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2stfyczgd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jgysfyak.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2orecrsbk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wjuyyuep.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2twvrqyvs.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ejrimqui.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qhjmyrel.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fnnsryxg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qdwubhrl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tsimclfs.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2iaafvbpv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uijbdien.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2biwdnxdy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yxvhyzce.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fqmodtxx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wlaaeqla.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fvlbakzm.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mnxrbevx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ckexygsg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pejfjapn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hblwmeyt.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vyckytlh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2elypurba.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kixopjkc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2baphtlyf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ilagszly.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nrnybwfl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zvnwzxnv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2cwgjhdkf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2nvjgfiql.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zwtyorgh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yejivemp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pjjchaok.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfgelwbw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2quuojwip.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mzuzttzc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qlbeuecl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2utsowolt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kkbygoxp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2iqqwlahj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xntsrpvh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2kdeiuwud.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ojlrspce.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2regxelkx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jyvxawtq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2luexmrwl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2aqgfmttz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2fymjjhrp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2sjygzzng.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rysvtcmp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eliritzi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2lxdepsks.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcusbrgk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mggxouha.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pqfqugqc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wpimczuj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2brooonsx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2umuosdsz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2higapxmv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uynmvbuj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ykperher.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qpuzaryq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wbcnvjey.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pdtyhdcv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ffjehgvu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fimwmolw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uqrbtblm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dppxwtkh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wrpyglwp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzhxizwi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2trntfger.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dkzgcbbk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2itkhsbpd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mfawsymy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ooukcbvd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2glvcuifx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wnmltolz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tgmpnkpc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kaqdkdan.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kyyohpye.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2isjpxsil.html


<!-- 参考信息 -->