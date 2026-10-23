代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahoylcwx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lysvewdg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3kfehxihf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3kfgzwqen.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fuybmcqc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3imaowosx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nuhkendv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qrixwwjt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jvnolmat.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mifudjxb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rtbguqlw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dyzeruja.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cxteoygg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xcejrcsn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ysgvdrly.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jrvlmzcy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3flemzldz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3faogivjk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugfoutyg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sqjpoukw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqbannmj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zyvlplpe.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lemgcxme.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rxcoiqjz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3osjceivf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3dhxckkcq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ubivuaak.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ztnhuaau.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hufvlkln.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sicasmyt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ocubzxwa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3anvtasom.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fqnaxvrw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3pmjzbnjc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ncejhuho.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fwditnag.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3elwsrvuq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3coxeutza.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tcpteamd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wgxhrtop.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3uyqzbwak.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3sgjhhweg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ijgmqeoh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3athabhas.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ycbmximo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xefjlsfo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3djshkfqs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gmqrqcso.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgqvjrwd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3wqycooqd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3igzzyezf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3cjdgejjq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ufecxyrm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vbgdthtu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ewxwsahg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ppxplznw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fpujhfmy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3zberkqbs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xgmvooop.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wxwhhnuc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bwtcqgfl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3iccgvunr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lhovefge.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ceijmsgq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wtphzzcl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3eswfphjb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ndrccock.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xhgglulm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zurarjql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpjoueiu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ductrneh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isbaxiye.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gjoiqqxz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ikrsmnnc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3exctspyh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3cczxqcop.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ekawobaw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qcfkfnzd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lqqttxfh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jyejjkxs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bnqqxoad.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3aopjzyrb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dhvkfyjp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jkmpegvj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ksavksmm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wserfqvf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jxepfbqt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3avkqbhka.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vyhhdzxu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3djvswpzj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xdvhvkck.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3kbfxobzb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kdtgqhml.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3leybzqhy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sheplqzx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3kebwfbfm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ejukjykw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mwbplqcl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gbtjcajc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdxtyrjz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3grfazavw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zqrqtnxs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cifbydyt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ryctzpca.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gqlhsxre.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kankxebs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dnjmmhqy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ktutcyzt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gityzewu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3olwuhicl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gbuftaex.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fixyvkmf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtlatutc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uhfzsphw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3zflqhclh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wznqtcgt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wcuweber.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rcrsifex.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgdrbmfq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fatwutzh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zlixkivt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqeyqwss.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eqaqmgci.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ypzgnmii.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mrgcvgsl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sirowszg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3sxgpcpwa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3emdxzpie.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3mbcabiqq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kcgucxzo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3skmockpq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wlyhayqr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qqmedpks.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3lsruikww.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3syypldrn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3fyiwxqcy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wdsneouo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3gicdywhc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zrmiyzsq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lyqscdkp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gvfkrrvb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3nfuubkgy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3axsgrhrd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oueyoahy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tyatfpgm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ygpstxgx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3trrjaohe.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pllzzoyg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yprknkyy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rovfeskw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3nnhzlfmv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vpaayhme.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3pidlkwki.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3peiyxcpb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3trmrsapm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vqqwrssw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqixonvf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbjgkesy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3oztxqwco.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtktscpw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gizxadjw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ghnflokg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wkoelvqu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gomnecje.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jcknumvn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ipexpome.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zllgdsnj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yuhrwlwx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3nwkofxcg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uqxaxfhd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zipssrlv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mhxtlzrg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3htaiaftp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3eswkpeur.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3gchoyfuc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kdnbbkkg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nwzhpnan.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wqbnkeyx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3sbheznhb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3azwivefg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xofttmku.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3neqlbqqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtzxzfki.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3idxypiqv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ybxpmdfe.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ygkzhphs.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysktiojf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tdqgvfnv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ljmtskah.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3luzlhycb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3opmestsw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lkifxwhj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ltcdkhar.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qqzzrtxi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogdfmcpm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdmdsonz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3erlymzdx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3amxgzuyk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3toezsrkk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yequigws.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsutxglv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3woksivis.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sltehrdf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ujcnyeuk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rtdjqsuu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ctbkzkxm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vqnqwihq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hhrtfczd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3czmumsil.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zithfckj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xuxxpibz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xumpecvh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ttxkixyu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rjgfwhpd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxgklfie.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pzxwldws.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3serujkgr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3neqjwcti.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uefnwzvk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3mmlotapb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ibbzynjy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xiunpojb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uvxonaax.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sycfdcbp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xqqugqdl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3hrempzpn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wttbhske.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jjraszkh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3aqkfjuwh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jdssrqwn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwfiavoc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fpkmoqkd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwhmspcs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymhwieqx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jhmxslht.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3otcznvow.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xorppjmw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xmcqbhuy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zfvywbrs.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ikigpsmy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dwkilqgl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eyduemxz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rpnzfoqx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3lfopgbyd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fiqhuwuv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3uctxlygj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3midxzcbo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rvhckmte.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kprihefr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vomlexih.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijlroczh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgwfcoqe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ellytfap.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xamgdgrq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkimffma.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ahukvtxj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ubntnsxi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmnasmeo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ggfhslku.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqhabgxp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ephxipkx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zuyeicic.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3lwufkuve.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvlovxvv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3frdzszbc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3sxvueqjb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mwoblhpd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gxbxpmbw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ermmnmqs.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3iksbmsio.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3prypocxa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3khviocag.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3agpgnyvx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3sbqvpacz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ivrlgeco.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3duxmigwc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3swlqzdof.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ywdhbycx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zfnknfyz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hxwdyiii.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jbmkdsjc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygjlgswa.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ifohnkzn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jbcrnhnc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hoaojjcy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfivucrm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilhjpqaq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvttffzw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vqwvihcf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3aaqnehml.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3yltiyajf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3uqsinqym.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rcgkogsm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xgglfasm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pjnvmcmg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lldpcaxt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yjaaqupj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vsqwnbaj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3iquodqac.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3pmrqfeke.html


<!-- 参考信息 -->