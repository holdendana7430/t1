代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2fywrvygx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2evtjcvde.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2tfxeojxt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2mukryeqg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yueljpaj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ueemvybc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngnzifvg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xesmvcua.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmexdnfk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2muvslyhw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nwkttokp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnxeygfa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hewhzwwa.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncnywfsw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2suyvveyy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mhwefshb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2evafjlag.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pnrdkfsg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2swystcld.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gkatovwk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kbzeocnt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tbyjxlwv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mzxqrawa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ilruhcoq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gsvwnvmc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2xpxihoib.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2letiflzw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qxkzkcle.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2awgyaemp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2umktffpk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nqohplyz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bdbgosik.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wlrlklza.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cymhctao.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xsbiaiir.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tvabqkor.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2axqihfwi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bqvqelrc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqqsjyet.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2iepbwxxa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fzsxanol.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2teofajwi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pcqoaiib.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xmjpmwuc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lfqqwmwy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yemmzjrp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sznfcivx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vtjxbsrj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wmxsagwt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qkbesvgh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qvmcazjr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2eedaitjt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2uwhhgvgk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtdiivde.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2yaueoulp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iulxmyil.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xaboappi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xtnrivon.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkqxgmgd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zirtasps.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2uptkqicw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2teheuoeq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2itwsaijf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vdaahiqa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oauivbyq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2brmtivzw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yfswlitc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2apvxtjtn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2leyzozcw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2micohysx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bcnhkqhn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hhxynamu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2amszkprx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bcvszkis.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ihuktipv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jduavdkx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2juygassr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgvalruv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mrrelege.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2byhicuaf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hdxuxvoz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2cukgzplj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2igidxxfz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wbwmuaqb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rxsweqqt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jbxlyyot.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2abatvamg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehharhfj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zbmbmlui.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiyxvoef.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dpstwsko.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2yayfvpym.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2slngudpc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mzgczybs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rhpmqqyc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mqrzwnmk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tmcoqgbw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ayehpqya.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2txyryrsd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2gzafhvpg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xzcaddaj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2scutfocr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qenfrlnb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2flxvuhyd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2grdgztgb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ufasfpxd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kxfctlpt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2schumyqn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yvrpgyyu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jtotmsvd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2myyawgzi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qjenyitn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2njzxyabx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2trslzlme.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nmjdwenn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vydjjqks.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cnsqnnzg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2licrfjli.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rtgsbqas.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mjatavii.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oazcywma.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rcmfnubs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ulwdvtdg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ofwfdufp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wiqmwqrs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2quktizav.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wknxhbgz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yswtrhor.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2omtqjevq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iexcoxyn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uybkqcbl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iymdtzbn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fyrvcego.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pcubarum.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ylsjvrlw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kbtjevyy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wffjljza.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bkefpafu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jzxovlkt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2pwfalvfq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2mpvyvagv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kxtgzppt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lewddisa.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2eiyjlrnc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oizxbqdm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ssvickau.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hvmuijpj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nbkuxxwe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qghdwrsd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rrvhxlzx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2opryivuj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ynhfhhyh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2sauisghn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rmliqdxr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bozshidp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sghermfy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ncbevxgc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eahekjqh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2thwlzsdr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlnjpnka.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mvutvlng.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ycztydsh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ycledcvd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yuwkviyq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ljnfodmv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tcorjbqn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2pbupcawo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vusdknil.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wludvoxf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efxgxubd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ukafejku.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uandqbjk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ptatohne.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhmfwqqv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xpkcvhmx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rtnsonyk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hwipqgnm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jtjbzvow.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2oznoimwc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ypxnrtmt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2iihzpizn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tweflezs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2rgduyune.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qidzsyev.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hulvhher.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2lwsmycxb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rmxnwuww.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ewhclgfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hngpnwil.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dxkychcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sorvtugo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ojeeolzz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2lwklyqfu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuqorbua.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqfajdod.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gfxveodw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2cxtiuiwk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ukpbildb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eeidqhyu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyyzqnyc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lewwocvm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nzxkrvzn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzvgjgoi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wjqltgmq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ourpyxce.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xboefyzg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ehejusct.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vcahdgju.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ocsyfimb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yvjoahit.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ikpvttke.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ccgxdrnj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2desyxess.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nbxjpiym.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wcxmugqn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lupcqdqr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2huahuwzn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2rguhflkk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2mehnszjw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rayqatww.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyuxfefp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wouusqyv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hjddtpdy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wxyrxsmd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ndovdrnk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2utrplfug.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wpsupczf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2dfyzcuvk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2hpdagclf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyxknqmu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxvaovax.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gpledmtf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rdnflteh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2urdtpyfj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2yzsqubse.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzfposlr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2vusuuzby.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2aznuziad.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lbolqjkd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvclmgtc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwtehvhc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qaifgddz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qfctsmkw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2tceidgvw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fybfmzdj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qvlzmnld.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2dilchefr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2nnnwwuky.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ctwdymxq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mksjmhkw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ivzmbjmo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cxcyzldo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2gowmeqze.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2umtlkyur.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qvcyyswf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lznggeal.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dqtjtyka.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qlqwoucv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2rgjqyseu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rizqvjeu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ezapjbbp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dgzhqgnr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2esmsyytp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bdierksv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2bnlajqbl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2urthzpxn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2odmvkzaf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2doonhiew.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nlktqozb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2thloehsq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2culavdfr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2akkslpmz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uggopukb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vkgdywjs.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tyaudkxj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2anlwpdqc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nfmrjfft.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2emetbgqp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vlmukcjh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oqmddmyf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jarnwyon.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ojxpyxta.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kzetivwd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ucinsbiw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqciptan.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2smrtqbyq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yblgnaxw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qshywbsb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2phbimeta.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2nffigtsd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xbxfzicf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wpjepulg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2elkqrhii.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2elwqzjti.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kpmktipe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2itidkqtg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ysamecrk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wrchqmaq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2seqgzmag.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2eswokyxw.html


<!-- 参考信息 -->