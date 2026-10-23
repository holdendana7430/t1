代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ejuwyecm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jqwtewac.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3dtulmype.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3yfulhvou.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3stlfmtqg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3goqpwebu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mjqujeos.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqqxrfxm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ijbmhwcz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fkkxkemh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3esanbcat.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3avashrnk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3dlfqsqnx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xmdgceng.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3bdmzxzfs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ejemcnfy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3odhubivh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zuygllmb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3igucedsb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zkcpewcp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fdzkekgd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bxfwmyab.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ktfblyad.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3uvtuwmtx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jjrupbac.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gytstecw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3evouwqxo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xvacbyea.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wgbqqtds.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ewmbkjqh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kqjqufte.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3btwirjyv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wppmjxnp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3twjssxqx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3igrenxnj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eebmhnxx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ybqssiwj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kttfldko.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gpkkbwsl.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qeouccra.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vvsiswcz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kyqokjaf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3yzjcoznk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3wkdelpqz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3vtmedmpc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3cxbiarxn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3plglrfhp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nylfkzvl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3phtuqmlj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wfyfqrna.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zskiziqw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3zgvgqqkf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mdromfjk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3scgplynb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jmbdxafg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vrvqjyfj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lgqjgnln.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mehajshx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3stafpmkf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fxuddvsh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3pbgergjx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3aatrqobb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cxulkogp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3omurfddk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3idhjptmf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3khxqzfni.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zolrigwz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jbipnhpn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ppxuuowd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kktfonfi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ajbfqodq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xaoreodx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nuiylmni.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vsgammdl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ioxyjlxy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ebcvksok.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lnwsaeso.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3racdveaf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3fmwyjshu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lreaupsh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gdxuycmh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ryzjbbcd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3tgdsgewt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpxykcyt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgtanpnm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrvzdfzb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rnhzubrw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3cpbyzdom.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3uekywdtm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikuksfvq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wbpyccqy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3llqeljnc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zoagrepl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rwgsoeip.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cvvjgsct.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3mlkxmfou.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3cgiaofey.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pihixwkr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wnunbtof.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3dkfoielo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rpzrylft.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pmbkjivb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jerbozox.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nkkpoohv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dqcenjrz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wjtxlpkf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vhzvapsk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qnhgawgf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ibvqsxju.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kvpogect.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mwwpnnmg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocuofcft.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hsgvxgzx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qtgflmpf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ecokbhxz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wnnnoqwr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yetifcqs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxwkkmhr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3peaykcac.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zyholiot.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krayuqlv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jbkejasn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bbrbvsqd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3soknmtew.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3areihtrb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dnzftvim.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3hdvldeav.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sbquimkt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3smsyvejm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fedhbuyl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qliqzoxv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3yycyfqxv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jhareqza.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fxafywod.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mappjkds.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3poouhiov.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ccjhddee.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3etcwjurl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bqcpquka.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fbtuaaqf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3svhzdfsh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yuuoowvo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3opaxgfci.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ewhetvhh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3jsouzyon.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qahpuhzu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yvixbwtk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mjiyntcl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sqqvstak.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3smcqcixo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gshwekrp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zndkmrtp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3kinyhyrk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3fmrgkifd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytkujpao.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fqeqxdkn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrvgovpn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mmojncqn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zkaccxzb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aaoqejlm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxsgomfb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oujxfarm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yhkrwgaj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awzqyybb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qbtfxoak.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jncrsojv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jbuynyje.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ajgqrjwp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3eptyxrkf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yeijphtg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qcsjmhxa.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ctylacee.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xnsxmbpo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3orbrvmdh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3hzmwadbk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hkslzbgm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3wjikozbg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3mceiuwat.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3uyxjyrgw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3caeudxfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pahjcoyc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3jqvjafoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnzrzirk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xiagefvy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3npkredjs.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mwrsjjvj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqgofsvu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ipbtkuep.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzaslymb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xnbjwrbf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3kaijccej.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vglwisxe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ocnthatd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kvlukghn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3sdsxqdjb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iirxapub.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3elrjligi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3raomxaxp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lonqodya.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3epzospix.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaijhvix.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jjqvztxr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zxtjzotj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hxnnxftd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gnqgrgbs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fpfdlblp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3jgwduhxm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3kppakiti.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hkrpluzv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ztdotowd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xhxisfmd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3iemurcel.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3owomkdje.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3acpbwgxl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3idkaoldk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jcqjhrcj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qupnlinh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sjttstgt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wbhmuzkp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3bpgwhxfz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3eczugnpf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3epfdzecr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mdqihfyw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qspboqfi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgpryeew.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jvjrjixh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cscclymo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3daqlxtmf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wgzqskaj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gtrtwwjt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3avmzoxwf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzylnzqw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wjgdmkuo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ldzgbzgw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fdwogfcm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mlfrdsgg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mndcscru.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ovfejdfz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hgvpfyba.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tlicggsb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qmfruqvj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hycnoibw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cztwcayt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3sekzkcsq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lnzpjjdy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vvqthaiz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3anlfnjjp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3iorpthmz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3eggapcef.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wskouoqy.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybuatnsr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gzjupnbs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zprcozmg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ajcutnnf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsrntxez.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3rilocqne.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vmhmqqmz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ijawwqmj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ngxedaca.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3sbawpkgv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ymeckrtw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3igqmfcmf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xcsstiwr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecfxrydz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3tortyljz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3wyktcwih.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3epcwvqth.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3bpxtkmef.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ffsljgzh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3buqtkvqv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oqibwzqs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kphrnuly.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3yvimdcpg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ntqlgfkq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3azofgwqq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ixnwympp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edopwbeg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qrdraogq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggiupnwm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pgmjlfpt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lwmvcwyd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3yaalrkna.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cqxfgjwd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ijhqfizs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hyezmqnc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ybsnbajd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqfvxrpi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3evojgtfz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dpxrdxyh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zdojzhje.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uaieaucm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nacqxtrt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3dawqwtfl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cogrfkqh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mdoszvbg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dzavmuel.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3njqhocpp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3kypgegpo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ckskpkyp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3pugqnnht.html


<!-- 参考信息 -->