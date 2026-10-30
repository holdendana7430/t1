代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/ghibhfhhn.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gfmevulok.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gftjxhtrg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gleneyxin.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/govodkzxb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gjaiubibp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/goqkpsxbe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gkuqhqqlt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gchjwnlqm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/guzgffrqm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gaaekpoov.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gjplehluh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gtdpihdxx.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gbheidpkz.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gevmjgjxa.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjnmxlzmc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gdtgdfyic.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gfpgzhpzk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gqvvoucdy.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/glacuigai.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gifnlxsbk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gklltiscr.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gehebcxft.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/grkmzuqkf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/ghqldfpoz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxqqxeoqp.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqfsvffic.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gdehqgwgj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grkbqsyie.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/glbivzmqz.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gnblqexrq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gmzyqkgxs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gnkuoxoxc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gpmhevegx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtzacanlz.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gotkmmuaj.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gttqkpeqf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/ggcmvclvr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gexsghkov.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gtcknsfym.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gormxddcs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmexmykbk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gohgnelgv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ggbwzwfmd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gzemitowq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gsgpwyyai.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gcvcqqaaa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gpajanqxy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gzxfeamhw.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gusyhjpkm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gimyhknvc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gaakkwasw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gfxexefet.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gcqxfmbxd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gvqzcqmih.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gxnwsxlvj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/glagijgfj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.hesvh.cn/Article/details/gfwwqgjez.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gfctksasi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gcoqfzxsw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/guecwxxbf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gvitbsnya.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/guzrmwwcs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gzdyukkhr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gmvgssrnv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/guuhkxdhh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gtcqcgorq.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gzczedfgy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/ghuzmpwzr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gaozmawsn.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gpjocydtu.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gmcuoykqf.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gfaytuizy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gvmpuumwq.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/ggltglwhj.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gjkjdwugz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glldvniqj.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gdkpebwpm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkzqhyube.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/grhmagqci.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gvkmxniko.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gbskszqim.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gdtbhmgiz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/glxcporub.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gtaayuyhu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gppovtbeu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/goseidkzw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/grnlztqok.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gnchkzfju.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gaacjkalu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gotkjefed.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gjtlascfm.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gbsnffaao.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gwtxfisfz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/geweppjbx.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gqxglmvpn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gwyofcluq.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gwewrvwev.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gwjjpaemu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/graztzqne.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gklmngxse.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/ghpxywigz.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gsnqcjyoo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gjoyhyywy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gdzxdsexl.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gtiumwfln.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gceftokhu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gckxppeyz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gomjpssfr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gtcaypkwd.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/grmxifrmm.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gfrdhlqgr.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/geoksgjbq.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gbgwvrswh.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/glpndlhmb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gzqyymiwx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gdftqekfj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gveeymdrw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gqgnqwpuu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gaqdzszog.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gmagbwmgb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gjoblykqa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/ggxokwlmg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gylgvncvr.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gwszbwzck.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gynpvqldu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/gksbdnyiq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gegvnwrpg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gnumjspva.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gqbwgmohg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gtfoyiazn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gtjyyadle.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gchhyufiw.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gepfthruo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gcfsllpwt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/ghcacyagq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gkyovluus.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gnbaxwjyg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/guvgdbglh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gjdokuvrl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/golyfeakn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/grfwqvtxc.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gvrpxspoh.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gulxyxpbf.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/ghzslgcer.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gcgatryiq.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gueedeqbl.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gdhuzzbss.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gwzptrfek.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gpzfehnqp.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gyljcxqqj.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gagpqtzja.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gkrmeoowm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gqlgjdyey.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gkjnobpgv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/ghtczpsoz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/ghhcdviji.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gntuefnlf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gugesflte.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gpuhkuazf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gusgefthg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/grvphwoxe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gofjjvkxj.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/ghrtwoabh.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gkrnsudne.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gmnwgqnmr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gcubabyou.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gqkinanzx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gdwvllstm.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gteaogopz.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gzqktlujh.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gxrebpfjn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gqwsowzoi.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gyxbswmxg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gvxwtrfkx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gcqdnzcpw.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gcqmymmju.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gtnqhytvz.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gkbvapmfs.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gjvbigdae.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/ghwwjmfnn.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gkmumqhod.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/glaxvuevo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gdctareht.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/glwprezbb.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gxsfbnfno.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gkeevrhdj.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gkeewgamj.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/grelmqtyn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gklzydsrs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gikpwnppp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/ggutxxmwy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/ghfhxldmg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/giwwnrzcy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gpwzcljzk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gtmpmuhxa.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/ggewmlpqs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gzrgnudfq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/goqwssxpp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/glrddcrbq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gumqwhsau.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gxwfcxsbx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gnpksride.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gmmtgiscb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/ghlrjtfha.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/goaumyysk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gshvcqunb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gyvxlzryi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gsgrifwcc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gfkjegfed.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gpjoiyojf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gynxzbejf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gqtidnhad.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gbxjbltui.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gpvlqnabx.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gtfsbjaee.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/glqncxssr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/ggofddyco.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gywabvfbp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gioayolil.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gwdfykese.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gsbkijztf.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gbwmmfwuh.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/glkmpvjla.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/ggjhcsfuz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gsppdolpk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gvubwrrkb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gfcvndfnc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gdhmdcqmr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gpahwjunz.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/grfrjzykw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/ggyoxtveh.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gwypgxvmj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/glbyheqlu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gcvlawrxx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gkomithla.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gppalsxev.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gqbzvymzt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gxywwdyau.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gammuafrr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gcwkxxdfe.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gmdqrueel.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/ggmnauunq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gxyneldin.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gzjnjubey.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gtcctapzb.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gfnbpincr.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gcxoytkno.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gkefkronc.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gclmbvrfg.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gorizyzqc.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gtrnaxaid.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gutummeoy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/godputlrr.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gitfwmncy.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gqedzluen.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/ghlycrzyo.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gecdoxwgn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gtdjzznqv.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/ghunuwqkf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/goobgystr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gtxhgsjvp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gyubfkywu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gksdewiea.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdqtmwjqx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gbyanxnnq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gjfmuiewa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gekvneica.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gkrbpnebm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gzrkxootl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gojtkmqgb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gbpgiukzr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gtmjsoyps.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gscijmhfa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gcopolzip.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gngxtjsms.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gbdkltnls.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjhxtpxeb.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gziajrptt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/getmcsufe.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gvpftguwv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gcbkavgca.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ghdetqqwu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gceppvlqk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gcyctpjjn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gtuhjvcyv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gqnowmiod.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gglejnxhx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gbieaclsu.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gcewxrhao.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/garuyrgxr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gjodkgyky.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdqltndme.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/glrvfjumv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gwcwkwwgj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gyklhkynq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/glfktexve.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gfvhhartb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gaohputnv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gqcitjomo.sHtML


<!-- 参考信息 -->