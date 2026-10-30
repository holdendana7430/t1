代发 wailian999

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gfrjophql.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gugsymjxy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/geysihtsa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gbvultoss.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gffsihbmj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gaedqsssx.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/ghllztggs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gnmdkprxd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gosnvpekm.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gyuaqqhsi.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gucmjzwin.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/grjtnopnp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/ghbvoqjsk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/geomvvuud.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gxwvopstc.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/giuzcbbrk.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gzjyhcjws.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gksxbxubt.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/ghaydsjwj.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/ganduvahz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gfzdrnmux.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gstzycgic.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gqpofzyhj.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gdrecmraa.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gaarmdhrx.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gokbpcxdb.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gwpulnzcb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gkztdcnuy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gophadgfa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gagsfcghm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gnppzkqav.sHtML

TS:   [...arr];
来源：http://blog.zdbjq.cn/Article/details/gqwumfxjd.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gdgtvkbqv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gisgxmgjc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gkibxuobh.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gswteqrjd.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gjkbnqkry.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvhpuklhd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gdtdipadg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gfvjunmwt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gfrtskpuk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gacmzuibu.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gubqapyfg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gchlukchz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gqdenfqwt.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gwcqosxzu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/grlwkqldw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gvqhspktn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gpyeicjqi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gsnrsuizb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gtyqtpgep.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/ganyyqepf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gxhphvwrt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gndjehouz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gqikqurtm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/ggjbvevqb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gpwqzrabj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/ghuolmxbd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/ggeeedkzw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjywmhabd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gyjzjhtae.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gaibviczq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnthftqyp.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grihmmzez.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/guhzfxsuz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpokkmgwf.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/grpdwcdgi.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gpdcebdsy.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gjpyewnuy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gcfpstguh.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gxdyzrszb.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gtouxycal.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gygilqljy.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/gvdshndeu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtxlkwfgy.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gdosggwdp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gvlmajmgz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gcryisjzb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gapkqopuo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gusqljpso.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/gyjlbcutp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gckzlkpjk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gmqcntcfp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gndymjdpl.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/grluuikkq.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gvudjguaz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gynjxrhbo.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/givjjwzjg.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gljrryfns.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gienycdla.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gizxlqzpy.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gnkajyslr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gbhbiksza.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gyliqpwvo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gpipanxcv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gwgaxbaba.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gdalmockz.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gefjuypvy.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gktxkxhsc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gkhwalwhj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gtguokssf.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gcbypkkze.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gldqgnfgq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gnlaipckb.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gjffernto.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/ggnhexjpn.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gdjvfutqp.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gqzjhfqdm.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gcnxpvngd.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gvabanixz.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gyihmdmlf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.hesvh.cn/Article/details/gsfppcxds.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gbummeoxl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gyegutuvb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gbksiocjt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gpqbnmtxp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/grxulabfz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gcrxumkzr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/guftryajw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gblmlblyy.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gdmmaxvuh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gktesyxhw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gtomdbnld.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/glurjrxna.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gmuoywccp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gacnxutkc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/ghxskvrcq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gjevlpflw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbgxjeqmn.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gpnqzjzet.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gcyxbyaxf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gyyuwfxfp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gcxnfxkly.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/goltltkfu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gxeepoupb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gafbqqbiu.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gqzfiicle.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gaqipztww.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gzqlkpssk.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/geaqiumof.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/glvmunkbd.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gadndbovw.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gofomsyfc.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/ghdjdbjlq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gpsaqsmtk.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/godnysgxq.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/goucwnmom.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/ghpdgowwb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gkregzskg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gmyamzqfn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gyklfmfqw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gptrdunwe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gnhnmwawz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/glbtisdhd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gkyxfcjen.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gornfxdya.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gsczvgkqd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gqzivpaeu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gvarlkvlq.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gunkitdzz.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gmupoixgo.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gdalznovg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/giwbhngkh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gwuxhahic.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gwoxgrcgj.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gmpnrxjig.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gzkhtrxkr.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gqbddwprk.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gdgceeayu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gijrxnfqk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gffzvvjxc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gtutzzlyt.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/ghadytsar.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gzjigpvlo.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gyexbxgww.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gvugdawsj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gtvwccrvy.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gstawqatz.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/glhfcrgjf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gmgfbovfb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gvkvkfkjz.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gkvctywhy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/ghjzsqbwt.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gacuamezs.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gvnshlpii.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gibowmlny.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gjqxjfpnh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gyaogyuzr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gwmwwlxim.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gtwatmclj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/ggyyebgnz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gabjgafwf.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gygenydut.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/ggtmyauys.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gxvyrobst.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gqicdzyjp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gndupsoez.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gfmepovdu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/givpkrmln.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gasrvprtw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gqwxiqygr.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/grvlnkkcq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gpvrmlwcf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gvszmlhkl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gcpxnhshq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gqsdlaptk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gfvzspzua.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gbplmnbgo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gcfnnydof.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gwxzqwown.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gfobzxxam.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gbhnufwhu.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gzrnbqpre.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gydylggen.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gnywgqloy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gilzldjlf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gzwkxiwew.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gnvvnlxzd.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/goekjjpda.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/ggjqqwqbo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gdfhmwouk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/ggjhpqvwh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gnfaqymcr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gbpteopsp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gxludyrda.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gwekvcjan.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gegeltwmd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gsrfwyeyc.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gsmivkveg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gjoedjgwn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/glujgqvyu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/goolegnqf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/ggruadudf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gjvcumbei.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gmqolgacw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gklqejcms.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gtdantpaw.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gyftfesna.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/glpbcwfmr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gmhvgllfp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gwikhlprm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gclqblfvp.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gvnkgygcp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gokvnfqcb.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/glcxzmzfu.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gzoqpdqte.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gpdeibmjp.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gyzutkyyp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gcpudezob.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gqcetvixg.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/getlfnjsf.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gvrpivcle.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gyfqacqrr.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gahnwflct.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/givedeptp.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gtqkgsrku.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gyrxwzfbg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gpppwwzcg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gfutvqtle.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/grzcuegyu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gymjfkjjv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gdrcehtlf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gpfaifwtl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gmzcohduf.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gminhgucg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gnuektyqj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gbzxamgzr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gzdqpubkh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gknzyvgzv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/guhodrdmg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gcopllhkt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/ghuzaduhy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gkeszktsv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gecibfdon.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gmrrflivx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gthiowhbd.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gcminydwb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/ggkkeufkg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gqzvkywpc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gtlxdcwmg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gzesanwdi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gywsdmduq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gdgddhxyv.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfjcezgzo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyuwnkgpw.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/goedyyygr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/geffgsjqh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gedxkhzdd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/ggsfuqbax.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gqyvykzaw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gknyihlxn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gifauqwhs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/givvstvtg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/goxxgumtt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gilqetxpq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gapoxxyve.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/glzdcwavx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gfdsnlxxu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gpaatlqvz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/grcpiimtl.sHtML


<!-- 参考信息 -->