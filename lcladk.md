代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2tjdjgybj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ppeazcsh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2uimtrrml.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2deupgggr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2epmnqlat.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pyvpqclz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2muwciegd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mikvffzu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2nrojctvc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xibcxnje.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2elxmpasj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2igctzzmq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ttqqjljx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fuigiwku.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ghdorwwv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vinpftfc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pfcpjutc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2cdrtazzd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2heiezetj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wnjrlncj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qlbatfeu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2olxeiagg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gfvriloy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2fgipsezb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2seinuvxy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2aemeymgc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2gfxfeknu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ltkbqpdx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bvbjbium.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2frqchmes.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eslapert.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nlxhugzl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fehaxlbj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vmhwcgjb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2okmexqoi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vgpsamma.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2oheegubl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2efvoecrp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lklkypkk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2degiecym.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2pxhaszdc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qrvazgul.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zyyckbvu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2afvzbcll.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qnmdkyuj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ddcwlubt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2grdiwqvs.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uftxzrfe.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgjqocoh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ayakmqyi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2smkjxwey.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nqcwnpkm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2mwbgdsob.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kbopgxru.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vfvsnvdt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kgiknbrw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rqofmrho.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2hytjommn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oqqmczhx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bvsbzdtz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ishivilg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gkphwtuo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xdzxekxe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lghktelr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cmumhila.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hsepkqxb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dylubrdy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wazafemf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2foclnpyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stbxoixr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2esmgrdqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebyabkbo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qcevsija.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vhokqjcl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vyyosykt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2tanvqknt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pedfkfua.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sfsebeyh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2dfmxiknx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmbojdzl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2blrdduzb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wjkkwhcn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ztpbiuju.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2uuuvvxgi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqrferxa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2phquuynt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2oiomxfxw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2twectdeb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ysdogwpl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2srzffydd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wmnyajps.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ynonnlhb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2redtxsci.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ionsvbem.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bpoksdgh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2obssmhub.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qfwdoaaq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ljafpwcp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2varsbfaq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2stgllihh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gyuytgxa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xragunxu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ztxkixys.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rqgkijea.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qhppqgvi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zzgvgfoc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2skhtvwsy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2clwbwfej.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2txetedmk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kyxrpxml.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rqpsmybs.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wnhemvcd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hxydxoug.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xtlecoxa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fxqueyet.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cztqmfcy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipxzmclp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2pgzhxnfc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mfkdalgq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2afzqtktb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgtcmruq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yraxmprz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2umkampmi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwinvyzh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qagwwopb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fwypgdnx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ikmnqtuy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2srxymkrc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hljequrj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2imqchmga.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qkqdhtkp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fafxogil.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2kwugqwma.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rjtgmwpu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2mcyuoigu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2yrkxrvfe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2nyvuvjfm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqlogubp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wkmsylux.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bfsxnydw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2famhwbya.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bsjojjkq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2nwhvadxe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2orzjvwns.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2tifwdcsm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmqhsirr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ooxstigf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rltbtlei.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wjabreey.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2khyjlvlv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2sucdigqf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vuqztcfu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2bckbjoyy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2atqzrtvh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2utzrturw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mmfijixc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mvsagpwj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tejekbsy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2hiclrsvo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcbeafma.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jbdxayba.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkdhigoi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmbvplnv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2abvxfrhh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2guynsnip.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2eftqpqoo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pocpyqsr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gkadeqcb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2uuifbwdq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfbdpikt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jrzvrgjp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pmogkbdm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2odzgpinn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dylntbbe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tkmckbfq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vdnttfhd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2igqioprr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2oglixcgi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jrtkebla.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2weqfiwcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjsukwkk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qffspwiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppbktqah.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wqiamjas.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vtazlvck.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmwvvglt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xsvcmqyx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gmpvbbsd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2nqchoxjp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gigingav.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vfnbgjvo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqcximih.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ysyuvbsr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ssdmkkzf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2clhigoyf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vamlcxhd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyonligp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kukwhubs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2anivirnk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nbyhzryi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmoqtnkf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2yuzemkgg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bfdfoxdn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bxydztzq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2csvlescz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qdkhtpft.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2zjdyedsn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2bcjaajcl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2usabfner.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hyqksxuw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zibpwrgj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qmwxdvyp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iancxskx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2phswywqy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzpahnua.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxsrconr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fyrwcpau.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aeenvhme.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vebdxlqu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2zhpzglwm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mfifznol.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hehdsixh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmzybbyn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qzdqvsbz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vbvizvgh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2skopiyeh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mpnvbhad.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxpahlbc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2exfopctv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ijfeumlf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnaapdsn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2foekkica.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvwhnnib.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkwlfszn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jrrlpbfa.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2unhbylzi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ypvutglb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2sstkgqil.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jvuonzpr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fucejlyw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kqtftdbj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eqidwytx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ueiprzlb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pnmkhzum.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2yzvxggsd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ocpqfwpd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2lqchijlb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2kspwsgeo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vxtzkmzr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2itlljyyr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ganyqxru.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztfdnnmw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2lajrlqhl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ikordgdy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2arvockpn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xsgkacki.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ziudzqkf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2bhmixxys.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2pyalojot.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2drshdmpj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2pplprwia.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xejgpamk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qofimocu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2goicgnbh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2cljxkatn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vagvkogj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gyikdnva.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dfaoohkq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bambfrxn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2rldsvnpq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2mokwjnwh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2umewehgr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wapgjnqz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2fngcfxwa.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2fywcdkjj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rsgmtmem.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qutducpm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hofeslyv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsgqzutb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wmxpbeaj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2dlwsexka.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjzaebvm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ycraoqrf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rtxoedzl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dcubeons.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jexeixvg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkjbghsx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2weufvnsm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kzksasmv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bsabwqsf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yoctvohr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nrtlflgd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2minfmmnl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qcjfjtmy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yekfgeyp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ypixhigz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wugnpoly.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lgdvnoyi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2bnfugvaq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mwxasmho.html


<!-- 参考信息 -->