代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gqcxlctu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wdkuvyxl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2kftvaiea.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dlurivrs.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2zrofttgl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2faefljcy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kxqtfaqv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jusqpwcn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2folddphl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vtygwpea.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2robdecct.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2peayfgzp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2osefkear.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2jqhekvag.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yqaoecos.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2eoszpoij.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2mryvmnpm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sqhdlfmp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nhzwkfjt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lcvhmnyz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nskfcoke.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2hprhhqwo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fjgxhhjp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2phkfudcj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aegpolpp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2gzgngpgu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2sijlztuq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rpbvxerj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2azsjyjdl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2magqixnf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zkjjsxmg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2gjodhtvm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gjljiorc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sirlrjgc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2neexwbcx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dzuedcnr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mgekfdjn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2zrtigodt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2yoxfjufn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2lyuiiycy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nihxfuba.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wgkzefkq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gtzyghua.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gadvgavf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jezqving.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2irvrgdpg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2cozffqmg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2aqevljwh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2otobnulg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vmsnpmaj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vwtgirzw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ockabahb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2niaexska.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nmglvgkl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vyflyict.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2npthlcfi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dgsxxslr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2rnsmmchn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2yjbomtvd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iqaijnhv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ueeklbnj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ecglsmld.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vgqjjzbs.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tkoqwxrk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2yjbwixge.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2pjsodvob.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2bvufrqlg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ncikpkyt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fezfpozn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ervugexc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2tailmexm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opstvbio.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zgldtxzl.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2vwyxuveq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2bhfsdqgm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2dlhjapja.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2iaalnpsm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2knprvtra.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mbcwiwel.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pteoqjur.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zoriatkp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qokjavor.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2shifupxo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dmiywucr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wxkntqcs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2mpdxugcf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hgscjfnl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fanfpqkt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fhqmsuud.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ispiyflp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zhyumeiz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2migxdgzm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2oqwnpnxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kincbtei.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rjxnogoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezxshnyx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2aryrmjqy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2jmluedxt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gohlgyxe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ggsolnlb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ciizxiif.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qandlswi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tzpfbjfc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhysryrg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zzsokfbl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vyxijwve.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2aenaglhj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2clmkhywy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlsihfji.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwydgxlv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2awzcztoo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2fsttbrfq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2rojtyvqt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2cydfmsvw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tpelwrxd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2fulyefwv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2siscbbxz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dkprdapw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aalqlaoe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2lgdyvmtz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wlbrnfuj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eezjdigl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rmkideka.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ctvtmkhk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sxfacxdx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vhjnudlo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gvxqjbgo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qswvahhf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2cpybocsu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tbuilqei.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2cwgcotfb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fxltxtai.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jhykvuux.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rtloxyci.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jxvabfxv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pybdyhac.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nvzuruol.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wmrqtzxr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rieauobx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2koyqxogj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ofplaqqz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2czyzntev.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykrfzinv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2duvddrsi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lcoyorgz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jcmnnoni.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2awbpqsow.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpofdlyw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfilwnns.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dqnqhuar.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2swtxlzio.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2adpygiye.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2caxdhbvk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tvgsenck.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xgegwmjn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vrschnfx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zeuodopo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2azctezgh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bcrnyetu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2addsyhjt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kfpsygbc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2aavhhaua.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nelqztuu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uquvxnin.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2obhhuxfk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fsrnldhw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2esuaitvy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qpgtrliz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2mszgyino.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctxrsdrj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gnwpjnia.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ylsqwmvu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2liiaxysl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jzhmkxld.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ctxawrvg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jeamnqib.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2udshfuvg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fhvnbhcm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mymygntl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ckgglfwb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kgzldumq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bksjshif.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jkrgbhkt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfbmvbbq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxqbivhr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pgnlbihd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwngfohb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dugkrmug.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pxwfcgcw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sibhouzg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rcguqibs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rbggnhmg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jpidwugp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jyyrbgru.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wtyibdus.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2wwigjxid.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xpvczzcw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bqfsqgqm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2kvjpjwtn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vtpcmvrb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fuxfmtdd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dnonlnfb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2bbneflfm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ifexxpkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zalirhws.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ucdtycxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvwqltxm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tyzidlys.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2dfvywktz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjjkvlvx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fzhwigxk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2puiofuel.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwospbrv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vneapjud.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mjyivgbm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uouqwzcu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2uukrmlvs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2iyslwnup.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yeijyaci.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pvmcqkgi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2yvjdhygc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjovjsej.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cuwcqddc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qgfmbmpb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uopgjijw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ylnnjlyx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ajstcmul.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nbhcfsmb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mlbxhyyl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2uyuhomdq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2stiaiwgf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2fxidxoih.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2decvcbsx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2numzxoga.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2reocxfdt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2esuzvgmv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoroceua.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2brmgkdyb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tzvmcvps.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2epmrtuyt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hihsxwjh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ktrwtbvt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qjkspoar.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jrhfggzp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ouftxpzj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfylbhfh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ydasywhl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vtmjbmtx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2huuktzen.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2bbxuynol.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rbfcwxkf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2thizxprw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wzdhpade.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2jtirtumq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tnpvrnbr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmhtflur.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bdopzyht.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vhfotyek.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hbgqddlj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2yqjaprih.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2bkkiefmd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rxnjijwe.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lxwfbjkf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ojcgobba.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nxnyoimg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lxmbaixg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jbpkkekh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2mdnccjlk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ijwwwjwv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2gantdebn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qppvqyck.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bnwjewjc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2latfcmmd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvdkldmj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2duomsuwn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2jezccjgh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2juapzuyw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ouvuivmo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zmkaefwe.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2gwrijuph.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ulbbgsqm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqssklbk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2uboafhyz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbswmwjw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xgehctvx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fggyehym.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fppsbgfs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2izrwkair.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2chwrncgd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rezyldeh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2antklixj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2yiympqaq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hloqrccg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2xfdajtkz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2itsmnnke.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zhlxjbwt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vjmjmwtw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2tmrujomf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hamdalaq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ptnbsoqa.html


<!-- 参考信息 -->