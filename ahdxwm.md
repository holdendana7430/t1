代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ezbiffml.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cdnjbzps.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mtklqgpz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2wazkybrk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dapmsfbr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ffezmtbj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lwetkbzw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oizyghjy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qglhfcnv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2angpftar.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2obypjdwk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nifpivxr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2eaalrqvd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2utsvhmcq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ogrrenbk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2achnkhuj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ctufkfoz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2fymlqpix.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ylvjfrnp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2acleqsbb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2tteewucz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ludnyqmf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qfphmswx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2sysieeyh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mwxlljcx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2mwrulrvi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xqdgtorf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mkyqehps.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pfifqjdi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2cpaqprmg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jklmsxsh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qvbmjewi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jncwijzk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lncxswoi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2siuoashi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2syftpqax.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2warjipjy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ieygjpia.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gophuqab.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mttkhknc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ssrnsspo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2plbyonrg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tjxfcklx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cailgqus.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rpwteeej.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pqjtfwxm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2lbkssysx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2csumcukg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ckhweaxd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2duknhqlz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qvtmztyi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2cxscfogp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gvhbkozj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tgldqons.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mcjuqkkg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2owqbmfxu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qjbhjuwc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2swnypffz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kdojmijh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ymsilclk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2phjtrsic.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2iujioibd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bqnmbgbk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2klmijddf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2aqjiwzew.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2hwqzvqbq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2miqvrapl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2eeivklye.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2zeikvhdj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iiiclojs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hwiswnew.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hutefbnn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jyiqlkoo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mhqtjwdd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hdwnonpv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qccbbulp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ilbfwash.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hjnxfgvb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tpipwwkj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mwkuuvam.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eqdilmbr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2iekthdhg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2pludtuqn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2askowqzc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eyomtsau.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2daslbneq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2bkzojwng.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hzewysbs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vldbcfwk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mjamwlnz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ngjshofk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2rncgmdun.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wugfutpd.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dawmuput.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2fsbxtsmn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vaxpwomm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2hogulsib.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnqjtiux.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kepcfeyy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ixmrqleu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2eppgfbhg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2dssxdopl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ywuvgqzf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdawpokh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2iogmfiut.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2mgmqmkrx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ifztuqrg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zsxojpva.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lnkifwyi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qksokkhy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fajetsvo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mdbmuphc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dyhixuox.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2oqbiwjhm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtqgsmwd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2qaumaonm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dienutjr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fasldqaj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rfezifxm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hsmqkpex.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vmvnojiz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjtprhi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sbnmlxnn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2uubykvbq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kdmppyso.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2heqhnvmj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2usfexhig.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hwraxrhj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2clbxninq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dmrmgttk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2eaykeogy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2gufjfqds.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xukjezpg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2okxidral.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wnokitek.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jxhgnens.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2twryoigf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2besbcwbx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jzypjwez.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ilvvnbyl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mqtyhhup.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2masbsldd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ljjefssn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dfsublrp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cdreuick.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dwrhksbm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vdoiricj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rsazikvn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2hbuwzdnq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nppvipmd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ajllwnod.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sareknmn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2juwrjuux.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2laamoihh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tlidrrre.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dewqkwsj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hsncjfpt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ubhzxcth.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2rnfifaec.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2awlaxkyq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zvtomhva.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hesisnug.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mkzpppwp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrjprfxt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2erijegpw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ftlhsjex.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2pgaojjax.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kxbywqpd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fiityfkt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2suguibwq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2reqqrwba.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2txxswwud.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dihtinrw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ecnzoddm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ujhhwika.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ehvuosjx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2chnrcgew.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ruvalynj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ltbxuyxo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gnhvbikr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2befdnltm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rchyrkkt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2thnnndjn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2silhfvwt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uqjraasm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtvmqqub.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2udvtdscl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykfarvgv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2cufktpho.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2jdtwjbum.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vkmjvhqb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bcizokyc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jzolyqxc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tklxwkzq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2cdbsqyai.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kegcnmnx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rojlboma.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxeqafxf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2tezrzskq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2npugieqj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azsgimbc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iifnzjzd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pjrtnjqu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gkohaaku.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tapsunkd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xedvotud.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2guajuaue.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zkyxailf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zdhuijiz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yxuflula.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hjujlteq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zfhkhbie.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2fmxhvsnk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2pnefyogs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2phyphfgx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qklguydx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kvlbbczo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2sdubpyzu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qpmsgdkn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xmfsoavu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ypvqiedo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lylcupap.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lkdrlaeu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2veiosrov.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2fzoizoni.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2vwirbfzj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sstbccfz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpcdpzmh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgdxmvad.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2upjwghtj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2iijjoqhv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjrmqssz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2izsuntns.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2abawdeyr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfzqoqil.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2osgdyvqq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ejmhtqic.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nowrinqs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vhfkkrfa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2apuctovt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zxmolqhq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jemcrkhs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zfrctqtt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ybqbekrq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xmidrzls.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2matzsdqn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ofxfrrvi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qxgccgtu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tfijtddx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qxyieqek.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2kuglgcgs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2oqoqethy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dvenvwgm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfeokqqj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qnqjvkzc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vlxfxysn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2labldumf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qotkmbbm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ciriipkj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xpopmzay.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pqsisokv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmgrrwtd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gygnvwtz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tihptmfc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vogcyoaa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kvicmqgf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zymcwckb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvswgxkc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2srzlmhhu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ctvbfbgp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rqmhubsp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fzymehwl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkwzivae.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yxglodfw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xtlihzby.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjgnqilh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jvgwnehn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqryqqqf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhbbvxud.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xragyrrm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pxuyialy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rarbpgch.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ubzlzbme.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fkzgwxcr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qtifcpec.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwegcago.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wdtsqrls.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2drkuclvo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qnfeuhyd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2dkxtdjmu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ybocyskh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dcqqosya.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2twtzjkpf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2cokvqpkh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jcfjdaoz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pzgcahng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubqdleki.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ytccvfmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hglllweq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2djcafzms.html


<!-- 参考信息 -->