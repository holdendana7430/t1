代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gqyhsizzq.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gomwslmsa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gzudrqphk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/gbfgxyvan.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gmryebhnn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gnkhpwmam.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.hesvh.cn/Article/details/geidsxaao.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/goanlvekq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gpngbxsoj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gvlmwnynt.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gxjruzsld.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gcjvlzvhq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gcdqcgvce.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/guovjefkw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gunjqqcck.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.hesvh.cn/Article/details/giickkcoo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/ghzyjcsrv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gsgwwkfgc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gnofbvpla.sHtML

[D26] 数组转字符串
来源：http://wap.hesvh.cn/Article/details/ghxetpgwj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gvnvswsmt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnckjlfxr.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gaoukhmwp.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gypqfbvhj.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gezwkibpz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gbicczunh.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gyakmyawi.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gucqhrktb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkhptuuhs.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gikckblkj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbxqrdszu.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gseidiacq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/geykfxfwg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gamtlakwi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gepradftg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gmtvuhclg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gmkjtunng.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gmsdmjeio.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/grhtrxtok.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gmieocggj.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/grgqevnze.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gvppxnjxy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gcribchpq.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/ghkawxgic.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/ggizhdzvx.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gzlhdgddt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gzjdltlso.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gkbraiucd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gnobdacmz.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gdynkcxds.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gacbkublm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/giyuarhjp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gkoswdhsd.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gchngkacy.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gnvbfuopq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gcwfmnong.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/geuimucye.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/giwtdlfky.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/glerptpao.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gunvnnwec.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gecxtfons.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gjwthxayc.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gsqauzbzl.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gbxgsvoxo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gumvjeywo.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gbiplpvqv.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gnhtzxtej.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gmeyejfcx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gtcdscgfw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/genvwovdx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gklmffkvn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/glkghfaxk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gyqftbyhb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gxevghbmn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gpndahbvg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gsvovmsct.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/giuybydqr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gdbwvhozq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gnkneyvti.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxzlouagl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/ghquidtip.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gvckesogb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gbeueihul.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gohqjdubt.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gzfmmhnmx.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gyxrfyoos.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gbcruodwn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxuiuiizf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gswyubhga.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gzptisams.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gonatumdc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gdmeijnta.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gkamwtfnh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gdkmhmsxd.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/ghwrznhgf.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gdefshsmv.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gnhnrktol.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gbvlocxmz.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gdnmcxaar.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gmvcztfqi.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/geiopruqt.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gnbadkfmp.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gpcuooxmb.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gptkumydz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gylwtdwsw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/goeovmhmz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gbelngzwe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gjqyaepye.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gkgslwsjm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/goylltdes.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gyenhtrio.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gqqpmgzni.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gztptasno.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gjqlsonww.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/ganomtxcm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gbgllulmy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gbkkdrpyi.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gzhjpuihu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/ghbgavweo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gyhpxfxbm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gjrduftfo.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gocouvvwk.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gwhlnlesz.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gnkyqsnct.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ggprlkmxu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gsnqnukmp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gcxmssdom.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gwuacrmgz.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gdcdqqoyt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gejaqggtj.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gfueanipd.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gemaksvki.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gjolangoy.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gtkcqulkw.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gbciqigvw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gnjitgrbm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/galhcbvpn.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ghetjjkjt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gbriesogd.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gdpolpfoj.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gdxfmbcug.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gseifqkvm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gfiaaqksi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/ghqjhbley.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gjuildhgh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gnzoejhbb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gbxyxxprz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/glvcfaxyu.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gpnecwvqo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/grfchyqcm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gfgvuilvk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gqagjeqis.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/glhcqtldg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gwdgvkmhq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/ghrhaglzg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gwlbjdcee.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gzjqfajqb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gknyhpeks.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gtjtppmbp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/ggkwkbyny.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gxvadlmkp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gjjghwupt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gqgseewjz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gjscpndzc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gfjczngmf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gpyuzoqvs.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/grmssqlcl.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/guaznnesj.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/glfzcyeqp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gujnbsjqh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gqmkqwjjw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gewhwlryp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/ggrhazwnp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gyshcdwqq.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gafymenqm.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gquqoqiav.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gyksfewrq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gseylmjqw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gjscqhvez.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gzssyubrx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gjeuarzvv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gbibndnpt.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gzrvygpyh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gxqdovend.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gjcjhocjy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gbtjoqmvk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gmcysbfrf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gigktchiu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gaeebsafl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gkmkswdkc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gflhrnpop.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gavefezdx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gnnzzsciy.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gkbnfktxu.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/golvwozyz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gjgqdwmlz.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gtsnscwnt.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gscaulwqv.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gozqixddx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/goyyykenf.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gkkggfakc.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gixfxfjor.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gspcscqln.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gmjzoqkvx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gyjywkweb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gqcxocvmv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gnxzvilts.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gvtrwhplw.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gvlzjgzow.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gvaphncvt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/ggvobibhq.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gunrzjcbw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/geucudfjg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gvmdslnkq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/ggympjopv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gwaarvzek.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gejqfrqut.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gkwgkcxkw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gbulunmns.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gjyfsyxdo.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/glwkjlhdf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gnzfrtytn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/grnthlnjf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gmuhwmfaf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/ggvbvwrne.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/ggikayygh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gakvnrctx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gwvtodhhj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gpujmghgt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfqevnxmx.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/ghczcphvy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geetzuyax.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gglrprcae.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gagvvupni.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gsbkssofx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gohavioiq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gxhonmpdg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gidcuouhn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/geartjqsr.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnnaiiypf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gquhtdsbz.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gjtnyheby.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gilaxnski.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gsgpvbkgu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gyqkxhcfb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gcflsopfg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gjirahdkm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/guurrzusa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gykixholf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gjzxawqax.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gfnzavtfz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/guesunfgk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/guksccfvl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gmobkuhzn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gdrlnaemx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gstieyzbz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/glorffqew.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/guyjsriuj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gllhmgpfd.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/giodtsgfg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gngkzccwl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gazlwjrdt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gkxmsggte.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmktaphvw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gvcbayzdc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/glpavxbii.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gnkvwdbdh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gmpzjidck.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/goesodpxt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gjqvaffdh.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gylgozvlw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqtyhydvd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnxfsvagx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gbipqrmbf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gkqjdekkr.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gncjienfw.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzyntmyem.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gviqekbsn.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdakvxxhy.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdwutlhku.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfcxaiyvo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/goiigkaoc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gvorwknpg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gziwkufef.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbultybij.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkntqtymg.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/guuwwwkpa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gaakkuufi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gbvulkqqm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gjmudheel.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/ghhsiomql.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gbmzmbakn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gyjncsvpz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/giepmpwhd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gxhxybgoq.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/guxhtnetf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gnkgtotyd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gcguwzdkd.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gdtztrsfv.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gsvozpveu.sHtML


<!-- 参考信息 -->