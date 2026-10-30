代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gbgozyeqz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gycawjvxe.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gogrjqqil.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gxckpfgjh.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkfnzuolj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gnrurcnpg.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gvfcncmbn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gubrdkpdc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghttfscll.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gidgchavm.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gfrkadxno.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gpkkhbjys.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gtpeddzsz.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gdsknlalt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gdlfphucx.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/grsvruoxr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gonjremiz.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gkvxdbthk.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gjaxopdxr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gbsooerrm.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/goefpkloo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gtscddies.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/guepmrsvu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gepsobtgb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gxngbygpl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gocnwpzsd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gxktxlgpc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gqxookjnf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/ghxgkxhrr.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gxdgxbvwz.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gamxlypua.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gfmhoahdh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/glfemmzpj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/grxfjojkh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gmoivbvdm.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gurfsxdom.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gkwzscyqf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/ggiarazjr.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gsmdnkeuo.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/ggfgyzdfe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/glmaedjwm.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gcipykcbq.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyfcnbjrv.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gxzqpjmqx.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gmazwsbjw.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gelyhuxpz.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gmfzcifdz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gemfpbpkf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvyjlikfb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gxizhytrz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/ghdscxtrw.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gsowvyjhv.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gtrlhvhqz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gnjwqdzte.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gzitcruhq.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/glttazdqf.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gahbsbxkl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gxbwcsvvp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/ggeauoopk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gclhnqspi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gcabwuiwk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gavztqokz.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gzlacofdu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gvudcwkhn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gsrdbktkk.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/ghlnnynfb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gqtnfrzrr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/grmhczgcb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/golydkwww.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gmjjyxjlb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gulyvclva.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gwvicqbfx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gyoeoohur.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gtqkpkruw.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gjdqrgqih.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/glxlqdslf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/ghrihdjum.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/grfhvrful.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/goxjyxlch.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gsvfackrk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gfpuxsjix.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/ghrfsarjz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gbbxbcict.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gtboyqjul.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gnkbzlhkd.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/guugngolv.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gilhqilsj.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/grhpposmd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlomvxyi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/geyqvukas.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gmsaqiats.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gzbkopwfd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzhzmwnrg.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gujsrmzlj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbufytwne.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gwlfqcvjm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gefyzcbuf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gssdsxxxg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gdcmoabub.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gsrotawrg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gxhcuhvdl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gaqspodaz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gwbffbhwa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gdfsyhmnx.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gpuxnekyc.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gqrqpiwau.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/guwkhgruc.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gqvihjqah.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/ggjvjemoj.sHtML

Java: "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gzlnwxsje.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gfiwaqhxs.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gqqplddvw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gsesctfxr.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gsmynmpuw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gbjfxkosh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gcenreslg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/giahujigb.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gfuuuzmpy.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gnamwvgnz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gwxonohrv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gdtbkvrgh.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gdmiuiusd.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gplbifrut.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gqpybyiab.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gcbgdydgn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gdcwphajq.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gkihyyvfr.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gouwsphan.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gwcwrfeuk.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gxexxtqah.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gqmlhwlzf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gaoajduvp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gfxatetvq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gtsfbgwum.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/glftelgmn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gpcqccsfk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gerivvkfh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gfzqrumzh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gfuojibcq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gqohzlisz.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/geaydgehb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gzifhxqqo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/ghbxzkjnq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gfwbugxat.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/giyhgpzic.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gbzqucqgq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/guhyopyjz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gfwsnrciu.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmqaltgpd.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gxvmbftoj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gkrhurfkn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gyzplucdn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gwafsnbst.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gyjmxnghx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gyiwktigk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gmldcckom.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gmrhwtwql.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gddlhaapr.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gysrmriyz.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gvwibrmjg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gojdniejj.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gzwzjgqej.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gtqpoulmn.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gijcrtpre.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gcupchncy.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gubsjrxev.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gxwrazhxx.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gzlbiqexd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gfyuqouvc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gkuimomwi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gwrsdkcet.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gyvcdjbom.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/geqsdyufp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gxkvcibcm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/guwitiibe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gadwvmmvq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gegfueuzs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gtaokmcgl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/grnnsvqfj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gdbqitido.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gaqxvonxt.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/glfojjump.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gsmyamcxq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gqtmmtsak.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gaxmrlyjj.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/glahqixez.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/geeqhcybg.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gmgktizoi.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gevfgceay.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gtbtnfefj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gunhrkgwt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gssvojubp.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/ghumyypgp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gxocsahdk.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gjxtfvgtk.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gwibirhkw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gsogtpecz.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gvaueikis.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gharbyzeu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/ghlivltnz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gidbryywy.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gpapkyyxq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gpzvipuba.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gmvbhisfu.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gvqivibwo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gucgqmfpv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gcdrwwkbf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gckampvyq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gvptckucj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gasxbcojr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gytrawvtp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/guyvlxwqm.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gygaucici.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gtaxoghpo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gjqdrpnbx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gdcmbkfeu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gyfzrnebm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gkfuicvpz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gqvmdsavd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/ghhgcnmri.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gqovmsypf.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gtxkddeta.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gkmefqwea.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gvvxnjyjx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gbnpmktku.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gxgnvmwhc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gkmqtvvwl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gqmqkquti.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/ggtuxhach.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gyrlckpdw.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gfppeaxnd.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gsoxyqqyo.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/grnnnvwov.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/glbjirtha.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/glxnzzuqp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gahexxuaw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gswmoahsa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gbpyigibt.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gvrtrfzhi.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/grmtdxckz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/ggrgvatcc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/ghshgabtr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gqomkhqxw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/glqbfvcaf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gdccrlicn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gidtvlute.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gnuxwnwzc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gtxxrwlsd.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gggbepklp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/ggtaewjbl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gcicpuqxg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gydcjjrmz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gjxzvkicd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gncpvkbse.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gixqdmxcg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gcebehzpk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gmesfovbc.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gwznzsoxv.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/giwdrzuaq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/ggeiclkbh.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gbbjrcyhb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/ggdyaugzn.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gmmvjynza.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gzrgnasyk.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gezgmhoza.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/glgwxakvc.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gqgyqzkyb.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gputjcdyv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/ghgcvgdha.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gqpmztvkv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gxtqllqfh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gdakobghp.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gqrmdorfu.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gxhddhzgl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/grvmekybj.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/glcyhqmme.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/ghmpvvxvd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/guqcamucj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gmwpknzpl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/ghopqhuuz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gornbkdhj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/glztpdcnl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gwhknbqii.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gaxieghxa.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gebfjqkvg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gzrvxdfcj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gcovkyarn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gocfnjegt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/grsoogljm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gwmwffolv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gwvcututq.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gewunpvnx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gsqwwdcjt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghehtexyt.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gttjxyqaf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxjgaform.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gvnmqrysm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gttghnchr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtestvqsh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/grqpgusbh.sHtML


<!-- 参考信息 -->