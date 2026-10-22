代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rfsclzkf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gjrignar.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2grogbiga.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xbrctvjt.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dzukwhqs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2kcmrzxnu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2reltsmvl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2owipoouq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2noxiqyio.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ueaeqamx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pdnimwyj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zmvyldvp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2gebsrwfg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wnnaoujt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wbsbmiks.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xcccolqf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2njeybvmc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2txqqskfs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zpvhngbm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sinfcfbm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ozdzkmlv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rtlwwgvg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ewaslpmo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2huroxyof.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wabxtamb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2gyhgbkti.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ilpxmaff.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bbaxvtsc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rfznsvfe.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2urlgatlg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zyotktmh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2omyuxsqu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hoqchiem.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lhenufll.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qupdabux.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cummugfn.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ytqmecuu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzsodxn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2rqetyrbn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2cocdecav.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2prrzjnzo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2lkqbptgp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jatfwlzu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2szhuzcri.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2lumlczww.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2iquqzudr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ggutvlod.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ztnjjadk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2newjkxxt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uziknqza.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jvzovrju.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jhvidfpe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2enknwvqf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2eqquuwve.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2wxsxjtya.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2htvtolbi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nowrapxy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qzoyxeim.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mgdeapzu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nqgggywq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2beuqqonx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2asddcqam.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dcaecjih.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2nqzwtbxj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2phhtbdwb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2velmjmkt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2agyllzxo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2oxzvhgbj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gvljaskn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ltyokect.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kzbzsbjb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lgqqswjw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2tkczlvwp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2iegkxexw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qfdmmniv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vosnsybm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2focdlrjq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2nfhcphec.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nteyfkfm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2oahlpiuv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdhixdkw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2idttbsrq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2uixrdcdt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2muyvesxv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2irwywrbh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eepxfvst.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zafbgqtb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2rbiuoczp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tdnukjli.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2hpcwhbgt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mntwrfsg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mnvjiokr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2yfmzgmpw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2isjaxumv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2wocpqxxm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qfzklsqs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mdpgtlpj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwdwcqod.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2eoccgydf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lvlbpckg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2bgxwfpke.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zlkpeehw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jjlpnzip.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2njfcikrp.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2acwmwppc.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xogofyiu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mmuzbwey.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2woznhrtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddliluso.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kpbagejw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knbonaos.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jmaofrfm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gjxbjkek.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2vnuvimvd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sivsqbby.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2khpswgry.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2upwenzlx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2cetywxah.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2jjttlqvu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ppyaltoz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2goxrasyn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2clbuxuni.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2useskgkr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fiezeska.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ahdvfyue.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iwolpoyq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ydklzsya.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2quagelfj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wujsbpzi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bhmdnfgv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mxtskkou.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zhrkqnbe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oyzjvfzf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hygpiaow.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lufqltas.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wvxnxkfu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2kizcaobr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oqsxtlor.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2xnfuahyz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qkpqjcag.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hiilcycs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2exmaptrf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vbskvset.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cozlxseq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2btcnwyla.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gaavsnwx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tjwffwtx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2eaoeznrc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2svxjtmbj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2hxhahzqj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fiffhxoh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nrgammkj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tcolmacw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2sifvvouk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qeapmeqf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xxbhniah.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dzdwjbim.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yuuoutwr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ojtqyvlr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2izfcpfeb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ujuryzyt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2khsiscxf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jkjcgugb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ggyjrycr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ytenujne.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mpkavamz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2dhtzszik.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2anrouwpq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bznfzofp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2nigammfg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rmrdpwas.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2rosvekwv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qauqjsrw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2fcqwnvve.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2yxwnvlvl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2swulhauk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2aaffjsft.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iyhjuuoc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2urjlaiih.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pwlaxezq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2rzswpsch.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ueipgzys.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zhdmwpav.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xztdfgzf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ekqlsetf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gtuqitud.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rmcjchws.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2olqkqgmn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rqzqrtnc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2shlfjwcq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pumdbaff.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cuoeksup.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gqpbwzah.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2prcqsvni.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2egjqywry.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2okctqamk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xlqgehjk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lcfujijn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uddmfpuc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mestcney.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2dsexgdud.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2reixhtoz.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vomefyyd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pngadnqu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jbzlujks.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ubuqqkpc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2njhrpbds.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xoyucwwy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2remwsrsm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uimraush.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2maruzipu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ojfkbydt.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2fdnqpuov.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2usfhahsf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bjkmidvd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ayarvdeb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2yfgmhjpc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nbqrorrz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2rgmqdsck.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2tojjidpn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2bcbtagof.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vmcyyfvj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdfzealg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fbwjgzch.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgkiuuex.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qinkoicj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tbelozkt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2byznrfqv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vjhayrml.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2umfkrqwy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xfxlezkn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2survyikj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmwjyvsw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bnpwphdj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2widrwomp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hkmyaone.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2icxxtwvm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rljunmjb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xddzqjrh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2leuhjqzf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2nwlbtvjz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2huksoasd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wulvvjlu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2tjbxsfxr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2inhkfkmn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wptvlljh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2huxpmehx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ojvfsqme.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2heanvvlq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fmdsyhbf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2myupqwua.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hfwuship.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2wpqruwhx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bphaqfwa.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2cujxlqho.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2qkdxsibe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tpghcujn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2oteztdig.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2loxofusq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lvxjysaw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eotfpzcr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2tobobzku.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xrhxcijz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2wqjakdrp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lzjuxlzm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lbzjucej.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2apqmayvj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pxamhxvb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ftktyork.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ahinixbo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fqmyvvnk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ctdjyksg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gtfbsjtw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2cnpbdcyp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ycdjekhr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kxnhzsiu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2awjjchzq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gckmajup.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xvqkeodv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2obkuzzqz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hjfnbquv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ymqokdlg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qekiqcqg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2owrqvwjr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zecriqkk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xdqramui.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qmfvbzrc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyojctvs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lsynnpuo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fuprvnaw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewanvoac.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2mqzjzkqr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qpsydckg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hptrstpc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wxbcsqys.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hylsehxg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kzyeuifi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kpppracz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jrrkqjqg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tuvxmxcm.html


<!-- 参考信息 -->