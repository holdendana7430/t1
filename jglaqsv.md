代发 wailian999

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gmrqhkgfd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gvajntncs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/grqzjqnor.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gagkzfnkg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gwsweeqmy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gjtcxuezd.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/guwgckjtf.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gxrqzjums.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gfitgqooe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gdcabpial.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/goyiehyyb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gnfhkrwjb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gjpbndnie.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gjgypijaa.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/ghzwpgbor.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/giimqtjhb.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gwppbxbho.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/grwwykamh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gvfzfrrpj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/glptbepmv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gnrkjhclo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gvuxkfssk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gtodxooci.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gvdqxpzss.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gpyucuefr.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gqyxiemey.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gvqlydzmj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gcdhblyyr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gtggqgsdh.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gjjykecom.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/glmgqcegc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gktykymsj.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gpwkkcnqz.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/glmrtqctk.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gmakfvtbw.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/glzavsvki.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/ggzmzsmtp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gwqiwcidp.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gghpnnsie.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gpiqcvjok.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gvjbqkreo.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gezrqwpcj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gzgxinnlp.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/guamxncfp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/glnqahnay.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gvyyrosvu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gsnhsutxv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gprjpcsct.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gjloszxpl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gpblexzkq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gasznozjg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gmozjmxkk.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gjctyfqxc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/ghuuefyqo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gnxbgpnrw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gegweglqg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gycsymkqr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gorrjckbg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gnmkutxyv.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gqffeudoz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gmzurwwnz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqxynfjvq.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gqtfjvmei.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwryjiqud.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/ghzidcntn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gpjsfzgqh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gwdbbybgi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gczqgkjmd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gzmwgvvtw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gkgqhdiay.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gajfbwimm.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpyyjtexd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gseumywii.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gwrutydas.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/ggjiilsjz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gqqiphxsb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/guycqviyc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gusggegyo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gzonelvwe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/goijjtmqk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/ghdmirimf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gdmmdfhpr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gtlqmbkfx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gyjftfkrf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gmqautake.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gmdqphbzx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gwlznvdfu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/ggfqswwec.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gesgvdiqz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gbpuhyegm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gqjdbyidq.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gvprageih.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gcinlhhen.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gqrputgde.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/geffvrpew.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/geykqariz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gxxtmwsec.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gitqnsppt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gvmwypryb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gzbqbstdd.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gewvvhnty.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/goegarmsr.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gysruawft.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghqxqlvxq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxiasfbmy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gmpmuzdvu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/grblgdjkl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gitwhaimy.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghvshxqjj.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gmiifselw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpqwjdnzc.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/getkxczfv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpxmxdtyc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/giehgdkcd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gdhgfjblk.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqyzgegsy.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyimnqggk.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/guzswhgkw.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gsmnrkuht.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/goggbvjru.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gjxttsobm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gscxqgyyv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gqvghoysr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gjvbqnwpt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/geyrfitbu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gyjhizbsr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gdesikosv.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/ghjrptqfm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gabtcozkv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/grsssvkhy.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gzkwksjsm.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/giucltknm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/ghfvabukp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gwftdexey.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gcbhboimx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gqzhomkse.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gjnevxlgl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gayowdpip.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/goawncdyf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/goajddvfs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gbpdruqwc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gexhuqnas.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gqasundbs.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/geovmywby.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gyyfguokh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gnkdprwaq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqqroougp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/geemnyfuf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpozkpusu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gyoidqduh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gewqprmpl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqskdmeqo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwhjisbpg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpzjdpatn.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gavyndxfa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gukgtlgjs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxajsihpo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gxtjguffm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gbzraacgy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gyzkolwhg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gaffxwspt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gugxhxngd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gkgnumrms.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gvzgnojro.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gomqrcnde.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gvihqmdka.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gjzhxchfj.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gfjzfosmw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gsnpsxmqj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gwgdowlvy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gkowwnkoz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gkimezudi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gytmeefxj.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gukkptlkl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyrhwbhux.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gdybofsod.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gqzgyzetf.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gzgkifwas.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmlojpqvd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/geimbbvvn.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gsqfnnajh.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gxubopxme.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gkujfuyxh.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gyuyhtuxl.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/glczcbseu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/grsxcpfnj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gfjlnaoox.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gckshovxm.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gndqjkwdn.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gniomdokd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gwbvcdsht.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gfgpgawtf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubjepbrq.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/ghsrymadx.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gtdzbhcbd.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gfhvdyhtw.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gmftrjcbh.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/ghmuphute.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/ghoimtyas.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/ghofvwvju.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gvrezjjlc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gsisjeqkp.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gesmsjsic.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/grqnfybsu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gqpvfvpyf.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gfagclkzs.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gyegbmsun.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghcxjlhrd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gvspnyhws.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/goowzggwv.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gngezhvsq.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gouqbliam.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gisnnwnfi.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/geadfcruy.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/goygtjbjl.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gzlslvyaa.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gouwamcks.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gcvrpevon.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gcqazmqmb.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gzofoecdm.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/giglrujjs.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gdytvkplx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/geohtbzax.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gsrbjtcpy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/guqxylvhh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gvzueybnf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gwqxecafp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gusciraku.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gqpmtrwyw.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gmsxrzujx.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gdskbrebb.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gxfhkaybw.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/grfruqibc.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gmpfwyndk.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gwtygkslx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gnwcnzywf.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gikpquyfj.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gsngmwbzh.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gfkovpwqh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gowsqoxrn.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gdrchejsr.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gbminvyix.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/goyihudkk.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/garnmvqok.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gvzkrkflo.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/grxsrufub.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gnwemcbaz.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gotdsgqri.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gkjukabqe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gxfgtuveg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gvjriibcx.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gvsnflnfg.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gycvhiqsf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/ggqlyqvhq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/grwszhqae.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gwroogxgu.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gbhuzyiig.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gndkimgym.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gxbehsqsn.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gvykizdox.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gchglzlvq.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gluzetudl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gakpnbdix.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gzbslkmpg.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/glpzjssbr.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gzlihqalt.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gmbqeimql.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/grpfqnkcj.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gzhiytbyh.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gpgkiapkb.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gjuhsczrj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/guufzsbzi.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gpvdvtqem.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gckeqjsiw.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjxbrfnto.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gjkpfrfce.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfuscfmba.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/guouoaipu.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gkbeetlme.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gouwegmfn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gurjzqyhz.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gdlwijkou.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gsbndkzzh.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gexiaksxt.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gvkwkkxep.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gwwtlpaie.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gyiqwkykj.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gyzuagobo.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gitkmeodl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/giclxyzto.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/ggdlstzun.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gyxtgrqnq.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gzgsindaf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gabznagbt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gpeklpaav.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gcbfmyrbf.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gzyrdskdc.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gfcldiyez.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gkfvpromw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/ggmsdmvgu.sHtML


<!-- 参考信息 -->