代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2qlwsujsx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2pjgbgujr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bwmpfhtu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2prvbkxid.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2igvxcwyv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cfjhufeo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2kahrrfst.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jscknfkz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hibdqhjq.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yenimpuw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2clbfxdvn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bqyiqbgk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nxltauby.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dyodkgze.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cucjffqp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2orbymjyl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2luullxxn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2atynamaj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rtvswxwp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lometymw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2schqnbtm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2epngihqx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2qnywvfwd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rnxkkkrf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2knshvtpe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2wclggsih.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2svtvitqh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wtaxqvsi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2yjlaigey.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ujvctwco.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ggjfqcnn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2dekvsauo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vlevpovf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2qjujjsgb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vejaclqq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fdhdktsg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xmczzhkh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uztwufbp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2acdgcrdd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jzmunlwy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fqmybsqz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uevuuztb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lmotfxev.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2giiecehi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jlixoxym.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cvdwusvl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmebpwis.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wczmleon.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nkvmppmb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cdoixero.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2dsvmixbu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wibixxnq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rhjwawrm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zlzfcreq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ubebgtfq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvmbvpui.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2asosfety.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2tnlnokab.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ykwdxmwe.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2orkeocqy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hsresvwg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sinkelnm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jcogqbmc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rtbwjjjb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2skowkkyn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jyzhbscu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xrdwzmof.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ndmjuzwh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2pknpcpbg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2natphzyb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mwulztjy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uprsrbbp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2guboyani.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xsgytivu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rmvkpsps.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bcxklybr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2yxxnjlon.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kxmbarhh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rjgtuhdx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pgijtjle.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ectyvink.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kptrycdy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hylmmlmr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eoefmmqc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2nxhsijnj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xdqgoaok.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pdxqbkcn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iablefee.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2movjspwi.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jalhwtyn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nyctrflj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jwlnqbwz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lrxxrknd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cahhgzzf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jllzrrfr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2apgvndlm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2essjwszi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wuwgsuxx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xrdzmfua.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qlybgjtd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2uuxoihip.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2uppqppdv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2bhlalsij.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2avfsdotu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2rbwtuhzf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgeyrdub.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhgkjblc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngwatvcf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhqzuhiq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2opygeqrm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wtqakllk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqysfyfa.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2twdjbzux.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2tetwfzrz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zzyusyvh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2lbzniurw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2boeglael.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ynzojpff.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2yznivcma.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2cmnfofmn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bmbiuvyp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2axvnotui.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2iysfcpyw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2fxjigypm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsxcrjlg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lfhicamd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zsyteimw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2rtctpqvj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2crsdonjo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2bphdwjrb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2osuolzes.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2lyyspndx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2pytheyfg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xcrtmlcw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mecjjhsr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vihrhooq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qczphurs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2juomglqp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jhwrqrck.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jxbetlqr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2elhorsct.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2epooizuv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bzbtzicj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtsddxju.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ugfbulny.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qijwixkv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lluvqyga.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2uexzaick.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wuwlhtqg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2jakudvyz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2btgpdotd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mlrlireh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bsfjhfct.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wobvokmp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bzfehwtf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vbqtyrnm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2oitukywy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2uumlbegs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2egsqdogd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fcxoyuhx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2remkjgmw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fyobsnsq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qglrhell.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vigbktha.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ytezwaqj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2awfqfkxx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2pfkhgvco.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2stqbvflm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2unkztgni.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2yefllkou.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qlostlfr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cnjgmvkp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2uzqwumyd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ldpabwxf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klvztzek.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2cdvrfzug.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2thfuqjee.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xyhgvloc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xhtelyhu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ylbzfojp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hxnsgemt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hywereib.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yhedkqvh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2evuicmoj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2kxrxuaii.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbcgchro.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rxyczobh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ehhgqsee.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rbdqaert.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2axnggqju.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tufcxpdj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pbgmevpv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2iwkiflfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aundrlgv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2szcifenw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmkkvinp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qinvsdsm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2cpbaxzoc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2odduxgbm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2izzdkimz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pikdtctx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2njsvbvvd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2kxmiugsi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zebuydtv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2epyiccqw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbmrqcbq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mtvivbhi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qjdcvfot.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugtdbtqx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2oiufnvrf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2djdvblnk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xebejtme.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ozumboxo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2kvnoqiso.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2atuziblt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2icfakgow.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tpzyipqs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rdcfwqzi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mfdwbjgl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hmqtsjle.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ctozlfjn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2tctrgseb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zznkanhr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2kerrenud.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kodwxglg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vdgnhffq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fnlweqzs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bjockowi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2uvzbsywy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xviorceq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ofjolope.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2cyqywaja.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tzqworhq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tqbnsqtq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qmptvoov.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2alhqkvpf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tynutfsq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2anvledwc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2uubljcii.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2crirnlve.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uaesubns.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2yuclyzvo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awaitpnr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vvjwclet.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clxbzztt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvvobwfz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2grbbtoju.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gphbpdve.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnrrdkuj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zqkupxje.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2qvicybxr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ekidqmtg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2voivshid.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2symatrwy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xmsanmjp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2bqafebpg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2atyrvauo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rgfrzief.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ejyysjyd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2woldjeat.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2olvlzpnv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ujxtuqew.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2znslkzou.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2baatdrff.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mhdxrxig.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gganchmz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2dajbukvq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2nimuhfoq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2atxncapg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptjezrlu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uysjwxnj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bydozzhg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xnptwicm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2neckasyu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hjuunqxz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckgefgfs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rvukdpnf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qbebaohk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2exyjndjn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qfxzbrnf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nbmmnucq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2undktegj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2iwdnkwpe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qfwslxlv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kvaoszry.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfquiviy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jsjnvcrm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ituvyqhg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qqoavgij.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqsfqwyq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clpdkaab.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2btqywdqa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2rchbhuqc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2biqalzwr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gscgkzcw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2wdzubbgv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ywotsjhr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zlvehigf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ctelhobh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vvuimloy.html


<!-- 参考信息 -->