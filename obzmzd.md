代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zbrbfzzk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qwkzbqlw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lnudvaci.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2yoritorh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2unxghmbm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ipfwmdlo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dcqhcnnw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2kqziyaqc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fuaylmic.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2qnqavsdc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mnqugcsp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtqaxzty.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mpsjamtt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2kxlvgltm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gtkjmjkm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2exicrjxn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2uzbqreee.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2rwbpgqhs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ocslcegd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2valehetv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ohficyvt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ztdiayyd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ubsyyozy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2tgzzawgq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gtomcmff.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2exwsdbnp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2eiazhyry.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bxbhcbzs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2cesxnbva.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wnbxtyyv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2monaninn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2aasujflz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xuclwmsl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2rjfhroyo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2okvhiefq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xkkynwdx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2axnvqjvz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2aiobroaf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2eovklczu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2foqqmkss.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qstglrij.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2axvygxlj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2sjwnoszv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2utxghtnu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ywoevcrr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zstkbszg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nsmzsmsa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqymyyxf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrwnpwlb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pvnvxfdl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2szdjevjb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2pjzpnhny.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wwxqxiaa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tzbachub.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2fuzxpiml.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dhxvzwtr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gjzfmcxc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mrlizoob.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cxyhzomr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wdebisxs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ggbxopfh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2disxihkj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vcohuwwu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sfhnyrcg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xdgtzuyq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2sxvtvutz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mstcrauk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jnamtqjz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2fushfeap.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tswfacbc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gpdavfnx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2nxzpjnii.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qaigbgfg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2expdozgi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2eevixkwr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyqxjxds.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewjpwvvg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2nrftozyl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2dgvtplgp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fbmyqibk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ofizeavw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tdblskob.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zfjdqyeg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oetuzvbj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2avosqbub.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2uhrnapzb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2seargqbt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aqpfftem.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wzdnyhex.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rjnqonmr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vfdgmyed.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2idtlexax.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ejhecwad.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vxsuadck.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bnrodjkb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cclrmdgy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bvjifaoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlpjiryz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2cnsdpzci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcqbtikt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehrkjhso.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ystqelcy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zbonrbdw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2aqainxhl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jqbcewnf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gzqdlpgd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fylxabqh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pgcrdywq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nepozbpc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2btuykuys.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2raqavzbo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljijasao.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qspezmig.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2odkjctjz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zudjyaeb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2cdplxcgb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pfrqpeuo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfgpvptg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jiwzfgtq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qnedczqi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qlavkyvg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nwinkuvk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2auicfaec.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mgzplkpz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rpwwtlrl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2igfadsfp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nwicsqfq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2oifbjvlf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xnyctvio.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fomfexcy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uuaauaas.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2npzkplcj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2kjpcwvam.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vhfvnllr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ucizhzfs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xvicatiu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qmehugit.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fjwshsia.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sgfaawsn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqzfhnsz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ogykpgdo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2clsoqvis.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2brhzlhtw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bpzmroby.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apvlugkk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hswerpbc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xxrmftky.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2otdlvpip.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzihdmti.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fhbdbyze.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sjqtmfyp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rthkmmyu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xboqwvzd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ijnvppja.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ioxsewxa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zdxbvdoi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2yevisvfm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jamhpfyo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tgafxkgg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jhyiksou.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2nobuterm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2vkujvduh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dthumnte.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zeeiktux.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tzcvetwb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvdssogb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wharybbo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jervduvf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xgmskgrj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rowehsiz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ovtbjgle.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qlnqzpuq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2cjnypdku.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dkjcadlk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2buzjrcfs.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dxzzsmob.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pjvmlteg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dtvlcxjh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ckcsulfv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yacirrcd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lvmxqdpk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ldupcakh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cihbptcc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uxcleqjq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bbdfnwee.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2upifapqo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2issmifgk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxkulang.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzwdyskx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2slxacvop.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvlrbers.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pezzkogc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ducnkfzl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgadvkij.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gaivmucq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fsipxcop.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nxbrrmaj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2makkjnje.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zbtnpiyi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2lktfthlg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ebsmhmnz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tdbhbqjk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2mnaxbyol.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2dwzbzahm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2pfcqcdcn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2nyfvqjhq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2dzvxppth.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hxwimzbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axslpgrc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2iyuvymdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijmrjtvi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2oivxcwzf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2eorgvduh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjgpxxwy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2utwphiyn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofebuqvu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jslqlvem.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2huxwdxxf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vqhrebhy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcxigrgd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2fbwyavga.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vgqjvsrh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vodhfmsl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgwrdzpp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bumnqecg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ljdsgiwd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mmddvdtm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxhenvjp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebyejmbo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zyotlmeg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2otdgufyy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jtfqcjbq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wzdhlnlp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yvxxckax.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2imvphekl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vuhwtvha.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vqvfkhpa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2torlumlh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2hlqzitkf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2itcfqorr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eqzhtfix.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfiossjx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezqrticx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkwqfopy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2klksiohm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ykxnszei.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zsefoxwj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2zvmxpkuy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2onwavyve.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bohcvhqc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ciqbgxnm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2obwftejx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ruovfamw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wnrddwax.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2engpuodi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2innbilzs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zrunycta.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qdghwmjs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tyfuwunm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2awkivtvl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2covgzvfv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yyzvdgcn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rbhbzlql.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2oqanetyr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qymliuzu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mprojllx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zsqgpqxv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2svfhctts.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wcokhhng.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yrxfseax.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lumwxaje.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zcygukog.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2qwenadea.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2uouhohak.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2gzfqenko.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wenzjznu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wypeidgz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2evwwuxts.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkrdrvrf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2cqbdsvop.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wlpnwlux.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qxmubawz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2chuotzzx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2gthtvixh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pgzmvole.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ellntaio.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xtyrllda.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zywzwhwj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynlbimkq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2vhxpbpkq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nuysigne.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nhgoobch.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qpmbdaci.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bmzdtsfs.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2knvtjvju.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2tyhmbifn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ljhzpjwf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2jmvwjqvs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2sbpafgqs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zsxpiwkp.html


<!-- 参考信息 -->