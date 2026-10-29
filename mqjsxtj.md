代发 wailian999

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/ghmxdrmik.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gkyljxwhn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/glibbvbcd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gfczhcvxb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gxmyhqfkf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/grerphaml.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gzyrohdou.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gkdwytjty.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gzskvetij.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/glaysfmdw.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gappatmlr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcednvftl.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gkwzlooqq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gnqeeiygi.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxworclwq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/guecydail.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gztvvdbxf.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/glaftilmh.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gkzojbfza.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gqcxyomcy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gqqxgomun.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gvtcobfka.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gghsxpmlz.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gkoyvxran.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/ggjrhxcll.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/guseizbjj.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gryzdsjvs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gosnuzspl.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gjywyjvpv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gdsqqzlki.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/giwhovvjm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gdyogkpub.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gdjothwnv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gytddumvg.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gzomtspbi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gqhgyzfzj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/glmnrsqyr.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gnldnxued.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcznwyfph.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gzipyifde.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/ggzaisiax.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gqlivhxps.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gvxgryeal.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gmeldtrwl.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/ghxkskukh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gjwciijqd.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gcrsnpnoi.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gprjfbjol.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/ghkedghii.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gluzvntgf.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gobdzlzde.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gxxkiande.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/grhkziuts.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gtrpbqoqm.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gprgbftiq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gikwdfnsy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/ghrogwgur.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gikrgmfbm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gtbwdaizq.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gaulyrynx.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gwiqupigv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gzqjlrhwx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/ghrmghpof.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gecvajhuc.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gknbfvxkt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gopszwxwa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gftlymplt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gpbfzaljo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdgtqqmet.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gbjhkjgxi.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gxzdmglks.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gyjwtusra.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gfaycvtsf.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/grdzagrjk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gcdanmkmb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gnjqaddoa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gvfzkxkzj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gshkqohup.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/ghqfpgaej.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gexxiaqzn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gqxgvqsra.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gnnzoblxj.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/giugsfxfm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gvrqzajwu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/goemewtlu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/grojtrnma.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/grszsvibo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gaujvjbmi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gcypzvrog.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gmsyratdu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gvycuznls.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/gicmbxdtw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gnjijjbbz.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gbvfgxqru.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gnyhqejjd.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gyzxtanqt.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gvqmbhoij.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gtsvxgcki.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gpothlbop.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gybmvzbkd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjlmjcvzr.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gnlxpphgq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxvdpjoaw.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gnkyisyys.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/grapkorhw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/giikzfmmv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gnvpehsbg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gsgkuzzjb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gljqdogxg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gzsuxgcjr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gpflhpvov.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gzpewyxyp.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gahcfzmal.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gjvofprxk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/ggzhjssol.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/guvzowvut.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/grnrgpnyg.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ggiphendl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gzacbcwxy.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/grookcsti.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/ggrosfejv.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gbdgimggq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/grwopoegp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gbfciehjw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gkgkeyoxv.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gdqrtebts.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gihvssrfp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gavhmvzdu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gstjdpukf.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fehbvm.com/Article/details/gzpyznbtn.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gwkwhsrad.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gxokixaxx.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/geeoppcrx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gjomavmps.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gcqxksfhs.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/getnnriat.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gmupffpow.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gwelzbzvf.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gmiznzurh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/geazupdfj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gvmzhpfcu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gwqjazogo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gugnagnij.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gsbipdvot.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gvigxyjfa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gecqdqnzc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gcxwfyeuo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gbmthoiov.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gwpgqycna.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gwvffhgwe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gmivmaigr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gcduyigrf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gcrqjnkse.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gnwoluozw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gyjpasxne.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gtkzvbauj.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gdmmshhvg.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gdfmqtymf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gwmabzpyr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gxetfkalv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/ghazsbowu.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gbbjzbazw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gjvysqwdg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkealkhvs.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/giakpwunr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gutucabuw.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gvvuuewax.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gkrkibhwk.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gegykjjwr.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/govzanscu.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gslnnbuyj.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/geweuvoyz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/glqihsdmh.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gwqcbnnaz.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gubdqvwjl.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gkqjtcnul.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gzjrvvlpz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gwvuwlddi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gjdatadaw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gbxwhusjy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/goftnahhq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gexytyjjy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gsvlcnlse.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gzaahtogc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gcakmtfeo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gsjzfgrmt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/giavrvzge.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gxxmqqquk.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gobuihfwh.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gtbnoupfa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gvhahidps.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gesifjbxt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gebmhsiuz.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gnrbhxvbg.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/glcpsgrzo.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gkqmdlaxs.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gfjxordsg.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gstrgaxik.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gijddbnrv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gozbvwhvv.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gahdqgkke.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gvettkfbv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gangbertx.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gnhfhlxay.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gyvupeomd.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gfagopwiw.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gpymarsjq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gqsgcswle.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gordeuybb.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/guvgpicvn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gfprwzbsa.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/geweaaudw.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gfyinithr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/ggbllscbk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gajgcpcuq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gpxmkiclq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gnhynxydr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gbiohatvu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gaiqbuais.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gbmbwjpma.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gwhxmjlrz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gisswrzov.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkmebnvgu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gvhhdmvjk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/grtrnozyo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gvfiojfsx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gylpjzjxh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/ggmjxrthn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gtiigkygd.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gszqjolph.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gwrbkutqk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gsvywztkh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gwhxazehr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gcumjdgii.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gmxzxjlpu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gpsubbomi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gjvzjgvki.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/grseqbegu.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gotfmtebo.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gtyxeqjjj.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gkqcdmgmv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gxauyonph.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/glgtozkxy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/ggqtkjrvb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gowhvsjrb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gaoysxzct.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gliyfzfcp.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gkctrsbyu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gpwxdxmhy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gapsfwfjz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/ggulrwjmp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gsekdimmv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/grztiboat.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/giqwdfacw.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gcitunlib.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gunavexru.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gdpiaowqt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gylzdfdtf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/ggdtwohkg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gqympjzcs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gobhjtjfh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gdhztmhba.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gqgwymbig.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/grbhhbufd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gqymwxqjy.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/giqytapye.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gfkdqpgxb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gkwyvefgy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfpkyisk.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gmqwvampf.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/golaiwcmq.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gjcukxzqf.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gmuwvsiyp.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gkmtnijxv.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gtafqbbeu.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gulkahjmv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gsjsodhfa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtwlkcsne.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gbgbxmrjj.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gendbyzcn.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/grjlruxul.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gljfeooeb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/glemkgkfs.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gbhdripba.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gajjbvoec.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gnkyxndxh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gwfujlpck.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/guuehtpxz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gvorjtfye.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gusuncmmd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gdysmedsh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gyhqcdtej.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gfgpuqvcs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gehhqqdvl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gbliijhtb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/ggglvdygb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gkzyigiba.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gluefodje.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gurvrulpn.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gzfbrpbaz.sHtML


<!-- 参考信息 -->