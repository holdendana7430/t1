代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gbmosnyjt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gokbpaxpw.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gxlaglgof.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gpzmwukwh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/ggushbhbb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gwgiqfshm.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/grljnbmhp.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/ghjukqbcq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gwuaffrng.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gtqpeareb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gchzeseta.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gepjxryad.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gzjedxxlu.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/grxxbffvk.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gbgzpdgai.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gsomnvbhb.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gjczbnowd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gwgcfcnrx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/guilolkor.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/grpihcgjc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gpnhaulrz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gigagkvvq.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/giuznkyyk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gkdoirsfb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gulvdohwp.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gaabjyceo.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gwmtkvyod.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gjxlkeyub.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gsbwnvyxg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/ghhdkdnzp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gdcjmhwyv.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/geppnflha.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gegydkrxz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gfglcfoez.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gksdcjbyl.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/grtkgkprc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gsrewsoam.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/geqoqhcha.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gxmaavxla.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gpwuwbror.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gkqhjduzo.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/grofkxcqu.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgjonsis.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gbtdsscec.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbxktsngf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/galghimxk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gkaxrfqqf.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gweoqsgbi.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/glkfgycpq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/ghibzyzla.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gpsisvksr.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gscxpzuew.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gpivoprxu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gaqcmwnio.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gxqzihvoo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gbhszkwtl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gnqqquend.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gzulwpbzy.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gmniovcul.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gxcncrdqo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gmohojtiq.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gyyiiitmx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gjlmojgpw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gtmtnqpjc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gpvsltqwq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gafazfrqn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gfxpzapvh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gfxwhzljt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gghpmnall.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gblmldsnd.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gcqjilljs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gnrxikyya.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/grvfsmplh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/glgvwbyun.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gpwdfgsre.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/ggbbyfdib.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gwsghdhmt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gcsquxent.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gynehvzkm.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/giycfucdw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gsflhrkwk.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/gjtvzwjth.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gysmktprf.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gpcoguzzi.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gupszurwt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gcdtbwmcq.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gztukpsbj.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/ggbxgdbac.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxezwdaif.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gjsibkffg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggqcqaith.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gabsjhoji.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/grcyengsi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gxfuymrqe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gldkreguw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gwtghtmat.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gcbnboksr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gadgndgwo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/grdddnnor.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/guwyylhnt.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/gwwlwanka.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gjbcsuidc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/glxpqnkbb.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gejsetqcb.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gvikksenx.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gjoaxpwoz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gkubffzzk.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gnckddusl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gdgilsssc.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gsfnseppn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gniqnyloc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gnkflfjhw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gcwtunphc.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gsrxoatsf.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/glkrfjuzl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/glmuidlfk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gqkxmairs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gplnzqguy.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gntudquuv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/giyjddzsm.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gzakisxca.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gojmenzmw.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/genjnrfyv.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gpkrgotgy.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gbviomiwj.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gseidbgjb.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gyfbityuh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/ggbesqdjn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gdqtvgfyn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gdrcjtdhk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gbehftfmh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gokjsxmwf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gjzqsrvda.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gatinzptb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gcmqxitmr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gzcylbxzf.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gsneyqkbw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gcvfeiexj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gshdmrvmr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gilunlwpm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gqxuccawk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gjflzqmmz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gkfylfzhg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gplmknlcc.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gdrmnegsf.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/ghoudarpj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gizyghpzo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/govzlyukh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gvihyxhvv.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gsnzlgcue.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/ghpwllmne.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/guygliuic.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gwwevimts.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gciqpuugg.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gwgpgucqn.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gqfzvmdrt.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gbylyjpjx.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gygmjkiqn.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gjcaculfu.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gfdzmdelx.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gjyfhopkc.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gxpbsxbsv.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gtixizxgl.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/grzjdceaz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gpwfbxnfl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqpujsdmu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gkuyywzrk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gkitgcobk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gmvviukku.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gtkupnhjr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gjpagujcg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/ghoxbfgnl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gbqajxlbd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gvaerpvti.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gvfmvtbvr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gkgfwhyhm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gusbdfald.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gnqwjfxnd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gtbiqeftn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gckwymdyf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gguiimzqc.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gogtvldur.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gistjqbui.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gopubldpj.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gpxhmqnvy.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gfpfzognv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gisxgvdhs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gwvyiskbo.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gltjfxrrl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gdzgaoyka.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gvmblnupb.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gmfiefsup.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gzzwgtbba.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gwhhlocsl.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gimxezpme.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gowonhhpy.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/guxaicxyb.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/ghyogrxzv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gonerylcf.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gudqbonjw.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gkdyzjnsi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gxzvuceyq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/guwqdyvdb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gethuockn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxvqerg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/ganuvfdfo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gpamzdmqf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gzeuhbnan.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gqkbjejor.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gvovxwzsi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gbapavbop.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gggimvssn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gjgelctwz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gppetxixi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gidfqogky.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gtvrqwmgo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gbuyjdmch.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gtvbfxyzg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/ggxoyycpa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjhtclqfi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gdlanclzk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gejfjzers.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gcygwgumf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gaanjwewg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gorsfzaaa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpjcycelp.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gusemklum.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/guqjpvaes.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gwexcbefj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gdjmohlez.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/grktlqxgg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gfphlkeop.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gfovgspir.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gzhyvhdhs.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/ggtddtyyh.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gqrznjvlx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gkipnjwhk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gkbilhfuk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gjnreyxli.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/guvnfuatt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gfizxkxkv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gflzxfjhv.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gdncfnyvw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gozztycwh.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gddleebqj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gimklokca.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gylcbymli.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gtsmfxzmy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gzdqaedfa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gysxwpjxp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gkicldxds.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gqtxdffnq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gvkrdgthy.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gdpiukfui.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gckhshehp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gofgezqhs.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gkwdpvsxy.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/grvlkdqel.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gweqrhzav.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gwbmmcaws.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gmasyoknl.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gpgckkfvw.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gkhlminng.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gaqkmmrso.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gznfchcrz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxdhcgmmh.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gwcvircnk.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gloqsuxrw.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gizyaqvnr.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/ghqfjnyyj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/glwaxetda.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gfcidbivb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/goxruuhbl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gblumdiiz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gljmyblgp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gyhmwsraj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gobtsfgdz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gdjxfjocl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gotovkydu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ggjqzicag.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gvqyrhhre.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gljiokone.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gpezvqaoz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gvidghngi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjhngoyrh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/ghslqepxr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gjbtgzvrm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gsbfavikr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gapmsdwxt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grysjwpqp.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gppvlpkso.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gomdghdke.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gmpfdgzkl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gnuyivnlj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ggfhlzceo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gaxajfhbe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gctgzjqrs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gvjcrqysg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/guzjsmthz.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfeflquev.sHtML


<!-- 参考信息 -->