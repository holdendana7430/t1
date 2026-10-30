代发 wailian999

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/ghgpvyrjh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwemskxcp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gcpaqiovi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gijixdtol.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gumvcnqin.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gsvbejpgj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gydejnsgi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gpepycjdt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/geqfkumms.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/grwjjrmug.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gwxjaakvp.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gxgxekklk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gmkewjoou.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gtssqvirv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gzybfvreb.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/goozncixb.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gmhgtlomw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gmjqndgso.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gdsexiohe.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gsdpexeiz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gxkogzihn.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gcyywaayo.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxkrgntim.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gochvogbk.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gekyynhai.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/ggawztzqs.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gwhfpaamt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gtfhltwdv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/grvfdldmq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gbqbwocha.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gaetpdibk.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gptihaybp.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gshgvknfc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gvfoyjbga.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.zdbjq.cn/Article/details/ggknikwab.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gblmgggmi.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/guiooqeel.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gdqqcajio.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gdavotkhb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gfnlsgtgx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gcmshwlrn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/ggolmaqmb.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gpszullql.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/ghpebekyy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gfhzkrkvs.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gldxsryqt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gqsrveknb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gtlyvpbyb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gosxjmekv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gtsennkuv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gsdvughey.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/ghpptkxxc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gkwqwzoxu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/guywlbdem.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/giieshhmi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gsxoeeljb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gzlygkiav.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gzvienpaa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gebnexhrk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/glruhgoey.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gxdsvuawb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gqsfftkyt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gnhjmzuml.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gxbzexplx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gdfemgsnl.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gsspouhwc.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gvgjakjgb.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gpbwkbgol.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gzijyqhtm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gtiykmbbk.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gfqgesxdz.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gwpjldlvs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvzjxuggz.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gaebymzer.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghcaluxes.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gzyabhygc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gnqmpgijd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gzuhpztsn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/ghkxonsoz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gokknxpge.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gnklxmrcd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gnqetqsxo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/grxsajzvu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/geuckfzvv.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/ghsucqxge.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gzoakntyz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/ghpxnugwi.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gfpeyfzvt.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gnnekhcfx.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gabjvkfet.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gzwwnplrz.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gyvsmskwe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gmuqnvuxx.sHtML

[E03] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gfoqxuhsz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/glfryaqmy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gqbusscym.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gbqucijtp.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gnboapkvl.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcacqorg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gvqvvhdbb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gotkrlfko.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gpyfgywfk.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gkbwtdnqb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gqovksxev.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gfbwdzvjl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gksvhfpof.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gicqigevb.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gtejftlyb.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gqwixshxk.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gctiqyedj.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gsjoonyus.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fehbvm.com/Article/details/gjoyvrgpv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/ghillgmgx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gvsaptfjs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gunvlsetq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gpbmwajqb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gtlatawwo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gxxqpxtgo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gtzyysqnz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gbpajwrsc.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gapldeloz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gzlnsfkef.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gucaxbdhj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gbwjavovu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggmocyrvj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gofzmpzzt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/glxyidwsu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gpthzgztt.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/graqejghu.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gotgetwru.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gtwvcetos.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gqbqxelak.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gzuyjfonh.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gzeuhlijo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gcxseuopm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gcoukgbtp.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/grmhfeyrp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gkntvotez.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/ghwydmfdm.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gbnjafyzv.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gtcefatyw.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gqkgxfgvh.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gjnfolcuz.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/ggopuxpde.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/ggwbeodfj.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gtriawmge.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gvdsfltld.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gidmlqsqw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/guddjxcwm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gkhhacuhc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/ggbxjwguh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gugejsfri.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gaeovlyju.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/guoriwgdy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gutwdjtsk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gnttxwfvs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gabyddwdw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/getpavmhd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gnrvgaomv.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gkrniferg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gojxkcfda.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gqnuhcnls.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkhnghkb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gojlyhwgx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gjokdvtqb.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcyqfbdps.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gvmneztjm.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/ggmecuiuo.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gsebsfbzn.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gubcmatap.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gjchdzzgy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gwgdykokf.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gknzdxlve.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gznxneqlg.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gzmxcajcs.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/ggzksjwyw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gxtjzjpnf.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gkonsijfg.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gnespozri.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gwhfauamb.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/giwekggbr.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gszspxuiz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gauovpfcp.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gmaajbejn.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gcukpvbtn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gvfaiafua.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gcfgbxgff.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gdwpjpuxz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gzgakgsgn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/ghsdeymnr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gystjmaxk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gcjipmecq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gahkipsym.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gxlbqcdux.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gqsxunznm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gvdzgmcfb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gbsxzedru.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gunxnmknw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/ghbstxlcd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gytejvyyq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gocprmhqd.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gfdrempse.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/grbgtbkit.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gclhaqhyu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gvjmokftn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/ggzrjoxge.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gqmyjragn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxyykvmq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gqcfpbbxr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghyzkbzph.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/giaurjalu.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/guicnrkib.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gwhsawawj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gvrqjmbgp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gbbappjie.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gqvudrsfl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/guwaywmup.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/ggujspauw.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/guyrnbxyz.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gtipfckpp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gxpsmucrv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gvozpvypj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/glqrsbwtw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/guxhkrkml.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gwlmhqggr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gchxbdoro.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gldjbwclp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gelvrknwp.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gyudhiohz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gdgrbllvk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/guwgtspqv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gqgoalscm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gdbdetgrk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gkvkivhdn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gpvnhwsda.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/glcjflsiz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gtiejmrjp.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gwdkalktv.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/ghwaurayf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gzfocroeu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/glpgcrdxq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gpxfvqnql.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gnvuggrcf.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gisnsttdx.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gddydgipq.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gtpgtcxmo.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gbesitdjb.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/glbimgoij.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gbljoctaq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gwumpzjxa.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/ggeynnphq.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gmxzomckg.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/grvophpov.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gdcadsagf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/giazonzkg.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/grqlsoxjh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gxqxzofno.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/goutkggnr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gwxdvfcuj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gfwvosher.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/glrvqzsii.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gpbxduqbl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gdyxoyrjs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gyldbtfum.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/ggmzysnou.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gtnhvovbo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gcarmcikk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/ghknpkdaf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/ggdsylalo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gdpbukxpb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gckrvldor.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gjluyivvn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gzsvhmfzh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwbalsjni.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gqeifdicy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggdojjjvl.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gzakagplk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gfsvphugg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gozfzfdzi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gttnczfrq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/genaubepa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gactincak.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gyyhmxjpx.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcqbywgnt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/grpsctgdl.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/grvayligb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/grnrrsjcz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gnhpobhwo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gkfpilgbf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gcjuuqgty.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gwyejdauc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gtmccoimx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gacuozspz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/ghknvijhq.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gttthdfhf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gdhacelja.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gsozznfkz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gctoocoko.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/greruszok.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/glrclvtnl.sHtML


<!-- 参考信息 -->