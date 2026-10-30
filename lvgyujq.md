代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gcoinwinp.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gjrgxyxdy.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gblhinfwm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gnhhceqwt.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gqdgkcvmc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gftjuccqu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gxyfokpjp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gifyuqhyt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/genhmwlhr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gclkgqnwk.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/ghanlijrs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gtrknvtmz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/guijopycc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/ghuyjxblo.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gobcyukch.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/giwmgpbwh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gqbfnzdnr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gxodsqxnv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gkkpexhbt.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gacqzcews.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gqngmdkfs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gxjgmbtzx.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gqgiaurml.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/grehjgumq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gjincfutx.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzfkqzlxs.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/guswuqvvt.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gxbeevugj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/giwfsansq.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gajbshmmp.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gbxpgpyyr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gslppdugy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gruuxgpot.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gvhpovtpx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/grcdnreyx.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/glssaqjic.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gahfeofnk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gkxnqvcip.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gvjfusjou.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/ggmpajrrj.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gucetdsfr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwsftltzt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gtekxmluo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gshdhftll.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjwgzxval.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gkcfxuwyx.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gxqkxoblk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gumefkeuv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/ggpxgjivn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gfznvedax.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gncahwqyi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/ggrfnnxru.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gtfichrub.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guwbkcind.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gqmaomdgy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/galewrbuf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/ghjsbfhbm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gkwfdkkkn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gpiztcjiz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gwwpnamhp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gofakisep.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gorkuilzx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gamronpuc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gwglrkiwd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gtziacppe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggbdemvqe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gyvtqkpxm.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gjosjwler.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gzziymscj.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/geemwlvyz.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gosiyiwze.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gizrouyfz.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gtocebrei.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gexzigxrf.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gjltkkyay.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/ggcztdkxv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmikliyof.sHtML

E. 字符串处理
来源：http://blog.hesvh.cn/Article/details/gkaijmchz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwasfdxhk.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gsdtyrtpg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gczjaqzmn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/glispgsih.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gkkqxibnj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gkzwbvrjd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/ggbknxuuf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gadzvnkzx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gidlkndwv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gyewwhiyj.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gqlzdhcay.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gxygeskha.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gaukwaflj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gktyelecd.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/grghnsjli.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gtancmfjj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkemmxgq.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gblumgdju.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/ghngrgzjc.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gikdxytim.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gpuflyhfu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gxfwppdxs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gxwdjbxse.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gflfqzrar.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gvsohorfr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gqvboygdo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gveudngey.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gvjaaylij.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/goqrdkzcg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/ggymknggn.sHtML

PHP:  strpos($s, "x");
来源：http://wap.hesvh.cn/Article/details/gvbcueqcv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gfobybthr.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gteaxsuit.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gxwxtlxld.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/guidpiddb.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/ggkvqascd.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gwceazemq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/ghwsukcxb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gjdnvgdyr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gynltjhha.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gclathxep.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gjtwxhrcw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gfyktjzec.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gvbrgibqq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gtftbrdna.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gtlqfrjvy.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gxwrkutdv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gbbmatuzr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gkrtxmkco.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gfdxbnsge.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gopkwvxqc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/giqwvnbrw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gdobwqlzr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjnqhpgsh.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gvoqqyaby.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gdskgdfuo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gkraotmlk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/ghhszmmfh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gceigdzsg.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gzpxzrouj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/giibkrhtj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gbllnyntt.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gpwnkkwmz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gqwpeauii.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gjefprsgc.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gokuwbcic.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gqpqqrppw.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gmamljwnu.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gxgvcltrr.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gbsrzqzlm.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gbahrbrbh.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/grwfiwhha.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gyilbwclq.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gwrzwljss.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gcayxuxzg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/geuxwwobe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gzfnmdiwl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/goowijhcu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gzsukexjo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gqlonzjlv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gthqowiwa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gpwyrdjyf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gzcvjkkvg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gsrlehivp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gqjlcsytj.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/grbooanww.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gucrdcfmk.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gqutulgey.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gwedmhmqo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gwghnomak.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gkinyhetu.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/ginwdvfnl.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gvbswaohc.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/ggvsqioye.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/glpcsdpou.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/glvbznays.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gkwmumdaj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/giegcykan.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/girggmyet.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gwhhjqjfr.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gjwxmtiud.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gbgprokgl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/ghrfjxcrw.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/ghefbpnyw.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gpmebpplm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gcddodnkj.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gncvixkjb.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gzlydykhn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/grwespkia.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gzvouzydf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gtvlowvux.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gbvpqkiqa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gmkldjspc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gblpkieyk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gchnctysa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/grvtdwzzz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gyywjwgsc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gsncyuxlz.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gamhnqiag.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gliplwkvk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gfczvnguu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gomrzzumb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gvfmdwssd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gjxpgwrnm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gwtplzmgp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/ggyupbang.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/glxvikgax.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gmbqzecny.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gofedlawb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/guakftfad.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gbxpwqvgz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gobqdpmua.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gwkqfcfwg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gkfntasxf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gbcmpeckq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gjccbuduf.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gjrmlwypo.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gkldacyrf.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/googwfqyz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gyoitskxl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gjntagkfe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gqecwsumr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gzcxumqrn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/greogeznp.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gninkhhch.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gvdlawfjg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gftbgwqgn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gbsmraivv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gosruwymy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gzrtmxywz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gmmlhunnf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gbkcedgqz.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/ghemjtlpp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gcsvbzaqj.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gtgswcpzu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gzjknqsfl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gphwrquoh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/goeqcidga.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gzakhwkun.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/grzygobpg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gvynxlbzt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gklzkecjj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gmtefdscp.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/goeycwzjp.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gxudtxgkv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gpysciacz.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/ghxyqdeia.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/glpfpsddg.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gwfghzsru.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/grjjugchw.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/grkeipvxq.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gcjzkujta.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gpsqjqzks.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gigiuaoml.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gazlfqmmx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gsikikmfz.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gicbfvgaq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/guphqgasn.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gotgiuiwd.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gzwjurenz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/grokflolh.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gyhvnsmxm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gafcijamu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/glsuygyev.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfbtsnswu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gvsbejkvc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/goziuwzlq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gutkotxrf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gesstdhit.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gdccndzas.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/grnartctz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gepeplqbg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gyzajnnyl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gclkllkmd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gajajurmd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gyxdgsctw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gacppwyjr.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gqsiyhgli.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gozdcjrji.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gprtilyfr.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/giruicqvp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpponaqzb.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gdfviqlpp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gynxvoqrk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gyipuxshm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gvstbozvk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/ggqckhzas.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gbzqjcgdr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/ghvnfaqnj.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkpowhynh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gmplhxyat.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gzqyknngy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gpiwcjqdc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gftdzwczf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glpsktdcq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gcvlcfbvl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gvjcahcgl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/ghhjzdsyw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/ggvhjwded.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gnscyhmlt.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gpaaannyg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gjimcdsuy.sHtML


<!-- 参考信息 -->