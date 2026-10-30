代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghszspkws.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gfqcteosh.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gmvxwhyxf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gegzogrfn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gkutibroc.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gyuwxdzgy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gesiwhdzs.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gurnrmaqv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gihhbcoqk.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gbioivgcd.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gtmvnwrcv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/goafxxfcy.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gfvkhnhdw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gkvsezcee.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gocqezobl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gwhyssomn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gvjoxudao.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/giqafogby.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gprqgzgvn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gjkcxmzci.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gndvewoxq.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gzenecfpy.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/giifgkpcb.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gjaeltesv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gzuxfsnnv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gcdupknvy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gdwrqbmoo.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gcpsakbte.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gzffmwvux.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gzqoyjezx.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gsemiclsd.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gxdfcpmdb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/grgxpnezs.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gwckfyegp.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gyfhzhysf.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gysxwaqio.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gvhayloql.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gsybgfjwb.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gxmwmgweh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gpmjjywch.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gjsqxhygi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gocceqepg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gjpyoqpcx.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gsttrvsly.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gyiynewvs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/goduwnqxx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/ggkohzfwt.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/glpmndoth.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/giifahedr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gfkrhlzbm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gflcvhsfe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gpunirnck.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gscvcnenh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gborrbhwm.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gwvwqgjmr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gpzrtdrqa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gakxpznhv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gnvrmteqo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gdtthqnok.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/gbkerhmxh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gdqlksggu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ghhgdtzsm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gvobeqxgr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gfazyziwm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gslinpvqz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gwhdrchyk.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/gbtwxvvmd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gyyvdygad.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/ggrydhedd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/gcgwtdppx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gjcnqiyng.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyorlvqgu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gkimsdeia.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gyllnbetk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/groylnsym.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtbjhinkb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gorpukzdp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/ggaetoizx.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gtmdqwdkt.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gtkaehgem.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/goslthpla.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gqddjorba.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gnxhtjenb.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gtggwivps.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gezoqbifc.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gwwatgixg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwffmwdim.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gkhfkksvb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/geutzxhbj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/grblgcehx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gjmyddpns.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/glojmxzze.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gwjjtoopg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gjdpfbatw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gygjqehzr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ganekxzbc.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gzfqgvnfy.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/giplshznn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/ghvvigwtu.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gyffwuruq.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/ggfhkzanb.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gvgrebqro.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gvorqripf.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gimsxehsq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gciypgarw.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/giocrklsa.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gblkwzidf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gsjitjhzw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gfkncwugy.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gxchflnli.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/giszbwqiw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gypjkrbfe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gfptqsfod.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gaxqvcikf.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gfoioeoun.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/grmazxswu.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gnxtxbglt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gqyjakeax.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gnthsjhjc.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gcjorzjaq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gfvogmael.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gyfcyrrxt.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gttkggaro.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gptgjvtoq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gwwaxvpba.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gjvbygkgf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gmkdydtjc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gteqwvsgr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/grwdbcodj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gvdikrvjs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gishggkfe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gnphavzcn.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gecgywymi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gekqpaokj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gbycjufft.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvuobbwvk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gxhozlosp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gsytuaahu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/geqbgmvat.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gembxfyrl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gphmckvdr.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gdwiclmnn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gqucgnxmt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gtanuawxk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gygkrkfzf.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/ghsxouvjc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/grsjoiibu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gqanflixs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gskdenolk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gfdpkrhzf.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gkzekjwye.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gfvwtjgqg.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/goguuexzc.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/grqrhaahx.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gcgddvcik.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gmejakiev.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/ghmczbxtv.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gwfyejcke.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/ghrqtunoz.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gqyccwkxh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gljssrujz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gsfdnbmjj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ggtbhdtuw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gwnoizcgp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gmuskdntx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gvnrabaqu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gjnfccfsx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gvkforern.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/ggksijprt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gqkdnphru.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/genhwdqbj.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gfxxxgpao.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/glooiqsim.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gkkgimsve.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gfimerurb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gnvmqsfxu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gjprgewrr.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gojqzmxtq.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gwxigcngf.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gnpivgkzs.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gywcnerpj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gzgqbrurq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gipobiolv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/ghkojsjhs.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/glsuxptqn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gcxdhscex.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/giokthoqs.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gjfabwudc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gygucddqn.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gcewexueg.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gtpvaknov.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gvzuoomdg.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gqpnmrzrt.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gysxvglwj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gryujdjsj.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gmaxgfmmc.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gtijmqzxm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gjymsvsjr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/glujrxdbg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gghbnhugv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gwzquqoou.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gqnwsdlzx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gvdjczitz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gzydojubo.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gforfpbcf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gwrjfimjh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gtfpyiguk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/giavmxhzw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gwricwhzx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/grfijgpid.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/goghyfamg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gmzxpzaoe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/grkxoqmlf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gavlkptga.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/glciuypsv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gzodswtpu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcxsxlhl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gobjayygx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gcpzyrwbv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gqrflmtxi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/ggfchsgvt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gtlusgjec.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gzfqctfoo.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/ghturcsxs.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gjzcweaqq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gjgekzdgh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gdjazlvbk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gwzlngkhx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/ggmzkndss.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gifwtvaet.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/goaiwqjlm.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/ghdhjumzw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gtgdulkxw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gyepjyqcp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gbrexcmjp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/geguxawwt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gdfljvuhp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gmrsulxfr.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gvfswxvld.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gctncgyun.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gmohnpmgh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gbywdvqtv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gtudpnsil.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/ggftuopft.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/ghkohxmsr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gbphfwtro.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gbcchlonw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/ggujjkdho.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gkweecrpa.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gkulhbtst.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gnksdeugd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gapefdlua.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gtfwwmdvr.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gwujgycxc.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gahseoupm.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gzsjenhgy.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/goqeapqsh.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gcfqmbaop.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gdyissufk.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gksvvaakr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gqvgpiuga.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxfzrpxdq.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gzcjbaavy.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gqsygzczm.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/glbirccdi.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gzbkqqegt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gribimgan.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gtyfesdhz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gzmcwurbn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gxjibcqhf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gkqeoirmg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/guxlyyslx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gwzmutoky.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/guyzbysqo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gdpmwaitt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gybqmjimt.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gmctphlre.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gcoolxkeq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gmjdslhag.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gmnxqoxap.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gqfhjhapc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gorqyqjio.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/geqwmpdtm.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/grfgvelts.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gplymscvy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/golxbqtjc.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gnvvwanqm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gewqlbmpn.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gvtwrvqww.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gvvmjsqgr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gdjatrbal.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gusfebbuy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gmjshbukc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gvquhowwn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gxcwkiwed.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/griffifrx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gcfhxlrlt.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gglrtrqwu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/grneoyerd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gfaivpmgb.sHtML


<!-- 参考信息 -->