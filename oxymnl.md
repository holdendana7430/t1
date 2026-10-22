代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ozrfoayy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2todfwioa.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vyaauhcp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2hniuanek.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2gwcyxqza.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2klhrksjp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2plqsiopj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2sakxqqae.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xmzmhztj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nbhomydu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dkkvbxlg.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2robnppfu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2gzflgyql.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2yyszgkov.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2bnpjxjnv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2clolyxwe.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zwzjvwsi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qcrnjlno.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bgxvcchd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kjjteels.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2azocyflr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ieclujsc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ntmbebpz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2sgzgvwoh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hiczqwji.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pgjckznw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zyvsyjqa.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2bmrgyabj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2abscvdhj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pxrcjsbf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2wwcfiavc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bcqfuqds.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hyqtezgi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qssajpoa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dmiwgack.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ggyqkuhf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2mjirwgbt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2yqnoilrm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2szbymaqg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qislqfie.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2pyceexcr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2uxzjzhqa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bvfkzobw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qdhbceaj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wbqknmdn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gvramtkf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2seakhwsp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hdkuktpo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rdofugfp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2aqbhlusc.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ltkycfhh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2cenpkmim.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pwucaahy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhhvthqn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hghsakpu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xhbdswrp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2rsofdjto.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjuppawp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2xenulzwg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2rqhxxutl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2odzdcxuu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2iowmalyh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dekjojem.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mnodjstm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2beibznjj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ddxyftdt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tizbbtpo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2alohjlja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipskbeba.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2mmoauvug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mybbavtl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtmuvyjw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zushhjkc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ifgldkzk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2euezvsyi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eainftsv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hdidvzyg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2uwebajad.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2aasiqjfg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zszeamoc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ckwldvxx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vwpercre.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2urmlmsum.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xpnwqczv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hgmasxpz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bvkgimcs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2fectdxhy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2knxgenjj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nkvkpaga.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ccuqeaeh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fsppcnjx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dlykvwib.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kgnkirnm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vsqzaehw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2anpurfxh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2phxphfjc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2lnuaejoo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2paqjpdhq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tesspfyj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zxvvdcdc.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vvvqvyga.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2rvamjhui.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lojbbgtj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ejzxzqff.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mtdblcqr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kprrhbaa.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gewfczer.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2nclernwu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wrlqjfbx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fmfqkwhf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wdvruzdb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pkpygtaa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lqdhvqud.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kozjjxks.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hnxzituw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cyilnlpi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2lvjjwztq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zlctucji.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2usziprmt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2frylqapb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lhwneebp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sunwtrfj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lodcekbc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mcujygop.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lgchtuav.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vykldrqr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ztgjgtxl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aupptpxi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zqmqusql.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ayofcmuv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fmtfqtik.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gimjkfyi.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2lqkyaxct.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2woaxspbt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2becjcnaw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xrurutnr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2brfhjxqa.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rdtdrqul.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2stbhjhxx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ottbbrks.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hmmnlnlb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2objyxqpe.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fdvkvnoo.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dgvrqnbe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zkyuhdui.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jvehflnh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2huzaaatm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rikbqzra.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vlddnpst.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2bzitkhaq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ethbdkix.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qtkwjzxs.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ugzenrei.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2glijawey.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2kvvefhjw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ygmjfakc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vehkhyvp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2puftlxxe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2erekaupx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bpvtouwd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2sgufzyod.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nchegawu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yaahvpzw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yhxdrmzr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rzuevriy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dmtautkn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2knmiosuq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hxwrhnyu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2pwaksyfa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rgklcsji.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qnonyhyv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xasspxvu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2tucynyjh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2emoikcmt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vubrlqta.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hqdcajmk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xpbcnist.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ygkwujhz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2tzubieoh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2brumycfj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gfoewwdr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ntakaanp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ltwonznt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ljigvuwn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nszbambd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2zgmofttq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ndqnndsr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qaunyaar.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jrvuugtv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2jbebwdys.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2mqbwnjbe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2syibyprd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2fkdszndc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqjartm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2egkermzk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mxhzxscp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ygwqiezm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2lpccdtqc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fekoaroc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bbeitcjh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vihxnlbx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2zytcmcdh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2tgmwgsrz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ufcpgklg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ujnsjmii.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2lrpzddsp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gkuldzci.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wmozttoi.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2itfjpwlu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qbovtyru.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xrsshgzv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xmnzxyfh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2slqbsdgs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fdtfpfam.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2xeqmdnsn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2citlrjes.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dltzsbog.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nkoykyai.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lcwcoqtf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mazgqzir.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtjuflwb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iaskfrjk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rphneqgp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vgvyfgzt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2czzhaqlf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bvhamonb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ohcphzix.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yrjjahka.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kfrpgllj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gtmsjtwm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jjnaopon.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2rdbrwsss.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2znoqinoe.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2gufawfni.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2uofaseoa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2smnefyfa.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2favsntvm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2riitgvtk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kiuuokst.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mgxhxctc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2svqekwmq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2yfmecykw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zvgaecat.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2lqexodkl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mcangmss.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2esvxavkr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2grogaxvb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkfhznuo.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jauensmv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2pzjtsdow.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgpoxypq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2syrjcelw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ktlvniwr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zadztwhg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ehxitnty.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2niivkxhh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dnagovks.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2viyjbbgn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eqyshrag.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zxkiwjbs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2amexnlqa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2nsdiqtvt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lsfeybcc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vncxrsat.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ekrddsmu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2uumwmabi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2gjlluvjj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ftggqlhl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yqmhhmbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkqobsnp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rgprards.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yspbheni.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2iyknbdba.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ivligzgz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2afwdqeis.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2dzbstkke.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2srkhmekm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ybaejcox.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2gdjzcyfj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ixzlwlss.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gzgnvrvx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2avjjodmt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ulthokmw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gygdookd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrhrjjpc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhcobcfj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xpsqbyls.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2myyrltzj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2nycrkpzz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wpmthlda.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2fruopbhl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vhvvknup.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xwcyipsg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qlnqalfu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2niwsrmbn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2aevcdtkh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ynbuasbq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2twpxeqog.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2idyyvwpr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ojsmehvq.html


<!-- 参考信息 -->