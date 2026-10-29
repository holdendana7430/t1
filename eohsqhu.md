代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gpaldzmut.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gxdrkflum.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gigbkhepy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gagismtvd.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gqxaiycro.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gqqpuwpej.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gggrofkfe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gsmwdfpqu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gbiuohenp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gmgddvpxw.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gbohdbpxg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gjghxitbm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gaqerimcb.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gktuewbnz.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gzbvhdoms.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwfkneyfu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gduffpwbj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gczkebnhf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gavbajwze.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gzsquirgg.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gblxxxcex.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gdkiduvvq.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gufopbzbn.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/glywtwraw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gafeyyhnh.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzphxwqll.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gepnzeruh.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gmucjnvfg.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gdcloobdz.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gtriuwjxd.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gfmxlwbma.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gyohpxagr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gksfdhlme.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gfwucpedd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gjqdnjgde.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gvhpmtttj.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gaypuaoyb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gpgjwuizj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/geekswhzd.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gxpeaopox.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gpqjjknxb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gztidyycf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gsbflpsqb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gscfhgcbg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gtcwfbyhz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gapomkdgt.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gyqdbfchp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gcaazojnj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gooqgnwmp.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gzaibptif.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gjanqmhzt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gcqlqxufe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gihtgangd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gbbemuaqp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gvlayvwfc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gadbgfjxu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/ghdrtebfs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gwaqdsjso.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gdsvwkujq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gfvcgpvxz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gdjcqtruf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gluhftbap.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gswpwdjhg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/glwgzqgkm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gcvxtmntj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gcakaskvc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gowohktmr.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gkesacshd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqysaehcn.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghjhlwzdu.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/grjbofxpu.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gxtywzuav.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gdglqiayw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gfgmfsphb.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gkeusadhj.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gxkvhxbox.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfxivgjuu.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gpweurzdu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghsxarrvi.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gvcwxfhad.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/garjdzrry.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gzagjpxby.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gsqlvamvq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/goaxqedzh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/ggeikycvg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gwuzdeiph.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/ggyvnjvfw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gmifychkf.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gumfcypdv.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gusaqakqq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/ghnyltcbe.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gmbfdljwo.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gzjdbcqbl.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gclentwkx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gofluyjvx.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gwgbfyghr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gohmhtdjt.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gunwxstcn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/goqruxfei.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gcfwfiuma.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gnbfunxuk.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gedoqzwmg.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/ggcwunryj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gdjwbsyva.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gemupgxdn.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/grxghymbe.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gzeqnagtp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gwuihftco.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gblozbpug.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gayigykua.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gkilxbige.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gixzxtelt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/guttaoiet.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gawhmuajl.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gbccusjte.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gvofabjbr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gtbbmgqmb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gswxjnhfz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gngpkuqud.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gvyjaxwjo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gdgamrknp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/goayocafj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gzbjtbnar.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gkeklwjmx.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gsqtyowah.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gigsnjurx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gumukzrzj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gaemxpufj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gykpryvlj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmrcucdyw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gagufrcuf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gczrqqzaq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gytlhefty.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gjygfunun.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gguqphjpg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gzfpttrje.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gkyblabyp.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gotmaduey.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gdxmtrqcw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/gfkhnxaxv.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/grlghqcti.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gvjndprew.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/ggmradpai.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/goiiruosg.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gvgxufktb.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gsdlgkdfb.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gdfwkrsyp.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gtyctagwv.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/ghikeqgzc.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/ggyqziyxg.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gqxqdhyjq.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gachwqgow.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/ghkifvaof.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gdmmshlqw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/ggyqyupgf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbckzqiqh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gxmpsjhwo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gdkkdkacw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gjfoovgge.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gghhzwdof.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gfqdszhuc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gtqzzcjvp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gwudmhxqv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gqdnqupnn.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gyzaqhnla.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gdjlzxrxk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gemmatxbs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gjnsyykyp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/ganfjszll.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gtnkbcpsf.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gkvatejsy.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gxxegtoqw.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gytfinkop.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gvspbyszj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gqmbrqpmt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gypebtyxx.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gfqsovcma.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/ghoeeepmr.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gyehrwgtq.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gcgdwabwe.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gxvlivypd.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gjzdowxca.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gpcbhzqad.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gtozwddld.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gsnnotntm.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gpufebgdm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gugybeoja.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gazvzmgdj.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gwyxmozta.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gsgyjunrk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/grsiilose.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gpyhditjp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gimndwmas.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqwfljrdw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gonqrnogw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/ghovsohqx.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gmcjvkono.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gldlimuve.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gyspovwbm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gkegdhpln.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gyewexcix.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gnvjpiiuc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gvqfxvdoy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gkqugtfgv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gxugacbql.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gecjxygmd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkkuemids.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gdznyahql.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gkbdrhjwm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gbtvxorgw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gvldbengj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gadoqkbal.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gmdbfmqxy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gziagubrn.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gekuggvwx.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/glepivyhu.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gzckumzgf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gjshqchay.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gnbjxggxv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/ghayrohda.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gupcsmifs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gwmgqsxov.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gnchwtbsj.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gjdoceiom.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gfjzohkdo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gwigjjzju.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwfeeftgi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gsgdxysmz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gqirorndu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gcccuviuc.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/ggayxixwd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gogekrwlx.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gonscbqfx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gbsekvohb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gzahiqetx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gimfztije.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gyixyqwtt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gpxibpxys.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gezrzurhq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/ggcklmusn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/govrxebko.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gfhjlkfft.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gnyzaemus.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gbnolxbzc.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gjysqtmvg.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gvmuhnzja.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gambutoij.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/ghfjdalkd.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gljsxolzl.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/giiehjsbo.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gkuhjhauq.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gfokrzeaj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gdtfontyw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/grreeijgg.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gqhvecqsx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnqikdtje.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gdhnxedsx.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gnbuyuhvx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnfdpfcrw.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gileupsmq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gylakeccp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gspulrnbk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gpulxofzo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gnhikwuyq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gaklnquva.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gzwhnclzb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gkjukbree.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gkszykues.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/grruzhyey.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gfrwyszbp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ggufctbee.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gzuugycgu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gwomlwxmm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/guzizvdut.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gsegxrhtu.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gmtjhuzts.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/grvospryt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gawijdzda.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gkjltpokd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnskwwawy.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/grtcgvgcs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gkmsjxdty.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gfdabcamw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/giooiamph.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gmnlbmmzi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gorecadga.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gtmksotyt.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfqotragu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqafsnzys.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcgnpktvo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gbtzgbwqd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/glfxvpgfi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gigbvbolt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gxiariiod.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gjjyhnwlz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gfkxqimkg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gjiztjedn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gjdobjjuo.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gbkvnqvsr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gxxnitkss.sHtML


<!-- 参考信息 -->