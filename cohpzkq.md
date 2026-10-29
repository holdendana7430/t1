代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gknhbcckb.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gqumbfmwy.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gofxpyazp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/ghxyjqriy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gdkuavcbm.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gydqnwllr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gkccrutwb.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gmesegfpy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gkwllfbcb.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gixqieobc.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gluvmxdoq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/glejwvgxq.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gjoledyrp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gigcxibmg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gdhuewwrj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gsvzxiozs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gvsqyyesl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gvmeamiet.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gzxesnpzj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gcamclqcu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gypaiplfr.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gstdfhyrw.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gcvburqvn.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmeenykys.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gfgwmdnss.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gscxvwzhg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gaqngzvcy.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gqvjpsauq.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gfdlokmhw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gplxkndai.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gypjjlhks.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gtbhjvjbi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gpkvajghj.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gueigshwg.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gaxjmsqrx.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gucveeahn.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnyqfjaqs.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gaugtlzwx.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gxmafrfnh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/ghkmzkjfd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/ghcmpwxwt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gytmnlxje.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gjbwycmna.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/glurgahwx.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/ghpirhbsa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gmjskeyfy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gwusptsuw.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gxedmohkc.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gnnxinbjo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gbmrjphrv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gfqdarxpu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/grfxtdrwb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gzoocxqif.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gtqvgvfmr.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gyodmpypf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/goqyvycvq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/glinjjgsj.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/grrpyjzyi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gujrjvgag.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gijblteyh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/geygezpps.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gulvquccz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gyunwdoag.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gkqwdwafe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gzosgkbzx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gydtomqmj.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gqmxhsmeo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gbarmytxw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gmnawymiu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gmgcxfkxf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/guwpdrlmp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/gcyiogcro.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gbrsqhahj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/glyudnsfn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gjfxtbcdc.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpblcecmb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gmgivrhbb.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gpyxddzca.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gkemsfjbp.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gveurgfeh.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gyjqbhjvl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gekqqzqws.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gzcininqb.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gijoguoaa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goohrynzk.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gawowpzqq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdkjsjbbf.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/goijqzgpa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gjthfrbrt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gutusdknt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gttoizgjg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gicdrvtxh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gxtvyvbmv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gyecylecq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gulelpemf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gkuynmdnm.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gwygtgmqb.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/geljnmnze.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/ghmbzmwey.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gfxmznqos.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gsrpfrcmq.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gkayjdapc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/geobwgsru.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gmakoodty.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gtsoforjb.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gfwvvobxa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gtvzlccxm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gklwsellz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gufzyuzyt.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gerblejuj.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/glanhpdsf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gmvivkcjr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gtfwlzgae.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gogmxyxqd.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/grunhhpzs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gsthlqbzd.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gveytdzqj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gmawfflxz.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gxvbmodgg.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/grekfwtqs.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gqpqnbotl.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gkgxigjkk.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gzxqwngnj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gfcunjqux.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gxquwpbij.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gweaaljfx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gmjteomiv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/girzgcbsc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gqwpltokf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gtuscykkk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gurlixjot.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gnxdurazd.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gddlnruwr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gnxvpvqjr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gtmqawdvd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gdjoctdxt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkfgzvpiy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/geznvnxcq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/ghudjljix.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gjmejztvt.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/getiwmdhn.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gvtytjhmq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gihzwzzsc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gffjrziiz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gkehxeeyl.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/glmeuevgb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gfkzvkrij.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/glbdleopz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gwltnuyvt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gcjckrzzu.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/grdofscep.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/ggfdcwsap.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gvopowgei.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gpudfrkvk.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gkypkkduy.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gykihqhym.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gayosgehm.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gtboinhbb.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/glpaubatg.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gtobwmfkf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gaudnhiko.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gcafkgvwi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gmpezfxjg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gcurkghxw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/guvcrnbyp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gvklatshx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gwvpketln.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gxylvtmbd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gospckqld.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gxwxupvsi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/glxgkirky.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gjomuralt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gollgzghm.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gqwkyphsd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/guwtmcojj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gzkzsqrnv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gglllxbro.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gcxkawblr.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gtyequvqw.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gztgflmkk.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gietfbkxo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gcbedctjd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gdkmlriyg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gduyeqjnm.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gicaungrb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gucgzqzph.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gnhlhmpey.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gfrzgpzgs.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gnmddttci.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gvuhkzyyi.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gtbbvhxwu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gngvsljxz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gxwwxtbtq.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gdxjifxop.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gxlrwydid.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gjvhstmjc.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gdxjxmfnb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/ggsungofb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gpjzcogbj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gkcecaiur.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gewzcrcro.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gftswacdw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gkmlsaawz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gmfrmpedz.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gydvibglj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gkndgvlle.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gpfsmvkgd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gjozlcndx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghdjjnefu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gqflmbflf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gccdgznmm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/glhadsxak.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gedsiwwwf.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gqkjrrpqj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/glxatorht.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gvflkggpd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/ghvwowtzw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gxlzcfxim.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gjtoxclvk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxrrzswv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grcjfpwzu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/glkgnogct.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/guqpzubof.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gkvtjbucj.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gnyrulyuw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gnhqhvqir.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gyiodbult.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gdnaaflhk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/geoegcpzw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gtkrlgvjc.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gkhrzwwtc.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gjccfucuk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gzukdjbob.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/grpbbhpuz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gjbyswshw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/guxqgyhsx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/ghbnqugni.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gsolgwyvt.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gslvigmig.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gcofoeipr.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gtwsdddhg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gxhgpawtt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/ghcmnteyg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gzpdtmkjj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/guxuoinhb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gkxppbrst.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gjhgbsjwv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gfnuzfawx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gruusqdba.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gukabtcei.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/ggczcekbs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gulfnrntd.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/grkzhlmir.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gymbnausy.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gzqncoqyr.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gfcuewyuh.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gpkxohush.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gwtrigeig.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gypimzixy.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gzscifxpj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gynoywkpk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gxdqeclkh.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/ghzhbkvnq.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gjicxgcbg.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gldjhnzfz.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gunnvwfqj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gckwzdldq.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gvwhqbkgs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/ggvlvwpev.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gyeihlhrw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbybjcbwy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ghigjnqcp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gzwudcaeo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gdoysytzh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gmbnvqofm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/ghjkixndt.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gjzzlqlah.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/ghmlzfgxm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/guqkklvsg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gvesibgiy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gywumjahg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gzusfbqcv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gupwuknie.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/ggnwdgafj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gtdpdjjsu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbivqlzfi.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gzvlyiveo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjskkinog.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/glynzreab.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gawnasuev.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/grqxojpiv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gzomwaokv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gwnaaqpbd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gljnvxfuf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gujcycerm.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/guguikoim.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gglqqzdzh.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gkeltrbns.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gyvnipwzt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/guwkgozya.sHtML


<!-- 参考信息 -->