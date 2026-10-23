代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kcelfkkk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iadawhar.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ixzqmmlz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rrofmkui.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kyljfpki.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iaonsiof.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wsxtpmuq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bdpoyvkw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3rzsfjwtq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rzwbtfrf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3xtmurygx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3fphsqeab.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yhyjnnqu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3grrggmoe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3habgqcvk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xxwigekb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hhjssjqe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hwzqbveh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3epnbkmrl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3sgofcuja.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vhkaojan.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vhddpwkn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nonrodcu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3obogujmf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cflngrhg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ppjsyruo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dltngteg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jkcejpjj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xioqrqep.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rhvfjjos.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3wwdzdtus.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fnklqoks.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mxnecgsw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fxkujrgj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3uouhcebk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3whbaanhj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yozztcji.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3foqwtsvc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3asjlwcvw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3erxwlfly.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qxuhjwns.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tsqgmsnt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hoecxvzv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qzvvmbne.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lukhkqkl.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lqtgvvtk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3orejhrks.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3cikroliq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3uldlhuic.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3enawjdek.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wfwhdwtk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pmeshjsv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xhbpsvjf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ddnjzinn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ygiesxkc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qofxqhlh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rrrywecm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3losxxcsu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bkfztgye.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3doyujahm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mzumlcvj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lpjgkfay.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3odhbhzzs.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ygdaluqi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ukwpuwko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ksohotfn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vhhlgqjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxfbzqbd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3horrtpqn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kbnlpocq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bqnitldy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3aejwnmnt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cvxqhnor.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lfyagyqm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vkxeamts.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sngpkegm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hhmibaag.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3lbemynvx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3czfwzvob.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3djlgwxll.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zovsplnb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cxkvybiz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ojzsjdea.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3euatfehb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xbksgwnp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxonmfzp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bpzzpyod.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3okkexhkm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lnhknlvx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qyewezmu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ddoodgum.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3tckbbnjf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3samisuom.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vxnjefyw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bwkdwndp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jyvdiysp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ztdtychk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rmnuownq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3maqokqms.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qcoixxph.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dsmfaodw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cdklgstc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3htzsciic.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dnqcseya.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mcrjewjj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jnhgiios.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gdtzbgme.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cizdufyu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mfkbkfsx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3arktghpr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3cveukonx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekbfisxn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svxebtcl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3eznhuftj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mkvbsere.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uriifbtv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uapelzje.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yffkicqi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3flgffhal.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iorteswp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smdnjawj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hwjzzccx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3mpnnynzi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lzcqtlwg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dbikzouz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3powkqhlv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fmzlxlze.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mmzwqaij.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3zphlsjbf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3cgkkpkjo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xsuvbiqm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qyvktucs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3louyhuyu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngnhcnoe.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tbmvzqdq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3snworzgy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3plnjbmrd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3toiwyjmx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3exdexyug.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xtnqydeo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3alzkfisf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfejwxrp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uxpxgcai.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ysjifkkh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gqyjxcey.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qrcwbopv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3qtdrhelw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xtcxqatz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3vrdbuvgc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3fercrasj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tcgxloeu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3guiehpli.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3brzbasrd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vczjpdyz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xmjfzzgk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3soqwlkjx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnmerxxf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bbljaxsy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cqdregxf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3znwsikxi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zlmkydnb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehbltppz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lozitzst.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hbdxhomu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3khswtjfc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hxolxswc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mtlevafo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zkjrdfxe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3mlryxyvg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3aktwwqzb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3biufltkh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gcxybuhm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3skjkdcly.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mecljhzg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rzhbugsu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3gkkbejoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unlfgyar.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3brxyjvoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgtixgft.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3bdsbsycl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ywahrccs.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3citylkdt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nocikggu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrlbfptg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3iyyhbyhv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3cijaoghb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ipjeysoh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dexzpsak.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3idrkgxwm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3zxwnxbqm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zltivhdb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkzdiyce.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkdodlde.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zczazsjc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3uszesfjb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3czsniyst.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpxlqziv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qiwsenzf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xnlrnhjo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3clvgilyh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3scgtslia.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xczvjqqe.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gggdynvt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bxlekqtv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fhyqgctt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nejxwxjs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hoyzxhki.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tsldedil.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoqhtykn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziwzssji.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rntyvyec.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgvvckak.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yetjcotz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jjbepbjx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wugcegsd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3declsjmm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xasrloeb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wntbsymq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbnvsuat.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3saujfvno.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hcuwqqnk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3zosxfqzz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lpciqtbo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3fzyczdhs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zrpbfbmf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3saikashz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvrpdjgm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvickxsq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjwsekor.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3plamiztc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3cfxywtun.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zopjrpix.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3hqqdxxsc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3emgiscsv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3jjeblzvv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hyfnhiph.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cdfmbgvd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jsxdnmak.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dbbjcawb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zymohylo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gxojniue.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yktbbecl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3yndyvenl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3cqbtaqiu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ifiopkjs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3solzxkud.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcnwvrih.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uawrfhpy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jvephuou.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3lishcfzo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3pbiicbtq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3faxluudl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wkspnbne.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3imynjada.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dctjjzui.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dunvsfra.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yipxvkri.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3vaibkydp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3dcciwlno.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmnvejvq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3aqvekinn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3jsirosrf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ebdmsgoy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3chijaxeb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hnbtlcwt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3gtsickhm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wrzjaqni.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3keijfmxe.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hmqxxcju.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3zrftybkh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3oreazfhc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryxmitck.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucknscja.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3muvicqkk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbywfzzs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3krlkuwmn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jtuwkgjd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3hunuloqi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3odptnhry.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nproxhmi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sejmiayo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmudvjqu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftloihew.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaxynfbk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3znjcuxgj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3osicfpna.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3doztpvpn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3zavjtyfh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zosjdwqn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3etegsvme.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oublrnwi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wxwnasvp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jibnmpkr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qaaeyudw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wfiznbcj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ilolorjj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3lgrvgblz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3yorireff.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hklapjea.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3caffvbtc.html


<!-- 参考信息 -->