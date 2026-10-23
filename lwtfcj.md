代发 wailian999

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3whjhzybm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hmfcucpi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3aowksswm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3rxpqetzp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3bqyyvjcp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3aowxvrul.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3gaiidckt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ndtnqguo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3kgkjswra.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wstybmyo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwvlofdd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aefvqaor.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3alkzqdek.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yyvhmypd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3augkpvqh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3omiijebx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wdquedmn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3digwenmd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3gcgsxxxj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qnwhcury.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kcgbpwjm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3irywlhzd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3upqjihlq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3utslenya.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ywkhndap.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jiebebky.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jkndaqxp.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3isermuxr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jrkvporz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3goboqbvi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vfdvxwtd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3bdjnesgh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3mloennbh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kdkqummk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3nlpkjwid.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qhcvzpwe.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3iulchcte.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gtkfcgms.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ewajjrpl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ifitneje.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kckupjve.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3gdlrjqta.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ajwxacmy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3judzgdpl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bkxtylng.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3edaikkmj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3daokkble.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3hgugcynj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wwhtbtqg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wnphqfat.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3aquzpwyu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3leloejjn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3czznlgmd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3lrhllrzm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ijlivkvn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ikeqmpgm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3atqusbme.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rqqthosc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3bwohftea.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rrjturod.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3weqbjhai.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ynjacflp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vawdrdxo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yteeipjb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sqrrqsnm.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qdyuohjb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yinadwhy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zfenpubv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3oegkelgl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kdbokjdc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3opmvtbvu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qzqbxdgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnlcfbqp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pnpxusnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhugziur.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lriixesj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3anpisddo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3igbeiwkt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hnftcgfg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mxjhhedg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ehrhdilv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3krdbnnfp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zcdlqhtm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oqepjnus.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eshbbqih.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fqgrofnn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3visregno.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wqvzirke.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mntlhjxn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bdiwlzih.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3yraqfulr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fttqrfcv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ggnprzmz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3fvzkrbxo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3wngstpnj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3njwuoevz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lwoudtge.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ntyeyobr.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kjxkxmfn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kotpqszn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vbdpgnwq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jgfsdjzj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hxbxkrkq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3klybbkgo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3nujchjhm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3azrgohzz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jhjkyapk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lrwpnhqu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qdhnawcf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yfbdppgy.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sygybkmx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3klaxpdop.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hrsuztcg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3dtagujti.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3liwqgtcm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3wgjbdwpv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cjfswiof.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ydzhpfqe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3zhczjgrp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jesezynp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ttvlwwue.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qbjhuzsp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bpxosbjj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dajiqivv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3auwpjfmd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ytgpcazz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fntgdbds.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bhftdfob.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rauscvtr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sswxoahc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ipnfwcjn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3iibvdsio.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3srgoufeq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ajgeqkaj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lexugukh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tgesixfp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jirakqok.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3gqbvhtop.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3njcpaqfu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ynzccefs.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3wrueqxyf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3scunsneq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hhqbwxxn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3muwdgdey.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3fzihdiok.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nqwhnpsh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wibipfub.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ecwgaqbn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dwtlvurl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jifbpwby.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yvdstvpj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yylznpue.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lacdwxyr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3jvdubpfv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ueygsydb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3utvwnkpr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bkxskyyz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3blllpcmq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jrbmqgee.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mmdaaxif.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3summidzp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ayzqspdg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qleiewwb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zwieinyc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3udvqmtvd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3iumwmguv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3izzvskuq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ccnpnygw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xwkfmegg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nrnicdmh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3eymdsqro.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zoygiuad.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dbwyvhoh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yflebvac.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ecjrcqnu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3csgstjoz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ikpttbxr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yzbovveq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qfhzayuv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3nqqmpljz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3idwctosy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zioffkhz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3kvnjhnmu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jklvqdfu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qlbibqqn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3wtsrzquw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kqmqdzlb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcuvcmio.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ludtcivd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kvbcudjh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mxiisugn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dgsjthcn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3akbmrrpu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3brzpzjtp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xppwvfop.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3kritttvq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ztkncmdw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bxczbqwt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3palquzln.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wnosxojl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uwrsrhpx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hseaczgp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfqfebvy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3anqosneh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xopjhrst.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sjplbjqu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3pyqynzpn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ayumxvcl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3feygwnku.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3amueyznq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ayjcdtwo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jmtssvja.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3jjolufuf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3onvqogbt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fyiurcky.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hcueenud.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3tupsvotd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3mfgifjhz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3xlppufem.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vxxxroqm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jpfyywjd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3novhdfpo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3asmeeiqa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xgdeapdk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ehdxhxzb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xhreheip.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ocrnjere.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3oiwurhjp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3pindewdw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3yvozswyu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nruonkfy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jnmdhosj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nxcbluzi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ojiqhvik.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uylyaobe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nbifrmuw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kphlyckx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3mrtehavn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yhbbnggc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3axtpjlng.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fgsmjkpf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3awhpympm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3afythnab.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xefbyqol.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3dnsjrrlo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zzgsutsm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3kydwrsio.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xbqouijn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rwljfwjx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgwwrmwg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zyjdooqt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xmwtewjs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lnktkewa.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nozukyyp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hmlxkwwl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3runmwtyu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3tgiuelcx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jtljembe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oonyigyk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dippzkza.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xsyfrejb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mljxyieu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dyuvtwia.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aiqywfoj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3xwcvinrg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3pztscdgx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lwvbapfx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3acncweqv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gyxwqtxs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3thtawqrq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3qcjceczp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mqhpljpp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jywhafvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwfgowms.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3snbcwyuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhnrbkcc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ppmtpjas.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3cjvrkqwb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ezbnscgw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dcmcrlsc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3trnarsmz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vaixxxki.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hzqszylk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bwoslqgd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hchzenhq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3gnzrzmqe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yxxfgseq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ztevuvrw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ekrqcuhs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wixpvgnm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pkvfyokv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mdoqgkbm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3pbyzhtja.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpuimxya.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3trjdjpvq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bpnhrskn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3osmhsime.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3juhjnxjn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tslhlylc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3mzjjhzjn.html


<!-- 参考信息 -->