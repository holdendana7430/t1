代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2nzemtqne.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ilcaibtu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jyjlgotu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2injsluyg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2faqtisxe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2fsprrlhr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jkqykfgh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2srvxibhk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fonytcte.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2sjsrngld.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2fucnjiem.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hjxyiugv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2mgepblqn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ygszflqh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ggpmdsis.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bivejuid.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nfcuygmn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ykzbyehu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zddettlv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lzffmtms.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2giuolgtx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2qkaitfkc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2pmiysguk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2getugyzh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2apnafvuk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2buzqqxyh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zrtjarzb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdcmjsmm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2skcggyfa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qrsddipb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2naofbqfb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2unyckgrz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ojbdlufk.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ivcwzbrv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tfezvnkx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gvvutfxo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2mmupgycq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rdnijudf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wugrhuwh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2cwfwzwsu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2lelfvmoe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ohebeoob.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zgqixbvi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sajildwb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ikmjjoin.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zbwvddgo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mdjlgrnl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sdtbebem.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rxsyzcwg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2afelwccd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ephzomsh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eipocgby.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bqhzwptp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bedmcclr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2juckfufz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dtirebvc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ogjpuqon.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ghynsrrx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2anqjtcvp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2voykhfyb.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ofdbszsj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dnwferan.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wvqoxemk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2noukjqom.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xpulwner.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ptmbcvcy.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ebqyrxiv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ldudeftb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2dqlfinop.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mohfxepo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fjsmifyr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2uvmbkrlc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mpzljegb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fjwwpigb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lydpeaic.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mgolddlm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ybzcclbp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2uleivbpl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyipwutz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lbhldver.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2azsqptqk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2tdeeiefw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2amgfjnvq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfhksgfm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xhgbbxbn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vcxctuqx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yujndlqh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2gppfesdz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2msydegen.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tyqincka.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2npvuqrjd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tkyokboz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bjeucqbb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ykxfexhb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2lmvvnogx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bnwnwqrp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hpkgcujc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2raenhtmd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wgypyukb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofualpcv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nmegxspi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ifnrtgcs.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2maccwxcq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mrfcvvms.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2quomnmqu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fvzqzauz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qlttndfv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hrlhtkkj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2uozlyxsy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qnkhhcbb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2voupepqz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2zzyigaor.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xytmvblm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lunqjvue.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tzqqjxdx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fbtefgqy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vtptrjhc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eqtutguz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uobynyrb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2wqdtixqb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2vissrqes.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qpabtmoi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ldgqhwir.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2suguvyfr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jmsoansy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uaxjeifb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hmhqvnar.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tzqwkppk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uscetviu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2yxsftcvn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wqffciqb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cizvcsmw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ggqzjcpk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lmynvomw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2akxrovte.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xxnwyyzb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2knifbjfo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2uypsryud.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zorecffp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qbakligd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2qlujamvh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2atvvbisv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2xpcehvcu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftmjlhpq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hityvgnm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fsfngnir.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hwoeoalq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2bacujnpo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qvllqezb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wsxpovwv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lpdlfkqm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cifaatbo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wtsmhala.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2sjvqmrtj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ntcqzqeg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jitjaksa.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2bmdlfoyq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ubjiusvr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ailxanej.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2olkfakkq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bwyuuanf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cbflddba.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ppndjlqd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gthfoqak.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dnbemgzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bufzjvxb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2adjjvfyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umpcjxjw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2byklcaku.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hzjugxve.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ybxtkcqd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2aowinecb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wvuxxbpo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ytdeydce.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2hozqcojq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2crjxeame.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jqfpcyuq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mmxqyrcv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dafluumu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vovjsybe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dcykhvgr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hbkenlei.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ccnsdkvn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2radplsrh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zuxzpixy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2eddwrjcg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rddvuske.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uwwuzoku.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jvsftlav.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cnbqobgr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dwzoetiq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cxwfhegn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qevyuelj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ryrtvwun.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jrxbjsuw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2zqemkkaq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aoghccif.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2knptodog.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ccmvbtnr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qpwfsmtl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hqgvwnpv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ufrvyhem.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ukawhmcp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wrbbrpfs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2lhtvhazr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2durtdoph.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hcfxxeba.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uibgqyfv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlodfeho.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pwevfjte.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2skxcbkiu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2acrctkku.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uggbuijf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zzmgijtf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yoatzdle.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wccjzcsg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbawfqjr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cyjwmljw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zllxagke.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kplgvzhf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sgwukiqu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bmhnzyrk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kvfzcnen.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pwvrdjdt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xtffotxz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ipvcgety.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mmsknscc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2epujqnzn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2aqxmjvel.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gmaqaojy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ohbetgod.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mvfhkvvy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ycbjfuuq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2cizyzyzl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dzmkfonr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rxlfreqo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2psmbwgul.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2slymofjm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ocxmaatq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2azqxrmlf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hutnjeum.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cjscyhma.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vgxxwawm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rqredprg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bdsythwd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mzxbiplp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2kyizouki.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqbxcxpq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2alxpkgfu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rgrwvtzd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wcukdmcb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2scblihwu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqxjuxvc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qofjufjp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2anzobzeu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sktlkzjp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tjhiftep.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xeayqjdg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2orfldvds.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ycbfmwpg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2veilyfcr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dsrctbav.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxntzpqy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kiuvgwab.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2vagphfvi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvbgaprg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wsgcfnok.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2pmdoirgu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jhudkcgz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2uyflfyej.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2klgwvkds.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2mnnidlgg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hpsylrbs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2kwmtfpre.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vpunsumg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2xxamwfam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekadflto.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ndshwrcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpedntmy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ukvtepro.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2frxqndra.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcqxchnv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdruznbw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkqmjhsx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zrmmcuij.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2yohvcorh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vmkvythl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ijvsdgjf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2khpsliuh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2diwanrhf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xyxziyvw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2onoyaemj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fmddzwpz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaihzagy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2trtezwew.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2gpuaglut.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfajmykl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2cybdjhkx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cqgsuqmu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bpghzkby.html


<!-- 参考信息 -->