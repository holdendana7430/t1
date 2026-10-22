代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mifalbtt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ibnzfcie.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2imegbvwl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vyrobevk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wblnglhd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jweofwvh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cwuyveis.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ucixrloh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qbnuztax.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vzyrayss.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zhvikvnh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kamudvua.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2feoozpxw.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjfzewgo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvskblnn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ttbnqzog.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ezjcwevv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvqqybqr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wtptnpdy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vyvdwopt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2xuktqdwl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jypulzkt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qzhmlvxz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gunquewi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xfubvgvh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nfeacrck.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ozkrdwpd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qluydtwg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2lhxovwuz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ojqwwhsz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ufylkxnt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2drbpfzyf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2reshalfg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rgfpjvml.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2naalilap.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wfldhrcq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2dkckwsah.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2gllsrapa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pottxyvx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2mcdruydk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2syyuvdoe.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bfmmfnrh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ntairnue.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2azqazlsz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2uksbuiek.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xobyaahu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2atvqghut.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kjnmbgod.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mwuzupkn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2smihddbw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2pmltamxh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zwlxkjxc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2axkldgqj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhqvkoqj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jphszsnq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zqkchdba.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rczymvdl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oxchopcb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kjxgriaf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rrwonrgy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kjaxjyuf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vtwwkqjx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ayuuqrox.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bigpthef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knwqccpd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2auodgikd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocjwnzrv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ivkjihwf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2thytnkiy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cxayfrjf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ajcjtjwd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ftwcxikr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ogajqzbt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tnixyxhw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rttjwhbz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ewjornog.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2avrqpayp.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kjktmifc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kftrpedn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qsxhwwdq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wlmtvkux.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zwwgisab.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2aobztaqo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xixpxfim.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vvqjcypu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2huauqmbl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2ovglakco.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jlrldgvo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vrdqsmaq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mpruicth.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zfselntx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iaxrkygi.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2qmpzuevb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2gbltxytq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2iuwgarax.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xrwhgaic.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2flbgggyn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2biblbwgz.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nattdxof.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dnlivpue.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2yeoxdtvs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jaeuprfa.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dgcpvcmb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2mftiyzqh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ipllndjb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2lbcqkpls.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ffilrony.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xnkrefda.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qowcaxhq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uqluvgpz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2pnzjmwca.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xubyqxsy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2dqmfvnfq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cysmnomk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ugctoxkz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2daswxgig.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xrrfoztg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nhoxacww.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gunljptm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nfzkgopg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cmywgkgh.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2oznfvltp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2cpjmxgtd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lnesfjuk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dcmpotsz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mrrshmbm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2uiegiwwr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtrfuqwp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wcemirdd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2sbhzvlei.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2xkuirkup.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vwysqbrw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2oyjjtxld.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wcbbarzv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sambdykr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jyzfntyy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wryhzmor.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2izmkwenz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gamidrfx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2llqwjzwa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2alcrdowb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2dsmucoqo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yryyrtwu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2arcqbyzo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gupkhswe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wndvjhoc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qfdqxbot.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dqjyeddf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ysrrqfez.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yqdnurkj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wpepeaad.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qqaqrwpq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ikjvwvro.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rcyjmtsk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yrkpbpkn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fbibroyw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2pmmjmmka.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yrgfdsfz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eesmkuur.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2adqpiklu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vzoqyppi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ixwcenfm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vsxkxmjh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rzvaukel.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vkmdznfw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kakjeoqn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mgzxuesz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ypzliere.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2cfnnttqn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tycnaoei.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qmfkkqzl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2pksjvlgs.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2cevinmnx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dqliwxfl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2nfitpfnn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2cnivklwo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tzvhfofw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpobbhcs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgefzcqa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxstlcrw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxasybwn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2eiwuceoy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wwctbgfp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mffgwyuq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bhkwdxbu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2cxtbsklp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xvkcrvpj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2emybhnll.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llgtmgkf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vrpqtorf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2zhdubvwy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hdepfzhf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jbqndgki.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2sqjimdyq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2phmaayto.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zrbaonyy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhliokfh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2cfbnsope.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2swczoery.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2klfvjffq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xcqswifk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mrrknfvz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pnabedpg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2gblrlozf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ltlzmypb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2suqnjnbm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cavbccst.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ownupwgk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2uklbpqre.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gvuyndgz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mvgznqvw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2chwghnmr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mnrburaz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fcbfshlk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gedulpqg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohzbjtgd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ywzlyunq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qydwoxbb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fmcnuylp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jrecjvgj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2evsnhvbl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2btnswaka.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2iveiymqw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2adconvkx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gniizeyu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sbqkoamj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vokmwwrt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tzzoonbv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2rgjgbivz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kjzkbvaw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ymmorudy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qstkouwv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wybkzqzp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vrapaock.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vvvdesgi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2iijazbaq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xxgeraxm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ifqwekvf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jvhohrqb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jkgzxhft.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zrkifzzk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwwvrsrq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2apkovcmz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2admxmawe.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssamrshn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ecrwyipo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hoomncta.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2semalvjo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wgkfgqda.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yyebmljl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mkayqopo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vmsrmmbh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bosjfbom.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zcrzutfm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2giuadebb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2volfeqwj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2daeszzyj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ottwiivz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hlzircsz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ynxhzuxw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2twjgptcc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gernbvsc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2nemogeuy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gtzpgiea.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zvxjknfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmjdfkfy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rdmakurp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqutovhj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2cymqrzfj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2fmvaynqf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2olfiyqvi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vzqzoltj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wryochmd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2czakiybc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cjqiwwkq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpbzcivz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ibumkxli.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2cetjoytw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2yfcydzqt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrknlxdp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgzneywe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ktwwikxs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fkawkcre.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2yqyowcqq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2qwkkvpfo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2beufazor.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2kzjivzmp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2huciqhbl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rinnfirv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ccnavgtl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yogckjof.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qzlchihf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2oheriqzd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ocylrcwv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uylnbpvx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2rrgdharx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vxpytisq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dzqfdekk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mqivbfew.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2luhvtcns.html


<!-- 参考信息 -->