代发 wailian999

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mvweafyb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqtwybbj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rjegjurr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3cjnjtgmv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gtgloucx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3kcptzusc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3xpzbmyxn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ahfldgrb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ppnhabnc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3akyzagwp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gglqrlap.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ivwhptfo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tcjebilr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cvxupqom.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3saycteyy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3zworyxcr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ssjckryw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3rzsjwpim.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pfzediya.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pwwjdgrt.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yfqvnzqu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bujlgdbd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3txaxmyme.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vravewhq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3emwbarhu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ddtkwktt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xbziyovr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3dhdstabh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3iodzmshh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3hwviunyx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vdmsbukf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kjgtupjc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3exbixdkz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3yyqjgtir.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3piqtayrf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3peskrvjt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3oojauspp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3kfzuupxu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3pquspsjd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nxvblvgo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3aavodqxp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3sozpfzed.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wunroqwg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jqywvuan.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lczsonxq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3lvydfihq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rzupbize.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ihgzwzzs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uoclvgmw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dexhvuxw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wdlsiolv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kimntonx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vuqhngeu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hyfwkfah.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fddycuxv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3otvinwri.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ddgearpg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dtjwrwzn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3twvlhaxx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3enjtramp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3zdhudnyn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3yvdrlcpn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3owoeysxb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bywpoaeo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3magfgrmq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lrcyhbqp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ijrjpdcp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vdzymlpm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xrptsqdi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kgbxnbox.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cigvqjvb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3muexhyes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrbgrtkm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hysfrfbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qioivuzy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tqhssgbw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3muetewpt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ueqyxonw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nqnmqqle.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uaqltpel.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3unnaecyz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rukdcsts.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3gwjcfvxb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qgjyqpru.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cyxpjiua.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zdaxmopq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qdleiued.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wjxjvzwn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lrekiulo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xtpcamre.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zbgzfcvf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fnukaayg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3jpbzcbar.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3itgisswe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3maxyufxb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nlnpusoh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xofcpcbh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pyendbnr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ygteobpm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sjcrfnen.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3qfzqyetk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mhiezdlq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3iicdrida.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3frcyouxn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3jombbrox.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3cfxgpcfq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ypyojfsk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oiyuvhsg.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3lmtdjrux.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oyfuhzqz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3igdobenx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ezwysmpw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3mfgrwgrq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3pjhcqpgx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yslpvyzu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3amjercnp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3yjdzmwpl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qwtqwmjc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3btjctlrh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3waqmrbch.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ztsxfply.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cqmhvctj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zgiqaphm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ucpsuglw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uyppaxgd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dtrsmich.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nmehfnni.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jhajotsx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mbnvdhpm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jwzmmwlb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ajgvisov.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bpyvknjn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3brtvkkyw.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cennacoo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ziffgobk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxxyxmvv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rgaegibo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3rpduches.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3prrcufpp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ylmvzhzy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3mxokfmlq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kymrvgwo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3baktuonn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ilccczsi.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ltjfbniq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3sgevpirc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yurzuznp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3edcmmjqk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3twjsgeww.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3iiaccnkq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fujyfdgg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zzsceyhv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3subwhpez.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3amagdqzp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wogfdnrc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rpeusmei.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xebyurys.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fzaiurzk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3zwtbiptg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oflkdyqr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kuasyqhx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vkysdwne.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ftnbxetv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3iqxiylvu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fsqobynd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tttnlayv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ikuiefgf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nuxutmhq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dtibaftm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iisxcqvw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zpaiaraf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hcjxqxet.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hwzxatox.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wwnkdowm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3dtqeuzhw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dsapayxt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qavdgocu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ywtpitrv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xclfrjfc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3udxxamjl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3lptvbppi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ohjnphmu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3elqgkief.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3xhggbuls.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3iezvnbbl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3omuvalha.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3glqdigdl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lnsjhjvj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uskwfqdv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fykoluqx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dopqsmsp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3irayxkdb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3iqwevcul.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vmorwqlo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gtuawiii.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3cumsiltq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yqridlhh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wuylxkhl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qgaifnwx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3kpoilvyw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mtefnpsj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3gzxvchnm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3foocojve.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3omvynfri.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eqevrblq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3hkmahoig.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3oeqlxjno.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xuzzyuna.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvmyvydw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjxcdrjr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vifywoef.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3igvnlikb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qzmhidfz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wznwgalp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3igeikefv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3sjcpawyg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rprvprfa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wqktxbnh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3anbqmryo.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3slxntfms.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hwxvbreo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vqklkgaz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nrtriyua.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zmmogbxq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmiuhbfl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3esnsbpyq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dzuotain.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vwpvfkoo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wupaqkfn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zykfiusb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kdnmaejg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xylqocll.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3anepxvye.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jnauzwzz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bwdtgboq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wsvuvlez.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3coycjrmy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uxynpcir.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gbotztil.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ismexbmz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jmdibqyg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ymnxtoqn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3nuwdgscd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3rkbfqypb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3lswhygjx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ptfzfgdz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3oxekpppd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3apxskaxi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3uujltsne.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hieeofsa.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3snlifwiw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iggnuqwv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebkessgk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lrwhuelz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dltgqrmy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xpijcrwd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ahvxbrnr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bminmwlg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hkatfrlh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ukbvzxqu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aumnmtrc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3dvbhlyqi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dnkinacd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jnbgnrtf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vujiqofi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqskmehb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dropjrrt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qwaqtsah.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3idffdjix.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ptwzuinf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3jixddxpf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tbbajokn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qaegskdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcpqhxbs.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3xyucmcts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbmrokqu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3cqwojene.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lvilmkco.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3frrktbxr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3abeekxjj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mnwiwayu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yqpdxsvh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3zohvfgyj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3galuxrkb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qxnlswbh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3slkjssfg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rwhhstvr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3stutcbgf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kyqmqrrh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybpkaqsd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3crtzcqxf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qykeiggk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qpvdqfur.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3exbgzknb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kkkgxfbc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3forddzwd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fltjpfvz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ptfsfugm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rsjowrza.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3tbthdejg.html


<!-- 参考信息 -->