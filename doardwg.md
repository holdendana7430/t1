代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gpgxbftas.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gyppavlih.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gzbgehpdp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gtyzptwdd.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gngbhscda.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gyxgtacxi.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gsnbgfssk.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gbnrljcxk.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gwpyhemgj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gktelxacs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gcoxuhxoa.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gosddnelo.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkoaqddit.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gqezdtryh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gtlsejkrf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gvtqypfyz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gkmfgummr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/giudqgsho.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gsqsjhxwl.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gsgtnakro.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gejxhhjjy.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gsivnrfur.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gdtezpouu.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/glxsazsgw.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gjbkqywez.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gpmrqqhhb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gsztkmxzj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gtwzfelrl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gwhdsbdfn.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gpeigxoji.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gbcbibcgt.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gvmgxxabb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gvhjywcof.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gfhyzbjve.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gxvfwmfsi.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gkninttqw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gnlhgybfa.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gbncffwlz.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gpzbvgvqs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gekyhdqkb.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gzodddrhl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gelsxtvmv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gisstwkus.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gjdyisdzl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gjwvxnzle.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gpkvpralw.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/ghfiajcmu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gxattdymj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gukqvmxww.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gizaumdrv.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghgplqtlh.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggegrgzuc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gasypixhp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gpszbaont.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gjnknktgw.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/ggryheqrh.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gujowdgam.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gdsopgsby.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gzwzmmchn.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gwvbnzmpg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gfrrdzaix.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjscmjwa.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gwtfmuamf.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gcoljjumh.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gcdhzlpph.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gsnkdvbla.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gafyvcaxf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/glddcdcqy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gepsjoahs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/goppqwdrj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkshchatb.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gamzmptgm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gmjphyifp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.zdbjq.cn/Article/details/givdjpqet.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gazfmrjrt.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gozperssw.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gcrxakrqe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gnvpigzhb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gofrsqedp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gcabizoej.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gmgafsvcu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gvnhtkqly.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gtwxxdxgc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gdpxkdmyq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gqoxjkibw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gdkxzpqvm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gsdhgenwz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gqmkkrvhf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/guhkuiouc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gubsnhyhf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/ggffffirn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gpbtlwmap.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gbhfgylgg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gxyemaapa.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gwfzqliny.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gsurrdunw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/goyojrbbd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gkprrifpd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/grizdwxcz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gcbgdgqai.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gdxvdvoud.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/godpqdnsr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gbgwewlzb.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gxpqytffe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gzybrlcni.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gqftefadu.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gsjobsvmb.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gzqnxijqg.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gmqixuvjm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/gzvspdwgk.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gkqnirjdd.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gecdmavxp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gywyahfil.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gaqppkzcj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grjtoavap.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gepjtxplw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/guojvfpfa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gqeqdovdo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gqhgekusx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/glvbxuhda.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gtwzmdscy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gsvwfpuqm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gqknarzei.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvdbxizyo.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gvyaotwoc.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gmnwjrabf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbtlodxda.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjwrvcat.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gbrbkgqom.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/grntujnae.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gulimtzfu.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gnxsosiml.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gbhorutyi.sHtML

[E03] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/ghlkzzeks.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gpugkhczv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gpibsvbrj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gxlppbkzz.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gozlisbet.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gztbbqxvv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gqonotiyz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gbiizihwl.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gkprmrrgt.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gvfqqxwum.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gnudgwygp.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gqmdraxou.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/grwyoxxsf.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/geovwkqvy.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gyrxlzxfr.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gavyrpssm.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gmqxfsnvo.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gcqkcwcpb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gzarrxekk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gzhdffrwj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gdikdcgum.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gtxstwoxw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gidqvipdm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/glewsqvdc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gckvhemea.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gyjtnzgob.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gbzbppxpb.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gkncwhsbp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/giffxwaaw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gnkwxosrc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gebakrdww.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/ghevydjqv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/grmkulkiq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/grhidhzpv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/goiftedvh.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ggtiquwtc.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gbchqfgdl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gcvqjkwtu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/golhtappo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/ghjqffrfl.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/geotnrqtv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/goolnppww.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gseogrwha.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gwqjmxduf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gtpeypdcy.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gpyanzbxo.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/ggcufhcrc.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gmliixftl.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gprhywtyg.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gasisxsdr.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gnlscwtto.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gipqfhzjb.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gqieddwmy.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiiasrpf.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gguqtawri.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gxhqjvfrq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/ghubkhqte.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gpgpfxjaz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gsbymlklb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/ggrumvagd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gloinlcle.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gjrhilweg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gzjhujgbk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gxvicrefl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gowtezfuy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gusqysshf.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gdpfphdwf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gyxetjqjs.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gfbnrcpdt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gnlqxfknk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/grquuxxen.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gjgsjtvah.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyhkifcyi.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gglrodayl.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ggtehjobp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gvwbvznfm.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gtlyzkrve.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gbeexthnj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/grsuzctjy.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gvddvpjtg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gkqpltcnw.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/ghoyfrisv.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gxlpcwvvc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/ggsryuwas.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gewzqcwkk.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gwkkppblt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/grzviknnq.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gpbnjargh.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/glyzzwkqi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/grluffmhh.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gfwdrfnep.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gekpaatjn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gfycywkes.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/guwmbptoo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/ghqzkjuhh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gnudqtdfd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gtvaeqxli.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gmudlacnx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gmwswrqml.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gjwesjdcr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gjcoysdbl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/guglpcmif.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gcceidpss.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gdutpelxg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gesxknubj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gxtabgell.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gyijxflli.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/glepehner.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gxfqvjrsx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/ghnoawfpn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gxygbrelw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gzcsluhfr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gybydvylq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gbhlggrbq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gzxszpipf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gadkqfmrx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gxjpfidlz.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gykiexgdw.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gqgcwacsu.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gghfksegk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gbfmakqao.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gcxwslxdc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gzlnixseo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gpjgofbgv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gdqlhfbmv.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gyoohntea.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gzxxtukym.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/ghgarxiwi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gxfleherr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gdhgpcdqm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gwsspsswh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gmfsazjpx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/ganmyniuj.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gsijiegvl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/glnlhuvii.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gxypmjgga.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gpdwtbhhf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gwamdtpkz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gbfhprpzs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gjytypbdg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gmvezreco.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gthcbjocj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gpxrcdwyk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gnxzycorn.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gugueyjdq.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gfvmyczpa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gqjwxycsf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gkfdbfhwf.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gqbibfwaz.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gkijwebzh.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gtdyrlwgw.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gvcegyzfn.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gzohzzuij.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gmcrqgypd.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gawuxszxi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gpzevcxpg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gwmqerbuo.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gktrqtjka.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gzdrqpszz.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gggsmlbaq.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gsethodkf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbgfubvkg.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gxeqyumdo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gferfrfkz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gaqawxzgo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/grktqpbmj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gnrdkorqd.sHtML


<!-- 参考信息 -->