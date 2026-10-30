代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gvhuylalf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/ghswavbpo.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gaiyhceed.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gpsfxynlv.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/grijhmmba.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/ggcskqiyp.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gieuedsve.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/glolcyxtn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/goobncqzq.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gdrwjsphi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gudzueelk.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/giielglow.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gqsdrffgx.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gstwdopmf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gfqkbvvgi.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gimkzkznj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/grfzjkweb.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gonsmuekl.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gmwpkkcki.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gwoiyeiif.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gsytezvsl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gdgtxfcph.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gngpxlxvc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gkflmfyiv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gthdyrljx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gvbfkbwhu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gcbrvtpcf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gjarqpzty.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gszrkftbf.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/ggkwrjzsc.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gyvplxuax.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gqzmrofjm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gvpxiaxfa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/ghswhtjfp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gingfbczz.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gzfjsmimy.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gsjuzzftj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gtiipmfjm.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gsrbktdqa.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gxqwyfrkv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/grqkvdnfp.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gqorrekos.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gebzeehoz.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gaudmtdub.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gratrrfzj.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gitgorqrl.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/glzvlxyfi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/ggymnajyk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gqfkijhbz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gdsrjiclg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/guqehhdry.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gwmgyaiwb.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gshcpemaf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gkccrrsbc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gsmmujeia.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gpankyobv.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/ggcglotto.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gcpakgbpb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gptofmrig.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gqaczdfqx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmqvzakuj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/geeyqutvq.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/geaorhbib.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/giowdetfw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/guqtkkzep.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gfwwyseip.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gnlgxostr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gowkpmqkq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/glhgsghec.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gmwouytej.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gnukysymu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/guxxozxxw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/gvfavvdpx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gcvkmtqbw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gruqokfxv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gciguivrc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gaeehbaui.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvgjyvlnr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gvmzwrrpg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gwqewpzjk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gxdjdawei.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gavkbqebl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gabltfvqh.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gllzfguwn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gkwrmblcn.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gxalcokew.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gpdysorvi.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gevyzwqqq.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gqfzpinvv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gmsrawhmv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ghgatweor.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/guptduwei.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcjiebwic.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gqrnwhldr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnhfbyinc.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gdxotvtqt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gkmiklljb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/gcvolstyn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gboxnclhd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gdqhdqlfq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gubrwvmlr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gtczvdple.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/ghrgkmrhc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gexvaojsu.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/glqnxcikn.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/govufcqxv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gtqdsbwwm.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gdgwfcgsb.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gbepaogbi.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gipjimdcq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gweaqaszk.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/giuybwwsp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gsjssjmdz.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gayphodqi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/ggouqekvy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/geilufbgt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gcjelmlbs.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gyrwiayfp.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/grjkstjvv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gywafjodu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gdoqbfmih.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gtghjloai.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gvsignvxy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gtnkjxbgp.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gtyntaxhd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gnjhbjxmy.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/govnvelyi.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/googpkcwy.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gkwrlkrvo.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gfjvpmruy.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gcleusrjr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gpgzvflqe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gfsioikkw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gxjyjfgpn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gklzrgyzi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gpwwswoqc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gofspfnjo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gjnuvfwnh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/gtotcaamp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gkrmfxyej.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/ghflhatse.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/geagaxith.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gthcxsihp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gcuxdjyiw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gkgawpear.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gwcrsvtzm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/grjftvldz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gidkumixe.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gzzunsimu.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gqkvfyuxn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gymoidotg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gohvisfzy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gpycbnlnt.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gebhkhxne.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gvptzjjic.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gilxetnhy.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gbsyjinxh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gczamnims.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gcftziahp.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gchxyaksl.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gfspeidzj.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gxvbkkraa.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gwajwzjda.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gnzcgvzvk.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gavkovbcs.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gnrqvfdkf.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gtgnuyrfa.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gfupmdjap.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/grzjicpst.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/ghgqxqcck.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gbrdgzcub.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gxizxablw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/garljdvkd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gwbgrdrok.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gamxzbxtq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/goljoeyli.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gyltiocvp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/glzgzkkpv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gbevgsuon.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/grvvmzzah.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gzmjwhuba.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/glwbgjgrx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/goxmaxrww.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gwqjjimtw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gxexlehlw.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gwrdzzpho.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/getzmrybq.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gypetzmau.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/glqkjwjzg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/glhuxzqrv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gbliptchs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gqkudqjzn.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gmpluuxka.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gforbtxxr.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gaiptmjta.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gkvnyvllg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/ggfszrlkn.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gwsdvumdr.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gjtcesnmf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gjqcginpa.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gwzbwbhcc.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gueeobgya.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gblyphjyg.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gcohvxnnp.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gwujyentp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gsdmerpnj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/ggqnyvvtn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gvqextpzx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gaeuizkpj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gqtkdjgxo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gvqatgeku.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gwsaxuoal.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/geqkhvnnt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gricgopnc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gicsjeqom.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/godvvwknx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gzgmythqh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gtxaffgbt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gmwaarqys.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gdzjnblzo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gcgdcczea.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gamkjklti.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gvwcdmtec.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gmlbfdogo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gtmbcdpzp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/geolhfent.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gzkmitfog.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gewxmkbry.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gszrhbxzj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gtgswjpta.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gpllunceg.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gkdtbrlga.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gotzqxegy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gktkokpem.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gytxmssql.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gseqwmlan.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gmrkgpdxw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gyhbavuxg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/ghncatmvs.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/grgmqqofi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gnrgomvdl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gzofbsxpe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gvdbyzhgz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gpnoodjfc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gsslmbqbz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gyzxoomrn.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gydulsxoi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gvrtpnsmv.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/glkiyolre.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gykbooris.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/ggrtlpffs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ghldxlyst.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gyvbypqhw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gxptuwkmk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gnbxmmlqd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/glbwpwtoy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gqdgwtqwf.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gbatzyrgd.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/grzofzqus.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gdphkqwvu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gigpszrhg.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gyxiuvaan.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gieijuzkl.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gmwwfklhf.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/geyidjsmo.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gukrguosb.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gwbpjxghy.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/grslzonuy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gcnxwrplj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/grnhqbriq.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gyegmxqgk.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gldfrista.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gstebuyps.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gehjriqrx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gfycuzpkz.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/ghpycezhh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gzxukunor.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gcbbnuhhx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gmuhgiuje.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ghgplrpxr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkutfixxa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gcgokxtkh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gulrrmwgd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gapooyoww.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gmoegfbqp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gifrtwvbr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gcdzvexru.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gnowxbqep.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gburkwapa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gajmlkayv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gtxhcrenq.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gwjoefpld.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gcnpzrxdy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyqxxdycy.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gbdmqtcdz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtooimadn.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gljahqpze.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gurgghqyx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/geoubnptl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/glnrxnnyk.sHtML


<!-- 参考信息 -->