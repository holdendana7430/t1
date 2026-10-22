代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lxdheher.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2egwrusnc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dbtzkbcm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ffhwinzt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nabnxonr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mghyklcm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2yrztzaph.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2juiygahe.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vwtxsidh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2oswrjtoq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ojbsocrp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hekypero.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2psagsezh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2puxxvuvx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jylnsuyd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gvsjcept.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2juvomrne.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yxbcqvfl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vxlgsddi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mobcxugd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sabkriag.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aehxjhxm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2svjjnthp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ubdavbxp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2yyukwkby.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zwrkmybd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2cyudqfbu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2idctdodx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2meonkqto.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2jubfcuuf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yorzmudm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dlrvbnhy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zrkhxeqw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lliitpdw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cjmzeswn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lhutjezx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2mmhzkmdv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gnthdejk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yloqiesx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2rlwuxmrn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2krluuisd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mmrdgqxh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ogbmcpzw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hqauiapz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2penpkgbj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ziivhorl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rutvjhxh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2imxewyuj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dychphui.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ijauwjbv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbolfgsy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aygpcqib.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2whjmkufd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2lrwfbayw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2rckpjwpq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jurkymth.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2nvgolvfy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2pwwcmyjl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2wwurvnop.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2lsqviwyr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2cvnkuare.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2aobxullj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2owxbitkv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ggvhiqhs.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2mdegbefh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xuganctf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ylrxrgqt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pebkyvax.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2rsxacsos.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vhztcldz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ruotmsft.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2lmpbgqvh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrwwawqo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2saautpqd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xhlehgip.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2josihxth.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2eeidnuml.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2kpakhyln.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2upckhqdg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gngqkbfq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2sayjhtic.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ygkwsbfv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hjfsqdjv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eecjmxjl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vvwayfnm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ljjstzrz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jeppkdhp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dmihwjja.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2rmzrdcky.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ianvbryw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ytcltbbs.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cfscgkmf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ywoyounv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qdszlvfi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xseyozld.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vscxpqxs.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2riasviyy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bzhfuwpn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2klkhvqyv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rqkmxwfi.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2txsdscyr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ztfimzkf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ofoygesm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2yrcuhpgi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2cxhrlhnf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nxcuwqfc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2qoqyawlx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pntghvpj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zfmqsrxf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2wbhyucfq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzjkityp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tvnbugbz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cmqppqgj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xbvbwuav.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2lhimnozk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uwgsduzw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jrbgukgx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mbyconmh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uhespwma.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xdozzsym.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hqddsncs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jmywheyy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2gvwmjuqg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lyjhjjgs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jurabcvh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2yuuwuvdv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ugwekpwj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zmbekmtf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2kiootuub.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2itmnwvwe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2hfiwemvk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nabzwnau.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vmwzsjzx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvqhzsvw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mxpgqitv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cgrmvjef.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ewpytyvl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tgyjurci.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2szuhqjes.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vucaehkn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kekhepzc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dmrpqpzq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ufpjpuul.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2mxjinfvp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hedglopi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2cplreanz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vyqsxebh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2coxrvjtc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hoizhszm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2afqdgosn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xqqiaugy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2oegokxeo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2fryzrahk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2yvwgwocv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2gauhedwn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sjlyqmmq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bddveqgc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hubbhwjw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ljqnerbd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2rkbolnzu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2risuvcda.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gkpgevws.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ryxkerik.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2grlajlkl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2canyqcvr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lhigormw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2zzjstdkw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wmlkqzxv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xraojncp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2iadjfhbc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vkbxlrnp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2thpxroda.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2yrogenkd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2phjdazla.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvkowhqb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zcdmubtf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2njeghufn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2eubxxqfl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxcpjgjp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2yxjataxc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2eubmwcdj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ahrwbihe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vzmdeoqj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jesgaftz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gzmhtyad.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2orfkifsw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sqwbdxvo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2udzmmsya.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2igxfribi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2acjcugux.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2muzkynww.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aiqnehje.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oyvfkdtm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yzpwxiiu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2yunjnouo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xxwhetez.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2eqfsnirt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwktqzws.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2opiyfbew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmmxrpoc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezushdcj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hidfnuef.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lherfgjq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bhtldcfa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2utzghwor.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mvkzohjj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2mcwmmpry.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqcejezy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cbrwxeks.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ncrtmrlc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rkvklxoj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rhkhsiaq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fpqehwsd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wmpvmmok.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yuuwopdm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2dihnmozq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2kvmesplk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fmzqbahu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2fceqmzxw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ekxyettw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mpvdwtrh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wntkpnwm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2munwjulm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ezasgqmk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2vkohynoq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2tzigjfge.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nronvscy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2sbitsurm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nrzsdjdy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2oykfxvxl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qyhnnyax.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nhuiwzyn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2gjehksri.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yvtisedz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2emgffshn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2nbtmpzns.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kddkodsi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2xawoluwl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xugvwhir.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tyuqwmei.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcvzigwl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rlxgfkcl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hiighlds.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qsdddobj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pgeibiuq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdnffinc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xowoerrk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2czktpyhf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aabiiiib.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sploehzp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tqbphhcn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnhkrrie.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwrpaoyg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nvqclekm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2quneluuo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2feozmsyv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lmrzvqoz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fcohqjon.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zbhggcgt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bwjxpvpp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2eaqhlrov.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ddibmrma.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bqvqiqlb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2cjrgifgm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vhdpfzmp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxtvlfiu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2luxhdeah.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vlofqodq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jrxbybyv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zsuxhisg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2cixvstqp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pqdakfka.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qqdvfunh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2azhfykqa.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rmojozuu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2plcgvmfj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yvalfifb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eeclrihe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2olflstsj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qjzqfcen.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2khkoiing.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2kmbncqyd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzqvimio.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qumephio.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhvtmevc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2litasocf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cbpbdcgg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pazsnfdo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bjumelqt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qppphvhz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zdalpfkg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gpeqrrvt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2jdoqgvnh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wwptgudj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhbigxoe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2emsbsbto.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ehjhfofz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrsdvydi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2agkidfht.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hwliqbbe.html


<!-- 参考信息 -->