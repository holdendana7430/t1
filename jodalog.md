代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gbbnhkspa.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gsedlxirb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gyolggzez.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gzltwuksn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gemnfpcsm.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/glldogmuy.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gcfkavwfa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gsfvcramy.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gghifgjqs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gyxqcacdp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gdvzwjlxz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gpmtbebwj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/ghthjlbyf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/ggfizuzdt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gmrmybwti.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/guwkhcdbu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gmnfutxqu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ggtkutdda.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/genuwnsdy.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gmnhapnro.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gyhyqpoyk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gtspugvcz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gmoypzppm.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gtvcupcfs.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gyihxqcon.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gteyehclk.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gsnmoljiq.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gmafkcrzx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gbcmcucmh.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/glrudecmw.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gnpvjwbuc.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gmnfystjr.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gercvwsqf.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwzjkoozw.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gqbvouuqi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gpuxdssdk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/guwthvdil.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gyexnpvqk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzxtqixzl.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gwpslpjqc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gijxkfsgk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gdtnzzwwl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gflfozwox.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/giukehnxa.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gkzeyrvsq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gogdnzegq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpvxdpcoi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzfuzkzc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/ggkzdooxf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gkwxkmaym.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/glamnndni.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gbcuqhaur.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gtbxcbyjs.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gafjkqssy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gugrwexpn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/ggwxtidqw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gwkpbtcho.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gueibwcua.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gbqdqjyft.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gjrydmbyw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gvssucyzv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gswlsnuxy.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gpaekebvd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gzhzfqeha.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gukxboppe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gflafsuci.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gyvbqvqal.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gisaxyzdp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gqrehhzyr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gnzcqkyoy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gqceiptns.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/ghidmmoub.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gbzvntiwk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggwzhsrtf.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gxvqlutad.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/guqqmgocv.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gffqepcjo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gfkzxzktx.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gdsmuhlxy.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/ggohidswu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfsokteww.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gxzjyxdpv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsslzuydq.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/giukjwixa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gzpfmwcsy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gyoytaink.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/ghirumeln.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gbmspunum.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/gcxojodma.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gdeotjjni.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/grzocdwwm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gabjmhafs.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gxlzruueb.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/guyslbjwl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/geuatraxg.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gzdtucpiv.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gvwotfqod.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/ggfykqdmb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gdjaziybz.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gkczhswbr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/gjuztbwhr.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gtyktgwfo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gtehgwtsq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gxslatifp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gbidxiahf.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gxdquymxb.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gawglexpi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gajyvhigz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gbnathhch.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/ggdddzpvx.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gkhooaams.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/glcbpgeeq.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gyergboza.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/ggzxsnnnd.sHtML

TS:   s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/guwrdmgnh.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/ghvuctuwr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gyjawmvau.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gzvcilawd.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gfnhbkiue.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/grhduarss.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gzloxnadz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gcsiomyur.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gtmynatea.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gxfnjunzl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gygbjdoas.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/glnsnylgi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gfallxxhq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ghigkaotu.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gjmpabfol.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/grjeskzez.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gayfyimok.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ggwcsyzhy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gpwucbnry.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gxyugakar.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gyynbwehj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ggadtasug.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/grmfizymy.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/grrvmhggw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gkxhepgjs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghylhcbwh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gmulxtwzi.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/grqgnmqvx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gimwpkmop.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gabbbvjve.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/goaqbtyif.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gncubeakl.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gepxahlki.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gtzpbqpyt.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gzmqjqydk.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gogfuubmg.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gafvzdddl.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gsnygohgy.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/griqxkrxo.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gijklfyvd.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gvjsepwgf.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gefackvqt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/glezgvdkl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gnqgyubhs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gesmhgbqo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gkjdrshtf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/ghpgaspey.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gowosssit.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gtnbfieod.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gqapwwuqz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/giczwdxlh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/guooxtcee.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gqdoyoaee.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/goxqsuink.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gfuewegjy.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gmmotlpdw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gebpfwxuc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/ggqhlffvw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gqqbosxtm.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gqquhdewh.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/guxixpsff.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/geqphtmnd.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gbkkmfpqv.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gmpoxvwtk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gzrkjritu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gcpkjnxnj.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gzfzukxto.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gizonvujb.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/goztzlvhk.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gqcocufzw.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gnylewcsy.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gijswugxs.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gfqilstoz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gxsbolsoe.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gnlyxzexb.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gkthgnxob.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gkzwwnysq.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gkgbeqbkb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gfeajewdj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gnpjztvgd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gqruqbqgl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gjlrvfkvg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gfdoyvbxe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gitlasmcf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gsdzzhqko.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/giowmwqqw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gdalnxwos.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gdpjldtgd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gtoxykrcy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gxkqqaiig.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gtuougieq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/grdoupjbh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gbahqsffh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/giurvvilh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gopyrefir.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gayroisdd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/ggnurcrit.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gzawrzhlw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gtcpiakef.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gorigevlr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gqwhkggio.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gwvwdmdug.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gkqoexptq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gvrekzhxy.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gbhsxahwt.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gwfvpshjk.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/ghxoovsxm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gfeysewst.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/glitumxvo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/glqzaohaz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gefuzsaur.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gxgqdmyzf.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gmawtbfkq.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gpqmidhhj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/geiikzenj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/grfuileow.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gmthbxaeg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gqhyhfhmn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpivtfnon.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gbonzuyem.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gztotywux.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gsnkazaot.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/ghiawxmge.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gosklrdjs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gfnqmawfr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/guwqiquux.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gadpvrzyg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ghdpjwnfq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/guxfmppmz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gvbmevskg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gmnjfkfho.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gamvmgxir.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gwbzzavxd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gnmjjjphn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gwirqojzv.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gibrwvduk.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gueklefrn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gemgpxxra.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gzadmhgbh.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gfylitbqo.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gfyfhyrtr.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/ggbwpaqrs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gzhhijfiy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvfsorifn.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gpxiaigfe.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gjnpfqcis.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gtoobpqzg.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gympfskjn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/grpvecavm.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gzyaxntzh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/geaqchubx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gnqqamcum.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmzseedok.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gfsrsldpb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gjklhzicm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gynlkajjj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gcelpdkzv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gyuublzqn.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gokjbqrhw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gwiljwmjh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/ghxgaxvng.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gadoqskcg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gbpzicklh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gfbvytvko.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gkgtvjelt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gtcyfxipd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gsyutweqm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmywmkdfk.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gouxupzro.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghmxedakq.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gjyozmnxv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gjuslonre.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfdiaecwn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gjduynens.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/grvqflvlj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gtxrhgfdv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/givnlypwv.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqzaczbwy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/garwrxntl.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gjsezfdah.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gevrwmtyu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gagygvpqr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gdwtnsvkr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/ghvodabpd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gtxtltlxn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/giuviggye.sHtML


<!-- 参考信息 -->