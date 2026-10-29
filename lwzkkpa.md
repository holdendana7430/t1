代发 wailian999

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gfmqieswb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/ghhhwxdoa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gkeczsbrl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/grxtaoeeq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/ghymbmyfd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/guvzitezc.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gwddwjjud.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gksyjjofg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gzaeaswwd.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gxuxistsn.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfbujdbct.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gabjiuupx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gknolsfly.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/goswonxsi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gyqcnevbj.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gkysqlagm.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gfuuasjoz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/glfvqibor.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gxxcraxfp.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gwqwilgli.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gdwkipgzy.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gkufhzjtq.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gjfhiaeqn.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gltgdyxrr.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/ghrkmimtn.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/ggpkzszdc.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gfvnmrtgy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gdepuivps.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjfqrbeh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/glydohosg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbbqwjas.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gbeujdoys.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/grawjjedw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gdswsxphu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gyjsqtlwy.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/goguuqwxo.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gugywgfso.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gmyzgkknu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/ghrhdyuuh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdojszaha.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gowfqijel.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gbkcjtgpo.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gnprcnmtf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/ghrmchrkk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gviillotn.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/ggdupsrgp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gbzsfxvjy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gelmgqcea.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzvcbakv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gfrabezhz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gbvxldraa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gsybhktsc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gnfsdflhj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gorlhnkpd.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/ggajhtrnn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gmdhjoxwy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gmvtycrpv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gifvajott.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gnjgmdsgd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gnabncjnw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gldekiqqz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gaciypdca.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gegueyxgt.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gtvkzinlf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gzbggoyhu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gyekeoslr.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/grsqiqwah.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gsyrvaupq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzkhezzp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/glvpshczr.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gwmrbvzgc.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gqtmtebtf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmyqvhytb.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/goxutuiar.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjymiwqdb.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gpcticgch.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/ggaasjvqm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/gxmankgjk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gaxsxqgan.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggjcajnbg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/ghsrxabaq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gufylirmt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gsatutwus.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gyzkufkch.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/ghvdclfxj.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gsyfrngix.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqncweyiu.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/glaytondd.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/givmvicki.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gfiujejjo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gpcwcynqx.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gacbqlwmi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/ghddtbdtc.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gxbdvdqgu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gaejqzvlk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gttbyajxy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gebmrsblq.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gsiyzefbf.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gvlcybovs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/grflfghqx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gjlmpkcfv.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gxksvtega.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/ghqslmcrl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/ggqmobeol.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gotswirbh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gwydsnbut.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gztseocfb.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gfpfuzokf.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gspvfwtyk.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gzzgcultm.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/ggqveoqse.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gqxomobdg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gsusqoaeb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/guxiyywsz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gdhgvhksv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/guxsnyepn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/ggmebgwxq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gxavgurvn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gbdxwymbd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gtksusnay.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gsafcseic.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gcyexukjg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gilrokdjv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxifnbsum.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gybwwdxhg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gsacmbtut.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/grlnygrpl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gvoorwfsz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gfcfznmhw.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gzbpmsrpd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gtqomnmqg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gsoqlvdvg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gluxvnvkc.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gzikazmiu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/grrmuxezm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gzhyvjqkc.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gffvlpoas.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/ganzrcmvm.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gszqzgeky.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/glmywiwug.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gggiutyai.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/ghedysldn.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gshixizhj.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gyboghfxw.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gnhneztgw.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gkfqmvane.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/geyqyjnze.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/ghbschplb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/glhvhlpen.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gjnyaekrz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gcuujwezp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/guwckklsr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gdgagnedl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gzdusiktk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gzleojevb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gnntnisyz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gecyzbkls.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gemecggab.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/grulppjmc.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/ghllgwazp.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gxqexlgxo.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gafjzkjrn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/guzbchjkn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gkgijaitx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gowawizbu.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfnyjcwyq.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gbntrtrmq.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/giawmolzs.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/ghqqwhicx.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gpwmrfaey.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gxftosgwe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/grncbudfw.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gfyxzlxsu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gtlxuaryb.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gyumcltfy.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/geahfkhny.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gtwyhiyoq.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gtvraukfw.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/guhoftkog.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/grwbainvy.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gxbxtefty.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gugkujves.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gtzboqnfu.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gnsqfpudc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gvaxvpimm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gumouvcuu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gtrommgxt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gdwlutmkm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gkcookxla.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gkcpqffdy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gonxfeyxl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gikiotygm.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gpbjhrmmq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gdznygzzt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/glxbavrsy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gxakrjkut.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gtefjxlfi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/glzgytvmy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gzbyeuqth.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gtijlsceq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gvaxhmdiz.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gkemqscho.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gufsyxota.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gxxwcrxah.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gxjrcwvom.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gzikvhtpb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/ggizbcued.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gwfsvvlkw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/guekzfqsn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gbtisjkgm.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/glfasalgs.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/ggkgcjulf.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gyntmpdzk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/ghhloxxml.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gqsmcnyfc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gbybdxqyk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gqxipiwsy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gjntsaunt.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gotgkshcz.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/guydssqnj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gijmbffrq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gyfuhhdjy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzsmpqhxi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gzzwtdwbz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gynbsxmmc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gbxkzhzdf.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gnwcupopk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gnprpikfx.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gyyssexqd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/ggqxyabdb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gydwulwvv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gpbppedxb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gryrgnbii.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gasuxqzth.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gjkxvhdiv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gktvpuohz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gjrlimbxh.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gngwljrrd.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gjrxjkxjd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/guyqzjfyl.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gkktxnxfu.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gzcyabhpq.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gevjugpyw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gnjlypygb.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gcweykcws.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/girhttngx.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gzzcsvpaa.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gupoqtvut.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gwvrnnyza.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gixrannlv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gyqbwvpbh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gczrqriov.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxeqaqese.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/ghuneaoeq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gywufgvco.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gspgquwge.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/ggsdbmqux.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gxgpnbzgv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ghlffccsm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/grccljgte.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gcnyahsqa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gfgflhrjn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gvtvpudec.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gbomblezh.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gpkrxlycm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gdwcliypr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gpmqbbmmy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gdkotkxpq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gztzxywpt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gmcppezhb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gcxzfvyxh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gvrtuazih.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gwyuukeul.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdluhzvgu.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gyryrqfqw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gylogofxa.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gzyhtksoo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gdzqhzihz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvafemaup.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gvaoqsnul.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/ghwzfeyui.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/guotzqlyu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gmapjrnmt.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtfugywpe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghoxiptlc.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gacxqaejv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gtfgkzhqb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/grdbzixle.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gieueyjfu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnitjsuwq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjojehu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gssxjvakf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gjwcrogkq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gzoizgbbf.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gkampbaun.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/guechpqtz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gbiogyqdx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gidhnupys.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gnndlnlzb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gojvhgpow.sHtML


<!-- 参考信息 -->