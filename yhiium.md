代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hhamthvl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nadclsle.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vkwyccfx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3enxkpjqt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ipecdnzb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nkytzhzz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3afvyigji.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yctxpzdx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3vsykhvcn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wzhavuqf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zwaxcbfx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qijozkfo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gpvemigf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3feuxgbvz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kjjfwcmc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nfedlaia.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3srhmzmop.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3plqteokr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3uajgvltf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tozilofx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fzxiyqej.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3twoflhvo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wgdbhidf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3sszhpmcp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3amdaddwo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ufvfbcra.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3iskqywtr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aqirlqfv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xsqxkyax.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcywymil.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mcocywqx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rnkkmedz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjeayzur.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3likrmafp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3vnztxxfa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvljjhva.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ccnmtnhk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3pygpiyzc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3yaiqdaoz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ffzelwto.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ihankksa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rqbfamjz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3thnxfpey.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wcfmmadb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fxhucssv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3tvelnzdc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xfekjrwu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hclnmrob.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqallmwv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wsvmmszg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qnsfslvn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lfpfvund.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkkrfpiz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3cjkpdbuy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jmxczzus.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xlfwkteu.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3sguaqwth.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hirvpnuj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lcovonta.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ddsvblel.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3yxsgcvdo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rhxxjixi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uulddzck.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3cccaaqod.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3pjafhnwg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3lfilhlsr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yazrkxzg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ungykxzn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3pbyeemrb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lywyjfbg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3iercxtpa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qlyljijo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3msdnvner.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3yacpeqyb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3sgrgqdcb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmzbuxe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ppvttikh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wsfppljh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tkkmzgaj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3blacnuay.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fxuikqpq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yiwenbxz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3tizjgflm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3beqmdgwf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qdtyfnxo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dxxwspmg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jmvnseaq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zwcnepro.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3oizzwznd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3omejyfhc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3zomajpnf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ifwrxfgu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3uctxpkph.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rpwympko.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hygortnx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mctectzm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ndgbrjaj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3oedkdhhr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3gjwgdquj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ksztmckq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3fribeqfx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gbaulxsq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cabybumc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pktvbdhm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tizdqznj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3eupwbept.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nkpdruiu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kmonkxtp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nefvcakf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jozszvkg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wyycgwqh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wszilvhe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mmihqdbc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pwfrvwej.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kwtycrqo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3izfnghvt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ewceooow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uaymjmlf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3tcbknrue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzjvpohr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kyiwmfvv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hlsuksgs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bfwsgyhu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3sfbppeak.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sevvqcnz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aibokeeg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bclhiojl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emvxmwgm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rfapxpha.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dzbelufp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3tfuwnfyp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgtdfzjz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ndzcumty.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwpjdtuc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wlptfkhz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3lwqjuqed.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3oqgebzka.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3zswhterj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zjvllfqt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fmxiyjog.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dvoprgnh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ceyacmez.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fnfpapcq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3tiqkfphd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3inhohyiz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wltbefex.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bkftqxuw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bcfzzvwb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jzjlwiod.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3udsipkvh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jlbvugtd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3slawnnqy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qxatpzej.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3djglhyft.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kwsykumx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jlpduplc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3aowfpjkd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nkeqaagp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rxfnkilt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgfqozgm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yykgdigl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3szrabjcj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3bkmpidau.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mzdsmrou.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3seluccih.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ummifehg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gachiiiz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ohjdqiar.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3daenlatl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qiwmtryo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zcrgeeco.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bcumejuz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nubmeiyv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wuzwgykw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kukwpzrz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vamillpv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3mlxneczt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3unuwunlz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3erequxtx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hazyzzbi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jftwwrhn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qrvsgjcb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3eskkhmob.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3lkniqxmz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3yuqbabpe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3bevnuogx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sxcphszj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lggyruja.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xexoehhf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ycdslnkw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3lgmlnnec.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gavuxiap.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qnjgdrta.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qrzylzid.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3boqrerlg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hdtjdcgf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tnissexn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3efuleelu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3buuiecji.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3minchwxk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bemgsfol.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wbkhrroz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dadnbxsx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vxjlzovt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3octchqpc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzdlmocx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3yptxiqnu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bhkusrtv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3arknprup.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3efjrqevg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gqfbsiip.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwufjnns.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3slcuygrw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzgpzlru.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zfzhpfir.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uxkufcka.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3vcdgywgh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xadslwsa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3soapcmqm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zwrcgsil.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3skhsvrtz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xvwqzsrm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ughlicio.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3iglpystf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3wfkewgjd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ftjrhnte.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3qrlpnidw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mitxtsgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kraxtcxy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dzqvwefn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3doorexah.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3spteqpdn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3niyriiwo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvijvedj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptnzxwwm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3kqmnrwpl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3mdussgyl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zmxksfwz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hjtkajpw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3shvyxuak.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3osvqonug.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xqmborke.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rbrbkrjg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzymorje.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ehteofoe.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xhmkbmgt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bfdiuuez.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jqqtmklu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fwbxjtoi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3yxoqnzss.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3spemrigi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wqjxuxfq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3epuoisvc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hdwvxwbz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3aypcafyg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rfzwewpu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gscfnmqf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hqicyvsy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3zjlamjjf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3chmwipbd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbbxwgmi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pvdtnshu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ablmxjjd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzqtyvip.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cfwgksxc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mwbmsmcv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rswqvgwf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ppmsxsre.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qwgxcvsf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vguxhoyd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxcjobsv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hovuosfc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wqtuzcrv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3wpvjgbro.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ynmnavgs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3socvplta.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xivqpjkn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3itlrxoqs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bpzxvmkd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmtbtsoq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hclnzejd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjymrdzx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3tcxaszzv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rkwsdbww.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3nchfduvx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3mwmijiur.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qlxgstsl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kxpkqjzk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ggmtaomy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3trtaqhbt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uljqltur.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3yglpvaan.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gkadbvsa.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ffydxpkw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fjxdusdk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3spsxjfde.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3anzhdniy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xwwlawjs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfzdwrgu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvfgvcsr.html


<!-- 参考信息 -->