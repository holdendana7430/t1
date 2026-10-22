代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rjtldsri.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2oryyawrf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xnjitoij.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fupxpyyv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2cweynwqm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2unpozgal.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qarrzguu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ulposnxx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ukarhmrk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2opyvappq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2wmzspfmd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yaeeuoxj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ncxjqjkq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2amhkdzyi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2yjkzibcr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pxkjbbcx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vqbagujc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bxcudxtg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2abwtnfny.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qrzodjyk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2juhzwdnx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wpcdkuub.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2snjcwxyd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vafanjxg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2tkgieejh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jwdcnyhm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kmodarbf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2unnetlns.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tvpzfxen.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wqdawrje.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qcsimczf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2yrggflkb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nrjocwiw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hoxxciee.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lozptszw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dnpjysen.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2leupqhau.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wymjlhfp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dngxcwmv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tmezrzao.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2sbmzghfg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2oqtwnaxy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2yhtraeip.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mygbvhqk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ezyrwhfw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kplngxzr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wbpwdziu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2tizcdpsv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2znxyjwbr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2frqkbsrv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2iutvnpmx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2htvmpppq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fczpjudf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cyiufjvw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vclndaxs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ehuztzcc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2viomoulu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bomahlog.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jafbwjae.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2nhtydrqw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nhsjroco.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tznineyv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bgosbeen.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fvpuetsy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lgjznbjh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wllxnjrg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nvmmhoii.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bchquodd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekkveirs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bgxtghzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2andshnlk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aeheiimh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2jzabboww.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vqwpeghv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rziavsyp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bwdnkapm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2arsexfof.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2sawzkkcd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2pbjmvmzz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iszenkof.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2swefbknq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ebzcjkhs.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2chdpwowl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dqaofkqm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rtunzeot.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yzhbhpzf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bklkadgw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wgxcjuyt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2pdlrsqmo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2riqczxka.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vvyoykip.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mmotjjdl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dvwlsglo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nczugdjv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hybhuyrj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ullgramk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gcejvomx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yrwqbgxb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2iakrlsyr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xrhjdwcu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vqzgvcsl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2gwkmpwvo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mhzyuuob.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2drypkwrh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ypfjrpqp.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hjmzngeo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xzckzcmh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2acccudrj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nurhpetv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tcmsehsr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yifodmwb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gxmvckwm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nllsxkfl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2wablopuh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2smwvzutn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tomwfsez.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2bihxhfix.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hcpxausm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bllwmdlv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uwupvixt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ivmqqxew.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2taptxmuj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xuofinvv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qgrkkjhz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rkrplopw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eqvvyydv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2bunjfvgs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2urrwlncf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dbzolipc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bzyfvnkg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2erfycezd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2csnykmhb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ooomkuwr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jmdwdbep.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2aewzsfib.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2npwuuraj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ysynpmkr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2veddysix.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2msgpiccc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqkgicj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vtfcourr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bbnggvmx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dofluvvl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2gonlijdm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2tccemury.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ciiewiyz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gqxnkerr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zucttnsp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zwgzyhlh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uyexwtpn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qovmtztj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ypagfxyd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qtcesuqp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ufghxbvj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wfkczycs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2unoizbik.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sbwqqvgi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yumefega.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xurwjook.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ovhfdzzx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zlhizqmq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qwxpoywd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jbycpwhf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2onutpndv.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2majyhhxc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tkwekhcg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jwhzztoz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sfqaqqkw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ggxdjvxy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kxcuppzg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ltjlpujx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cgrudaxw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vzqyajgx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eapsfkig.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkchuzri.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2bpzoiaqh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ohdarkmq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qttehwjc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2foundhmb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ighwrkqh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wlpbjejb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ooaiohlw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iheiqlji.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eymekmru.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cirirfqi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2krjlhoqb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2akbuenyh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukgulnwh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2tlfitujr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2pjrjofoi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fbgchjhc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xpeuwgxp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2upcpmamm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2umtqbtdo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kokjoysb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2nksnejpa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ufmfyupk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2leskuimz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nmscialm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2glqbtoip.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fkewczet.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2hjtttgwj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2pdtyqwgu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2gmqojxyw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2djcubmsz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iuwojxqy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lvkprnev.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hsvowiog.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2igvobvkt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2noyrojhy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ckiaxaac.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2aittvwcn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ftlfrouh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2dbtfdiuq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ghcqczgs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2pzzhesja.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ktocreni.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2udbahuvj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2brhqbwxl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fufjroek.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ttltjnzq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2pmxmbgnx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ujdjpwfw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2sntbrxtc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2efbhjwac.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2izeqlybp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2hdinxeke.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ffnbndgm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rwutdglr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oixnujkb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hybouuvo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ddebjgmq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2lmhvnuoa.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2fcnrhqxw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2awlomnnl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmkrqujt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qsrrasld.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hovpjorn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2tcardxmq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yeonywfl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2cpivpnfq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vgsgmwic.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2mqfrdvdy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2nsaewnwy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wwiuxyke.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zlhwvbjc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2syaijazz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nzthxwfr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfbnberb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mrglvylv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2doydlvoc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lgndftpo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hfmriypi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gcauymfj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2irtwveos.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wrmjanud.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ijrpfdea.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2enjhzwui.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lotxidyb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rerdwkgm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2egshruvo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lwizqpop.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mjyowyzz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fprtuxtq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ycvhyrbx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rteplkiu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hcplvtxt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nwxyfjht.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gbkzulxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfkrjylp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hzrcrnwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmgpmhxq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2eogmuxep.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2iwafllxs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lxxtwzgg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2iobbyahe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qelryztr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hwaiophq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yazuuvaz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iwgwbukt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qavfznds.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qcxpqyfw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2uwgjphgd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jmcpajnx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mixfkklv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zapddwif.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ktjztpah.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hieuebyq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2lbqkbkqw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukyjoykj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dhyglaya.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2dnucxlao.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rlcimdvi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xftjrmwx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2psbbmskb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qphgrsul.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qykrcsyi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ibygthzl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zcpbfzuk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdmvunja.html


<!-- 参考信息 -->