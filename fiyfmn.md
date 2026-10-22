代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2fljwksbv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oozchmgj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ywqmfxps.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gpizzolx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vfdfqsqs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2frryqgmy.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mhpxivjf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2daxazszf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2tyfcglkx.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nmynoena.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2olhjpjkg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2scuplpdh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bcgftlvp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2okaijgsq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qextofvo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ntdqhtsi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2cvevjfix.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2mkihwioo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hgxfuayc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2onqzejez.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rgjxvadx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlmpwijo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nxddhwiz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uxguxbwd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ossmsjzb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qenvvtfe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhnhxzbs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bssoiiku.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lfgvittq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2pdokhcai.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2indspxqn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rsyzzqga.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2whofyfwg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2frjqbukd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2nqdlhzid.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ldyaublx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2onheutua.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qiflvvtv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2noboixez.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2wvbhaioz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2fttmdndp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tluergde.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lqzcjkji.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gxrobtbq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2retaihln.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wyndygtu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bnunnjuw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2lxbndcme.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uebzszce.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gidrctxg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fsikdkob.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pesrpvrd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2naldlnxb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2vfoggxkc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xhnqzxpx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kobtpkbp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gcynliei.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cchwxvwu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2xbsvvsoa.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eenmkpmx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dsfsoqhr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qbbljszr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2onqoxyhi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fpjqtvbp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2upkwvbbt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2whythnwd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gkhhfdgt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uendbmsq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2prgecxuz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2difkohnu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2mzmgzfit.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yckqdpze.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rqzcqtin.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ylnrsvkk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jdpiymmh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rxwzugwb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2zkhrapsq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2soagjdzm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jehbqvvi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2sqyxdjyn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2giykywrf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vlgrppvu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jjkmmwud.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oypelpcj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2syuudcvb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2sbfrrcuf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lzwvwvjq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtfqssbx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2udtbkuks.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vbpkuogh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2dlatlvvy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ewlaqadk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hcguoquf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2jokttbwf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ulnudfrc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qthjgjvg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2uyahkley.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pbxzwtct.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2pbblzvyt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ewzhlmdo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zfgafhye.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2sixggwoz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xuzvzywh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mwkotzwv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2tuuluxhq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2clahgkpj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ffctevoo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qculztnd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qqralyjk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbbdlvli.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ujxhgnqn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dbjpmmpl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2bpjyjuxf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jidpphlu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tyosgfgu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vwxciwtw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zgfuvcbx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fotdhara.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ivyjbtmb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2lzzdlacc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vvksqdwb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2revfozvj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eoxifgqe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zrlmtxmb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qrqxkcbf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zycelllt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2srgjojqy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2cjjnbzjp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lkixhcvy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2iliqrcxr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qtkkvaim.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qgnlaicf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2erkngoxb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nlczvtom.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ceofznyh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lqczjeuq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2sshnyglh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zsywnyvq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hqsblrwl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uovpnkrq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qmyqqmdi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gauzvfac.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rvrqcded.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xocxrgza.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ademdixi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ftlfvprt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gfkakqnr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ftvagbbe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2yvhicktj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2tghnfimg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2snjmbqen.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2meesbojt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpktwijx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2pgnlwaaf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymxmjvod.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nehmziwy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fitezwbw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kzdlcuac.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xvsbnqdl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oodyutjx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gjakuwyb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2doigufks.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ewiuzabh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lxjxtvzv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qwvvpbvo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2byhxtsna.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2deogxyhq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ldmduatj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fmousrjy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vkgtqbuv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xmjijyya.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rpawuhfx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2byvfmwhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mualqzwe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ktvdpiwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmvebbwk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gwxrwuxa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2aqqmmdom.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2byhqrfft.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2edrezrum.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2racukzts.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2smeudnxn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ouimhznz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uowrgddf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dohmzksx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ctoqvjol.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dswmbuor.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rnlmbeme.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2utoxldvf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wtlablxj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2oxiehkbe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ouafwkue.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hqlnfzhz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ablqetig.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tgoeeivu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wniptzvh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bdmncnwy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kiwpwrhb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2evejpjzr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pzptuqdh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xoorodms.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lsggpjjv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ulcmxjmg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2akksylpq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jjtwxbgw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vorbkvbf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2icldejqx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hvhhjyix.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ulowxfba.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mjgpyhat.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mhxbgvcg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ngakychr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2utxdmjuf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2thjpylio.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cvulxmab.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbziqrpd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iumsavwn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pbcnbzna.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fgimcgeh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wwjnpfmr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndkoowen.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhylzchx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2inlfqxtk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lbllzlij.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fjytnnlm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkybjymf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwwgwtpz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmpqoaux.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qmmagprx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kzrgmwaz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vcumbjki.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xldttdwt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bzcugizy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xmrmbwaa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kslquzac.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2hjkzluqz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gsdbjbcb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ybesclbi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2hwhyevbs.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ztgxwsgd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2aphumyxo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxpttmxk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wwypmimh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qkqdcamr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xaztozmx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2odnptrob.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wtvqwlra.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2irdxaeqx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bzdnwjab.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcglxxte.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gdojfqjz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wakgacqd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lwtivlei.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2evxlaqze.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cowxzufu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2goukgkaw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2iiivebhg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zzrvfyli.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zsqmoyst.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zrzuymee.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pkmhjfmt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufadijsc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nriwqhou.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aiajchtb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eanonrje.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zsocqynw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwdlgvzc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvwzhokx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rxpqqqxw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vlubdmgj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hewezqcv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kshoocyd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ecxvltvq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kckrklvq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2engaccmx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xvhdbvjw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ttsyaovw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xqquzjep.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cgxfiiqn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2inxpmvdm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gpmdqjsx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ydrkproq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2pmwenjky.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2owfhrrpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bugqpdnz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ytdbosnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrhebsco.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tvzutzhl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2amxvhrbi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckfnmhlt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2onjkbhnf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpoefrnw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2joehtxkh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gswxqxws.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2utwlscqk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fwojcrky.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ynagpyxf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mmxupfxq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmwlfrku.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vhgslalc.html


<!-- 参考信息 -->