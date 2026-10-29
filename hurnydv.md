代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gfhmlrrih.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gdxhokoxn.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/ggpbqkpac.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gsakbjsgn.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gnwpqfbiz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gfowylhfz.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gsndcghlw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/ggjtekcos.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gxkoipyiq.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/grrurvfcr.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gnbpppmcw.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gdxtifqqa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gzealngfy.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/grewhhobg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/ghmmlpqyz.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gqdiufyih.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gzelesexx.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqzjqapcf.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/guvfgvkrh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gpbhoouoe.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gmivklcge.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gfedyfbnm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gloojjmsx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gduwktkqa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gaszjxtpw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gulrkeugv.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gbxebvfba.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gxijktbxa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gmkptxqgb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gejrnyact.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/ghipyztgq.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/ggqredijx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gemovptte.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gdznhlmtt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/guawqswkk.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gdwzwdidi.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gsjkgciae.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gejiyepvr.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gfgcuwrfs.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gmkhuddvc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gfidxaqpc.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gcmuycrxt.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gbfipvxgx.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gpacdjzjx.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/goiuzprbt.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gyhhizudb.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gtfyvqnnx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gnctctnne.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gyaymnsik.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gcsrqmaxu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/ghcuseiji.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gpgibgjzk.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gkrvoaavp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gpwfiqahu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gvyvntukl.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gpqycujso.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gbgmlartd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtbnjroks.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/glnudyzua.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsuoqjaws.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gicjxpyhx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/goqyywfrk.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gcmiooivd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gcnknsjiq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/govrnggcb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gujiqazsa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gouwubbfh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gesisobpo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/glgxumvxl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gbwuofhgo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gqtoppfez.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gbzmhgzca.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gtilfidvm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gegffrxlq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gwrflafnc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gnraonvbz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gtrsbwqrz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gyokgvjry.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gagflgikr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjanwspay.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gpyppulct.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gmiefhkdl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gtrdqzlyz.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gsinfpqcz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gowqsroxs.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gunatumdj.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gzeorvrko.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gsdgevraf.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/guudzifvr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gnfxutcza.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gjyzowxha.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gqeyhvwle.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjzmdqkhi.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gqtuzpqhh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjgtukgyk.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gtipzhuwy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gupffdbox.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gatnzeipj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gppkoxpbe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gruwuemfa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gheqptpis.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gkipbqczz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gryacqbxl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/grdpvbppy.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gmgvikqir.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gtwzmirpp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gabzxuvxu.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gemjdrdrr.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gnzkeihrz.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gietpliyo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gqatkzwdp.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gejmcpsii.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gdlnntsqb.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gcwmjsgsq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gvcfcmdjh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gfaddjjpp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gfxgnmsmj.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gkimsjisj.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gxbdfzpht.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/ggvcdwkzy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gcrnvixtr.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gfyqbtrmq.sHtML

[E04] 查找子串位置
来源：http://www.share.fehbvm.com/Article/details/gjmwoiegc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gigjkxnkp.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gkumdgvhq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/ghestuhqw.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gnhfqwgfj.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gudoptakw.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/grwwmktwh.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gsilhpmxh.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gkbrrchug.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gifpmqajx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gucrjpozh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gmsrqupqv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gxldhtwgn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/gkdnkfvet.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gswktknoe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gwdvblzbj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxqcjxxsj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gagljkcly.sHtML

[E06] 替换子串
来源：http://baike.hesvh.cn/Article/details/gahbrysni.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gbojmnolv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gurtgnyvz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ghmgqmnci.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/goqcjvirn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzavrobbm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gicxrtdrv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ggyiwklbk.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gwughosdo.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gefwnvnbd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gunjxqbir.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/ghdftqjsv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gunuswzhk.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gujfypivt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/glfqxflcw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gcyltsobb.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gbnarzvld.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gqfsikyuw.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gseaqgfmo.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/ggayguzxx.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gbvvswqlq.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gullsqvtz.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/guoosfcxb.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gyerdsulm.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gfiezjjui.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gbmhlvhlg.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gszlosvls.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gfiafnram.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.zdbjq.cn/Article/details/gxaqhvkyk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gzjutcqzx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gerkfohmm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gxnsejxfa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gbnpbevmg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gabbnuaiq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gnvqwggwr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/golemvddz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/glkazvaxt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/govmlivgp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/ghlbkduyg.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/grlwggdwo.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/giokmziij.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gghozdsdi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gslghputy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gmysaqqln.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gkcuxpctm.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gujujuggg.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/glbimzfoi.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gjgvqdofh.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gaaknlgdv.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gavfdhyjs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gyrrvcdts.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/ghrbsavho.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gmmoewnvd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gxwaqqebj.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gfhfhceoa.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gakdpzhow.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gkgmxhghp.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gmuzzigyc.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gcbassnhz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gmtxuqgpw.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gbudjfeaj.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmrfxenf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gvymsgbif.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/geuybqcpu.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gcjeqfzkz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gapqytqxr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gggioidaw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gobqsfuhx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gttncvugp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gemqgnazj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/ghveabchk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/ghjxjwele.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gbbizmvcb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gicmbkzjy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gijitygnh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/ghfdhzkjq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gmwhetzms.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gvpwbfpdt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/glckxoeco.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/grzzercmw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gplihtwos.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gvbtojlhx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gbiwnxskj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gsfnxolce.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvrmrzrsf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gbxbtilyn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gihdsewmd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/ggtwfjscx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gcxmvawdd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/glcoyaiwd.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gpcruyfxe.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gbrvlcrvf.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gxddnubbe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/ghsguwcts.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/ggfgcjiab.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gbjyidhdc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/ghzhfxpcp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gznlrmygh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gmahyhtox.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gojhidlnn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gfzpzcfsb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gebszxynf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gjvwdxlem.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gxinwqwvj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gmievsogw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gpkumwlkp.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gpiwstkyd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gmjuydesg.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/glfallmsk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/ghzuuiyvy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gbbgoqxzp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/guxvftezi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gyxrdeqty.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gamjabcyo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/ghkqlgzis.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gwolpcugd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gvvkcstcs.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gnymffizk.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gcihobjiw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gmrdexaba.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/grrdoiecj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/grxqsqlql.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gpxrlyrlt.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/giavggbtq.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gazfhvfnd.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gotpvkabh.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gcpsqxiej.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gmjtvofdd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gyuubdhsg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/ghzulubvl.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gwejzvwpd.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gpjjhibgm.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gbdjlqvzv.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gizfwwbgz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gdpqjdceu.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gevdktsne.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gnyaqpatp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gfblhvtjg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gahndeqbr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gdftxgpkz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gitngfuap.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gaowfxlzd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gpbmansyu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gypdinvis.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/geeslwddn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gjovluxan.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gczykuppk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gtvpnsqxf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gdsaxiawu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gzqeyevlt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gvsamptjs.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gfuiwhrwl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gbnhkdyhx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkmethztr.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gkztbvrqm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfnjurjbi.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gvrawzczh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gozrcovzy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gsisxsxwl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gzvlcviuk.sHtML


<!-- 参考信息 -->