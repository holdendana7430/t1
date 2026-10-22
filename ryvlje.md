代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kowsegph.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bcoxcydo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kwgqvvis.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yipybeij.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2reecjbbj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xkbkfpqd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ijhtivlk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xmocypgf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bzrnmcqt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ylhusuaj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2czrtenft.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jtitgaxr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nipdozjv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xdohohcl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fyylsctr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ncfwioxo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ymoxtpss.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2osrlwogq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cnlcbqmy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2pvpxxfqq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jyrxqsxm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fbnbxkwi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vzqjnqju.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mjutrdbe.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xvmrfvmi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cgipqhih.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gussfomd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rvmtgnrc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ikzdzakt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lafugowa.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2shzazsgz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ljifwiym.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2elbxxfnl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mobatdyr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2szvbmzoa.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2zpukdsia.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2iftqpvhd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2asgxuaoo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xaqxvgjs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fwbvnxro.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbxfeydc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sbzgfnsw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2pjkxgzps.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ujkptvcf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vmlpazvu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vigxpfcx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2upfpccbd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pmysjwgw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2btihvaog.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kdtnfqrc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lygpakhd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2iwthkyqi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lnismusk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2myamketv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cqvkxegm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2cfmscxds.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2kovvkdbs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2amuyugyq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qvyrhbfl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxgxmpwa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2dmaqccxd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2cwegcqxz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2uodmncbt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2aqiisupz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rdxvchbq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tnbdzyyt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ppfqwart.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bhtyhacs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fetdsmex.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mslafuwc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2wjudlads.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xfathujg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ntldbtpt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mvxqsawy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yxecfqdx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhawoxse.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwduotzm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ugaxzphx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ayjzdczg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ueohsiui.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vdnmbwcw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ozeaebxb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2hlkcocpf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gdyxfkng.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rfgopbtw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ahcfjgal.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2krtizwvo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cylpuuio.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2nozmnszn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xtecfcta.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2xeqerzem.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2imrtqffk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dhkwdxuv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hreritcl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2sdgibdfp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hyhsbdjb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2omrifguo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wobqhqsr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2irsnzycd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2buqsedkx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2pcrdprop.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gwpjgwqc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lvdtyqmr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jumuietq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ystizrzl.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ilbvtkup.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2owfchtgb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ucmttvdj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bchuxnsm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hpggppim.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cglnvfeg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2estmeglq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mgdtbnjb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bbnrppfl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bwaidpip.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2medumfwl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2eqpsenjp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xizpdlor.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iwddsvwu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rochuwad.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mdsyobtf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wjwijoia.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cnwbsjfq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qacpuitn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tszclnjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izhphpjg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2lzljqxds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szyybpcq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xspwospx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2btkvyisu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ulvqnaok.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2iwrtiiwo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tuqvxonw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ucgpoinj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2orpxlbsp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2atktgbys.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rjuwzphg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2fwosoryi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2togrumne.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2cbdmvudb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvdgincd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iasfogbt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xfaoxsxg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2nfyrlvxv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vrcjdxlf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2nvdobchg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2utghtrbq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2axlthfav.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vjljccky.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jayjvwgs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2iyttyare.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lmxtrcnj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2gazrimlg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bfdszhzx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2calqzrwt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2absuvocw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2naxrxnoc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2atbrkoys.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qmybbzlw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ttbvhkbo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2sjhigjps.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cqeuftdz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jxnedbeg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2iyalztde.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mkeomvai.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wkxjvpao.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mtqlymcm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dwdiaryn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmekxyfo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yqzigzna.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zbsnqlxl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yfchgnyp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pghhhbfe.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2yjapbrfy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxitdmif.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jctjijtd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kppaqsoq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgiemtzr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2seqttavg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vflyundw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dldmyfgu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tsflgelc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jdztzcmj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hjvmgtmj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zoqiplbk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2smktdxkk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wdulgxfb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bzxtiecz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qowesbuo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wnruueee.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jmkowxzy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ycfgetee.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bostwgsn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhfrludr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2agsjwetb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yosrngvz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rmognkfe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ptawsdqt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rmmsvmsf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yqfijips.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2mkmunboq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2csnknxzd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lmdratml.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2toowtadt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vaiacifk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2owfuowhh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vpguevyo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ppeqnglb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2vieuglwg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2easdirlc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cereayur.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ccngmyez.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nimzihay.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdloxfsr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cdgzlccq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbgsqslf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hdojqlek.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dztvicpp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhwprqua.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqitatkz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lzethrkn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqewtzpy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2elvymrns.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ecqtrksl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2agxlomns.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjohxqag.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wieafuap.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gvigyqaq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2viejalkk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rtiobwux.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2uwpjrqjv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zhfijmiu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ikdmfsmh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ttzeporh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qqlgexfx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zblacxny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbmuhzhc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dssnxjbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grnqgjzw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2jywplzcw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2lhyryxsl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2nyltnnnx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqaxeqpf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ahymtwep.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qlrshpcx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2swwwlpdp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2oyrefyzh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2iuftudud.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjepvfed.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2frkfxoel.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qswlqzpp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lpssdiwu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dowziwja.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qnkqwozp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2jggvygvs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hipiiqkv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axfchgzp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vvzxqamn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ftnhmqow.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2sdjxvwlc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wkmohwfx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qlfihcem.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2pdocwpik.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2spxhyrol.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jxyivdfe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fcceemgj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2oozyylgh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eycuxxnf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfcmddbs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccelpcfc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvjjjtbn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfrdwdaa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lurvydyx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sdzjoyco.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mytkfudz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2axnndvmm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rtqizmsz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rkabbbnx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fsgxsisa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytkmsyjb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahgxewcv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2gecyomrb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gbueobbi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2cqfwdrnn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2lvpocuns.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xikvreht.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwcnlqdp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gzkigwcg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hxkrqcdz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lptzwcrv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bwawheve.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gbcrbvix.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2gpmrmgjw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2smswizrm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ltrnxlef.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2nisbxoah.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2atjgoavg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kvqwuqlb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fnxyidoo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xvhkyqde.html


<!-- 参考信息 -->