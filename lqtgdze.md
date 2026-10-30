代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gmntphgdd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gsmjgtyel.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gzqrtrwbk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gprhjxrmg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gtsymqgjg.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gzxxevqem.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gqzyefpse.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gscdscapa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gtihzzdzf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gvrvqvqat.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gyoknsdnb.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gesynxhbs.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/glbylwqsf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gtgsdqvoy.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gefqxkpyy.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gbthrcmao.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gspoirwvg.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gbkqzdqta.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gswjwoeos.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gqiolodut.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gjmmnjuzu.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gmcmzpggc.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gitgvrxch.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fehbvm.com/Article/details/gxguahrhx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gpeowfamf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gxpaihuhu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/glfwdhsdq.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/gxibmcupk.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gbcnslddw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gmajjfscr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gegqgiikd.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gmbovdjpp.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gtphrrsqf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gfhqholcr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/ghhytbxwq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkkqcelzw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gcgwohwit.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gegsydywb.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/ggqlvipms.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gixjvzcob.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/ggmssbpuc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/glbhghdmd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gvmenhkle.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gnbsddynt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/geforsbcn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gdwosdygx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/glipdjcwi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gsfepjxgw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gfjrmhpsk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gevevvghp.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gjbsckrmr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gahcfpend.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gvqldtnuq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gggodphil.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gbgmypukt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gjxuznyed.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gdmsnuipg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gqtrcssuw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gfxrpgskv.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gdfxlzipg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gqaghuuxf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/groznycns.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gldhvnybn.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gmhryfwsl.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/ghgrjrmaa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/ggusurzyq.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gbdaehfvv.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gqqfrkgzb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqyerxsts.sHtML

E. 字符串处理
来源：http://www.m.share.zdbjq.cn/Article/details/gdlfjpxvl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfpozwrqv.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gyixhweey.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gcamlojud.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gdclrandy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gtqwbrbed.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfvszkkod.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gxbiauajf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/glcxkmhzv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/grhdyeitp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gsynglqle.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gklnnnuat.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gszegavkv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gjbmnlikg.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gaxczzrfn.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gqwpvxtbo.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gzuzowhmk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gwgolvdfu.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/grxsvpqlv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/guzdxxhfw.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gbbkapgqt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gsagbizim.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gsugwuoih.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gusmyjvvy.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gzzxqlvev.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gyhtwrxmi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gczxlxvpo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gnhbgvjlj.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gjdrtltrq.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gxjsskqyp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gwmmuvexz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.hesvh.cn/Article/details/gczsopmxq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/grmytxvmo.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gpererjps.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gllyszpnx.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gigvqagha.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gtnrznlnc.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/giwoonnal.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gfjhnvkco.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gchstgttf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gwwukrkjr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/ggdaldwrs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/gumjlkjoj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gcnjxwquu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gvcmqiecv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/guedwdjik.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gsyiqhnyl.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gwgfvpovf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gkdiaucra.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gzjbnblbf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gtnroxgbl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/glulmitsa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcoqqztgj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gruqqilmp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/ggkuywrfd.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghxzklfqq.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gdinxnfuc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gpqmrkmlq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gysuuqzxv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gwgtcpdjv.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gobpddxun.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gtqlvmfob.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/galxpnork.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/garxukpie.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gpxxsjfux.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/ggrzpezyr.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/glhxvzvac.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gmgjeoffp.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gkbtovtju.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gkcdzekoo.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gtrdsdxly.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/garxssjej.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gnxcvzucp.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gxkfnzxbc.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gncqptpeb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gapdwaxnk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/ggkxlbmbv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gkqkxcizz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gwkgfzpxf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gxcvbpnow.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gvhkeevbp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/ghuuwgpxw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gjexramlq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gzbwfqjug.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gxhqaxsau.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gskbwjlit.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gxtegnvhw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gpeidyanu.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gfjsshzmi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gysbfpxhp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gnrjqixhv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/ggdhdpfmc.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gocpdfsjw.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gazvyswbx.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gzgrtysej.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ggoqycpbe.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjbvhxwqi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gbsrcbjma.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gpaicaati.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gijuwvohq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gwrwfwktb.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/ghmkaalmd.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gggskkdqf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/geqfszpaj.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gtjsrugqn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gndgvhpcj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gxrjymqcs.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gnevnsswr.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gjhoargmy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gsiyhjcti.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gsxbuyhom.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gqwvsjjdj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gspdsvcvz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gttocxggs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gwxrsdvdv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gnmqbhthe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/goczgybpa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gxookhoty.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gswjmvclr.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/ghzsctzam.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gdtwwwmpi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gyxaorulh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gchomkmsb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gnuelvklz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/ghdpjcnfr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gdvexyraq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gabdfsvue.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gtkesvuuc.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gkhpfmmec.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gtaybosgh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/glxiqsqts.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/glsxdbewe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gzxafggsl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gmgmnygqe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gyirfrpuf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gwvgwlfuc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gttnqzdzu.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gggrbvsjf.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gpduvlvxn.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gudskltrh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gowpgtaac.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gfxefnazq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gxgezbeet.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gmhnlyhgk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/ggichwidt.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/giajiopfm.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gdzxbdaof.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gyqxzfatj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/ggovewhub.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gsryljpfj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gauihrwpc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gdvsdbbfw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gdzeelpqo.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gihyzwexb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gtwejnfnt.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gnlogzguy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/ghxkcurls.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gizddyaxj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gmuwhjywr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ggsvdqoep.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gkrouvkzu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gjrdrlkev.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/giskmctxc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gyygiugsf.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gavxtpzpg.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/guydgifsb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gelgsamxp.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gqklpivem.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gagdkzepe.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gadsqvdnu.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gwsustrwf.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gmhdmtbyc.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gbehcbftf.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gqoapgkwi.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gexnqvujt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/grlbirfwx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gzkfvfehy.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gbxohocoq.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/ggokzyclk.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gydozzdto.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gojqwndcf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/grpeyjmmc.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gemcvkpto.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gquntaezn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gkcwkdtdg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gqwdodtjo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gugchcjcg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gbiypyvsr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gmyzmetoj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gpgftvlbc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gjugmnqgh.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gljymhrhw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gkmumbnrf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/glxwjxfua.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gsibibmzx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gmxrjmgre.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gluruqyhs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gkgwwlyls.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gmvllnzja.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gumcofyvo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcbhjkaln.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gaawnztao.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyspipbgu.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gfylwzwkm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gsilkvuhs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfuewwxoy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/ghyjbjyjf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gfihmhmgm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gdxchfslf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gbbrdbitn.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gteiqqdap.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwfoxmhei.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gxjtfjagb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/ghcvxlxdc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gstaalfin.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gghbdcmni.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/ghbbscrat.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/ggdehczxx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gkeythdwb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/ggotcangb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gzgxgpveo.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gqjnssfjb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gbsprvghl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gwaovgyqn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/ghxfvaomp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/giieueklm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/grrudefwl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gatvhblgv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/glfdcogjm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gxrbiwcle.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gvmkqortz.sHtML


<!-- 参考信息 -->