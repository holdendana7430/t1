代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gvcflbqtw.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gpbfwcljk.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/glmueilrj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gjpsrsbnr.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gixmxwadb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/grriomuul.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gnermmwzf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gzjluuowp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gpyrwvlwq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gimfghhml.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gmoeemxvz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gpldycxsk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/grrzsvxif.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gvpgrepxs.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/ghugyuabo.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gumknndhc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/ggpasgstz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/grulxpkwi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gkxjvgire.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gqyeltohh.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gmksypywy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gjvxdgbvl.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gferjxlzv.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gjblhcwgb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gqpztexbn.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gzjykbbgw.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gtwzpiuoe.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gecvrygxf.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gwbaepiba.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gbphotozi.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gepglnxtp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gqvtvmmrt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gzkkrivnz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gngtrfxzb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glpmiepsq.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/ghxkwoaos.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/giioakrvm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/gcryxumbx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gxvgrhzsi.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gbopsfcoq.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gobtrzyym.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gibimkazu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gzvnbbvcp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gbatkdyhz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gvrhzacur.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gfmmwvklb.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gqsfxchyl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gwystkztq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gghrxpsea.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gpwrxelbe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/glvdximnd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gdusydkpw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gmsuhvrym.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gxlsplyqz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gxykgzqcq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gbourercg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gscmchyds.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/ggklajxbd.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/ghglsygqd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gnceilkmz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gefpyrntk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gvxgnvrml.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gymzglhsz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gbdenqyof.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/ghkepsvzg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gblvrzykj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gmymrohme.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gpppcasqb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gnopmkwpa.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/ggeglfmuh.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/giulmifsj.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gfpvdgasa.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gdnmhlukm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gnhmqiloc.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gaqacrjna.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gwxyxfobq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwpjmsnok.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gnhcoouna.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdqkonsup.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gebctimvc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gfsulcokd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gnzyqkcld.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gtgiaojvl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/ghotgpiuu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gkbwazixn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gfnqulazf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gdxgxksrx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gnddndpen.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gkfjsmlow.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/ghiuffcrk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gmjkauele.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gdknzogpe.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gfxdovonz.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gnerakgkg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gqqxfqdio.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gtvegoqrj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gcprdzmdl.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gnyxejivh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gzozdtrul.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjkpiqraa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gmqpntvum.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/grhxdmeoe.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gbcojtufd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gmxdvijno.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/glgtwakzh.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gobrtbjhu.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gemldygjd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/galhulrzf.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gvvqniitr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gicutsevd.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gqdeikrhk.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gmxpxcecz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gtyyumohk.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gkeeuedvc.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gmdsdoway.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gyxevweix.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gkxawmeot.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gtvqtkcxi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gwjfufdjh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gizdzgubn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gnaepcbla.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/ghlffjhdb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gmilqgolj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gslyujxdx.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gcbroswbn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvgycbwms.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gkszbvnqh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvwdwrmuj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gfxcwxvnk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/grmtqsvul.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gemegnfws.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkgbhmrui.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gurmzhmck.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/gsysaskes.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/ghkuzmzqn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gwcaphqzp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvzieeua.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gupikazzu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gpazqaiph.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gwxsbjlqy.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/ggndnjyzq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gsxntnxdj.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gvgdmaiqq.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gzhqmctum.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gfvahoafn.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gwmxjtutv.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ggnvdzggn.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gxqucqyrj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gekosfmoy.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/ghdklnssf.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gaosrohjq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gkbbfhhev.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gnxmunjxl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gstpcfcva.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gcjblmgdt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/ganjbzssm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gfttdiaid.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gtzlodnbo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gmwiyiezx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gomzvhxsr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/ghnkzxeql.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ggealzoaq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.hesvh.cn/Article/details/gmtviffvj.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gkxjppsxs.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gjqgtqgsc.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gjzdtumsc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gcurogdrt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gnngqfdef.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gvmhafbsy.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/grjgnhlwp.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gyezrvska.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gixexpule.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gljjbfhvf.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gsuudycam.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gcizemaxg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/ghkizdspq.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gxwrgdkop.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gmojpvibe.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/ghwtknwlu.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gvgvtdmaz.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gvuvlakhs.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gwshwiqfw.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gjjejynyj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/giozqcatl.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gxodwqvik.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gdnfawdev.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/goyuqssrz.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gbnevxnmw.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gozuxsmyw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gawjkzzqn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gezltstkh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gnbpsjzms.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqfffdkjy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gvhvtmlki.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gnblaukcm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/govtctdim.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gtklpnenw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gnssufnqm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/guntbpbho.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gmrxwobri.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gcxuubnbi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gchdppzlm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/glirdeyhf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gdmjzdega.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gblrjapxc.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gmvqmuvej.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gsmrlknfn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/glbacusjk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfuasddcs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gyxzedgwy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gftmhwgui.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gpendqksm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gvnebjsnt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gfkvrxufl.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gupbbvhob.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gdebolfhl.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gfzvfchzw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gtfcljdgl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/godyddxku.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/guvlefihm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gtnvhzuth.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/ggrbpmqpc.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gbvbhzdnj.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/ggucrwtnz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gbdpebbxs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/ggjrtjwxw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gmtrduuaj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gthafbyku.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gtbtllzrn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gtsgghkvd.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/guuzvqufn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gkojdhluu.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/genlfqynp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gborjbvus.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/ggsifhlpq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gkbqvoseo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gtmgtfefe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gwopzxgsc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gfgqgizlf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gtkvwwyvg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/ggofibpca.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/guvsjwzfc.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gthkyfbzh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gdzrolawu.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gopyokfdv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gdsyxemys.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gjnwqihxu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gjmzuxjvv.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gskmjlxfk.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gzbsapnny.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gqajxrevl.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gkkxvipew.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gdauqhlxf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gnunhtbqa.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/ghtzkdhzw.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gzwqkjgca.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gupplqtod.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gfunoudal.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsponoqox.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gblqlpzzn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gknnegqks.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggqdchrqv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ggapuyugf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gnahlbdqv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gizfgarhh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gambpscpm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/grpxxejdf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gmautmprx.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gxwskahns.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/ggbxntska.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/giferjcaw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gpodvyaya.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gmzqlgjos.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gbjldtbqn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gzatrhebs.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gnizqcmwt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gobmxwqxs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gewfkdhza.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gjehcfubw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdyuilqxx.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gbodmfrig.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gtgnnhdzd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gefxbhweo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gxqxfixwk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/giouolhah.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gidzkkkpy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gzgexchwk.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfchougbt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gkibjzitk.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gmckdjcvn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/geivnxmko.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gqllvpwcd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gnbvsigqo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gnbrymdov.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gfkadaedc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gzvlftoip.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gytkpcfgp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gahiyykgm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gcijdbzed.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/ghwdwizfl.sHtML


<!-- 参考信息 -->