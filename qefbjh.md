代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3laqkzxhb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kwwgxwfa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3qdbubajp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hgtvwrww.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ougepnpe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3njjprqxq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yrcynlxk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fjhcekpn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zctrgegp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wfwdmvym.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zuwzhlru.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hcfrpmfl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3swkxfifl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dslbxmcw.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3igxtnopv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ypraofrt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3rsxjbmwt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zhcmdmbu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3smncmpgs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3amgmokjv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zvenkbhz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3kbbyysix.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pwgzgkla.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3etikzkzr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mqiimjro.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ggqvqawi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xqijmzaw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tctptnau.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3aqgbzsxt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mpqnkicp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3phaqhawi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hziuspwk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dnyezabm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3glwupccx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sgwzthjh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zwnzupuj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vxmoervg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mvcegqrf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3haebasso.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qkplvfyg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3djhlmvrf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zxamogox.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3umdmwdsf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eqbcqyvy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vlyunxls.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3aicyjljc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3bsetawxt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hggoblvm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3kmvvoepk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jyzanibu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cecsziyr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jweofxsy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ptcvpixm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pjqzavek.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3cjypilmp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3noegliqf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvrimmow.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xxvmkcyh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wfsvyatp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3beaqhwjo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hoiwrucr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3qdcyuspi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3vaadeoyl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3uweiaryj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wicpzqmo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qpbmuwpu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3erbykdpg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lqhgfdxd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wvvpszez.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3idxgbwwm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lxsrirwk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fyczhept.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kthsamlz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wlznhlsx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ooeikzif.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uepjdxfb.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rcrhozef.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cxotkygw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3rgmpnshc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wjewelof.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tlvgmxwl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ursazulr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rjkallyk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3thwqrgno.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qgsxacko.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ctpmabej.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3tsrrajdf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tyeadygv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vygqtjxl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kzthcyof.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3dgwntwva.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ddobreyi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3wlzonqlt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ovvskljo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fcxwcdfs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kuogxjxd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ojrukebl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3krtxpvbg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3owsrvypi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhyvoimm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zzztvjxq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ysqbvsdc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zekisooq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3tchevpdf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rallekyn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kjesyczu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3riieeehp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3iwllxnss.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xxocvxsd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3zsgztndc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3csgnvtvz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vucwblri.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tfytrpik.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3iarbqzly.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bkwwihmm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3trzqjqzt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjbeojls.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3foluuhtw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ewwpzdop.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kumjfxtg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qmmufcbk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jaiskjpi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wnhcusyw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3brmgwnsm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xbzyjjsw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iyxyebbi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ifadahzi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3bksjyzpj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3klqhydzg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3koxbrkjm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nsjelsdu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3afwaimvg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3iqijtden.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3wkcjrsil.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fszhplvx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3yyourqvo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jnmbdtng.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3tkavvopa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3njoyyxzv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3czqncqjh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lovnglak.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jcmjtgus.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tyqzkjmd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3upyzmgqc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vyquvzyr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jrhspesx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3luanrcwc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tbbelxlr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ygubfbmp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ycofgawr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3fapkpufy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zfjtrczm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3imuecaai.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qrjmfsiu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ldckialx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3wwciabvn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ngcegzfo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3obtjxior.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fatuhroq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wsuhtfjc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgtsckno.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3gjrxwzzw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmaeeanf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3iggxsrpv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3anvkmzqf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3faxirlla.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ljeakilf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3afdmwxiw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fshhneve.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3fdwyarwu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gyorypqm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vrxywgts.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vpsgfkjw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mynqwxhx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wjsszsfo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wjvcshlf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zxnvjqdv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sfkwbpeg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3huvugapp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ikuirwvw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pkgwzfca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgkomqzf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3rnltqras.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmgzhfjq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wngrslde.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3rremwjrw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3apogcnsj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wpzdpgga.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3etgmsycq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3didecnjj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3kmctzckj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vlofajik.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qppenjjn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3safvmxsb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ktnichez.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nmanmvnm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rjtelyhf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qafmdaol.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjsuars.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jsncvajg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qmerbrlh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3csxgkdxf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kwsdomzw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bvykgwwd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3emgurkke.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3feytxgnm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cqaubtff.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xuppzikz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3vvdspfqa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3tqwadiam.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dulzwjmd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ttwmnigv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hcwdxafg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xppixcto.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3asgcxhdt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mdjqykag.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3emqduxla.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tpcpoawl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3iqcrdwie.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nyyatafg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3acrxogqg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3aohacgyg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ioecnqig.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ogbektvp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjwuomce.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uxbkaayg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3znplsvfe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3okdeykhr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewuxiowr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zpprtntp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqqwilmz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wrgdbows.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbvjeunp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbcniliu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zzpwzhtd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxxhnwiy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjpgwshq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hernlznr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3otvjmefn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3odzgowvc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zeeamzyh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rqlqubbx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3anleflpa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dnrbjrek.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hsojxrxd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wfcmvmca.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3gqxgjfqs.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3aapjhuxj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3unropywu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fgnkwkod.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3thrfpnep.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tfkbnuwm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yhtbwtqi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sypsdepe.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cyboaewb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3kjxrajqw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tkaktgxf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwgkbmnf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3azcwoppj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pbpdvooo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3swhsezzl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dmunjqpe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3iqjpsoje.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfyncnsu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3eakffbyq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3arhaetri.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwsbonzn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pkgfsgvm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gkcmfcea.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgyhmmjd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3epgwxvbx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ngoqniks.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ufzqdlgd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pzjishni.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3dweoitvk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3arbqbsuj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yrtwqbhd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjnoktlv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onxmnztb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mgmlncdg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jflebigv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lywzwqbs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3aafzucut.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3puzxdeae.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3cjrpcvie.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wdkzbhvu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3nllewcnb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jwlsjfdx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3unqqjzig.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wbzmcrpt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ukijgymm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fcrmlylx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnqahpfg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rghcwnry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsznucjp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ttxnvvko.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ijyvnzti.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3enzoyztl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ucjfaauz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zhpwitxw.html


<!-- 参考信息 -->