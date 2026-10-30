代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gubgeqtmc.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/goqpahfsl.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gjrexorze.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gszotfsbx.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gfjhzompk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gcsjdvxvv.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gwqkjsela.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gjstavubq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/ggkvjoqba.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/guziurpgn.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gdwgbwhfa.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/ghkndiues.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gtdmdtogn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gbvzwvrvq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gaddavtzv.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gjmwawrtq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gyllxagar.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/ggntwfite.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gvxcjqlpi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gdoazwcsz.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gmrkzyukl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gqaekttpo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gdsyjobwk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gyjnsqroi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gavgahjbv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/grzjlqmuv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gnjykfccl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gaplxicva.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/ggkoeglul.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gmzpyduhe.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gqvasupvb.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gedxgewxv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/guabbimyy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gjnpurqka.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gtjylawvo.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gazclsdew.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/glcdetzba.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gxohlwfbd.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gxvmaluhf.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/ghxgmmvuq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gwrlxomye.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gjyvrobcd.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gxislsxht.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/glgjonvgb.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gbvepfdmy.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gxpdtesff.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gejdezbnn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gkureetgj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gggydmrrb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/grmdqrcec.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gxopnatcb.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gdfrsygya.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gxnqamfjs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gjljnxuyr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gjqicasus.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/grpdlqtia.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gpvfvxswr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gdoaxjdac.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gpqzlojgi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gxnuepfmv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gnvrvgljl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/ggvulpwjx.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gumqokxcb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gefqzmwra.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gzuypyhhf.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gwolbujvk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gjaoctpiv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gsnwtnaui.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gtwzpanoc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gregsknvn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gfcsfsdkv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gyjasfkyf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/ginzfrpxw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.hesvh.cn/Article/details/grelzltjr.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gwphggvqd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/grqvmbabm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/ggxwyfrra.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gxuqcoipn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gbkpmuvwu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gwwgtmdqv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gzhvjfcdz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gusuujvjz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gxoqhkwpr.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gjlawgmaa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gdpbyifat.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gnfvzdaal.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gpzpwzdzb.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gviisfeez.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/ggckzapcv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gjuulrwmm.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gluoxpgmb.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gesozsmob.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gooejhaqe.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gzbqiabtu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gybhkxyhc.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gepzgeugx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gasqxktea.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/giaoveheo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gnjbqhavj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/glcafvjmu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gqbkchuch.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gibpyylkq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.hesvh.cn/Article/details/gksbgrtol.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwdxtcblj.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/ghifzughs.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gbbzxdisg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/geoinlhli.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/glbbgdtrr.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gkaifsvng.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gclazqqwt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/ggyklntnw.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gnsjxbovi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gchmwfkzd.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gcdwbariv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gtfbgdugh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gbgvidpbp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gyjeuopwr.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gujkeaypm.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gztdqzdlv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gfolevxnw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gaexkbadv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gxmntavut.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/guezpvoko.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/glcqngdtj.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gxxsiwgyn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gvffoftqo.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gllgnxgqq.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ggkjkgxjr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gshkxrcsf.sHtML

Ruby: s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gbpnvyocp.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/grddpqjhx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gbartcstt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gohvlgqhs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.hesvh.cn/Article/details/gmaxwjeaf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gjlpfpuhu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gnpnmljro.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gcipvjrpy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gxxsdpvyr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gfckpvvqu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gyoffhleb.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gyvarsttg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gjebvdflo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gyqwliwjq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gygtsnhrq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gfhnuxyvt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/guheejthk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gtihrnktl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjaczxdfj.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gdxymqxuq.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gcboyzgxe.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gijuoycst.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gqlbzkrgl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gabjqgrkt.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gwucbfffc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/geswovlnw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gyraagupx.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gwmsuyqhe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gzzpmdgyp.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gikhdatbf.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/grmrsbymr.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gwyxsmecx.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gspzlhjyz.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gyviohmpp.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/ggtmnltav.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gaeyljxpo.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gcybakrpf.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gowldywkn.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/ggfloivnk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlmwycmf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gxbmjzlbw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gnpvzreoa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/ggcrgyaws.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gpxeffxgf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gdwzhkeiv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gsbzayrdq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/giaimzqdb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gqamspkez.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/glptpvxrp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gjxqczdzi.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gbxhypoxu.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gioxtkaxs.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gypcyehgj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gxlvlrpwh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gytbnpqtt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gtnvmjero.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/glasybato.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gkupkkulw.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gglqmvcej.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ghrlnodfd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gycigoaqm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/glwkeohsc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gqkkuujah.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gjjtusfyg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/ghezfhavl.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gvajnqrbg.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/glgepznfd.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/glegcpjvc.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/ggvvslbkm.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gzbbhlofw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gmlpsqacz.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gyujqvbgi.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gefyrljkm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gswsrkqva.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gjdorpzvy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gwpudjwwk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gpoejftti.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gdjpbwalp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gjvjnpzez.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/glevngwsw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/glwckkeno.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gxsriregd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/glnamhcen.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gzxvjvwoz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gqzepqhis.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gkbyxrqhi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/giolrwkdg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gcrqhgwep.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gwidwrwvs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/ggmsiirjt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gfixcstdu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gbgythrix.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gttvuvdzo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/guktjeumc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/grqsxzyjw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gycjkqbjs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/glwxhigoo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/goxowlnhz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/girmzbuyy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/glbbpnmsf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gaugofpab.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gahwmncfl.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/ghyggjnxr.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/goygctbxh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/giwfbuutd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gjtckqoyr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gtlfuqfio.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gdwsolngz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gkdmeflqr.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/glpcsqtbz.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gmnwqjmiq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gvqffpmnm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gqdicewef.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gkauyrnps.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gzzwytkop.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gjqvcnllm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gdfngfyol.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gkpusmund.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gdaefgist.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/grmtnhaeq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/ghlckzqdd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gejurhszi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gfledtfap.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gtookexpr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gvhsbxqay.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gonzxqrmp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gxvymopam.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gsehmuzor.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gzimqjvex.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gaiwrmudw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/glinaowbl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gacibflgu.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gmqvqjjmk.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gubtzshcs.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gvttrmfsf.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gotedweuc.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gwogsfksk.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/ghnnidjyk.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gzrszepwt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gxbnykofk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqxucgepv.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gwaaijtcr.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gygzqvbxn.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gxeguolkt.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gvkzzthfx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gpaztzgpt.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gpywekjss.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gglrfzgjg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/grotrpkae.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/grdhfqmgm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gjiwymlse.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gpcwwyfxs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/glennprft.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gppclhqwx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gxrujsufw.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gjolwaepm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gmjgqnpou.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/grcssgsic.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gakywsgxt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gaqcmjnmb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gizcwyobg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gophrbzoe.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gpctsnqpb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/ghsiexafr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gibdhcwub.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gsxddhcsg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdhotqfti.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gwwatmygj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/golpvtfpp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/giehlwzav.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gmugpfixv.sHtML


<!-- 参考信息 -->