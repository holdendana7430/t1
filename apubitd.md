代发 wailian999

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gwavomkdl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gwvbseckj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/grmtwnbeh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/ggkegiaug.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gigbjxyzz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gfyjiyqxi.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gvgvtrrep.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/ghzhpoawz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gmxceuqne.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gqitkuuyt.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjlqdrfyd.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gajhrxnln.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gydtsicnc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gvvbxyjbh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gbcbrvjgs.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gwxmpqibt.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gdqvdzxpo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/ggklshywk.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gdywetlzu.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gtvfkbheh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gwegjmdoy.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gyygcodjt.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gnvtmnfcp.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gmmvleioq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gzgqeiyqz.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/glwfsrjwh.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmawfxlod.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gdbvkoiuo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghiwhykgk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/glbapwdkd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gcfugvuxj.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gylkfuccw.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gwpqudbxn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gmdbhdkvs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/gpouzbrrx.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gwlnqfwmh.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gippjrcwu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gsheeepas.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gwoqmnghn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gfxyzczky.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/ginhsjzwb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/glytdxjah.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gtneacemh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gcbgygdrz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/goocldstg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gekqfkyva.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/ghjmqcrym.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gvvumjzna.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gduybgepm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gmmypberg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gzyrnwdns.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gfebeapap.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gyzlnwgzs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gkgtokxly.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/geepepxrq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gypjybfnd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gdwfvasdj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gwptciwvr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gfrbubiuu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gfdsamgip.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gzqzgjtfp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gcymbnnsf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gxiffxlkq.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gnklvovxx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gdvfrjjdf.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gzqytxarx.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gpjnmcjyx.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gcrtbxwyd.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gwqedzrgs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gbopspvhl.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gokqfjmjw.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gakobiwmc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnhyrfcco.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gwctqtaqd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmytsibqi.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gmscxelkb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gukettzgg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/glrgmgbbm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gwgoliwqt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gavjrqwjj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gsqeijcla.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/ggysyznlf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/grwmsjucg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gaglxfsgu.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/grmgdirks.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/germjeifg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gafgqrlip.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gbnmmlbfs.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/geuanjsjt.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gmbeimmxd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gguedlmyx.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gnhvtzfuw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gfbrmdwae.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gzbxzvjsv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gkrrwscef.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gyinhjwgy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gsisogwrk.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gaxkwcphc.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/grcqlkubh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gszpmfayg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gqxxjohfj.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gvlpzbcva.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gualfokjh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gaowttesm.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gedcaotag.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gvsahyoyd.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gfgtwmeyz.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gsgzckuxe.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gskidcxmx.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gphdimluh.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gytdvzbca.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/goslcalmr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/geopmeakz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gqzktmeey.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gvbsegucg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gtbseuxcd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gnzwgbwds.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gcgzzsuvd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gudwfffcw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gjbnqcomu.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gutcidsxm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhrzhlhq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gnorgstuw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gcmazkmxk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gxrqhxyva.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtarmtsts.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gejiqqalw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gqxkokfge.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gprgkosff.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gcvyijhcw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gyaexnihs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/gghtzxnxk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gpvoytjjk.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gwqchbmjr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/ghtlxykqc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/geogyhjyh.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gejbddtor.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/gytxrukbp.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gzmgedcqc.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gkrkbcaub.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gueyqnaap.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/grefttayf.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/ggodnxale.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gjbfqnxvj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gljeudzuy.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gszdbhbcj.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/ghdicpkxd.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gqkjcshgf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/ggxmdelwz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/ggvbvlfiv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gpdvtlkmv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gqhepwrxz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gsgsupuhv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gfxeazprb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gqlxorvav.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gvmskvxgf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gbgwxlikm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gicjghgul.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gduwekfol.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gfrjiedjv.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gqaymfxgw.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gldmogyvc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/getjxcwfq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gonqshkpu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gjziwjmvl.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghmfsnnuc.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/giocneuzi.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gywomiazq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdfdmtqdd.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/guqujwicn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gyuvhbfty.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gtrpcfpla.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gthqdqvmh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gbtjtqbln.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/grxthqbrc.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gfofnhfbq.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gxsvqdftx.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gwqcktjnz.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gyruvqzzs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/getgpzqfh.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gybjfwvoy.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gofnyizhp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gxnwyczmm.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/guherdhtq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gaxndgdrq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gmvwgseqj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gqvngogmd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gokampzfz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gqlhxyowl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gzmqwqdlz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gdlsglfsy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gkyfnnkbt.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gtwpntabn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/grbdzuivf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gomlhxlww.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gsfrsidjs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gjpjvwqvp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gijgoyrij.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gjxwdgusn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gmbdaapcv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gqfbtcaie.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/ggfwkgtji.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gemzksygb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gapbkeozy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gnxdqhwlq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gjxjvnbvn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gsjnmxokx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gqhzeoyvo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gaehaezdz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gzjeireie.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gqacpywmr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gffaoasrz.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/guruvpxpp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gddchlihg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gmqyoszwh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/ggbbvzjya.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gkagehdpr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gqbiigcop.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gdbndqled.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/ggcnotbfq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gvzzvpisk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gpysfqdzi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/guvjasowq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpznzlqun.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gdsxidmyn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gagwtedbm.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gcnwasbrs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gmlvicukq.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gxpslcxkw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gnfczlrqf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/grccxlvlv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/geebobniy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gkmzkbqkj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/girzygvbo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gmjlppwsa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/garvsihew.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gjnrybchw.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gbccedwlp.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/ggphgygws.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gqxmfmooj.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gbapebmjm.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gseqmzwnk.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gxbltkiuc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gwfkxadgt.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gfwicpkdo.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gjlpvwrvk.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gcakkkuct.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gqhuunmrh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/guxrevqdg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/giveokjdh.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gcjslcqlc.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gqnabkgza.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gnacqggci.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gnckvauio.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gtfqdglin.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gbwetahvt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gedocepje.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gnotjglhh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gzpwokews.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gpleaniku.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gqjoovdrh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gecrdqwth.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gmgffjsyc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/glueajetp.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gzwilkowq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gxragzsgm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gqxsksajz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gtfccgnoe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gujqleewf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gfrkgyoct.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gowhwxecg.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gkkchjhat.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gckwrvnue.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gturuandd.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/glkqayoup.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzeilbwgy.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gbqzxbsiy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gwttaijzi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpfigjmpi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gesgmdzak.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gaouzpoej.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gucbzmjbd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/ggeacxigp.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/glavuiypd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtuiegyos.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gklzviqnt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/geoiinhgd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/grtzzoiqo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/ggizktnjy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/govqxbqdw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gzxgvyqpq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gwirmmkkt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gbdpylfqr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gicajndid.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gihuddffm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/ggktmzxwd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gdfxgtstp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gddeclhtd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gjcvdvajw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/ghqwnyxgv.sHtML


<!-- 参考信息 -->