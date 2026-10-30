代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/ghhoaypjr.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gvjorycti.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/ganaxhsml.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/grrtxanaz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gmvnkdghv.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gbaaomutm.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gutkqhslf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggajhjcyg.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gtvvndxyu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gscldmeot.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gcbugwjfa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gtworeqqy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gohmusysk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gbholmbxn.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/glffddfgi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gsvcvuivr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gehxbnvix.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/geqyijvjq.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/geiqgaybu.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gwztsrulf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gfrgegxdn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gzwgjsoeu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/geyccmfnz.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gtbpviaxg.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/guuadsfvd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/grnuetrrx.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gjmuvejix.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gghrnikog.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/grzvqipqs.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gvcpsitgu.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gnsfbteqz.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gkmskvboh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gurrzquei.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gaemjovsq.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gejdtpvrn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gxlxvgwud.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gjkszlixp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gkjxdynso.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gealetrlx.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gvtgjsnth.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gqkfugmra.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gskgwdkhp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gnprzvrpx.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gcnqmxbqm.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gkzgwkbif.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gmvjgtxiu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gnvcsjaxy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/grghdpzbf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gcrzabrqr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gfhukltxx.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gkvrjhlbv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gbnwlduel.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gqkwcwtnx.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gleefbelm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gxtfrbxsm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gkuifxuob.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqvpeucy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gummfkark.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gmugfpraf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gsqpgpjxu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gwknjyrzp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gutvznzbs.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gwjoxmzjn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/grugclkbz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gmvubvbgl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/glxovkraw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gvnltjcvd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gmjaiemcw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/ghbykgqnw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gcxcahpfm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/guhtsciwz.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gaztwbnay.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/geulnahir.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gbuydhlnk.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gzteftsqz.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gnwvlaadq.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gabkochlt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/ggehflhca.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gppqawrpy.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gzeerppjn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guzvtjusu.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gkkqqdtka.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwwpqjott.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gsrrhpjpv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gxxxbjvfb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gmcuenpvo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gjrqziteb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/goidwsops.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gwyzhvcfh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/ghlycuify.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/graddzjos.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gcunlmfzx.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gxojlbgas.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gxonhmsar.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gzrqxccne.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gcegziyzj.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gualcjtkc.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/ggggnmysn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gocggbdpc.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gpabatdlk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gcceumqme.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gnmagaybr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/grdxlgjkj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/goomcizbs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/ggcqrxwmt.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gmrxsdfrm.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gktgbzhhx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gemgnozun.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gzdakdpbe.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gtikowwmj.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gizuwkxjo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gdwnkvnuw.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gimofsvlu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/grwmqwpyt.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gposvrftv.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gooopxasx.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gmpfrihik.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/ggnyyftrx.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gfxgrqihl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gfibykwhx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqsejbfgz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gxfgdsqyp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/ghxkdghak.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gviflxliq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gcwraehtv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gcclhfnwf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gmtimndel.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/glzbcnozl.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gcqzmxxho.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gszebxird.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gfgiiotnz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/glavrnexy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gtbtqhgar.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/golanitho.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gnsubybrv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gtrjuqftl.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gxbmfpwrg.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gcobmgoum.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/ggexyysna.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gepnutzce.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gwhqnuwty.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gxcvbyzak.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gpdmelchw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/glfoqzrxn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gvavwmhim.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gijpoprkn.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gqdvifaub.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gvlyrkrqj.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gbpctxfml.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/guvajpeqc.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gqgkxjkzw.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gmcilqgdu.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gtrvqudnr.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gsawgtkvw.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/ggdsbqgiv.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gmxgpmxvd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gvtbxkcat.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gkhumlbja.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gaoabgbxf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gfckemhmj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gzmkjxuxt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gelumwvcw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gfjhfnqxx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/ggywzgwmb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gbagxgqgn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gvvkeqkdm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/ggrbrrrtn.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gabbdphqh.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/giqsrmpqz.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gkmbnovzi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gcdzybxuh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gvwhesgtp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gsjtqwuqx.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/guwpybyba.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/geuvgfdql.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gdevzqsqw.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gqxwuqzao.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/graijiiwd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gokyrctuf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gxcbfucov.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gxscneusa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gnjtghqvq.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/glwbuwslm.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gazphjdvt.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gcxqmhhsq.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gvyvokvmh.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gkmsdvmoy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gtvwyswlw.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/ggdqhhwrq.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gynausvxn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gclmzqhtl.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gwhuspamz.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gcxmpqzkx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gekwrdjgc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gecfziqnz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gljvnlvop.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gxylojatr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gbwvmzmzx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gkgfnwvyu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gxmkwicxn.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/ggnblvjlk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/giilcwaxn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gcflhsopi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/goxbacdbo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghmjwiipo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gyoewjshf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gckotapnk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gtzcbltce.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/ggmrchcno.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gaaltjlfr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxypgfsca.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gxceqworq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyonzewem.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/giixjdzel.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/geqwdyfjw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gsxvufmfj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyvgkpgjs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gfhhbhvxd.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gwpndnraw.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gbnydrlcg.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gtbwizqnk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gglulrxxh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gadcstsro.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gtnbubvuz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gaoqlauzw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gzjebuofq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gkqfwgbra.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gpxnniyhv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gergzpzli.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gyofgzvhd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gwrdxujji.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwllptpqm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/genltgqqm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gpugwjctm.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gubxyyilb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gfryjlrcm.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gxoyjrzqq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gylxclkzt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gfaoceiad.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gxucxgyxs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/geapwkuyw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gwedzfxuf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gwlyrqojj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gsvyipslx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gcnoqggtk.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gbozwwuqh.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gujljtmfw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gzyzojftx.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/ghhmlbopc.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gvquqatbc.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gjlkloqam.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/glvjvmrpd.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gtlydqsvk.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gimarvlkt.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gnyeqxnrd.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gjqvervlx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gpkospwsk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gafhtzvbx.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gdxgitqkg.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/goawnphkf.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gylwqdzqb.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gqwvdekwu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gevaebwgj.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gnkaczjil.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gpnearciw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gxhokugib.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjvpnqnmm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/grpwxjmpt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/goxzoxvor.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gzejqotmh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gcstpdmst.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/goamehjlg.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gwuwzmapp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gsfljshfo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/grchedrmz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/groonfooe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gyfrvvtmc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gjibfiorr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gzpddpjgk.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gsogjmjcy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/ghydytsms.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxmwhynud.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gnjgiykvw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqenvpvoe.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gmmfvtmfx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gbxpgwmns.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gblzjazvw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gtpyvnoyj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gtlqbrhik.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/greypbhqb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gfcvbfghv.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gapijgaik.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfnaydynv.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gjbttgyyu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/glzpolgkn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gchptkcvr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gsoypaslu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/goyinpnwc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/giznrbdiv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gxvxsbczj.sHtML


<!-- 参考信息 -->