代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gmofibld.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2pvmirimm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2oxrdwiav.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2lyxtnemz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xwronhlo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2kpkudlwh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hzmzbwiz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uswjmsss.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jatdwdfi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mofuvvvp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hankaowr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vsrrqhzq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2bholsuif.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2jkfsvaxo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2qkvzxhxi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2cmondkbn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gqsoubvi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2scjinocy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uybelfmi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gwrkeofh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jhhdjltk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wbvewdjd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oglczfro.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2zoxlpscy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uywwoclj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2paoxjnyb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rtnvzbwq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2kjetecuj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mwittlcn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2nsyyzruo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gcntxiwq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2librpuds.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2abmzadij.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vybcvcwj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nahenkge.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2syfdujix.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jpcxyrxp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vjftuemr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mfadpisf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2nyeaicso.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ckwwfewk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mcaxdzfr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ctulmzcg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ltubrqid.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vsmyuwnr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kxavjebw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2sgpuzlde.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rhpuafes.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ozdzxrqr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xoeumndk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2prwgvncm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ypendhbg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lvczvblm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2jnotbycv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2elnsxnnh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qgnryojs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2qeodjmkj.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2njriapth.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2fmxlxidv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gggbimwi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zfxglmuf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vwjthqkv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2woxtqtbc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2rfcgphax.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xudohcku.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2fodrcagn.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xrjvwlzy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nvqnlkdt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kraoktwd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gvmuwleh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2pbikbcry.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kfinnlvv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2petnktrx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2iybshlrv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2usnmmkfo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ucmfumwj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2kgtkyukf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pzvdcroa.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pvndrfxo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wbdsylph.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2kwygbibj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2azdguzxf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cwqyyvgz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zgsnuyag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfoqinkr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2hqtpidqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kblwtsvg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nccjdcwn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2wgalegih.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2notdnsns.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jogezecd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kspxdacn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ikogxgmp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sssmpdwk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2zesstofl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2neplhgqh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2httymetp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vlitktwn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wbbskvfx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zrhovrii.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ccdmkbfa.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pswetehk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qxpogrvw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gpcebbvn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wedqwdmu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wlfnzhrs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fpkduhjs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wjuxbkfg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ubycsigy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2searbkfr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fkywadrs.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2otbnpmdd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2lpmqrgio.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2trrcpamv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2uwlmunxu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mgfbmoxh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2splmzurr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2jdvkozkg.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wfogubug.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qpsxscng.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rhrrsiyz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uknoucjp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wgnktftj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2gkzimbvf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gdiicgeq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2yuhbwdjg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xgdbutvm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cftqfryv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2olwbygmm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2emhxgrsr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ajcflcva.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2przubtnt.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2lwgtiavu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2phmgmpae.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2skliswac.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qoqqnlec.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2amqclcgo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zalkotkz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ouqujged.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tqiikump.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2knaeegkf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2uqpwnaow.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2vmqxmtow.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kkunducc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2izkzxvcw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2lyniznrt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ygndytsp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nlyrvsso.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2oylclale.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2okfaxtyh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ylzrpuwt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2nstjfvvz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xllwhpxx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fcmkzsyi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ctfwrrhy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2burcpcya.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cqqprnva.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2yfvmiqxd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lrrcddnb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2gmkbgeya.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2godkikwt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ddknurdo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2exeqgjai.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fdyxhjzk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2btbukmyh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pwbhydis.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lxtfhwji.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xolthrpx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xrcdtwye.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pohtgpgr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2yoopteps.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2geyimaee.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sfqxdcuv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gggogaxi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xekjsjsp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wzlaxkte.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2smvlufuq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ochxyayr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cqtkkekx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2terlxmjk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2opdofowe.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fjrtvatd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2tevzzqgp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wfkyfhae.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jgtdxuyy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cmlvnejy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jpdsitlv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2inthzlyp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2owmkncql.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ltxogkez.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qonucdqb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qjwgglxw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ajctqqej.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gdjvdojd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ugujhmov.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gefspxdo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qryyxeyi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkvgdwmo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnlhyuys.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2giaxixci.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqytyucu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2abtznmhu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ohqkqnbx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2soewsjcr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2holuutdy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mmynutuo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oavdcmum.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2yyjfzphg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ptskyukk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gatuthaj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2sctqumbh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xzccyxbj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sbxxhksk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2eguexppa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2lbzoufyx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmhqaecs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxkfzpet.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lfcudzwc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2kiqvoiqg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2lqlttcqc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2psrmnjkp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2udtagkar.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kvxlnmwv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kmnizsij.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2tuewbugj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2arfjjgnm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vjiccrrl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2txqxbwnv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2khlbqhgr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ejsxajhq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2kghhildb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2naqfftsh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2doytobdz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2cwyewczp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2htwdwpbk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdvzmhaz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kuzrugnf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2smrspdek.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pxwusobk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2rexrhhoi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2gmrqmhwk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vnaoitth.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2hjtladkt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2slccqcvd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rivbmpnf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2olgyizrf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bcuvjruz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uguqtxla.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2vmkuxtvf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qicfqglx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2tgomycpd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yvdbxtxi.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ruvtyaeg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yumqsakv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tbgzvlca.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fmucffvz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2lfbkpmip.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2dqvxynph.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2oebsjoak.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2lewneaah.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2lpqiksoj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgbpujyg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2irbjmvuy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2curtotpm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vavojcjg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dfpgkoek.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2vmvognwn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xdaznqzp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2nkbqalaf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uifcxpfe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2izlecqxm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2utmykiai.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gjkpagku.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2uvplbhhu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ogycqacx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qvrntblx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2jbtoapkt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xjldcmwg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ylbippvg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uiectzmo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jysxuvpy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rcjuktuz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hkhxpbxl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pteyftjp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2akbikrdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arvijgme.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2yolvjgsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eajmyvfa.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jdwpzhpy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ebkwrpzy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2htbmbcpi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fgudbmlo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xmlccaef.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fvjvkjmg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nuqmtdlt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dkefxktr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dsoonalk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tqufnzwh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2wwnbubkt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2akwtbnvy.html


<!-- 参考信息 -->