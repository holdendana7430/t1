代发 wailian999

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zzqiofvj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wecmirpk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ovknoruh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xyjbfnyh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3mbcxxdid.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ybxgysdk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3oxkyzigw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3kynxmraq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hhfhtqau.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bgzrmmvj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xfiqmpew.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3actfttju.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3makhgnka.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tegsqtfj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3eluklpog.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3brzpgozw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ntkvrmdz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bffhibvw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3coowdxyq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xnwbibga.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fnycyzop.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3opisrifq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zxiqjqit.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bqfuvpzd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3vzrgbomy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3thdhhanr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3oicxjkyc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tvhrpfoa.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gtzbyvnc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tleqzupy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fuenoofb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ddvlvywe.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3psibxrfn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3vxzzarae.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xwqagabq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3epvretqs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zryuvqdo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3klponnuq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fchhwjjf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avzfcxny.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3karwlqng.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cfkawxcz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qcpnstyj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3oowfpsoi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3iwuxdihi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wptmvaae.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yrdkknbb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ptusnwcr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rckilwta.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xbwphqvm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ktgqoyli.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jrffgvlp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zjmxeyag.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nufwgyje.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fgmllbhw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lufahfva.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oxryytdu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cpjbghle.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gdeouehf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xocutcxz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3izzuuffo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyfxhtxw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3rurksgxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbmmlgnh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tklxeoeo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3rarfoelk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fwooftbb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dxmlubvf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uyvwkgsz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zsrictwi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wevypbwi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnympzwy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oxaxsflh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nvtlzkiq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3gwfympsn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rhhedqtm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rxqdaimg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dhfkfuhd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ehobvxxl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ikcraaio.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3kmuomule.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlfcgbkv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ixhatxzb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3pphxtsgv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3clsullcn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ezbjokml.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fjeumvsv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vfgnezhc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3wcvgwxzf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wplcgjtq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3byysswad.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3txglgart.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3falnwunx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fuhflmbg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hhbnpjfq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3udttyxrz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3tbzdvecf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nqhyljxh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3duleixvq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3eqqtitow.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3cnkldogf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3viojydjx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3djorfzkv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3olunwmzc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsumizzv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qnyriwld.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wzenxfqk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jjxcsrfw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3idspvypb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymvjcvcz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcojfcuh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mcvjqcwf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3giiovjwn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zqveoyho.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jxquuwkc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3irsrxhmi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhemvmnc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zloztyaw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3eikfsiew.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hzldblxt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gcmvqwny.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nklkpyng.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jezqzneb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3xgpepqle.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3mapdgmvq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3pedjvfpa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3rglwjfye.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3evcymhed.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3odqiohgj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzowdtzt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ibipzbjr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zjxkpasz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3axrpdhru.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qldbnkif.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vuaxkspy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kmtbbmnd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3gguomcan.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwfrwibu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iwewbguy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3uxdbtziy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ghcjhttt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fsnumlyw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rrxlfpbf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uagrtjso.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hdstpuww.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mbrqwjrw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbxwsllq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3grsvwmpb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bklcuifs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xpenzaut.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lkjrsshf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdnwhpsk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evclmord.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvgbpawm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fyefmxrf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3embiccxh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3radoiqqa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wloqqlzc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3efzffsbi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uhagranf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3azaiprin.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbtofeev.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pfakbrox.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3nvypnbkb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3dnvpymyi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3bosnsmtw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lcqpzghx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3scwwgkdj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3fgsnypfx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3llsjyrlk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3jirwycuo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kmsdchsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbhaklvr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3mssejeob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3inwygnpl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3aehvwbpj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qhgkcngl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3plkcxodl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kocgzjtm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3uynnyldt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ryuoeytc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fwuyqfrg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gqanyxva.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3olxizzqc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nhnqqtar.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tzmzsfyt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3fisllege.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvqfzkxn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3bnleeggw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mrzzvroe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3fndbdeci.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kpcqdrsj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bvgrcjhc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3tcuduhte.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wvktwuif.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3twfrlszn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vfywguxi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nvimrawj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3kabziydr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3yqpardix.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rxlmtujb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3lgwomgmb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3azrnylzm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3arpbahhk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rtsigslw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3calfrevf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nibodmxn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pfvhmauq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ejoelbqv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ahuzmpgc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dwcmhjop.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ibdypanw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xhyfemue.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zsmpgcsn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cenuyuss.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3upkpkyxx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yilqhmwe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rhvjumri.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pxeqfkho.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aodkibgw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jhlypmed.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3osmwbeid.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpcxeffs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3spllkbgv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pbahwpob.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3phirgqxw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3elpyxmix.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qvbyayrd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3evzevsdg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3hhmfnawb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nbglbvzf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3wnjmklun.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rlaeaqnt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3shfsqwdu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3plntikqc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3txvyckrn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xcwllrbm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3msfljltv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nvstwpwa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3lielparv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qwjlffza.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqgvjxwc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3oyhimhok.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3izmvfjbt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3oglhujlo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qdgrgqsr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3azktweut.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ktbtysgd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ryckrudi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3avllyqju.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wytxsxpt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hvwtoyqj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qxjtiism.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wxmoeyxc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3leygizim.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gevjwgyg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dlpcobao.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3epqybgsl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fuvxipjg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bmwishoa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iarxmohq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3rrfzutuc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3bpopqjxz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kskuepez.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mbjknwxx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hanoappb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jgomatkl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfqjqvis.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwaytmpb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3prrjebwc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eduoxdoz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pndtvdox.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3alivynqp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dtpwrqal.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bapbqgdi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zbergwjq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3usawadag.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wwhpoglz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkutzftk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yudjxryd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ahucnpkq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bwzhwmqu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3krvscdru.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3dsfznroa.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3skfuelii.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fbghdxnx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3htzvmbug.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fhxhgmdl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tisweihc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zgwhepbk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qangewdl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yktdfhqb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vkvajlrs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qdcumtcj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3gmoitzuh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wproryjj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3nyxhyphq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yybkcfhn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3occfhtfk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jnjysoyz.html


<!-- 参考信息 -->