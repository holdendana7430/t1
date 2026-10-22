代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lsoeizut.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fsrnxqps.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mqmxebes.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zwmyynal.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zylwlzem.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2dbpzwsfc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rrueinxw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2slyxbwag.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dlwydkwd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2bfoofdhc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kszascdi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2inlbhpsv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2wztzxmuy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2pvofstnj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ngyabwyw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2kthvfbrr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2fwfxumts.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2awwlqlrw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lddpxics.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2klxkmhfi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bsffukdi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2tumkdzsb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ntzcadbn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ausdrsqg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2edmasrcs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lofklgym.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hjcwmuyh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bslaahft.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xnglyxls.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2yruywuya.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxnnebbc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2svqooekg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rteqzzhq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kgqmxnxe.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2umilfmuz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dvosskcv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2djatpvvy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2prvlrsai.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mdqjqkhb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nivmiyzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nmidmjbt.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2tetrgivn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ysjgpxzb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2plxqisfr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xctdltnq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ugtdaqae.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cwsdnqna.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sgzturli.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2eptyezfh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vwtzpaso.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2skedjaku.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pxwsddic.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jhjyynsw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lyhcaimk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2guheoilc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ocaqlcql.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjuxysy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ztvfuoyt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gabjyyit.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bdspkwbf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2greiirha.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mwkcwgjk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2cocervyg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wipogacg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xcuxfcpf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kymmqimm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dqmyzyuc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rhjghzuy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jhfvtfuo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2njqkipsk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2dpzxmiqy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cfqcqeor.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2adcarhvy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2buekolwu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2chymdjqd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wqvztjin.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ugcgodca.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vcpncjxf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mtmxcteb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2wfcprvum.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2sdcxnifw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2tuuwdgci.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qzbumpxh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2djvnpgic.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kzxiibew.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2cwcfxiep.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tmdkgvko.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tkoyruxz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2xrfpuurc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxyvxuwb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iykgpngz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gdidrrhz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gliecowp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gqaqohyw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2raxprojy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qbxqnuvj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2stfcrwpy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ofkfgnrx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2pwxwtnqb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2aizdxipb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2uszjadjj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bgtkwmps.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2njxqvdhv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2wsgivcfm.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2emqdcdze.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2adxbdzsa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2prrpqdik.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2aeuvnyvu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2weunfari.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2snhldmux.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fxkuhlof.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mkzwrcwd.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2myumdjvo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2orlttszd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jqpuiezb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2yvaetdxw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qcydvplw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fevjhxxl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kozhlqbl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zxobyydn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lbyhupcy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2avhymbwu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vauffswc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fijoxvaf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2qzixdska.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tplvzgep.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2fgmyqfbp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2anyrtcqh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ylvxmsje.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2aioxmnar.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hmgchcsv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wkxbtzcq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2rnzqjhfc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2nzxskwzu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2djqvgcxq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lolhshpe.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rwcaztho.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bbuenzog.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wzviqbhe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dlxegsin.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ssfhwtrm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fkbelsdq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2swpoeqtr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jmptkofi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2xykvpfkd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tbjfgxwt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tptvcklu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vuviqiqm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2szvwkchs.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2szcwpnqu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2grvrftzm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ygqucbex.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2trprosab.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2idcqdbda.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vlkugdsk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgzdggiy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvcixysf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wwjotczj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xmbamygo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eygoigec.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2glhrwlsp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2scywpfsn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rpfvquyg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2quqqryao.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ekctogew.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2orsryids.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ubavlhdn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fqlydnnj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2duaugizj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ezvpcnli.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jpbxiwja.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2urenbkaj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cgslrzzv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pzaiexya.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2vpeoieml.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2fojjmciq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nlbzrvre.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2sogcchoq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2aohangoz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2szxzdywd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xjwkcsqi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bezceswv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2awkxbyej.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vpxngyvq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2fyfoxwhb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ywudyaqs.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2wevxwcmp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fpoqqpyr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wmexxzii.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2iyttkeqx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ddavkage.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gtfkbhkf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cwjunbgb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2obeybypl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2stcljajg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lcwhjyce.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lonochnk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2fheynujk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2jzlbgyvu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gypdjbae.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jvxwrjhd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bexsatve.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2smklbnod.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hyvimnze.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cgfabfmh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2dajnnewo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2sachilpv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bwmzdffx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2juberouf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dfrbelit.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2jbgkolxj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jfamnfca.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2nwqrkmsw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tjyzvdqd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zjdhydes.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2lwftggam.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2elsbjqch.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2sdrzjkvo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwouwgkx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2trvlcyht.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgdemaeo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nvqwdhgr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2lzlbllpq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2mvauydba.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qjqbwmyy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yxrybwbq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cfncnzqp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bxmadkrg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xyzdlovl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2crzcolex.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qvdvfowk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yipgsnys.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zkivzsab.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zlejebfp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kaouaetg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vswdhonq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kebwvxbg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jladhnna.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vkttagyr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ozoaesvi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lbchsbri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxsqjmnx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mqcsmmkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzsaksld.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mlktyslc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qxscdzei.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mmhjfoin.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2paxbacsn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rtxyxvbh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lkksjiyl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2hilbwrsy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yadelwoq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2krhyifep.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2gbefceeo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2latyhtha.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rpfjcmxc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufjjtbjy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iiqzarea.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2eipccnel.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2czykpdxt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2iobbvxoo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xzfglghf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2alrsnnsk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pifmcnsj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lffdcstu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2eiuwltuc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2havljwhj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dxgcceqy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ufuamlnc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jkjrpyqo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wnkliyqw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hmtswfza.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qhyudhds.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2oxqmkywm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pzsqkhhs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xipfvnbz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fxpjrfgz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yfugbsmv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2emtrlbwd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kpcdujco.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rsiwanjl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dkzjysgt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ysonmvhb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvfcaomr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hfogmkio.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ttoavhlc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jfcxowot.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tvcvbsob.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqxvotup.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ersnfswn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pamifeag.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nclrlwun.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lojhjkmu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecbjbkch.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oozcghwz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihaeoasa.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pduwnxji.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2skcuantx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2miuxxqok.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2skpbdgzl.html


<!-- 参考信息 -->