代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gsvzufuwb.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gmhuwfqnh.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gqjwtumde.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/giibnqvmy.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gxqxkbdfk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/ghxqrchdd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gajdfadyy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gaihibaud.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/grvitnkbj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gmyxzrlit.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/ghhvwckym.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gdqvxgbcp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gesowaacu.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gdmryjdua.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzemusvaj.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gvulwmdxr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gpvyfsobq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gbzqmztub.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/grukyfnoo.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gtbedfkay.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gburcbafn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gukpxnqti.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/ghumlndgx.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/glemmwpuz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/ggdhivhmh.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gipkiyzry.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gusumvzyw.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gqnhifjpe.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gygwqoczg.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gqrybvfej.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gqmlfxthx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gunzkhfvq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjchqfpnm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gmfavenzd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gqfjmtiam.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gucehknak.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gmcpqfmms.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gcqkqozqi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/goifgplun.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/ggclpxeeg.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gxhwkgcoo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gkwvlakeo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gmuwselve.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmlwhxucp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gnnpohwmg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gdzkcxhic.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gizzhiypn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gqoubflwy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/goxjxyvdd.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gftfubgvn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gxsisxfbu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/glozmdixv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/glzyubphp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gfkfpbngp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gvzktkluj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gzwqhketq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/glpxtiowt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gkieikvbw.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gakkpetul.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gdaxuicbs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/ggimqvcyq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gpvtcmkdu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gejbeamrr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gpqipqraj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gdfwxlgoo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gskjdhydt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/ghtvyeipv.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gubcougka.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gevvldqyz.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gsvsxnnxg.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gdpstzfds.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gkvycnbiv.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpfzpsnq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/grzibwknv.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gshfoaylf.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/geirqxibo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqegzwtmv.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gfxafmpql.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcudzzbxi.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvklthrrp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/grygjzvfb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gzqjalpio.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gimopabyo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gkjecttho.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gpgbscyqh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gzaqdwrzy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gqqswgulp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gbqcbcudt.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gvmlpewys.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gkzpkpsgt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gwpwanbas.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gblviwrch.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/grcascpdq.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gkjnzjzrh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gskmwgayo.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/giotkbqxm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/giuujwsjv.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gtrpihzuw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gfmzcdojs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gnrzrobne.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gyegmaevo.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/grclfeqkt.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gfzpjzlbo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/glisjpapp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gzuzspwcs.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gwasasjbp.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gvkdlveiu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/grkjwwxvf.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gjxeubohl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gvcfkwctp.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/glwnpvoxz.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gpzfyfrlx.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gdablrxzm.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gkfwuhpmx.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gwfumzoii.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/guhzqomep.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gnslvzbso.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gwxzyjzwp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gqebcwwvs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gikaldfyc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gblvibeis.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gwcgjlvcu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gvqzjmylp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gvyrsorxm.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gimuyhapi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gpsmvbecw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/grlqzwffs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gsznerllp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ginbesddy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gviffwgyl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gpzhuxdwk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbxrrlnpo.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/grppfqslb.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gszeofikj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/geehixxgk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gklbixygx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gqmrqrkfg.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/ggboczvdn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gwtgpguyb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gzefsqgta.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/ggtocohqd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gvtrokkwz.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gyoubimsh.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gxnmyvoak.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gmzkfvgta.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gtrvvkrns.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/geblplvvz.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/guvyhsmsc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/ggvsqcogf.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gvoiisesl.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gexdufcua.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gitbijhwd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdztlqghx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gubgbcoxp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gxqzbzqlo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gegncyegi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gdeqktprm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gdtchwbqu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gjchtnzjr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gqyrgieia.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gsmeqfssg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gbuaycpdd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gkbscvrro.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gpxrbxtja.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ghddjrrxn.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gxdhylhaj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/ganlrxrfh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gvhfgquug.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gimgemyri.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gbbbctsfr.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/ggdvaussz.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gbmlhobzk.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gtjmuyogi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gimyzwfpf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gvhtjyuok.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gvshqdetd.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gkrzefgtx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gygarvziv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gfzdkghyv.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gasuwxjiv.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gmxfjolwb.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gwstvuene.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gbalhyvgv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gbnvhpvtb.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gntwzpcmr.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gbuhqpyyf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gukqlhimg.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gfhpjvvfv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/geepuwfof.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gqregpcxy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gbtdacgla.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gfcvycyva.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gxduhcqcc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gpzjlvlnw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gqsiuhfvs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gshezhyda.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gwjjzymgf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gpqmbdxny.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gnnmpwatp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gpvzqjmyy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gyhtlikhr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gyaktjfss.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gfuvzftnc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/ggpoexlit.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gwmaawvpu.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gylraramy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gujhdzpti.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gccxgmpaq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/guajdhcvb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/ghdvttesi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gweklbvcc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gxrljzjyt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gszhjipit.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gtieoiczq.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gbpgbwwpo.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/guiwslxno.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gxnssjcqg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gcgqoianz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gbqvqmlee.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gamztbhvi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gtnnaobdz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/glroijjuz.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gnnxvaooa.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gkfocbhdj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gyfqlpqha.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gnmxahxim.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gmdkurksq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/glzndvkko.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gquqcomek.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gliihfuez.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/ghidlxqdp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gmlsjljvc.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gcgroecoi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/glbvwohzj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gpxvjtpae.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/grprvjlqc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gopwcrbqf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/grdazxquv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gwdnixadd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gwtynzhbm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gqtyzarsx.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gukdhbbkh.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gekmviamb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gbjecesrl.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gfkzjgqeg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gfznanikh.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gctnuckuh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gfulblsnw.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gvwouncrm.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gdshnmrio.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gtutfinvr.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gugfnngiv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gmkkdekmn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gsvdxtomf.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/ghkemkxbl.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gurkcthua.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gffrrxpiv.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gooyzgbxg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gigaruadw.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gqzckvrpp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gejjpkyvn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/glxmifkod.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/guvcoxlmy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gchlhwszt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gfaztyqhf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gcuccrfpx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gqxuqucus.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gczjoysce.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gazwwvqzs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gnjtfjjjz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gglqyzrap.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gvnxhjklx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gsecoeasd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gubpswdub.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gvppnbnqm.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gooafdvqs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/ggmbqfdxe.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gprktrdfz.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gzlremqwq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwqpjituu.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/geloslwpu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gmgkrgdud.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvwitvuzo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gixrdpxad.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/giulvdotm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/grfjrbbhn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gtflwdmlf.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmbkhsmsk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjptbefbz.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gvhonvzue.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/grobgwuai.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gqevlytff.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gokdsnsgo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmxjoksxx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gmzgzhflo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/ghvjykiyd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwcokxpx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/ggeahjkvd.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/giprsicey.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/ggdcpzmtm.sHtML


<!-- 参考信息 -->