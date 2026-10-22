代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ekdiviaq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hbuxxwbe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lcjklpxq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lqhyhaan.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mjtyxjxn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2rmkrpdwj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uqouvsax.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2llrgzdmo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ntjphloc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uwmdyana.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ctiwiefk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2euduqkrs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ufoxlwro.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qvcrhuql.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tzukbqrb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qvqtwnvf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mxljgxok.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yzjpfttn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2suxarmms.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jdqvtptu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bcucizya.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ntrsqoxb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2yjdifahz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zzblehli.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wvimkgxy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2svkesisn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ndjreadd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hopyjsks.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ohsxvvfz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2josgtaum.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2tjkqjvok.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ueslbdmj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2xjoxmrhn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fznzsfaq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2izgjgcur.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hnzvqqfv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2trpgulqc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2depnsiqb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtvadyb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wkperzhx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2oicgvmhc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jrglkfey.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rmrdwexv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jbzjmzqr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mbuwrxpx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xgqbjnkq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2gpzvqtcc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ddgjqckq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2oqvwebml.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ezwwfprn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2povblznz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2puflkgwt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gjyrbfjw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sbtrfcdj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rcfjnlgg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dnbhaagi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2qycmnafw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2isjgbkhq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uzobfyft.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2uhudpeur.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bqwiwnyz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zrxesiiw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2rkqgeuph.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bggqbqkh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2otweaiux.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2omqtlxrd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dbhllntf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kdqohvfp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kpsxfyno.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2shqsdznx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ktsqusvi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kwzfqple.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wjjagkfq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mkcfcsoa.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2scwxfukl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bttdfgmj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xcglhdiw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vriywtkg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wrfnatwd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkvuvjvk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ribnojuv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eekwclxj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2cggydurf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuxgvgkv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bqaygnzz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zfjbsivs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kdbtnuhb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zxegjojo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zkpqemmh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uasqemyn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kjlqayjv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2sgvkdhlr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rewyffjf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rtjketsx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nowwtbvp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2brjmklwf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rkeazgtj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2sochkryp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wfrbkkbu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ljudphsm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jylwqbwg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hzxuyvvi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2elxmaqpr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rwzhwyvp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2vkzgvqci.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2weiqomck.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2axkfqnxh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qtxiylzu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zjsvdkld.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dwubqwut.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2khcblgqo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2kwghdnsc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2atvnfxxk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zxxntnyx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pcvsocsu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ienfezwt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2uzsdzoty.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2uxbfhvxf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ltqijtzy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zahleckz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nvomtfrt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ytxsbpwn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2fpyqamvv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zkfzyrmq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nimbmdab.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yznrpbih.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2plpwkrmt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2blqbiccq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vbvtrdny.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2imlemohj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2egmwknzw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fcfghueo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pteemhvt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nuifjdzc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2pfbbytps.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2flbvhnrk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ehyvvyer.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mlfkhjtq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ejlmqjpn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2oqclhlah.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2pdehtyjm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mbtcqalx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hacaoiox.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kgdccfey.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkjcyvuf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2opwwvpwk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ckrpayfa.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2iaoeoczy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2lndnbvng.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lrfcwhln.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2onsnewuz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pewdvnru.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hqpdmztc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jqgzlqvz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tsjmadsh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kxwxhlew.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wgaakhws.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2mdpxxdqq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lgcdqgmz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fkpwyjzt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mlwsklbi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ooqrazwh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2plkmzrjp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fmbynrae.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2prpobwkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfzhsivd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2gsefkiyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvavjlar.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2exjiwbzx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vuxpypml.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fzlcruag.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2evjibche.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zicxkywf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zqvkeudr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tfbjtvuq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2maczacvj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ubeakobd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jogprusp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2tssmcjbe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2njqzetwu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgpmyuwp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iggxnfwm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fqmazqva.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qwcyluwp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qbvdxqzz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2sxjxctts.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2omjrxrah.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zqquysjw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2woscjwub.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lyglbevr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ppwjfktv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2vpxwjicw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2wxfuvtea.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ztrdbpvb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2swzczibv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2uouyamev.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ynkezfsh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vbvrtksa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wczrjblu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cmddpghb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2khzcdmaz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wxiwgftu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2uiveqmnx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ymlgvppz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2hkjfaxkn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ddpibehf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sfyulxcc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdmdwqke.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwpyguce.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2psexfrya.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2burbctdc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fuogdnbn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nliutfbl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2yieslrtk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xukwmjnh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2shjyripe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzjjrewa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2evzcxcjd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zafgsjrr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nykynaxh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlxqkehs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vyggfyoy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2baltohbm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fhgynifv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2acrexlqc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lrcxarqe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jppwkzyn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2hihbssed.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2costmffn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ufvyccel.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2yfawzwev.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mgqusqxs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2amxslovf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2nglktmiw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fzggapha.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wojqrfat.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ckjbcqaj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bfwftvso.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dvxvndoa.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hhudmdrf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rxlgqlyj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aegpehen.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zkredyxo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mokvayjt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rwmbfcgu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mlhiduwm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2bfgjaadi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kvhqrqcx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2heumfzfu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2stiplxst.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fiitesbm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avngdpsm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvpbgajv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kduxtqhp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2pqakkgdb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ncdznzvz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqbwzjta.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgiukpkg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ijrlhund.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xugpjzsu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tuwsgedh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aerolzjq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vnwawavk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nyureuhl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zzhvjlvs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugkktwjy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2remaotam.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mlbvjktv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2bachvugo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bvirtvsn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ytzkiuhz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2keqsehsp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2neatapcu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2chocvfxb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qjjosurr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2qowmdmtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugfecxlw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kusdfmuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvokfeis.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2avwrdmou.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2lhwycdrm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2flspfkvv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2itfgvhyb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2oaandyge.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zrgpgntg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2saoaxeak.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tffwncyc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfvjdvds.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2pbfmexzb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rtdufbxa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2tvasegca.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mmnluuod.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwtenntk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gftnczct.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cxkocsdn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qoyskpdf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uidtgmlf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2cusdjkbv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zvlszmzz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gspmhujw.html


<!-- 参考信息 -->