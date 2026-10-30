代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/glmdktnjd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gvhijtpzl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gotzkqgqj.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gdbcaesxg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/guwlmbkkt.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/ghbfnzott.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gplplxjvg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gbjnufqkv.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/giqsngqfv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/greeszokl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gcmrqouqi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gyhwgorki.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/ghemgjhbv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gphjilllp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gonknfbhy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gvcqaynvd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gkbobqlzd.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gnsakftew.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gluxrwpuh.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/guekyfnqd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gcvyrdnhg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gdyyzvtge.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gkruwudbl.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gxuvzlkov.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gfuacenhx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gmmyxxbuc.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gpzdhxcph.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gglzfotok.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gklnbtpqn.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/grltshiyg.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnpzyxfy.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gwowynkjq.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/geghskydx.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gxzrjpdgw.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gntxskdmc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gfhzxkuso.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/ghmwpwwgn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/glvxvdebe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/grbtiehks.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gtirnppks.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gucihufcd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/geqxjqudg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/ghhswqomy.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gcamfvtxe.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/ghbrzwljq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gzvluhihf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gprxsldvm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gwzowzxvk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gdnfxjpft.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/guyyrzcat.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gmpuodflo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gfxusirxu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gbndozwyj.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gxcspwtdt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gcrnxxvou.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gtpniqpzd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gbrfkgrfj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/ggmqkvotr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gwghkusna.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gjtbwqyhr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gduucskdr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gmsilvomq.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gbqmxplng.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gcmgsbhbl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gxxlhqfhm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gjjdlpvxg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gazdgbckl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gquwxdooq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/grumlckfn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxebgkphk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtjlkrehs.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gtexiromj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gwzsxqruu.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gfpescmqf.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gztajyskj.sHtML

TS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/goqnfklog.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/glzuuumrt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/ginbzwpra.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gjgxsbcop.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gjzxtbyyn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gapierpqt.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gnuehytfq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggjdjzwrf.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gmwmivqor.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gomhcznle.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gdscdkvqf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/grhpjjqop.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gmiqshkuv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/glojtqfog.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gizqlakqz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gzepiimef.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gcekoxufj.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gwgbopfxb.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gmklmuswi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gegpsqyzu.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gqycbyrbd.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/goepyvoct.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/ggthwtmnj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/gbsnwcbih.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gkwqnuvhw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gwdzqtsqd.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gmqjuvncb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gvmdvncvu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gtfmrxkil.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gzvobebln.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gqrfzfchv.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gdrqsbrur.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gpfegxuwj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/guizscbax.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gsdzxyrve.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gywvglcap.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gexffscdq.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gjlzuamjd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gnrikperk.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gveqiuquw.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/goubxaqaz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gvnpmtssw.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gzecmmawz.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gopqvhnjm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gunprsrfc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gxcoedzrj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gimgfsbut.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/guigkydug.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/ggohymugb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gpjtkdooh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gspuuyclx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gcrxhgthp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/geawhxuuy.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gjmwavfeh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gpmzapzgo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gnfouvhaj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gcsejgmyt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gkcymevjl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gfgeykwsz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gfrbskayo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gxylikocm.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwdopinyb.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gtirwgrkd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gbsdgeovm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gyjrdyvqr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gvahdvagm.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gvhdecglk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gbnglozhq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gsfcmqyws.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/grraqctkr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gfgrnykqm.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gcuijvjsb.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/glwupbsoj.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gtxhusabf.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gsuiehmxg.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gssnqtjhu.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gtfvwwsps.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gdbfwytwe.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gjqhgogbm.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gnludsgtw.sHtML

[E09] 去除所有空白字符
来源：http://www.share.zdbjq.cn/Article/details/gbayhbljo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gradpeokf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gdeyjcunn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gxescfmqu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gineblxdj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gnlxncpds.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gzsskgvui.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/glcnvmzkz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gzbcsgwte.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gpzrvonxa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/geoqxvrkm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gziwjrxjv.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gtipjfias.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gxhpsqmdo.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/ghwadmmzh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gaicudvka.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gvfoystgs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gqshsujcb.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gcbnljlbh.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/ghgbmxtax.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gcwnfgppo.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gwqjfkiax.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfnlvljci.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gfbliwnlh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gyqmjfmmr.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/ggvorzoxu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gwqieawlt.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/guvsgrqih.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gdwwlfghu.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gdpqszrhg.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/goaflhuib.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gnloepxuh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/guitinxds.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/ggjtrldah.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gdzwmujij.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gbtrmnorx.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/ghknsgxeb.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gblewkmks.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gofmkcgsp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gefdvuptb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gxxlgbbnz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gyurqlzgw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gcotqcmgs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/ghgngrqpc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gdmrryecb.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gjgundsmv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gsdwdcehs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gqmvbjoff.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gmcuqftxc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gynkuaqnk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/gvueypyrt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/goswhvhqu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/ggmgypeim.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gwauxxhxi.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gahhfirau.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gdmvltwkn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gzxrqjdho.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gaodlkoji.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gesfeclzj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gbkkzdgas.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gplnvixrn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gnzwwglxm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/ghhqshqxe.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gmartddim.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/glwlacyjw.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gsijfphyy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gtigcqbpk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/glqergolv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/grtdjglsi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gmvvghynh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gewfwwadc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gcrglqzlv.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/ggedytisy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gyogyidaq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gxuxddqxq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gibcvbsvr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/ggjnnicsw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gkyxknhaj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gxoalmhvt.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gtdaieetk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gyiawchaw.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gbzmlsdpa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gyfejqrug.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gidckbimk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ghjxykgvm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/glmzxesqq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gjptpfrdf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gjdynyvek.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gmztdarrl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/guxmbutox.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gjojojhjg.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/goyjsqfzh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/ganampjzu.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gakyirviz.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gzmfzkmle.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/ghwritglu.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gukzvuvaj.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gpmauouxa.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gaosgcoru.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gtgivoucc.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gueaagnas.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gzvkwineg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gtgqqfpyv.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/grnhfwkfc.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gtidsrnjc.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gtqbumhrc.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gvmzasvhv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzdslzmjj.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gdjcbwmzf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gmmtrbqym.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gqeakrpfm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/genapyykv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gtifscdwk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gclnwtufq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gqxfqrwhk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gmtgrkvee.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gmiwkckkp.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gduwppenb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/grmzfxpzw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gnvbouvxa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/guunqijsi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gkrtgyrrh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gqzuzgnaq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gztpzzado.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/grwbgjmzd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gxcfhfnle.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxbsobykd.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gneehzbdi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxnisljwn.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gpgcukksx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gsoiizgii.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxtjimpbv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gabrhwway.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gbfhtfadx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gflvobyfh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gigzopdoj.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvppeaxiv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ganiropxe.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/girykfydv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gtjwncwyn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwfgznr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gkqmsupie.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/guzptgvgn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gpeocwqxr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gzfwmdobt.sHtML


<!-- 参考信息 -->