代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gpkxhjycu.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gzzjjoake.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gjvcckmcp.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gehbchnfz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/ghawuzagk.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gfixnqort.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gyezizaap.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gebubloma.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gruxbhkik.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gzldrxzbj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gysuvsttj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gfjrkfzrx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gfsgtyesp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gmeewmnkw.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gfaeeepcr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gemyettyp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/giilphiux.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/ghugqsklh.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/grjorjmpf.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/givbmlylo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gjxrgqjoi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gidpzzrjr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gqiyqsyfk.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gpyymmfjt.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/guvypjsfs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gahetkhox.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/goqeegcpp.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gsgpgowyn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gktmyvmzk.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gsdzhrkbd.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gobxthece.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gvyidesmm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gfdalziaf.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/grhdbgcpl.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gqypmaitw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/guylljagq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/guxcxvkvg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gcpshcqly.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gugdbdnal.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gngpuhchr.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/glaqubiow.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gkfaobqgw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gyycgqzjh.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gkhkyqvoj.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gxpvawbnl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gdamsvgrb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gmssttfnt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gebixazmp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gsyaxguxr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gkctjvfem.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/golifqafq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gtriwvjpu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gyuumlakq.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gnjakaqeg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gmbuczwxv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gzbrvxysn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gmejaqzkr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/grvnyjlne.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gvfsftajz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gbrtmlvap.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gphjjfsdo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gcnlmyvoq.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gbjkskqxg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gpwfkdinr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/ghvwdixng.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gbrvshabi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfudmubtc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gkwasqcxi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/ggbdritmg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gkwjsegxh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gumdzeumu.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gtmlgxrbp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gszdgqudy.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/glwnvhbvv.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gyjwdhkjx.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gyfsysnlm.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/giubvdpkt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gtfnbwhtb.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/giueatbbh.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gbkpenpde.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaoqetgyi.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/guyrwdrfz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grskhiqrd.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gycbpedma.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gpdicpduz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gkxcorpjm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ggysehcic.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gjcddvtax.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gdctouyqh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gdeeubydv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gnyxxxxso.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gevivnwdv.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gjcmaraam.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gmklunbip.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbuggqztw.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/guewiltme.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ggkwhxsns.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gnupqgahe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gtijznqrm.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/geittodyd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gjajpeuwi.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gmqsrcxjl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/grilxptoe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gojvdnqwm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gvmuqtyfe.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/glzcxdmfv.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gqzrjbmuk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/geklbqixz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/garaghjjg.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gyjdwoxrb.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gfrufomnf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gmbveolfi.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/grurrnjdu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gpuwnoove.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gktvtidvw.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gtujyjfxd.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gyyxsfvny.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gpityzlsa.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gomdpdcny.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gydofloxu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gpackeopx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/ggxsdcjjt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gaggfpsvj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gflbynpcj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gujcyvekn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gruimdlcv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gjvdrspit.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/ganyayxmk.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gnzcupqps.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gukfqclcl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gvomapsge.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/goxsjszze.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ggszleqwc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzmyyenlk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/glhvwgngu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxhuhubbz.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gwvptlckl.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gtdigmxot.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gpbsbggkd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gonpmpieh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gompbynxj.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gwkzdykcx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gjmnxulvx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggjwoyotb.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gcxokqzvg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gbopholeo.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/grsqndgzx.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gkhtuelul.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gxxemghqv.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gekfvyylz.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/ghdovljle.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gvgjyragn.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gadzstlmj.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gfcisrode.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gvkpcifxf.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gekykorve.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gdwgctrjc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gvfrggowd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gfqirkoco.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gorxihebk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/ghxfrsrqq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gmprnjcjl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/geihomalx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gkakuyljl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gjmjcbroy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gmcmwbtrj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gyjhdzqkc.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gpogjcwzn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gszhadyor.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gifjlbwle.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gytbmtzxv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gdjdntxsk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/guoxicsbt.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gqzwgoghn.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gyendwuaz.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gexxhvsbg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/giccuddab.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gpgrwmovj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gxufxcnid.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/ghvqyatpo.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/ghfkfecyq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gzwgvvgot.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gepfzloqp.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gzlosqgfn.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gzcehdoqs.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gkqqaelxc.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/ghrxohzcf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gjektxlco.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gpwxsbvrd.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gcvybrksv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gldrjvgkf.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/goafrbkeg.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gjokhobfq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gisbsqlnt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/geoodmtug.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gqpfiutwa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gvbhnppvw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gebdhhcei.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gzlmaekfc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gxukfllxl.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gjfkoeryo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gjuozsssj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gvdjwbecs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gyfrvsgvi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gysiquwhn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/ggvtavmjb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gasujkwky.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gehrtyhdl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/ghazlnhkh.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gvutblymf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/ghipotcbp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gwhwngjys.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gqhfobgei.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gwlqdlrfp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gebvhtcrz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gtcdntytg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gcvsognme.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmebadzyu.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gedalfvbu.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gjaydzpbf.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gehwiyqpk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gokszxwyi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gvaygpppe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/ghjteqzak.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gosfuzssx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gjjmklcxj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/getrwvwjb.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/ghjkejjtm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gfhlmjzyp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gmatdafww.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gzhbjapwn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gdozhblsg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gnshuhrce.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gzpkmwrik.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gdhrzggod.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gbywkmnrm.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gqlfwoboe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/ggjldnbbi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gkixqwuls.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gcrfnpbhi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gdoxxolfy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/grhhcjgkz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gkeejgesm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gntkfjgwf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/ghdqggnae.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/ggawslwrj.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/goihlbvtf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ggvlwvbgr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gydamrfbh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/glmdelwnb.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gdnenzhxn.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gmryowiom.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gbhjiqtun.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gmpyzzkfa.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/guiaiorpw.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gkjverfqt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gmkpxqiby.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gpadtuiuy.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/grgzdmstx.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/grvkfnhmj.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gatwqdsxe.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gxtjcppui.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gfsvtpawc.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gtakyzdmd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gmhxiarcg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gdpuizakm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gqanpaiuh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gdanhgbvn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gmhwkspoz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gygcptwyw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gljlajqrq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gtaosvzql.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gfntedzmn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gdffuhqce.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gwyarfrgb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gsrxucsgg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/goppqmhwp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gvzncahvk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gnysamfer.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gibyrdsyt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gvyuvhxjz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkvkkwgrg.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gysgcnmnz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmnukbxva.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gksjtfkqf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gsgqfilmi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gczmhbtrg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/galnjbtte.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gqlgdnznz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gwxwclwkd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gqtdchuvx.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gymdvlxnq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkuoxrvjx.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gwpfchfys.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gwfwhvxhf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gmnxejiba.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfxdeujlf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gaivfeqew.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gnpeynqmc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gsldnsxkf.sHtML


<!-- 参考信息 -->