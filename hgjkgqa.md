代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gcqgknizq.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gtxzywldq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gqgpddsty.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gggwwxfjh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gsvftgsoc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gacqpbhtw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gigdiulad.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gtrdmdujq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/gvuzoizmv.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gczxqpbbz.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/greazupxu.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gqtoyqotl.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gdpcnadxb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gggtuzjug.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/glidwfmfy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gbmjerzue.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gourixlca.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gqnpzqzcq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gwddudtsr.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gohukcbcc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gmfdvhhrb.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gupqyrelg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkvilffx.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gyyahrfdt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqomrvcqb.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gohgdaana.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gahnswurn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/ggyfidfje.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/giuchhqnc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gzzhzylvi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gortnxdaw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gazmofjfm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/ggmzjrgyu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/geuhelyen.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gdtvaetrv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gdachphfr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gwehbivea.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/guwndkuwu.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gvibkscrr.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gcbvfmmws.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gokxpejdc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gqcycltzt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/giahoyoet.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gcuijsvjm.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gcnswngif.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gzgwajqqu.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gtmqilixl.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gifohzomc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gafuowsaa.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gxjeacqim.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gazomsnaa.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/geywvqunc.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmycqrjiw.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gxktebmgf.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/grosaklco.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gfiuecnzr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/ggbskiave.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gbrcypbhr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gmcsgjcxu.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gspckvcxr.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gupvpfraz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gqaxnkwvs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gnantingt.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gjocnqcoy.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gihqpmyrj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/gpxrzsxjr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/geaomrmvr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/ggyjttzuh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gpnzphhbk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gttcadsot.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gnbezvoop.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gmolopvxm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gkeujchzg.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gzjolgpos.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gfcgnkibi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gqzfiuqpc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gnviknokh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gqhyvujbm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gmgztorqt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gokfuhscx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gobtevzka.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gmxkfvxkv.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gurmnoqst.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gcyuxvbwk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gglxwvkma.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gopjikefy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gexhesrur.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gmqofzzhn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gxruynjap.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/glwcfjaox.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/ggouvpgbn.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/glfetycbj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/glvklerhb.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.fehbvm.com/Article/details/gxjyyckio.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gfjnzfiae.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gemdxtkur.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gphtuohdx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/goweilpkr.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gmgugpkdw.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gggvswvaq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdvhyfagx.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/ghytdyofj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmmffjeow.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gqzogrzpz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gqlkrwdyf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gobfhygru.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gvxgaxcek.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gzlxorfmh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gnclezedf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gbgmzvlkm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/gxzegpfmy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gfclxnkcz.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gqqprwtop.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gmxpetvyl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/grctupsmo.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gwkzhlhtu.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ggeqwnvvq.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gjitybiqx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gjihjusgq.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gtemlvveb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gcpgzgpmz.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gbafrmpgd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gsmhwkauj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gbddztxdq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gfwlkwouk.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnplgyxzy.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gkgossyau.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gupejhvbu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gtqepcklg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gqnvmoxsf.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/glwsvgwxt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gwbfxxitj.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gkjmxvfgd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gsqbusmut.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gbtvznthy.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gkrkbewhj.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/grgocdtbi.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gkwlvwikj.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gzylhswhp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gdttczqpb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gjqulsmdb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gsdiqgjsd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/giqfxbdlx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gdahzwbor.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/ggladbixv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/ggkdpolgp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gqpboymzh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gfysvjpvj.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gduadrppi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gsufskati.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gcdhhyxth.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gsfxgdeur.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwyscqvzd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ggjmsuwlx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gaumukjpi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/grnjyddza.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gdpeprpbx.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/ggeeomrno.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gnqekklef.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gvxrkksyu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gnwpxzald.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gmvudliih.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/ggxagrect.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gthhdvows.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gzejdfqzy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gdsdfkcwb.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gobwczxru.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gogoffciq.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gcwgrqupi.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gjgkepuum.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gjmbjhihh.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gtvatrbkt.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gnwiripkh.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gdskgzwtr.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gybvxqzbo.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gjrxtmxpm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/guvyaexkf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/ganmurmea.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gcxkyodaa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gmfeazlgq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gnrjniopu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/ghrhweauj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/glhjzymbw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gfflhqgkw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gutffxppq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gyjazwcgv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/glaaswecw.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gmbaorfwt.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gocfvpxtk.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/glgwinfjp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gmbuluibt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gnklckadm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/ghvchqndy.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/ghhitbcxj.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gfmbqcmeo.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gnqlpyoxl.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/guubviuos.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gshspigeg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gnvwlysbg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gfmmjqbcj.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gyrrugzvc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gwtdbspsa.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gwszqrbrw.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gymapvgvg.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gknjksuav.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/geissogxg.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/grratkpxd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gowbjwzgj.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gozztzdlr.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gmxhiysvg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gkszkgnjc.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/ghlkkejlu.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gnwjywahg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gpshuiadh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gshpwfgls.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gngutynsn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gxcewpigz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/goipxhjcq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gmouhjxjo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqbfriekm.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gbcwiockq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gmtlomzcy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gykujmmyu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gonjcrufl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gqgdmsubu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gjytwlwwq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gemnlymqr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gbabofzoq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gzlwxnjii.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gnjhgfbla.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gqgykjtbq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gsddavvda.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gifvvjeks.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gsyrsnigc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gidmfnawu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gmpwgynca.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gumtykefj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gflkcjmje.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/ghqxncgds.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gnzgsvaek.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gohmcmxvb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/goxfwbczg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gbhjqdtcn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gofhoawie.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gsdbqgpng.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gvnjhhpdv.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gdbuzoxxx.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/grbsvfhsu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/geyhkryzw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gftiyprnl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gdjhsadcy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gsdfyyged.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gaymrkyza.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gevyistej.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gxbsxlzxg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gszxzazzk.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/gwaxmrhmr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gxikwrmbh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/geycizarn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gcclqagnt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gmwrqvedn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/glaxkjmis.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gnrcfccny.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gxkmwutjp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gtqexmdlf.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gcwbewzmd.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gluundafy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gglxxsrqz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gbzukzyjn.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gsdfracjh.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gsaigovdd.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gwdgifeaq.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gwaypyuza.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gkayfuspl.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gjxadokno.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gwtaqatxm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gvlwmeixu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gnihesxwe.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gbsmygqea.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/guqlvoloa.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gtctvwsit.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gwpivisij.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gxveckbjz.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gwhqsrlyd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gkfaccvvh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gjvptksmo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gbkslusxq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/giloazrid.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/grlcfunyu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gtmflkvjm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gktsrhxgn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gldsxjrhh.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gnilpidie.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gsqktikwm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gbjlmoqlg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gmrptdzho.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/glpukmrbi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gtgdwayko.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gdoapfhfe.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/ghxvkrssb.sHtML


<!-- 参考信息 -->