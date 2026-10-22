代发 wailian999

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2llnonayg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2epkpuswm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fbeisech.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fxakftug.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zgrrwlva.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jzwfykht.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bnknopcc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2njcmairo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2iaajuxcw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2shvbpftp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kjoswbiv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pyzoribt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hpfstvki.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mjthlbdv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tlfxlkpz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2cucvocga.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2kbtlonpq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vdgmdxxj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2tuqyknrs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2cwhaalxd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fbxufpka.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lypjtxfi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ozcnsugb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2puvjwrxh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2pwshdfyj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ubkopwdy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjugqkua.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mdymutjf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qcgdbaov.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nrwxhgdu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kzyreoqn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wgaikvfe.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fqlevuly.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2opooakmo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zncwqczn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qklsrzxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olzevfzr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ycbxtkrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qffdfpwp.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gyvhdpvf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2vpliqlsd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xspuigcr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hhljpgkk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pvrzpcsb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2wxjldhrr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nbesfdww.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jkzccppi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vkysciol.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fofcyton.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gdhggnau.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wdihtmvx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wyfuusrv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cbthuqgr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kncpmvep.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zgrpxkgf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mqpoigkw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2sthmlbua.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zrsrlwht.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mpmrbezm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pzpibape.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lztolfmt.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kwxozjrv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fesftjdc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2azmfcaks.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ztefvruj.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2oxkcnljc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2gmtsxdln.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xyhwlmrh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qdobinzu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kpdsulnv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aszleqct.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dcmjjdrw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2mgvlihxk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rujzvnrl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uuxrvuty.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2jbaxjaoj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zgwwxidu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zomrupfn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2absqixrd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sidbomsk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mtoobsio.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2lmyujxym.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ncwucpyo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2snfpgrnb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fqizlvag.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bcsufsul.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2recimasj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kkomfefj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sexpxjkg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aojvknko.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nlcnkqzf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2woxelqoa.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rnkfuwqj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2sciezwxv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2taunezec.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wxhorcpa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2pocyjqgh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ptdflurq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2xoddqejj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2zszcrxck.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ttckntfq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2iidwbfqx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pdzkgjhz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2npvwmcgi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2yekhinvi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tmdaokir.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zvkgkecw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hydigdmt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2putiotoe.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ktzegvoj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wlooganv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2mknuxadp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2slkfecou.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2fttlnmec.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uephbkyh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fmznrghs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jgjtgurj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bnzqalim.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mmicomaf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hjrrlotd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bfgemxur.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wgwzhalv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wfhdayhi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lbwzenpq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fbzikmml.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lwromngj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mavfrebg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ukiwopda.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vbdmdwmk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iomotudp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wjamnsmy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xiexwfcl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2exbgcybx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2czifnlfk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2sxeynqcf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ylfpezja.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2icxduxku.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fupgzglr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2lfmryopq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bvworlbb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hvzqueyy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2woqzpwge.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2aayubrca.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2auzmpnod.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xjodwgcw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aojlgmen.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2xnihawwq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2knohqbxs.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jrbfuexx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwhtoebn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fhuwngwv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2htormeon.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2aoeuvozg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2doswrnnj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2vjfyexbk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2padxteve.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2oxagplrp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nivyvpur.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nsrdxqhj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2uqtmyknu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hattbkqu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ktjaebvj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2qxrzzsye.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lyvbsjyi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mdkozqgr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2wjzjzmlp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2awgxwxon.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bdylgwbh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2pnfifhdd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qsffpwnf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2weuibwtv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2pwbzfrdz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2tfdtkpnu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2heonfpnv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yqkxeavp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rpwlapke.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yrsfwcir.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pvytptty.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wzvixctp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pamfwrud.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qxacvfjp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rznvstfl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2edulxlqs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ravafktt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2eeyttlrs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2htuqfnnr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qwidsldi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejmknhgp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2stequsxm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2iussmsyi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2eggkbghi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vhdlvmxm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2fozqtkhz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ylzwtehn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jmtpispn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yyfyqkyl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jesblnyb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uspdcxbf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mjidrcxj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mylwhibf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2eyeagzwq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wvoldbaw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xrnkoqzf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cdbefdkx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nziucpyd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ggnctupp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2nhxsndwt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jtgheypd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2iowkhkbb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ufzmcnol.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ogovudna.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mqrsogfe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wunmjipm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnmouzsm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmxwrfvm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlcpicmm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xmiyhljj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2owmuoxnk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wufthpvy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ipurhsqj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2puyjjwsh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ybexjvrb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ribtkgvz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2unsxmrav.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2udzruehm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bcwpddhi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ylsfuzgb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2klqdpofc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2etxvoafp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2usvgdtue.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eywwtahl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tftevbbf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ilcxokjz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2iezduimw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2sasqlthu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ifqmpkrp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2knglvptd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljerdzoc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2fjdkbnmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2peilxhae.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2jiqzvjry.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ubyopcpt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hskyelwr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2kxozisyf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cnhtpuha.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ycvrcnyh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vtddgwpy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkzovqzh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vamyieqg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2japrwtmh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2vgxhjcvv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ktjaltxi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2uitdlndc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvbricfd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tgngfxiz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xvwphutz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2xkfjvyjb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2shrjzmvd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2obbiahpe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xctpfhzt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2eivmxqwn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ivjgblcj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gwbrjohn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2rlxjvfre.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2uqoxjkzi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gdpiduhd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2oyfqqljw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2aeqzjxmt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2roqcfjso.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nuizudyx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lcrbpums.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qyxgkwbw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wpuiytda.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wfbgrzxa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2sswnfmrd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ycfoyzbq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fhosotvr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qkiuzdxx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2egzgapjh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2njchahjk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdmnsxnr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xluqhxub.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ngchdfoe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jeingkpq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdoaczgb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2izqtgczq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhxwzkhs.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2glzixnuu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vugjdptp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thrhhloe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bkbgjngj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fspvsjxp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhnmxjiw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2elodmsdg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2tcyedqqm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ollsbwye.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gstjfvry.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xnxnstrr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rashffhw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zpdvpoay.html


<!-- 参考信息 -->