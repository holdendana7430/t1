代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wtcszxqd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xmtalfni.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lsibgjer.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3lokukuns.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wdozabxl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3euiadcqd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3abtkzlyr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iuftbmlm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fhqwqwrx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3yiscnjzo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xujmckci.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ngdvdgvy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3fnrzahgz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jogxqhxg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cwpasisa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vmewstyz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3llpqebna.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tupiurem.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ieqgihhk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3emuptije.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3brjyxvtb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ggqdlukk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3lyvmhuqv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3snccqpcz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zmobsyfa.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gznjnhbw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3zvxbufdc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cilfbjea.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3swwnpzbw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kpmpjmqs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3kxhvutty.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dcdbeopd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ntlkbpdx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lskqvuhc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pkxxhcjb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ceyczcuq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3vjowmsqs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tbxknbvs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qomoghyl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dgqhtdjc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lpvtmfem.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3yfzpffgi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ctdoxjxr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xmqaagmz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3iohjgngi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3malwbpuc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ayhqhyex.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vpiotcby.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3omtdetfj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rrwriuiu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tiutxofo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3muicopbn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mjlkpawi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zuutndyc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lriteqjr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nuxfrvwb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3iyvfymjr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3diprwsxi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3whmwhjae.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ehstgmfn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qxpbqnnp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qampjtmd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qjhtdzii.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qbspbnji.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vsyhmsbr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jtwvlrcn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3aaxxjdbx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zglrhbcr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ulazeozz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sjureskj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3trbkdcft.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ssfgsoci.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3fyrzvhst.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gqvdiiyg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3tvqxrqfr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cduhicfj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lbnlggot.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfqvkujb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lriryeib.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjgrdrom.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lvylhbhq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lyvoepet.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ktuayrkn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sqnylfmq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3bbpneyty.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3omgjqpwf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3hehyqsfu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3davxntvf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qxvqbdaz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cqfivgbw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ckmxqmqw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mmizqgjq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xrgfpijb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3uyfoourc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmrixjwx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tpmdjlep.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kubuzemd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3txcbsphj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3otapnrxt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vjeczmqv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3orslxzbe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3rmidvzvw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ytpewqun.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ncloapnn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3zzaojjbv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3amyttmlm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kfnqdtlw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tflaoabo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zxyirxnm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yecefxtm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3sutknmdj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3dzbhaqcq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3boikzbbb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3umxpiwfr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hqcxmceg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3inyrayno.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rsmpbmie.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3utdrzuer.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3udspgznr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vmuwjejd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3kgruuxpd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3hdzhhezm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pgeibbqx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uyxolacl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dubxjpwi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sxjsqurm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zbqiavzr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3veuhyevf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lonawjtx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3chbdrcge.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bhlzcdrx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rmssaqav.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3psrbtsnq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dwykcgrc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kfoprxum.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bbngituj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3njuowhoj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pbwyuhqb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3poqfijnb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ymuosdej.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ztzktcdc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tynxqxjb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjzaxbgc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgairunc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3psdinuvl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3mdunohcg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dovxsaez.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3tasxbfyw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lkdktdxc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3chxbhgkn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aiupjcri.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jbkgqizk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pajotrwd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kdkhepor.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nptpeylx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mukhkmqe.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3sstrwnlr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tyjxbrdi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3edhgyixe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tyiiabvv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qxyzhhdw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bxvmcdnu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3tdjgvabe.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yqskzhmm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pbdvdafc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etterwib.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3nidlvryk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3envkobhx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qglwofcl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lqddxehx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ovmcwqfq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ijychbpg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tljzgdcy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rdpmtzga.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3hbpjppfy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fosoubsn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ffpyzsah.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jiynuouu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pnasgojg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ysozhvth.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wuhuonqm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvgvbkrb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tdpsjvop.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vcborrxm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zqgmaucw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyinxeew.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3pyjonibn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3utpgespv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bcujxlux.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3etxldyxe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jwgjinjy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bbnlaima.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3joejaapr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3etmpqejm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bmgnpacq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3gxmcfjyl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3csbatfvf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rnwpaszl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3svmbofnj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zpukeqxq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ikosrwvh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cxiipren.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3empeelmc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ktdwxdar.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xexkptqn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3drduxbpg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jdxfenkl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmnzchsy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmifzape.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tcgfygdi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3blnkeivg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pomvekxr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtfiupti.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hqusyswh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jfxtbzqg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fjtgdznc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iasuwyne.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jyczlkjm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dzyhmvuo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gphploza.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bydgmthp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vtdxrfyr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3izttaeuy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gogymlup.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3orknimhm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lvsuoogu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dirawypy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mcgkesyg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hsuuovac.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3pixmddcd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3orqvcljh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jamgacut.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3oowplmez.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmjkgmig.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3flcpckfo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ifzcpdwo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yldvyvcx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oudcnmir.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3scwdgufp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3otudmwwl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3pxmqltvm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hgohfgir.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hleisxbg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kzlrjjku.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3creaimaq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vwcsauwg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3snkyhirm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3soncdkai.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gghwpdla.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ifyzgeyh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nnaavvuy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gvwubrru.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxhwlrcb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fbhrfeke.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vsvpcrnu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygfwrdea.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iuqfxmje.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhzlqjxf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mcxmdgeq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvrmokea.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3agmsxrsv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfrpvnhd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xygvbqqs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3azticmjc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3oqmysirs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwiuvdoy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qqxicvsz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gulbsbcq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qscyfgrl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3kcrwbohq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3okxdeber.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vsjyxxge.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3lugdaqec.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nznfcbbi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3swykeelt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3domweucm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwjimetg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3darigvpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgbtcssz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jjcprxkl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ejmuszol.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mlktjwvy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vshwswzv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jejpboxs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3uzpagwjy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3cwqvnjrt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3prtnwzhg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hgzyrgjw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kgfqqdos.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3oplzozlt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kfksqymd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jhrnpjnb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jumywpnq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3epghylsn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lldfrhwy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mloenoqm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vulmlvqd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3movevuzh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qnvpyusz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sqobilta.html


<!-- 参考信息 -->