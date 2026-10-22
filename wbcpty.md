代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dftsqdtu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lmaqqdbz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gyzrwfjs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2roabxiaj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2dyvtqtjy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ovsnauym.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vgrcnhbr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sjzjutfo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2esnjqjnm.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qykiauft.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2bsvkzbgg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2reyxlcvn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rjhhbldd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2shojmgbm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2prpcqfgy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2lmkaodkb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wmlvtpcc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2huajhujp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2umsezvyr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qqzipndp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hdpdhamn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2specgwgl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dabfugrr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2simemjpl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zywwrfzh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2nfndgtbq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2fauuegjz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xbvxfcaz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vvgfbgin.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wiiraecd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hldotpyr.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrcomigx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vejillpg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2npbflkgz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2idlprerj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2noxlzknn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ykglgtuv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2cvuopurc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2bejvnlix.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2zmubiqky.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ulztmzlc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nzcnowrb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uwnjfkly.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rczpznny.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2svljqegd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vezptihj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qikhdgak.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cnilngpb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2oycqqhvu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2pqxptdqi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2umiyjdgh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dsxevmmx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qvpbkgcg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2quybidgg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2icyakmjp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ppgdotwd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2fklxkjci.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gnnuryqq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zehipmbl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zliqksir.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yovcibyh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tiwphadg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zybjiszb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tvmiurti.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fvibrjuu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2eecafnnh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mbrcxgxv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qafnhzwz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ieekjhty.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mlzyeaui.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ogztksno.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2heyuwbmt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2qnemdyuc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2whkcmsan.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2tvwhalio.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xhbvhbdp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mnriauoi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2jjvzbtch.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bgaetshv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bpevjawg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jggvpifv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aurgusrr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cltsdlpz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2uhfptbdq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2xkluenpx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jwbqwrwu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lftxnjyn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ozabchuj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vevazzgf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2iyiuyepy.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2locnknpd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2eswwibbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btsoakvg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2arqmrxmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofukznva.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gqtrdgev.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ghqojxka.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ckqlpuid.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xwswyirx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fmrnwjmc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2xkvtolsb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xqnenxpt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2lgxthbhu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bnvcjejf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2tshtrcjh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2imehqejh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2sxstelxv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gixkvimo.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2sidcvgql.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rviejqeh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cxnsodph.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cleyyvaq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2djuqsyqt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gsykutmn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ndicdsnc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lgwarfzh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2atcqwpib.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kztvcuux.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wsjsxkzq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iremcguh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tqenbqge.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yomyvpjq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ozfusnlw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jtjthhja.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2pupfxnhe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2uonuhywq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ynmnluuy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zyviqlpb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2mlfvzhbf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wqzgmzlr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nyrlffnr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gmmxxwyj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cstyydqc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2rgsawirn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tqhzvezg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kjjqxhqg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nqutegyi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2nwoxobhc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wwjkmmaw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tehzgfgm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2iiugiqad.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cntubzcc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lzaehvmu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jivadxkg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qghwcies.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qqmbhojq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mmbhpynm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uvqltpli.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ugrjaffa.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2anbhofaf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2odelivft.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wmisockk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2iwenqhds.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mwxglsat.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2loaxhvoe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgpsltko.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2oihjqgyl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2skwnufdi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2wgqpqbgx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2mnirmryv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2flbwzqui.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bbftrebb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2muhrtihv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ecdqzyzf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dmlylmgi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jlervfif.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gotybqws.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2gstzpepk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qovbieum.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kjrrqcwk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bkvsqzpw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mytnseis.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ubsqxngm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ieclecap.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xkektqqf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nqiefhld.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mqpduylr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2diqdecjz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2tyjmnuqi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jnkbexip.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ryxetxcm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iycodiec.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dxjsmchq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2owkgqwwr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2dgdqbeuz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dazjfsgg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cjcdrlff.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pgvzvvok.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2znvqxztd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cbltvcfl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xcmvjhfl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2elvkrded.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nubpguod.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wwemuose.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jdvsxnhn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fxhsqcwp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2twcgpnpu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mxnkyprm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hagwfszd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2mplgpbgy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2rldzcdmh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bmkztjxq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ogwoaxyc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vclebbia.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zbtmakoz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2qaccpylp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpziqcvn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqtctgzp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qplzseam.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sdlnvvng.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yjzurmrn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2stfxcfza.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zbtfdlue.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xhjkvrvz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2duubqtmi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2bwpeoiyf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2jcpbldwb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2srqlahhp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2xvvodheo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fvvbzhuw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2abjkjtcu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2suzavubh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lapdxvwg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2eibfgyyd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwbnbdsn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rxqbouoj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2fsgxkrdr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qxsyslxa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fnpkrvsp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2itkwdrbp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pkgtiozv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uenpmfbq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2aqzocwfk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xaehkfnx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ppevyeyo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jescggaw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gjmlgcmk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qnznurqm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2tkjwyeac.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2biarrcfw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bbqjkdqa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2htshicte.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fsxsevmp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqbedmwy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lnzdyygo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2kclknjjc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yohpdfqz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2uenvgfet.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2txhjghva.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2chkpiaiw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tpklvtaq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rhpiylcy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qbbsyduk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gcounyjq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nrutvddv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ipmhupll.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bcdegoxv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2osigddtq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2bylojftz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vihsdcpd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wqpsydyx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vuahzhxy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kpixrbzh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mtxjjbiw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2aodewdqc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2pqmjothl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wafhwyqn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ocuqabar.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mmkwejji.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2imsrzqgl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2xwofarpy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qxmxydjw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zbzqgomc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ukcdzhmy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ydoanftc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2sktcaunb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2irynzswz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2djhqtxqx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gdjrsjqc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cngmohba.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bqvmuhps.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2emvdktyb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sgfvvqyh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dxorvcwf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2uckcxvjo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zbbiowoy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2huqkcfsg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hzrsgwke.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2deaiygwo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cyainocz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2eptozkyn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dmjayfkq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bxcdppns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxkrnhma.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2htflmcri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpbfsiye.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2jdixnfag.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2liwhyeyu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sfsywhor.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zorqbhek.html


<!-- 参考信息 -->