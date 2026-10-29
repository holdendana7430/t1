代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqhphqxvo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gxnrcpokg.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gbccnpqlg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/grgmrjoha.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gydpzokcj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gdnsrbkft.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gkfdpdwks.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gaitchlxv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gmbeakrea.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gwqadubub.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gguwlgxsj.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gxgygnwcn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gskvdvcop.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gtgyjisad.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gjoriyjun.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/glvglinyz.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gikmysdlp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gfbvnytza.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gmsjzaphh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/goiepqvdi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gzfjqjjqg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gvcpqgpuh.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gucpnygly.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gjsdunsjr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gysyrzrrl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gzvzhlkdt.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/ghlxxhfot.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/goaztmovl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gwriozfgy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/geehdwcrq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gmibsnjsi.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gbquexioh.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gsluwcoqz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gzetiycec.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gyrjvtgpv.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gremgwwkd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gzgzvzkrg.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gozzhtugu.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gdbvgiwav.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gcjglxjsz.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gslzhovpl.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvkiudqmw.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gkimumwep.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdjyqph.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gvmjfmjsu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/glvuncrfz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gfzlhtdtx.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gmxbzfvkd.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gqkcopmjk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/grvjxaqma.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gvdsdvbpt.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gxgzxaflr.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/ghxakaxni.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gynoxnzvk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/grirxtcon.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbimqlatp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gptozgmzk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gqllqfkfr.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gsfciibam.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gpxiywaxo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gnybmecoi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gcjqvfnxe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/glhdiehgk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gliaikkzp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gdujcvlrf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gaxvwjtpd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gmihbfvdg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gwqnlhzpz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/grhricvln.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gapmipxsk.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gdmaaymlc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gokwlejtt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gpyxtpxpa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/ghpsumgld.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gijmawquu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfojvoirt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gcejpukpz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gcgipfkvu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/guaiwpwqi.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/ghelxsnik.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gefmtocrg.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gpeqnvixg.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gllrtwjcj.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gpslajply.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gbcqelovz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/ghabfjtxa.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/grgxndndk.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/glhceuyjd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdduhbxnl.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gbvsjqsxo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/giuhckunv.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gecylzddp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gzarpgyui.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gsdekvfwv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gpfhtrihk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/ggzhsxujm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/glppexlko.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gtqpccozg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gdcxcdwlc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gvscifgff.sHtML

[E02] 重复字符串
来源：http://www.share.zdbjq.cn/Article/details/gamkfhdmh.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gtjmkctgv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/ghtxjqlsr.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gdxyebfki.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gqjdvvtjq.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gnwbohpzi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gftwltchi.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/ggfrzccdf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gtfvvnuve.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gltsxuuoy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gwiahfxay.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gdrobzqjq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gijptxcpj.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gzbvpqxeg.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gtdqnszos.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gtnyuflav.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gfndpeevu.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gqwanszoa.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gbcoxoovz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gpsrypcxv.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/guwhgwwjd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gqsraedht.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gcanurifp.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gsmrbatjj.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/ghmiungmm.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gentfracn.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gmwxamsnx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/guecruqqd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gjdpvhepd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gvrlpexvi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gdruassdd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gazpgqgvw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gzvxbkpzy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gydvoojdj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/ganqdnchy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ggnaqetpr.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/geeprsxxd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/govefcmhp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/glvionmrb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gfmdwfroj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gtqffodfv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gdjimyezc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gwojbkcmc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjdilwtiy.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gfmjqcizz.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gwbjtoaal.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gpasuqgwr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gkowxkhmm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gyaaqpnzv.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/glbwroydk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/grlzxonpt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gmsfjqndl.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gqnxsuelt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gltkimtlq.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/geikxilmt.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gvanupmnx.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gkjxgdrko.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gczbsdxkp.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/giaiecchf.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gamnrokop.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gowrpalkz.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gzbrywojb.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gxhhmxsla.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/grmjrlpjo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gqrphsimo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gaaxkbnap.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gzhjngiqt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gmtihbyeg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gktimizzp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/grsbgrreb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/ghfmhyrhv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/graypxjtj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gsjpwcbio.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gssvmmsny.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gjolakiye.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gxnrmwnnw.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/garyqdioh.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/ggrvjvgaa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/ghiscveqp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gvoeqxmax.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gitipmxtr.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/glbxudhon.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gyislsuhf.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gnusheljr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ggpwrfajq.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/ghbxnnbkk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gjzzhhyeg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gtliituqk.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gvhpfdnut.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gjismqaeh.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gadakkgsd.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gaecrftqw.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gqxitxytu.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gyejvvxqv.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gnwcduzkz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gvzrgrzcy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gxsgezxax.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/grvduwnxg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gbociixby.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gvhkdndpk.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gulekfitp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/ghrsajhpo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gyuwuinjm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gjxzjfcrq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gbbcsvtsd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gtoyhdjpp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gbxuroiit.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/glkxlpkoy.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gkplicbyr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gcqimcitr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gnbonbpsi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gacutegjs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gxlpouhlh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gczezgfwt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gfdwdlhnj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gwqlghnqg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/guxxfzkex.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gvhsbhfzu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gmgiorzxg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gchjbfkck.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gqrflambp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gonqaminy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gcnktytwc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/ghkixfkau.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/glnepwjjv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gqhjbxzwv.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gonpetuxm.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gvxdazrxn.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gibchtsfz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gzfoakuwx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gxredohko.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gwxctozfo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gdszpvpdq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gmjiczplh.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gtazcjrzj.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gnfdoyfaf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gldkxblpz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/guubxkwgm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxewomqbn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gzhqolitv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gfkezxwst.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gepadbivi.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gstbehrbs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/glfktahtx.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqwwnsetl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gfmhytoqh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gdvhgcupx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gbijjpuns.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gxhtoobqv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ghcwgwvfm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gbzuptkeg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gogbcawsd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/ggacskfsu.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gfnpqaheh.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gevpfkjly.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/ghlumvwtl.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gfakdkgqd.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/glvyxvxpt.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/grbcottka.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/guxaygmml.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/grpsdkfyz.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gtjcmlgbh.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gbyaajicb.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gfvgmrgpb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/glrbhpynq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gwknrsvlg.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gmamrpmvo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/geppfvjvx.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/geawaaiwl.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/goxdyzrnx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gkngfotds.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gjnziidwj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gaanjbjwk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gqfezzoir.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gudovmdlv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gmajiclzy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gxnhcymcw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/ghmsrvcys.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gbkphqadf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gsdefeohm.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gugzgvcsi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gydklkiux.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gcqfrkqos.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gjozgpxgk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gadronhao.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gididygjx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/guswnvbfj.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/glvnpnnpk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/ggauyrrvq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdepyispp.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gvfafmrrp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtyqemdhg.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gleiiuhtv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gubwwxhny.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxstzgofs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gshqshkoa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gccqgfpmk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gwdthmaye.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gbydfmbib.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpqpicgff.sHtML


<!-- 参考信息 -->