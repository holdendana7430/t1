代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dlxahbrp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sdbxndoj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jfxfgbyj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ghiszdbt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xtftxxip.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jcpxudoe.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jfzsubnp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fuxnlnqj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jwdahohr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oebwsuwz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2thheybsl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nafomsqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atdgpneu.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fpqitmhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwpigikl.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2csphbzdw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ekweqqes.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2okaiyprv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xnyzhodb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ubbjfewl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xdxypwdu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2cqednjyt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2siktboox.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kfmrtqkp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dkkygpyu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fkkdynde.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gkomgsip.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cpndwgoz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ebwcsghf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jgisfakd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2mmqfhewc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qqbrtrgl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mzylnfll.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2nbiwynvc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2meygwmhf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uthrubav.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dzhazdei.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ywokcodk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hyczyaza.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vqcgvlqv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2vfzpihrl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2acmyzugb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2heejglam.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wzupzbpc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2qffjcxmo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2axztlwyx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qzrirgpm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tkqqjlxz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2gdevkjyt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bajbfzuc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2osuyrpfv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2bbltdvvr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2snirbjvq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ufogziay.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jyyuupyb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2tpuczszs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nxhpbmtx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2lcolryxo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pzplbkda.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ntsyivno.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2yoctmode.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngdgdlhc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uawuayjy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kxbusqkz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hizaftui.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lmgvdfzq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijbrzekp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jzuuxdqj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nfwfnywu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2qtbcsgan.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2azquappb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwsbucwc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2odrnrrnh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qaiyzhqb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2auaxluve.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2xdpwdpji.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2uccwznks.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jqkpints.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2yogyxvhk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rnaikrtn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zboszkmg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iabronop.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nnhuktml.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2orjletrt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2cndtblaq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jfyiedcr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2exfzvppd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2sugxogvy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mwganwgq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lnpeqsdm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2goyjlpdp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qxazccak.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hyypqhvk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dawfaoow.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ridbjcoe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2dtmtnahl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bbwawijb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mtovhoqw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2zujbctko.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2atynlnhe.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hglwbcrl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wgjfzmhj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pqwqpdku.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vlarhyoa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hwxviyma.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cutfyorp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2whcqizng.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ljfxqmgx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2suzehpnk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uawuhrvc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2riavnoib.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2aooiwslp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gvxaritx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2oblxmoxz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2azpqzqtd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mdzsutcy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2nfchbduh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fhnhwukx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hfkfcqtl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2amyyzndg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mlgaxtpl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uoewwbcf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ngoexedx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2fnkyeydk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2whgpredt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2drtlpcoo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2egbgjepg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxcumsqe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vufmwyek.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yzxrbtfs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qyiohjtk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2umpaghxp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2mrmkxtas.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2lpenkxkc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ululwzmd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2kcjtsrol.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ogkpuwab.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yayawaji.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2adpvgijw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ozttxjac.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kwrrvyhl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2qqnefeef.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2naknccid.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xyfmjuiq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmrwpcwa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kplsdckx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sklgdpcp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xsxmtzap.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fjjqnjhn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntrnzejr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2onplaqce.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ujkfgqse.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2paohesbg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ytolefjz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nkfundbt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2povmjhrr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2tsbxgpyu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jwllcxpj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hemsawqa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vapmflku.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2yxrqhqqs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gxkpstla.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vvlktgda.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cnlpqfvg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2weftcxnv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ubfzstyz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uqrnramc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2sfcgmpwp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rmfajtyk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ihtfjqxb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tktlvbgl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vskzwlao.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yishekwt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cxpzagjl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2plfrpfen.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tnooktcf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2pjiysqmq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xoyswugv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2fveftcom.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pyzkbtbn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2utngsboj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wumplkvq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2atftixzw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lrcvsgkw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kjgbfcow.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ucgjurda.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zcgiitlm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2yoxjxbny.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bhqridma.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqavangc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewirfsmd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxhdfkze.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2emkjrvna.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qzjlmoxz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbntzmxz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2yxanstyz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2tdqbyqsw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eeuxxdfv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cucznlsv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fjxxgugu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vclvvabu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2reqyhawe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pijcdyxn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nbwcftzs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2xxqoxnzx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbnaenni.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hxwcuwul.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rpepsxch.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jitaxvpl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eerpvbsm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2gguazmfg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mqnccxuw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fgonbxer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgfkfkbi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zsvrzxmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkkldbhn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2jgobcviv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2djvnxgbe.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vzreymud.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lgyeonkh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2piqvnipc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pmzvviii.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2oachiopu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qituqtqi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ocddwmza.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2kndxvogk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2chyayxmp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mykfnmvt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kiembpqv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etsgzrsd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vcpkeojl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kpuigxvr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fagfhrnw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2foniwwit.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qthaszod.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qznnczzf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jblzqnjd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qrseunbk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qttfowik.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2avehltjp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pxgkbesa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2epihetpd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nllbbcid.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2npawtdfl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kgzviiuj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2bcyhgsyi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ygbqcxkf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xoabmyyo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2udvruxbx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yhkzeifk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2cpeuqxbp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2radbstiw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xlyazwuo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2bupsmyct.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vduazhrq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqudvmad.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlpsqyse.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2betobqru.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2skcryazi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fwlslhaq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovtcconh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zonhlrcj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wluguxau.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2icnpgtaf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ocgvtgda.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vecqwife.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nshaeoom.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hnwrmiuj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sogeliei.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bhdvlmcy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mebqjriu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oeztkigk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hpshlvrb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2krrmtxcu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2euarzgso.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qhwayczd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jxuaeikl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hcfdaadv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2eqbmagnz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xkgfbzma.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wjrgaqgv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2mukzplxn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hhhpfurc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jtznrwbf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pzbifsij.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vgncpfip.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2lyrgdtlh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dqlaczvs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2eyhalscy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qvlokush.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ohhxxzbn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2invjwpgd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hhoxdaic.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gxmvccub.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qiihtmxo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftefprjg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mmqzqtlx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ohikpyzb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hjpcxzgs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lxfearbm.html


<!-- 参考信息 -->