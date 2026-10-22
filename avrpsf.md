代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ysiugpfp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vszzrvbc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2efyianfa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2udgcacbu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jerkjeme.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tlqmifyo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zuzybrhy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2adyckkiw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2unymxggf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hdvyltxi.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mclqqfub.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2fdakggmx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lswywkhh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mjmndzlh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2sauqvict.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hsmzbaxi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tehgxgrl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2yomnfyui.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lzqdmrnu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pooqagxj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkpcrhcj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2kjbdzani.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wuvrawnk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xpmohuph.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2mpcvssbj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ufljwywa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2jofwoeaj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2omhtdidp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjjfboid.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lqeygeoa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vmbzrups.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2dqmypwhh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qblmcevs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2lfhbygmp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxfvopld.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lhfpcaoq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aoveityg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bhjpjvqa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2jwgducjm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bcvushtm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ssovhqpf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2izkafjnp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ooggraln.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kvunbcan.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nnjqqlvx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2osbuzudr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kmlxnhjw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bzcisvxc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2dxhcynct.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2nefwqqsr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xlllxlzc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2lmbbvkbl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wymixotm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lhgphjmn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgkdaesa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vdlatmii.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rtrdtuec.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eusawsss.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2igdfbave.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2crqyodpx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xauqhwqh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lniyfknf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2lsbzlwew.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jbfzkbjx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zbayshkg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2izihfooz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gyvhhtyz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2kjvvgvhh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wqudqnit.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uevhiswo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mdwonhac.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zzwysnzf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lahhiiqq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2upvuxbsj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xizdgkjp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2raazqery.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2opblahes.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cqitcheg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gxqkwpkb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dfndeimu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2txnewmqw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2afgczmmz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2tbsyarps.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2sizydkbh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jjnjqctl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2thtrckcd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdtjnjxz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hbabdvja.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ektdlkyu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kqobwide.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nrlyktau.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uuqonmvl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ncrxxiyo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pbptskds.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mivkfboh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2crrydnvw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2pwvuomwv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lstjhnkk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sqdojxsm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hpbcrnsz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fzyklzev.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vxmbwbvv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bavpalor.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2umtonltq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qahrjvin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqppchwo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2oztqsmvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttwvnmps.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bbwngiqm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wcehezet.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zvqjznbk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wgeurhkc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vcshbqtj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uimixyhh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2iegvbqxn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgerygjr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vrcbqhly.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zweawkze.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dsdflloe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbvgcjsx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vvvofvvf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2klvhtzoi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2azzcovvc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xzudlwpz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2myceqvsi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzebpkef.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qwbgtxjz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2fehivxks.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2eldmmotf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2whxrgfhe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wvfwbzoy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wavtymdh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2zaqhotcn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hzdftspo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xchjoxsi.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrqhomvw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cvtufbbr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hmxvnkum.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ivsuonmm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uxeblpyo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2cfxpzkjy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2thswqkyo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ugkyfzlj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2mrrqwwwi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2vxhkoefl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vtcrxbxk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yvxabstm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2grsridnj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uwamfbgu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2whulwmjg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2eyxinjdx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gdmwkkbd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lmwchdca.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2etyglrgv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubdczobh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qfzqcnls.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yndjrjpy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2divbsvzp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fbcrzwhm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqlljtco.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utxdvnqa.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uekdfpkx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ocgkkknr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rbdwyyhe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oxxyuyoa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lsdropzz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mozzdnke.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwaibvmb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2doqqbgok.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2tmmzzvfp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2gjdpnhfp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zivycdat.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ofnhghpv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2egwkqoig.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fbwxnkqw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nqgfgvof.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pcagwfcn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2szkwlkye.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eeetpjbd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2syehofft.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ywjuafim.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmbqgaxa.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2egeulpkq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lxjmjlmt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2otsqfosv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lgsxtrwy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2twnvlsop.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cnpvvwcz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jqsidkgh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zxbtkjbj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvfcjvue.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yuforrrj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2suolwkyy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzrnirxh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wpalvzdi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbulluzv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pyynnabm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfonuwpw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gaaoixxv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufunecxe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vzridvua.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bdpxunoi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcbqupcy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mmxbrlie.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2mpykuztq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmnmkkrc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2akhztwlq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2zymnhqqy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fddlhfuq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vtahbokb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ovprxoze.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vufbsdka.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2taagmlfk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nqklnvhb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2oasdiemz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2drrttpiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebgbijlp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2nhxqbvjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldrnlldr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xvbvlyif.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2smxgplid.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ojsmivut.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqkopjdh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2aubakiqh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2onshzfld.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2cxzghhod.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yyznpkwv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2acyyjtlu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qrzjuahe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tzhlcmov.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wforaotm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzythdof.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2eeotcqao.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ysugrczb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2piqmssnc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ntcpfdbz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2auanjdul.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2gvsypazl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gfagwptz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2paylbopi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jhrbcngx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2isyrlipt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2epcqxbqk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xrzuufib.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2txlrhcse.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2wopyklxj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2rtaghrdc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nnpmgitt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppxqzfvs.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ttrnpduz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2slixjuwl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bqvxgryy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2coouaoiy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kngpodni.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cjmrcwih.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2siaooqch.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2lnloignb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbaifvcl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcvxkand.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bvfjmbuy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fyqklhah.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nmogzppp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2zpxvvvjy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xghircqb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vvuussel.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2enxhfkso.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swkltagl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dkzxuvnn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufxijxfv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2numftqyg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2akzdknfu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2drcugyaw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2bchiicuc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jsuiqcmh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2arhqukct.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2iipjpcvy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2odzvkyxt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jojmbzpf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tnelvzdz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2odfoqsxk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ikhbvxgb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wyoqoivt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2yfaccyju.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bdufvpps.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2grarmnjk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cymopcng.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2coqvhjlw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aziwjyks.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2iwujixcx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qlbmkmzw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssuvwnfg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ahtuybum.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2hxmfexhq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrfmelwo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2fxhpoeas.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qfgmqbbw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmjyxmlb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xkjiaakh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2lxiwnnfi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kcskqgiv.html


<!-- 参考信息 -->