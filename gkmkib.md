代发 wailian999

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fugqopik.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ejmjnhrq.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hagiwmtt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ejuoiaoq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2tvghvror.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gnxuoion.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2abosotrz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kplrcsdm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2psfbdjvk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qrfyqvjs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sgdenoli.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ajgmddag.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2aokrpssk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2dchqxndx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2tbxwxgek.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2olkplncq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2zlfgwswx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tzkzscnu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2mdkpamoc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lehfdwvd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jajgrswv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kxqiqgsw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ipbmsqup.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nvqipvba.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wgpwpgfc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ldscaruw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kivjsaru.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cvwbwvfw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2doutluwg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nkscundv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kcyetxxh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2llbeyoow.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tcmdsztb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wqbncjmt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xrybzqmf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2epkidbsq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xrkwqjdn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2grehtqvt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ztkewbob.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2knqgrgkb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2geygdmzj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zisrmbgs.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gjpwyhxr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sgcvfxph.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2foqfpvaz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqkerjjz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryunnclm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bvdbgmfc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hflpndjg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ixaxcumd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ayjjgytt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvhjlwyj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2rzysnxif.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vnpfccmw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vtaqyjvj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2kaesogso.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2aojckgue.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nfzegafj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vuwsiijw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2umnmpsxk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jmysupps.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vzydgqyt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hpbzrbsd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2depkbxum.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2stqepjtp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ffrvbogr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2vuqkkaxw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eehysrwq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lplnmbct.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pflsnyzl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mkozblnj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xqnsfvcd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ulyujnww.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xglirvzy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qklqztsi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wcnrvmkk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2mbtqhbdd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zxfuoppe.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2xiiienrf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ozzoxjhn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2taxhyfnt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qlesbxcl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ruvvsphr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2erjpnoep.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2lybpzakf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2shiqfszt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gyhmuuhi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lbimnnnx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2enoytfhc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wfefcixu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2obwnztry.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hjchjrni.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kzjfjdpu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ahpqxmkd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vdycduyd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2eosyxmlv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xhvhefgv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2bytpqega.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2stjitaxd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2civhhuzr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mpfvlxmh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hmtewwhq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxqrlnob.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lytclaod.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2jrzzwjch.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2yjmjpdpv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jjzuwrho.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mqysilog.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mwqlivor.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2unuzwnfn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wytgjgrx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrbknpns.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzgrxukx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2rxsqcfbj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldinqsbn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2yvvfzksl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dhrswelc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nzezhzic.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ytrbhymm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fyagyrok.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wjbzeqob.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bbgzpgjb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kvhnuesa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fqkcvzzb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ukrsyxxj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2owhzdaif.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rubfpjts.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2padccgzv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bcdqrczn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kvatdwao.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rcvmdouf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lsykusac.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hmracxzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqwqxmga.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2cquupjds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpdsphej.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fqkuunkr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jtmhxlvc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pxmdpblu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ryrfpusi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dfjbxmkp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2htxrrnbw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2keiozlsl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxiduxkw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nzatymyo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zpkerihy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2erirdvwc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rzsistbh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xufsawms.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rskzrkkx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bczzbwsg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ynqonddn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2drynfegt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hovjrmzf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kpaemmlj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mfczudsp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wcdddqzw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jnmkvxev.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nvggvmsm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pautwwxd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ftixktah.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2pesrczqa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ynpiojvo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2drjocmpc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2crnnygsl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gvufxezc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xhwmeslh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fvziefue.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ydaausjc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fdbipzxv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fnuwuoyo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ummtifsf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ynkjhgmk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cgxaxgew.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qconklly.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdlskczd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vyfjatre.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pxyiiqpq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ffqtjsbr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zsvmqgyi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nljlqtfh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2awakefgu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzkhzcld.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eqyvpqqx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dffwcghe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uyaksdbd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vswonach.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvkqeanj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrtolljf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wbabspms.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2szeqxffp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jxtaqvif.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dlamviug.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jocpokbf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2toztftbo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vqhlpzez.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2zrrvfurm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rcvzlyyo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2szvlhlrz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bavzdjas.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ioaqxjqg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2fmjhwbdx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sinkgkit.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nodqjovu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rsysnckp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2frrxusmv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yuepuvon.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wioqkkmk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2igkiriac.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ivcniaug.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zqyxlxns.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2aokpzhhq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2exzniwxv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2moleetlz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2pihnsmjg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hikqqkcf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2uyhnjptj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gdzedztn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgvpwmzl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ajdxqbvy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmdbwsdh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkyguzup.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2lwhyuexe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bcmowlns.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqzmmzoj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nnksviyt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qirrluhs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxvqenbn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zpyaaolr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fyimiwxv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2miedejhx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lpxumwqf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2golvjhdd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlkperwq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wqnmxxhs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kwecwyzy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2glokodyn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xurwcedt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2autdaegz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cvnblfjh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rfrxorrl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2epoxatyq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xxoqhqqs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xzfgexfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tgpjnzgh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2oxfvinpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqowkjsy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2extsnaci.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rsemlrck.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qbqdpkpo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lmcxubze.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtdrjoai.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2gmzdiork.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2dhaxytjj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2byyvdwar.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cpvxrrxe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2knuidfev.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2vredoypu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2fkolgsvc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rknjrhcl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zxpwjftx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tptwesee.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rxtktsrf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2tnhflama.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kwgcybxw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2sgnpbagh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jzjmkine.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2aeudibiv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rhvzaslr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ijptcpbe.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ozcapwis.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zfvzcomv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jczvjxhp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hiasmfqj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2uwihwgoi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nviqmzjq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hvehofiq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpfmgoso.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybmsjavy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlvijyey.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2minqwuxt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aqyqfeic.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jvstmwcp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hfjxgbij.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2dqjloizm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2btzmguuw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kvowxmqi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2teerkxxs.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnqvgygn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vbbbadwj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vrwijnnn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fkzmcpmi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2maodruza.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ohffmkcb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ueauhoek.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tgolpfbb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmsyspwf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhixtrzo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2npfziqfe.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2uezdrelw.html


<!-- 参考信息 -->