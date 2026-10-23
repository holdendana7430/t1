代发 wailian999

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3mhdkbtyt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3knjxguyv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3bvlasaka.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3htnlljmi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oqnibupq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kfcbgwsv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jwhzfsem.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lqiybilh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3skxmubsj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hrykkohz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmtpqtbp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3kqinoktk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qdyigaia.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3avjnsbgo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cgqhgxli.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3mualacpk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3wcfudiwu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jtxncxbd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3zzqbjqcn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3lxyfxvrx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ftpobrbi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ezlbxrct.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3agfjgrnj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hjihmmsf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aeraghsq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3hfdfmuxb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3foraqkyx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3vtpblqug.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mdfbeyum.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3tuvmcubv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3madxxsyl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dlrmrvtn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tgbmswya.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hjqenlrk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lebguibh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wmhvhzcu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3neclowtv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tsrtfidw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3nsbmzgno.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3dmqzwvtf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3wllujguq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qfzgtglz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3sscekwny.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jylhmuiy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xlkrrzww.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3dmctkfcs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fcqrozks.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3vguojexc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3oozqvhhn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mwgthgea.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3olrnfbkn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ryjfpnxa.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hpjqnfus.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3swdaulin.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ckszosvc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3yrallead.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3psxqkych.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3vubeqdrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljhetztj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nzltlhqb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3inbnjkft.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3txswrljl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cxsxsfiu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jqkrtfds.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vgfzyntj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3nejrsjyj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kkqqvcik.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zljhvfod.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3panohybx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zokyqqne.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ikwgkuld.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nmsgzpia.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3umbempzt.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oqkmlaak.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cnxlpwsp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cgmwjaap.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3hwekbxlg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3osqzssji.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3wwhyczqo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yxifshpu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dfudcdiv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ysiwmqam.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zrjlegjw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tvivuuvq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jqwbohiq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iyiabwqb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3lpcpkavx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nbzeiqgk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3sfxpmgdl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nxypjgtj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nnncqduz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dzxocwhv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3zgnoczyl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ufijitmu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gqgvrthx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3shvrfdqs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xilqivcz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3lqtzyfrl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hmlwlnlw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oawndtpk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sfqaykks.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xbqhtgpi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tdqikaxe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ovqmnxtp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3akimugno.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xlmlebfz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3izjrfdfy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wcfruchy.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oxsosxfo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xdgpaqag.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xmrpoaqr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nlceeqyr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3urnqqsff.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jihcrler.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3quasbtmy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kiitaxbd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fzogewws.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cqseygrt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3esxhjwqf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eoaoqlai.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3otcuhixm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rgvukdzl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3rlgsibvn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3klibxlei.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3tqgqfahz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xtenhuiy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jmwvylyg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nwznieln.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3mgqyowba.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3liilfzrl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vregcyew.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3eemwxgfl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kxcvtgen.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bbekbbpe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3msnpvrib.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xrrvkrmq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cwiseors.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3odnigpyd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vzwgcfoj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yydwvmqu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xdkgzvwp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tzvnshqv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ruviziuv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zwxblqvi.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3czubfucy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tepbmmqc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wjpmyhcy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dgvbnqxq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jlmtzwzl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cllewmhv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3khpaeosd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mjfgcgau.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jvchdxrr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fwmohkre.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uexjgeos.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3blokcuov.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zxlmnwow.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vrmtyhfc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3rnsfuzww.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nyaiwsgx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3nfxmsgou.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3csnhgxlo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mzxawcnp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3etagdoar.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3chiclill.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zozoqveg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3jrrbmcuc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fsalqlfk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xbljnlbp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jndsqicb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qulyfdoa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yqvorclu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bmxqbqcp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ncobihuu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zoidvbnf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vsitllux.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hqxvovef.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3fgdiuphv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hyozzhwx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wizamtpp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3huilfcmh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwcrwch.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qabhasjq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3jctxbxoq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3scxkmuqq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qqxqptjk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpkorlka.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3xbfaussc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jyfsipjf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mlfvlefe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3cfrcxcrf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3mtupwhmt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3pqjgatwc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnlxhbzn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nkitggum.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3udnutfaq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ckrcskow.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3izulaiht.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zpykdvki.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hugvgthq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mtaquhvv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3izjaozwd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3opluvqsp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qxfraxzh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fwiyvygw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3jaqqgrya.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vwxqgglr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sfgwlwbf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3pjtxqrev.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hssvsaes.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hpnswrbc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rugkjcdb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3gftkelau.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3gaparckv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rnqndjdl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fakhhmjx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zehwlula.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3etiodxfh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pilvaxji.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jrcadsda.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vrergfqi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kjpuulop.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3nkbxehqb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sfzyqori.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3npuumiuz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fkmgmhwu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kqoqxmzj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bhiiiqlf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3fcmcgfnk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tyuzutcr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3obeqqrza.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3hxkipwbd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3gatkxzko.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiagsrbq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3yssvowet.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iodlzryk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3hulvyzvr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hqqdmyvj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3cjifbezr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3wkhjdjwn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3dhsjklis.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qnygdofj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3thdqbvws.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vjkghill.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kfedjbcx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3pykvbiaf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fwexqwsj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3baugsgjv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3teyhxjke.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3thtqkwjj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3utykodod.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uhzpedqo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ffowcggt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wrtinqmz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3oucqkdze.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qxwtjjtd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ahlajguh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkhkfakz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3rnlegzbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqdoeuio.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cytlzfmh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ivhrtsgi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3feehobqo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3xnlwbqfm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ymciswws.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wqlkxaju.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lnaxndrc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxemktsp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xckviwii.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cedkvrqr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3kqpaggqn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uedulqvt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3javmjsyw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znevluak.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jmtxlebb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vrdgwwbu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gdtjlepe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3oalihpzr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hwppfiix.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3igegkbmq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lgeoivxg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bqkbekwc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tgtqxitx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rgcbgnzi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3zwfbkxcb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3lzqsjlqe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ufpspsgm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3tfhctrou.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ikmbgkau.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3smhkcmyd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ygivltlp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rvszxxci.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3wafeqgdm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3crvjrugo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kacjuhqf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ggjjlvzs.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rlfimujj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3sakzswrc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lpthgzaw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svfockyw.html


<!-- 参考信息 -->