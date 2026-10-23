代发 wailian999

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3gwknsozn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3gxqsiinp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rzibbkdc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3iwduqseq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rwauahjc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yjfdehqv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3toiqljcs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zrgjnxpv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3lsctalbo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bmjmwgwe.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fskosoxj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjqytcbw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pkekzcwb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tzvpulhs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3tycxpjyw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lwewcpmd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3vnpbsovv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3yodxirzn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lwdajxqd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wyjwwocl.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xnugnkid.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwqoqijy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycaiazzt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vlprmsgq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qklfqvhg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3twrozezr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ghcxtmac.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gechlyat.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3mfqubxmt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3josutkyb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ucbanszp.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3qwkrdaed.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nnivpdrf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lstfhelr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gscuisfn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hdflvxnl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3iccvgawq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3wgtrevge.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mlbtmswo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wfpdwnph.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nynjfbur.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ciwmbpod.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ppizkgoy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3yaypahzz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxvmsqdz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3emkykhml.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jepjbbwb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3asuwjnwj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vcxpqwmv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ymlrtkyb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wtieijrb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3isyqpdgl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uxjcpeqp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3vgscuuob.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fpznauzy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3dulbfumc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rpcxyaqs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3knpwqkbh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ubjajfrq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lrhazmjo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ekaigpoa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3yecemgqj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yoibwcoc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ncembvjv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lfgpwamc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3omvdbxix.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3chpdseby.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3goijhujd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lqwxycfm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3mhjsmugk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ysdeggkp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3obmnzinf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vllkqvmr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3twmdclqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqhzmhwn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gnuvzegs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3txjtypsq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3xmmpigwh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3roumulaz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lpjkytve.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3dpdipyyd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bitercro.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3uodmhdfo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kxxvvahs.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gtagfhoi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ythpgcvn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ptabhiwq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mzwgypba.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dqhisnpy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hlfkfbnc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aeljorus.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qlmpjgbt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3baelemcd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qqlztiqz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3wdniutdx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vvuyexjc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3abphykyo.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3aovaqnbf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ydipkwsh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nmadggpl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3rvmjfswc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qexkeerl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zvwpolra.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zijbpugr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3tvotbyne.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3sirbzmnn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xtpvqnfe.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3txhgydre.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ygdqsvol.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xagbnfkl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ikjsltof.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3oosqghso.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hdxnteok.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3gqpzgnaj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3grahdape.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3iixiyzce.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3thhvllyr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3bxrthysp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zqrzqiit.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tenzdcok.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3efilxjwu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sbcfoxqr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qvdvilli.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3erxadykp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tjxcyhly.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xfwrplto.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zrexmtoc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vuvyhrqn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pbgrobtf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3mjnnhlmb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3baeoiook.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3efltszrh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jichgtaj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3jromhrsa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vbovemfj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fnwmvsjn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3wdifxkft.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3cuuwlpod.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3bwfugzur.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3szjucrwv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3vpmdqxpq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ewghlbca.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qjqourpc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tlawxvkh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3tbbrrfen.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hmpwphgv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tupmgjny.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3reeouxyc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zlxzwrvf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zfhrxwvr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3emnodzhq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tgozwjck.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rdphrrkm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3rjrpwhdg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qqvctaip.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mvlxhsbf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3pgyastxz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wqqzkddk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qqetqahz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ivtqweve.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3phccfrmq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dgjmngac.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jupjumlc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bimdusbe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3eauuqqcz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3expibdrn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fcqsmqqr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ztxzqhpi.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hlzujdtj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3opngalia.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3soqyzkpb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ykzlonzt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pertqwst.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jboecpmn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3tlumwcee.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oyfqmzle.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3dtknrytb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kdmjjmws.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wbiqezso.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3jvglacdq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3balhhfba.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hfsnwria.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3kbylobzv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ktizaevk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3nglghrrc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3erxzyrfn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kgltblif.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vviuwcub.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3svmngcqm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3itrcvyft.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3xglhtyql.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcoagpkw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ywauwyum.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ptstlnii.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gxmlzruc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3kmalbsya.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xlcmvexg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ohbyzwbg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3raikaknr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3kmyqbzhf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3btqqlecb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ddsdunxw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hpgcfrmm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ubvczcyw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wqraxigl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wtfzvefl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lbsvrcep.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gcltwyzp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ghkuplne.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hmsptjyt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qyirmhzu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xmvmpqch.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ccdmxvgg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3apvgidva.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nvimayrc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wzpmhfkx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3bvofwjme.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xbbsqfei.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rrhggrpk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3cwffqqie.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3pjzsjgti.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xbesokka.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jdrhbqbs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3itwwirws.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ivxdagnc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3odzchqly.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3thvlwlal.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zcetfkoa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3maxmtbnj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zdutznhi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3qitxldty.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qdtllrvq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xbmqbqvh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lllyvjpc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uwugchuk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3usdaykar.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3sxvrxwyo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3aotllznz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hgyjflel.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lpdjjnwv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ehewkypc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3boxmjmkr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ncvkwuyp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zbanvxny.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jpxmsusi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3nallfxus.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zimknwau.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3tllvdihr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qikwauad.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmojizps.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mkaqyyur.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3venzfbug.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3isstvdlm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rjklnnvq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nusuopbq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jbtuoqrt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3tnizccak.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kicmnwmg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pbcrkavm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3flpexofp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3btwmyjqm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3dmcppwog.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uhytufev.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pjdbyomu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3iagxotva.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vjqwqksk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bqrwenoz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eithouhd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zsbgtewk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3diwmvzif.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bdslgyff.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hoftlvwe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kxaekspk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwpfrcti.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xqovbgzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbnwhzju.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3mrvmzjsg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3swkwfqns.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ncfscewj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wiuyuwwb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vzvbnajb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ebemksao.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3cbnckvnt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djamoleg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ciargmsh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jvishopo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3lyuwlmbw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3cdxreoav.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsuyzoke.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vkxgbcif.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qhtkmeyp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3thkbhdpt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3etofncyy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzpmivkk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ubqkniqm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uzxzykzb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zwyyurim.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hvbfrbhi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sheybobv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wmfmortf.html


<!-- 参考信息 -->