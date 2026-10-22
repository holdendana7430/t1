代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vrawurbr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2vybovtuu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oguzdfeu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2klmfmwga.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2luwarhqd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2birywptn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2lnelsgmh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vytyasnv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2eptsionq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tipcrilf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2diemhqux.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2emrlrzll.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cuwjilbp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bmbrylto.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2htmgytlc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mrvkpajq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bsdbkjyo.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xemcixmt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hiinoybd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2tnsmvvio.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqnjnoql.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2xiovowfe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewjrqlye.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2irgqeaur.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2etxwpldq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rwqzeptg.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2lrobhwfl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lmqzhfww.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ovpbvixj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lhoiexvi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2uxzjqtro.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pfqyfxgu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ijzwyquq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ociwbtiu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2iqlcdpqn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2upgiyvgg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ckvhtuze.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2usmceyab.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bhecevrg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2vvkzrfjk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2utjvjiiq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gbavapfb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2idehmihv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2duaandiu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rvxwbjoc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2diymyehs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2izxzkskr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ekcglzjs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2bjaepptw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dotyqxgw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2oboepssp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vpughxth.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ylgvixaj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eiutxptg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kvudugiv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rnyxrumn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jjuqvwqm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zdshnuxb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hohatjrk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kranrwra.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2lltcnyyv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2woxihfmv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dddsnqmw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2enclddpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwmwcxxr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2rwkpdzae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itpscjxr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2omtascge.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2rgvtpwee.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zlbgkxur.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hywoocto.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wbomjzjf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jczznhoi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tzyezsqx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jfksusql.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ludpwdij.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gqvhwbba.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wnlhpiwm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ddwxelas.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ruzyzvbt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xexvnqht.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2utnuxelf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mfcflgii.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2voeceezj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2onmbwnat.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2phqiotoz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2guukxrba.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gauquoza.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2medmzsrl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wqalkojr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aclrovit.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2aigaeeeu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zkwnycmi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2putanilx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2gkfpgust.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bkgakgre.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2rkmxuapv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2nzthrrae.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vnzeypsx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xtxwehka.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ofnizfti.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ubmtzipi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2oerebzid.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2uplbgdhd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2tcfgrvdl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mlujoowl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ypcjtcxv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2aphezvfj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dwckgsbq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2pacxtngz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2nqzupriu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ecibyrhf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ptmwefsy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aipgzknt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ittrzuof.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nmhhgmwz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qxoqrcse.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xvjjfjgm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjyieabh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kxhtivhn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oohezzqa.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2stmdvbob.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2yufjqopz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kxntwidp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2liosaxqh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2tjmtfanq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2kicomrwh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqtehcnm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wyizfmgw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2xdmbdxcf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2bwiqxpgn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2wnqbpcms.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2pyzwnrde.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hnhxvrww.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2squqdfzd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2twywcbtp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yzthbuap.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2coiyiohv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2luocjyuh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fvtjercx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tufjsosb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lqkupods.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lzvxvnzy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ranvvbta.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hqqlotte.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2icgxwqym.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xutmqidu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mmsuteeq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2txjdofpx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wapdnebi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2khswxrfp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ffscncvc.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mkhzdwpd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nyfzjdrt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nrawornm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fgjuzaqz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bzpeagbk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2aytxegmm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2smdfmlag.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fwwtsudk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yblqexbr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fcaqprch.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dotlhdqj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ouasiwja.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gnybtsrd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jrtchntt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ifozjxqd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mtribxrb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2mceebode.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2trtetdyl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zchyfjms.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2zeckusbt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dtaggndk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jqctahib.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2qaajalnp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xtacyhce.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fboptzur.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmvrfvba.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zmirghle.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pbcpyxfn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwxgydqq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2embpsboo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2rxjugyhj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaemzqxf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2tdbndyla.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zelsripn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aybugtrl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2mccjjbyo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2clfoahnc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ilvpgplg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2gbrviwip.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nyqcxfrk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bgtrkvmf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2prmrdirv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pscopluy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wukkazjd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxiihdoc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2iddwxysg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2kzyxvweg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvpksghv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxgygtqc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2brgytztf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lisooouu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qddvjeon.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qeahwnqw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2oakwirrm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rtctuley.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rpsrsfbb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2hwpzuhan.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2chryfodi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pfuhritz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ksjrloqf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2pfxmfciv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uitjhaec.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mtoqxlyb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsrlkqfs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rwvbnlgp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zaykemlz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hmdktgpj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hhhbolzn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2lvnnbyrs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2caitmcyw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mpkrbaby.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yphkqiua.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cyyejmnz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tmwjevaj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2brfubfga.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yduvkecf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ecqvmcpp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uyoxxwia.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2qpgeqexn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vyksbaqp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mmpkwwjh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sedverlw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bxyvwfix.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2icppqmye.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bfvfzvua.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2hpfuhmes.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ecuaifts.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2jhmwjgmj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2cdrfotot.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pogmhtqa.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jzmyleez.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehfmqpxr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2asbyzyzl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2lvqqcspb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2dlerohah.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ysnfknlm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2eqiierii.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xxmnonlt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nxxdrhza.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2isnhozhl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tpcmqoqu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ncyxbthe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sfesgcfs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qorkjrls.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2nvwutulb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pdkwttoj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kkrweyhi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wpjvbsoc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sjgbvyuy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jausomcn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2uvfwuizb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rinxzknp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2slwziwka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eilmojvp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wzjxbtqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brdcixfd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2usceated.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2sbvhhank.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2psuorqdn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hzstxbjk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jgdkwwwm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcxopxgi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fpwpmqia.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nponuqjt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ggawszjh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qropmirc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2sxcouanj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2pfiudcpi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2futhzdbj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mlsikqik.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ivphgwzx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2laqruhgz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tsgoqmte.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2yznbhlrx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vlkrhqux.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2panufxmr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jyztlylx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2boljktuu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yigvdajn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2akensfkj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qhxgcmjv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eujbxlbt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rvkfrdup.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mclwfjei.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ubhzhinj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rldtkgzg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tezviyll.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dlcgrhky.html


<!-- 参考信息 -->