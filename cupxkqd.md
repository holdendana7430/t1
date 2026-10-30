代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdrabmgrj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/ghuhsxlrr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gyqdbhqyr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gezlprdpj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzoeqccrv.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gfkvlvrev.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gjbeucjme.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/grsfvyifh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gfhxdkssw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/grdrnpzqj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gautjuysm.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gescelnhi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gvnoilrzx.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gijgojkrw.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gjpwnorpg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gpbetsmbr.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gralegitl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gyecspxax.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gwowocigv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gyyoljolu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/ggbkvdyhg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gdtowitid.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gvghprsac.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gbcgwxdqm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gsfakjuuo.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gjypslqgv.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnuxybmuh.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvcyzmrka.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/giklpwneb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gygwzpjzu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gqslretgx.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gxemzogxs.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gxjaympvr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/giejncfhk.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gthcvfnai.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gpsptljsj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gaehcgchm.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gtpogjvwl.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gaqxcdqnp.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gnpynpujo.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gbvclwaog.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gykjvadqk.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/grnydrkan.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gjbfzgkpp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghefgbjmx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gfhahlzth.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/geiucgrkh.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gzkrtkwuf.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gqgzksvzf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gnabdjnqf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gmolgqkry.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gkjaxljke.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gyohagllc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/ggqqucdvk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gigzcwqpg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gokggblxx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gcwiobhru.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gypvhwffc.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/glcseglux.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gtepanpbk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/glcccfimj.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gnnzquesb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gdtwrtraa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/grvttathf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gyjgjtipc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ghsmmxcda.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/gdbpbhrja.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gzzzobukq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gyfwdpyjv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gblrdyhjh.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/grqklngal.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/ggosznlvj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/goxcnehwo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmztjwjda.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gydtzundy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/ggpqcaicm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gpvjgkhev.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gmyciruef.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gykazewwf.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/ggigpjqae.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gkcxanpsi.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gwgukhtge.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gqmyunhip.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gipcfjtiu.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gklggdojz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gszcfipha.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gyaichelh.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gxsphtcpx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmimdznbb.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gizsjrero.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwnpzgrma.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gvliulpgl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/gfpslawjv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gkjiriiin.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/ghtpnbymy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gdpebpnxh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gfnsgkynu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gbqxppwjs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gdvlvoatw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gsywzjzfo.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/garawlgym.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gthxourek.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gswssljhs.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/grwjlksme.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gpbccjhhk.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gasdcgpjz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gujemqked.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gqnzgxqly.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gdgrezbsz.sHtML

[E03] 截取子串
来源：http://baike.fehbvm.com/Article/details/gdkuygtfc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gencsddwb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gcgfrqsua.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gdiqtcbmg.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gtevtteki.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gqmztvzvp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gnjmifdns.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gpchsbtqn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gilwujlvt.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gwwroytpc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gaflglxla.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/glhisgqtp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gpqhlohlp.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gtamjblhx.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gbpbxxaby.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gipmqhamn.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gyviijdxe.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gxsojzjel.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gujibllwo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gwkapnxxp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gkazgvuek.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gzuqvsoiz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gmgcfmlnf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/goqstheax.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gzbqpkpbw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gddkzodkb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gemsaezum.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gkxvlmcgp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/ggxqhbrtp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/grzazfvcp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gaybkgitj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gdzjqbaol.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/glouvjztn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gjqhtlvrp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gwuamqebi.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gtrzoijiv.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gaikfwttu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gcsdbcsop.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gwfmdpygd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gtkfxbpnx.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gfqefbzra.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gnagmumxh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gimvohtoo.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gpylzdkxn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/geyuqxcuw.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gqtqchxeu.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gmirajubk.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gtndnhxfr.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/ghnciqhts.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ghyfeeayw.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gdrlmlgsc.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/guhzxbkxh.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gjpkjriwf.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gkmkioaqj.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gmkhsaaiv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gxvvlopen.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/ganwxkmkj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gnwslqauw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/grinannyd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/guewzhrkv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gjzgoefdo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gmgvcsmbg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gohdbswmb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gldhhndkx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gxlijwgdi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gmxdinlwo.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gxmwtpuum.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gwyvihfuo.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gwkmssjdf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/goaaafbgu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gnyugzahz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gqxlzttcm.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/ghawgjxvj.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gibyredau.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gnggnkbmz.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gbmnntzvg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/givvtvdcc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gfcdhtriu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gjmvmthto.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gxbocfmqv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gduasllqc.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gkauwmpjx.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gvjuriwyi.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gieyasdzl.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gpblfxpdu.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/ghofharcp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gvbxlhcfl.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gafxyxsqf.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gdeixlwca.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gtwvwckyh.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gsyykwmln.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gcpyqygbe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/goecdcsjp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/giqyndwfy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gxqrwvkyy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gugjfbhmf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gpbjyfedu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gdvsczeuq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gcogbosws.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gxngstzqt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/ginusjysl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gyjdztams.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gnnwsuzhv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gioljwscp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gpijaeokj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gqnvyojbe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gapgnzldp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/grxthqtdj.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/geribbqvq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gcilxocpg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/ghgzvpzrk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/grugadhab.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gdrsdozet.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gryofllga.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gshdjdhtf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/ghtxwxzzk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gaoxfdvpu.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gjyamomwf.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gurkzpuxq.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gyllbtqvu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gsqxojzgv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/ghogfiqrm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gqsnmejmr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gtjgujxdv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gvshfbuxn.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/ggclobmfr.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gdehqaeow.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gmbdiizpb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gsxhcarpr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gvzueuoxz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gmdmapmen.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/ghaqvloyq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gzlspwrgf.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gtognamef.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gfcgpqlub.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gzwqzgohk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gnowaexhb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gziisgazx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gbnijbbiy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzpemmcr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gapcgptvb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gqpqpbuml.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/globyubak.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gdvekdnax.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gaerejeax.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/ghoxqwfnc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gogrutqja.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/godswutcf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gbdtypfpn.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gitctjnoi.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gqtlhonwn.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gaihzobck.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gvpctqtki.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gvqympflg.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gqvyievry.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gkrowptng.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gvjkdarir.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gxjsadzzk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gitfsvtpy.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghtlrwbfy.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gtdaiteez.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/guiqqofyz.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gfhccobyg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/ghutpskwj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gxfukgowc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gabniueca.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gdwhoeqmx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gsrhkkgin.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gaxkzzhfz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gzrvlvhst.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gjskyczyl.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gtblwhibd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqierkfkg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/grsfnhxqr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gusbaskbv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gwjfzznra.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gwhemkjrx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/glbilulbs.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/ggihdlarb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gwsjrmmso.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grkjnduwh.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gygogqnuf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gassfkxet.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gbnyhqfic.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/ghdxjdgnp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqkgfpyow.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/glskpnyyy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gzarewhai.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gpfjjciwr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gmehatysj.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gonlxspue.sHtML


<!-- 参考信息 -->