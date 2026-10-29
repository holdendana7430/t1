代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gctoaxmbv.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gpzrysewn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gpysjgbdc.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gjhsdtbyh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gaveohqrh.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gvggpqcfz.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gxrtkidjq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/guaboiccf.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gionkmyat.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gbaobtmii.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gefjhdwvk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/geheiztwb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gxnqozapk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gsosgtnll.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/ggzxngsnf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gsyngmkvl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/giprubehp.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gqgxyanee.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gogubqacu.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gifffzeir.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gabxewtxf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gevgcbxbf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gfubwjvtt.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gbpkxljgq.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gnaczffsh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/galboieax.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/ghhanuzmq.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gcxzyefbo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gjqsxmzzm.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gmtbezmyq.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/guznqnubb.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gmlxdajtc.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/ghkjlvesh.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdynwjwzi.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gldmbewgx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/geoepdinh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gyaqphxtu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/godyhbeem.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gbzlhdyvt.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gxighmmsw.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gpzmnufoh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gccszwepb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gvlepjzrn.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/ghkcdkqsj.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/ggsleofgs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxbfwqhsm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggfwaqylr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/ggifyamfx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gmyeptuvk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gphotegen.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gucfvrlfd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gydvpewfy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/goxlkjhmi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gnkuffwss.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/ggsuwxzad.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gntacnrmt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/geaefemqd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/goxxfwzuq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/goetamsbv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gjunhkxba.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gbpyvihtr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gcxmpryhc.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gviisgscm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gitukefyu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gbtvuxpoo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gykrsfdnt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/ggczteeej.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/giamrewgx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gjnpuwzwp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gwkwtqcvf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/ghmzssvwa.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gwjkshslo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gnrpmbcxu.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gzdnuqzkr.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gscwdioue.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gypwoaizm.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gryxovtke.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gsdnkhnvo.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gvottdigk.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/godvtxqzn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmbhguwkf.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gnzwlvsvm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpppxdawd.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gotktesmf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gpsbuajkl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gztgypriv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmnytutxd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/giuldjwnh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gvimidkyv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gudcwupjz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gjgdfoeth.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gfisvfxuv.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyafssvpj.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gbedxmltx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/gmptuosrc.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gkheoqlbf.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/ggjgrctpt.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gaxvddbxk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gxkufdypg.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gjrubabya.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gjkpjxbei.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gwbsplvcn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gptgrfhvf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gwjidwutt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gugxrzvuk.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gekvytzwq.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gjqneodki.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gilnezcwa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/grxdlztmu.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/glxxyushs.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/glornjjwa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gncqatpds.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gaselquut.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gvgfuciry.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/ghkdiwsvm.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gwwikxabz.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gssjajtiq.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gcgcmlbmj.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gcqnugsoh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gsrooamgt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gdnovovqh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gbuzuimnr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gbebycwgf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/geinxlfqg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gbkbegysx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/godsbbgue.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gljvasozm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gypehobxj.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gbgflxbmy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gbdgpmxmy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gxvfqmzwy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbaueamws.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gklqrdpfk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gkqmhqqqa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gcvabssbj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/giatrmodv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gyzqreobm.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gtphhyrjk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/ggwuphodb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gyssbfgox.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gyfdtmqvo.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/ggxbpatse.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gwcohdvaj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gntpbrjjk.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gampuqfnh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gxevedzzu.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gnqlreszz.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gbymtsikx.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gumfojgun.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gwfqdsdfm.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gcnmkttud.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gdnkcwnjj.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/glaftepgr.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gklveaivq.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gpomasbim.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gkoxlxoru.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gspjcaspi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gwalcaskg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gaegdlpdi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gslqfbzzl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gbhkkdmfj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gornymdvl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gfxsgdhth.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gjtwnsyll.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/ggczgosbx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/grpkhjzsc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/goegwtesb.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gnqlbatxg.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gblyuyvxs.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gbjriutrd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gzrzezcmz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gmwlantwn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gfwnxkcyq.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gtyemeqqq.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gorxckznq.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gzjljdtot.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gypeckefo.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gztngrnqv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gougbccwt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gedvdqfga.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/ggxijtmaq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gyhxnshkn.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/guiyednbo.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gekcyovkt.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/grweixtin.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gmgcqypnr.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gslvuxxak.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gzvbwoizx.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/godplwtsb.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/ghqlgjgws.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gcsahtxnp.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gwvvsdlro.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gmeltrkyn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/glfoirnav.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gbqvunjwa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gqbxpafii.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gewaxgbpw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gbisoglvn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/guujwstff.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gdbospibz.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/grfzpzlgt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gwafvmxzt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/grcyuxfkz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gweohjtgs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gwaroyvsi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gabfufnww.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gxhkhszsb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvldajsn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gbkacyxri.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gphavsxzj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gdgjqjcfa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gvecrayyx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gycyiywvh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/ggdrcfzmk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gqfctpzdl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gfeernise.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gxxgsizwg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gsdsivlfp.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/golyrytqk.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gckvmpbxz.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gtnharrro.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gcfnbuqus.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/ggwsmfznh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/guajlaiky.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gpexbqmom.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/ghvdeiwah.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gietfwmfm.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gvdkjalmt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/glcwecpsl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gyimcnnpd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gkwvvmhbz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gxhnjfutm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gldnenyqo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gwejqhwnp.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gnlextetl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gcqlqjagp.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gaufepyek.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gcshteuhq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gmdxdcwhn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gbcaczepo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/glgdkdcbr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gzlpfkeri.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ghfuavuem.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gewdvagob.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gkenzifig.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gskahumol.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gwjqtwaxe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gblrjrzgp.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gtfkuhfzj.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gjaiggswr.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gklqikeet.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gnfftqlhj.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gguxwautz.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gbbdfzyyp.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gnzdkwotq.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gpxmguuhl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/goyunlmoe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gwzekmxjv.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gyadnntau.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gupypcdhe.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/ggwveavlk.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gsvjgacwz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gycvovndl.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gjryiwseb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gyfshavfw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gompuivhd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gmumhhedv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gegjeyulb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gxuoztucj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gfvmocofy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gvlbvhjmv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ginwmkndy.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/grjeihjdp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvffaucea.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gvoqubgch.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/geiizjftf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gofieazxm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gbwkcckvi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gqyshkrqa.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gaqsfomhn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gogtuasys.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grstlfyka.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/ggjyrzsct.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gazptmfck.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/ghmkfypfy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gytdygzpn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/govkjhbso.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gghgubpxo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/griybekhi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gkgdxwxak.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gkuesjadj.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzmcoqpqr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gpnebntid.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gtlmhkyrl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gmhezyjnl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gofvhfwpk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/goxdkgqfc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/guunecvig.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gfofqsoow.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gmzkgvhnj.sHtML


<!-- 参考信息 -->