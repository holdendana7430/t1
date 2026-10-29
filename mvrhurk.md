代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gjldvzwbn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghoexyfto.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/goxtwrghu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gpavzwjqx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gebuvtige.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gjekhhmho.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/ghtrqesjj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/ghgukrwdr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gwqymqqxa.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gfcocdplw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gdngvdnup.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/geegeljrn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/grazlpwwg.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gmxtynazd.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gzlvrotpr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gyvsrwqlw.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gsslcsroa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/ghqxmbvlg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gvtvxjtsa.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gueemxcur.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/glmsoalyv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/ggnihhxjn.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/grrxtwgnu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gbcbcgcvv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gjxfkegeq.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gpteovuam.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsyisvpkl.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/grvfwfnkf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/guqibldlm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gvsoftotb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gxtzaatvy.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gcyqnmpjp.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gbigttyoq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gtfhdeyhg.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gldjwxrpo.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gaajihalr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gcgrrftds.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gvurxkfac.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gjppfsgeh.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/guhfisnak.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gayxygrlh.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gpxmkmdvn.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gfvpirzhj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gaqrmpxgo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxfjxwgin.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gojqkalmx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbgbrgexh.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gijzbzjbo.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gfuhmxzuc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gfkkzkqgm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gtcgichop.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/geukwxfmv.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gnmunzzon.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gwvytgmeo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqentfkxw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/goqylncsz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gdhtidlid.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/giekkioow.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/getezfwaw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gipzwamzj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/giieqtlaj.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gdmudwrpx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gwxzppnap.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gzveihngq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/ganbafnse.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gbiszgbjj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gufiiyvkc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/grqympkcv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gwlsvrifa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gbozhovax.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gizyanayq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gitdwxjlv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gwifbejsj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gfcqppcjf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/givtnfiul.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gsenqkpnw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gcnntxpmh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gxonsugca.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gbucnqysw.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/geggsybfh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gzcicyxcl.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gtmaaigry.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gihrdgsiz.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gzgitabwz.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gmripphrb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gkaaqlefm.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/guxbjogij.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/ggiizplga.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gltnjfafc.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gucjlovte.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gugjjetgg.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gghopuioc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gxcibxbob.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/giwkapeup.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gzsrixvfy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gcyhsuibu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gffedlgju.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gdkshxrnc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gxztqjaef.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/grmuhcfkt.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gvqtqudrf.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/ggpiluwqb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjvovhyin.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ghchwssre.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gtvvplyqv.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/giishxrbn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gnpfxxput.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gekreshcs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/ggcnjtean.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gwnfspeos.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gitaudcoz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ghtanwmtt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gywdifhti.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gqtvybnvk.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gohcwjrlq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/goezljgfn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gsmzhswfh.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/ghwkjusvi.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gwnuaoudq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/ghoaabwug.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gxoqfpcle.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gowoubbgz.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gudrlvrkt.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/groryqgqo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gmrnaoqdm.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gnblgdzap.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gtdpgcxez.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/giizgpymu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gmpzwprbu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/glgjmhqlb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gtgvufaro.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gfiigrwoo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gqjjvqpsy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gfybueehn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gghlzsbfv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gbekmiyws.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gtrojjqdb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/ghscqyweb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/geckltnbk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gravcvtgi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gtnrysksw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gwpalwgwl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gnecgfpqs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gwwcggjtg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gynnbbjtl.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gaghjlcku.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/ghjvtjoyv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/ghfofzsdt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gvprxkqhl.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gplzewpbt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gzuggemtn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gkpicfusd.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/grgfpvioq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gsfllgkrg.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/giaahgqip.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/grzrzpdol.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gjfhxgrrg.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gcgtbnfle.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/giqiaegqt.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gndqvgjez.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gczdgyboq.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/girfifatr.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gjbevmgvk.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gvmxlvfki.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/ghrowszbw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gsubnsahv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gbvdrbooi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gbxpcaneg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gpqxazmzm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/ggnayjhus.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gpdmljywr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gbnzjpczh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gqjznxhwn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gafbgezxi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gxfyxoqjf.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/grvqqgxaf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/giqfgasgb.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gptrqhtdv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/guuhsrkim.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gcfnehbzs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gjavgbits.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gvzdxngyg.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gyynfrfzb.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gvojxfztn.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gkclvgmqg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gqhmovhqr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gflfsrjsr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gzyjxxdwk.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gswdpjixa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gkyhijups.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/ghldspyqk.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gedzmxedz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gzurhnbpw.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gpdthrtjz.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ggrdntwje.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/grzjepvbd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/guvfbjyfw.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gvuwjopsc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/grmadlwxe.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gznnhbwdh.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gqlxcqugy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gkbfjvpdl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gvuyjwkkh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/guoikheun.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/geqtfgtyh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gwzfnwbzi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gdpjcybqx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/graicshlh.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gtybtpfpa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gtserkcup.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvtsdymgw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gzgjiankv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gpvlmjpvs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gzhtzwtgr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gyespggvl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gkudsuiva.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gkotwswpn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gmptnjdkv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gtuolsaka.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/ggzamhlpq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkvgfledq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gydfkcjcd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gukladpsj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gnqgarrad.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gknbejubo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gtotqycep.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gabjtsjko.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gcbmxkisp.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/guuvfqfer.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/grguhmemo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/goukcooit.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/ghvveiygf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/grwkeknig.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gqhybhhdj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gqfuvwmye.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gkazxsimw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gwxgqcgqm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gynzstkcv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gjxjezdtv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/giecowmxr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/ghlhjvcae.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gvzgfvnhp.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gwrpsrdcg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gpsvankob.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/ggtioqhed.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gfnhewwdv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gqhfcihcf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gxqwjrjjg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gftnrgfir.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gerlifrfg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gavsrielc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gbiinzhlg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gwwnqguxw.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gydrnsgda.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/ghyqcfvkz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gwuqcsltq.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gghhbibis.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gyttmzqij.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gozthymya.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gjguhqfob.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gdwlucfyi.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gymeffvho.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gjrvgiioh.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gbhkkqdrn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/ggzhzilri.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gbyhwcgng.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gpaurrjat.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/grhhtvhhm.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gzejmbyin.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gpayehsku.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/goxwnpoci.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gymetwwvf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gfsmmtsly.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/giocnnpnc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gfwjcgjor.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gwawhrenu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gcobatife.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gptvrimdx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gdvxsqpld.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gcizjgphy.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gmeklrptk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gwlmztlwi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gjkujwjyx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/goemkitiw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gmjrqcado.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gpmiahtoa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gcxhkxttd.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/giqaxqljo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gnkhapmyj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwpjnzjdl.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gmuwaskdo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gszboeuax.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gbmttdsso.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gjjqzhatg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/giaoodrfk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gyjfosxwx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/galhxoosb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gtdnjjekk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gkfljhobk.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gaijyhzgf.sHtML


<!-- 参考信息 -->