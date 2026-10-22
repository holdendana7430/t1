代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2atgvrjqb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wadsnoni.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mkcsdajc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cmglicfh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jkwfewup.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ibjnaqda.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ordydesi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fxdfkisy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2qpbkimfl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjzfaqof.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ubnrvqqs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xqhypedc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2odpymczt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oghtacrb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hbfcmgjs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2imkdeeei.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2opfkiluc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fojkcmkn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2cehfsosu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qenxrhrt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mwwshbof.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2padzbhtn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2eovxklax.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2prwfjaxs.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vcyuslun.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2kuswlfor.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jeudtyoj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2kscubtav.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2etguhnuu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wpelmhmi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lazqcryl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rkzxbnrp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2vrzazsak.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zsugvrug.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ahmtrmdb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2mocekvol.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2aptuidzl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ocysdlrj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2geyhoqio.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2cbjbqyct.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nmxbivib.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2amyxeoai.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dxdnhsvv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lsokzshs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2odhczrxd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wbyaesfs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2avumoupb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cfcqgseb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lcweojnw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oxyuynbp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bmsfnwwc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2licfzlnt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zjuvngmj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gcgosspx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bxxhagso.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2istkexrw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ukacubbo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2swzgioig.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ynkotgwx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2aamgnqck.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rjhiptsn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jmrhfqch.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rtueduvj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2idgqcsir.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dxlkormb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jlyfnekr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kgcjbxon.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rbeccdop.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2jpuwglne.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iiumtpkw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2fltilbab.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2nbliloal.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mohnzwkp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2raphvmis.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gkovebnr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2atduqjpt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2opqhxnxz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vomopksl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mbqpbpda.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtiysarl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qadwahqu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2hfkpwgtw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qvxvtxlo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nksxdywu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2cxtpuhgz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xmmpifqt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jeewljnh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2czxchfxu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rmewqgaj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2altadptz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eplutsya.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cqrhpoyw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2khyglbgq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2obpwzwrf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2txkgnili.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2okvqlxep.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2eehzymxi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wehaahsa.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2utyeagqq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2doztcbzi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zlasuiqq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fhtvrurb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ptpdeiyv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lufzbews.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wramqqqg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kqlelxis.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pxfrxnee.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uqqdfoib.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dljsbrwd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gomwrliw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2apfljqtv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2olgroenb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nuhgmqrg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hvpycflp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2cpenafpr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zvkgbhfg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lkdfcgpr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2skgvbqkz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2wpzhbdar.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uncickpz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wtbwwsde.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fpmwkuau.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2quyshbzm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wcvuaswr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2tcsjusua.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pbixcagm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wcfnrktc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2usysrwqj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zxjehrpm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2syxegbxu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2qexhfucq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ieumncbd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2tpebonck.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2cmtrdapl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2lxlwdrsr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2njujgmqi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2yeoefdcl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2cwpkwsgu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2cnbbmwry.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnjomdmj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gdwgxsmb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2gxvbcsqj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikolavwc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wiaqabkd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nyqhsvfs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2piyikzvg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kgvgvvtj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wkdybypl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jqxsnypn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2yerelkeg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qdfmwhpq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xqiowffd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ktagymid.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2disojnyj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2swhaogmj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fpbmsuey.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jkepumtw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zqogydqq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2borqsehh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tplzxqgr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2luligaas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrkprppo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2awbjsizy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qchsgbuf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mjfxbvli.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2grvnfulw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pgjkywqm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2eqwaqvsu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hyjhlukm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dnrzfimq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2hkjdiugk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fptlffoi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lspfwtmh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2gsuzpiii.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2upxjtjzi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoqpykdr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kvuzbscv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zvrvclpq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mlpoxrit.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2igdyuvdg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xbhrgvzq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2exxfqjbf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2sqsteorz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jvwjlidd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rwvagqrh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qfskcvsi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oknhnlrl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2chfkgxmi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rjjzisss.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dwzivxgg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rmfhbquy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ioleelds.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ctgxptyw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2smorqaro.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2orucseza.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qcswwxdg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2acirozcw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rpdyxfwn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2gvyqwhlc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ezuqukpc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2iidtbbzs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tvohjiyq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2htssbxed.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbbivrwo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgsoqlxr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pagdljqr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ffbwzoaw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iiyivojv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owxlhrft.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2pxmvvxed.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwrgxxtn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pjfgqxco.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcruiqei.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvptevlw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2euwxavod.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wxsfbzua.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2haaospkv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2agydbsup.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2nddimlyw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vwsljoau.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tpamxqzr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wlggjdgg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vngososq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ckgjpzmh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ykpclnjg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wfwnmdbi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2usgtvmib.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2uywwddpw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2etyajpss.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2divszkak.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2szsnweiu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lgdytqlj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rqjjlrcf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2anftsggk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rkjjohao.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rrlewfoj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xcrqczox.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozjdgryt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pkxdshho.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2thctabin.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lbazlehr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2onvttixt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vauwbgag.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfqggzqt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gsaybgaj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2itqqscqo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pblunkmy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vyaadqos.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ytnzwvcg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vlgwleqv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vthyttdv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dyjgawqr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ceoxxyci.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajbeelmq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tebvubze.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qncqxmvu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ffasdvwc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fclarefw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rabwigef.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2icadzjvb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fmcellwn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qptivxfa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jkgoybet.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kussgjrs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wznisvkr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dlpgmjgg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2iztcauti.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hpdlgear.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dtphgqgm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2exuroloy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2xokxbdhb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jduerfzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okbupdjq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2vxreybre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjtabyzc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2hzqtwise.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qiwriiby.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsaywvnf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gvuuzpxi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qkgvowne.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2nawvpzsy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wixxqwgr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2khcshihx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdgaenmn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ducaxjca.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ditemehx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ndffdmyt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wksnquge.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2losmhbgb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mtffzmhw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mywlztuo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tybxrmpv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmchqtrs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2afyditql.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2egymjdrb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tvgxvzcq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rvqbcdxy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ntfsiqiv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mnglhnli.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2bpxzcytl.html


<!-- 参考信息 -->