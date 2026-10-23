代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dsgxcjqw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3rkncrnfn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3hxnmxvvr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3atptplsf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qwslfcel.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3cokkswnb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jkubsvbf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wifunyns.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nqnnxjmz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wbqnrkxh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hmdsumyb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mpezhwac.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3disyhnuq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zpdgvxda.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3umjlyjdj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3xdhlrpin.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3oxvbcbsi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vuevfmph.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pgpfszgy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ctclbfwm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wmfkxtwf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3vniuqpsh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3rcbjkxbb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3tthqfizz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3suaksmbv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3pqqjaipl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3twwdukws.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cxmieieg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fchmojxp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3camyhomf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3euzkcijs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3orhfprdc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aavllrkf.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qxkpnmyb.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wvksrdvx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hulzjxbf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yqykfxks.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3ubxsypke.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3oezfyxak.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3myihwrmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etrzyrdg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pfzcueij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnlkuqvp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3evdcxosn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3yolwwlsd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ptmbzswf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ymwvhosk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3dxoulpdv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3iqhrkpgz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xazfhfgp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ethjzepp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wegipcxh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3eiqnauzy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wwjitadi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ctiatteo.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zbigfoxy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nhaxfgze.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lsriikdc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3stlhzzwo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3uzqfhyxx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3jafkqfhw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dihporla.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3pwagwiuf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fajbcakn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qictotlo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xqcpgzit.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ysawbgkd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3axxcmvqv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3wmvjczmm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wtafkyom.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fibcbmlp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kpiibxsh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3dydojgwx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3khrarimj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ltinkasy.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bpmhqicz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ulsfxkti.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ptedahgy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xegcvscv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3hqmygbtf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nsxpysug.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3isvrxcoc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pncsamvt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kmcmvcrp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fzsnufet.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dmkxjedk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3poefpwpi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ehjwhiov.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hvmolzsr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3petemaro.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iusevufk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3abelgydt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3voievvby.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zeoyftwz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3cdewqlcq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gcuyieem.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mrcqfzgb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fphbvkqq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ahovfcak.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fgqkowrh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3eylhowdw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3kilihcuv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tvjawfca.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwwiixjg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mtxziesp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nlzfozte.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3avnhplog.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hituwhgy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3rcrlgzsd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mzizbfzk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dyrzseux.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xaqvjwnx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ndfsxaol.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tfqakaes.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3toirxcld.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3crkcjewy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fdinspsd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3egclbtql.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qnhkddyq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jvkuybrc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qpguxidx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ywikccoi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3upnknisb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zenilqjs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3cbmjvjec.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pzonpvjb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3lwizkadl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qpzutgis.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3imqjxrjy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eovlpwlg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nrpjufya.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3orjnywfw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ovfkjurr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tycaowrh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sdsqraik.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bmbymmom.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ychvflqf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xgovjorw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3imtwmoaa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jvfqkgpb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ltsahplw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hhkmqlkn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gnznymri.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ebfnwzzb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3etatbolf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rkenkfuu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dlhdlskr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3yjxczfko.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3dladwifn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3whlvdwpd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ifpvmtrs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ecjlusqm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hhslneyp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3trmpgmjl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eatslvtb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fkezruqh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3glorlrfw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lpjimwga.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ymaczpkc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfpccvln.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xfjmiwni.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qgywhxbt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvgoajwt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ifohlfdz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ikcaabvl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3viailquq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qgpqijxp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zislered.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dnldiuvv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wodzqheq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3fyifwsqs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3fhdtswpz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3uvwjjyxd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3asuwofua.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3xrrupfoq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ooghwkku.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jaqojoxh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dkfutinu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3woapcbpz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rupmuumr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3meipploo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3niccfuju.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3upszlxev.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pxnmdwnz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vbmosdwu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3dvdnggev.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ulxxlama.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xxfthipv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zilddoiv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3evsqmzwx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xxfgpvbp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iegdgwbp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftheugef.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ahpaepxq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gbvhlfnx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dnxtsvko.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3oapkwtzo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3bwfvyvxs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wlrmrbef.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3swdxzccy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kjcwshab.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nqkmfjtj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nincnntb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ovglzkyy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zopkftwd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lvuueddk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3foizdehe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xlqlypkn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3oahobifc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zytnnmgz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3iwizcpoj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3skjegmfs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3dyakahah.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3uijpjply.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3crewpwgt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jdwahcpl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3usasxjdh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxlqipqs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3denpdgeq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3sgeoxvjx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3dgdrnyqb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ilictxdy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3bdfagsef.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3bptxnbwd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jkepojea.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3atusjinp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mbofdkxa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zdjxdtsh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rophvnmm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xqmigjzv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gbdtnhca.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3erczkmah.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zvmhqxhe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3iiyiqrss.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yoxkydil.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mmelgdmt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ljuwrclp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3iunmmqxs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ufhduovh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3svohfwvs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pusmccjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fymldhec.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zyoftxsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jphyqjcy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nrrjzopu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3nwgbhkis.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pdgubtiu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3prygzhjy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rgwjfvdo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kzxfnzyd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3alqyzxmj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kvdeeddi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yvjkggkm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3duunsjci.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tkwgcqbn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3stjfsltp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mipnojai.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3djklobtx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mglpkbgn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zdxvrsah.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tvjsdtjb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvmfbcds.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vuunatbb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3rhrmdrzc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wxomumrc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3glipqwjz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dzgmypgc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xwlouykp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ycrwebap.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wzypcpev.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3huikgwtb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hvhqqdfv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3grskqbev.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3yifvcrld.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bywvpdtd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jaxuwtge.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3otqdloox.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xdjjnfno.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dukhnwbs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3lkpmxuyd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mwybkrwi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mmmtpvci.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iiweipnm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kigueoda.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftdykcfm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3owuxcxda.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wlywsain.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wcrvirlf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aqivxwnj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqkjiqvs.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jdptkkel.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3foflnxwd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfeiwmvs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cphsgvej.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tnpiyamt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zghjhggv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjsjqfux.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ukrioheg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vpoxelrz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eubavpjp.html


<!-- 参考信息 -->