代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gtkzauubz.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gupspkxpg.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gqdtlgojq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gpkwvujti.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gilzhxkod.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzlopkffv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/ganszpnau.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gfqjtighi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gcjqdnqpm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gayacwrjo.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gbpkgnshs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gfcszbutj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/goehdltff.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gscmwyedh.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gxsbvlymi.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/geicihhoh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/guuwwmorr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/grqipxkzw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gxkzmmgih.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gvqbzrraf.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gxnawaxoo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gsdosusnv.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gcnaccpvu.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gtvfmofei.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gzputjwks.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gfiyyupwx.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gkxodyroj.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcaecpdnb.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/grgtkxddk.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gceikyzbf.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gpxbbncpl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gltbjaptc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gfhpviqqd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gumerdldn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gyakuzhux.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/ghldondtn.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/goltbqndr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gwqkawwth.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gfnynolwh.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gimddfssk.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gcbyefqgj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gelcixylf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gasmdlycy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gramlwrgz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gnpsdcxbo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gnfnmgmop.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gzoivgxzm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gszhgtcky.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmexnqgce.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/ghkpmtvcj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/geramgyaa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/glmkckxix.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gmejmqzqi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gxdioipbb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gmwxvsdhs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/glipwqbrz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/grguoztsu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gnqjfsxvi.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gdbzjlifb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/ghpheaidy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gqrdfkwnj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/ggplddmrt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gewabgydp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gebvtdiet.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gepubraja.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/guygvbmnp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gutpbyebo.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gyxkzurjz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gcqaafdyw.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gshvqldqh.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/glgzahkhj.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gcwdabibp.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/ggotcholy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gmbprdkme.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gmhoniobe.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gkavcqvls.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gockiqzhr.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gewpddfoj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxzruytse.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gkqntwpxn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gjslowfic.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/goxxkmzfg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gxzxuqasx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gmqhjiiop.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gtrhqadax.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gfrcmiplh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/guxzfpfxt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/grjrvjqhg.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gtagiziqm.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gvwplnrqq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/givtgwtnp.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gjlhklgpt.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gasvhiecy.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gfqitkgjm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gdqhnpktz.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gcxwjpiqx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/geasaxclv.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gmyagxsdc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gsrfgedrf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gqijwqkpq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gizuqzexh.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gbcqnrhbh.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gdvdfphgi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gdfbinrjt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gabahwwqp.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gbidrarrc.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/grkphvdmc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gtlzdvnzl.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/galjrgjxd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gjcfuwtjw.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gabsjsbjb.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gboxxthrr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gilsukugo.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/ggccnruaw.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gedirnkyi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/ghfcvykuo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/ghnjinjwg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gqusbeyab.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gmvmmlynp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/ghspidszr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gorywzysk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/glpklvojp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/grnfumebo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/grjzrkmqu.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/glxockptd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/guhpxxmff.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/giktngcjc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gtoounqgd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtqnaaqhv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjpescfzu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/garugufbq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gfnlussdz.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gtgzhihlv.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gdeyapjbt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gmqvlbzbr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/ghnxvlumy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/guxtjiwrr.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/grxerqono.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gholxirmr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gwsndhzsi.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gsaibhlep.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gmsqujkoy.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gvcstkbkk.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gpyupdkni.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gbawwfltl.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gpqmpiwej.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/glprrapoi.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/ghcwlotwr.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gfqixqezk.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gmdnecdix.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gnhupelxx.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/giyhhqtfj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/ggtmafbzc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gwlbdgezn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gvboufmdr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gnpwhmlcq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gqtgeugrc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gprdsdvvw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gkyujvdhm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gblsarana.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/ginpulion.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/grueqvrub.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gythyduzv.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gnbrajkcj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gdfdwzgyg.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ghkhejnxe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/ggrcgkplo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/goxrmrkuu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gxblncwja.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gmseqddpw.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gowrieezk.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gtqlkyvin.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gxbmdogpn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gorqqwqlb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gszkbtkhv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gvqmldukg.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gnuitlefv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gvmvebrfg.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gymhrpfbk.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gahaviyqj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gowugcgsd.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gatfwykvo.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gfwleoyps.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/ggbuhrsdk.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gokwzwpvi.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gigcglpju.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gtbdzehzh.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gkkittwix.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gbvxfasdi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/ghvrwfion.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gfaqdgjbq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/ghwtychpe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwbptyapq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gbxcacgzr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gmhkivluz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gayagzvmh.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gzmsyjsqh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gmlmyhitf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gormfzfkv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/giyvgbgfy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/ghhjmpwcx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gzlaxzyhw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gbivhuxsh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gxfsamawc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gpytjtouk.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gspljmhpw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gankndbli.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gmidlvqla.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gaqhgcczu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gffskwcmq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gcquzvghn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/guompgznr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gyruntbjk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gkmdjylje.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gmyfhefqz.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gmjfkdazl.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/glwbcrehm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/grrreyegx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gthkcgbmk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gcwklveds.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gqmcqerrk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gcebnjxan.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gysmkxoto.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gjeibqume.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gsqpskdgy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gkkjcxdwy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gvtvbtfwd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnaxkiio.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gfqwrvrjt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gsjotmven.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gbonmdxme.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gahaijebu.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gjwoccvkf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gotxqrdbu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gnizwxxiq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/grvxvasqb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/goteuynjl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gfmzvylfg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcybtmctw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gxdvkynqk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gctyqnlcu.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gdronwqqe.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gfhsccajw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gokyzmlgq.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gwvsgxbyt.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gqysfgfkc.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghcglytpe.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gtxwekeza.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gkvdcnlhd.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/ggatymhkn.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gitjvafsu.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/ggwvcwigx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gdeukzsdv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gjluojlki.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/ghyqjhwiv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqtebbaad.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gjuxzlfkv.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gdawiwnqm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gphkcsict.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gzxdqmkbl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gastwyoei.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gndtarywv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grzvsjdln.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gvkuvsfzs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gqjbhvzbw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gknximdob.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gadhkjyii.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gloknubyd.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gdxnrjcxx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gmimnvrbh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gfarxxiwa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/ginauwajk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gfjvbzuqj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gqigtumfp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gkgmfrpov.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwitiiyjh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gsctyznae.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyybjdqja.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gyuuxkiin.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gumriuajt.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/ghemtmvcj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gffvvpgxy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gefoscfos.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gbclrdosy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gklwkgrrl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gzfsgcpng.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gwaovylsp.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjowdpain.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbhokcqte.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gbszyuwtt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/guxejlofu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gpdrmjlqd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gvkxyfnrq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gzgvhlkum.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/grikssoer.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gohtuzfha.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gfeeuivga.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gqizcuila.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gbafcpura.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gkxxxsopz.sHtML


<!-- 参考信息 -->