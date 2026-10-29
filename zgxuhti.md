代发 wailian999

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gsacuauua.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gguylwmxi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/ggzygrueh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gpxgnvqrh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gjqmtywhi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gsdnsufdj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gzpkkmjkj.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gedjmcdhs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gxineuuts.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gsueolcyi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmoicchr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gplpkftvc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gjpfxkivv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gkaontdde.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gwohkybmd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/ghxiqfvxc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gmmbhagkl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gufcujvqy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gqsrbhfze.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtpmakhm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gpaydpuns.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gzrpkjvoj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gdhfexahn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gdtjlcpqy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gootdoxhw.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gfszzmlrz.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gbrkhvrgs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gbkxfpwuy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/ggjytsdye.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gfsyuolcr.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gybvhxzuy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gltwfrfub.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gomdwsqcx.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gzaghklim.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gnmxpcafn.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gsgcskxas.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/ghqdidbxm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/ggiuiulnc.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/ghxfjofsf.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gcjrbscsv.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gskykspak.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/ggwejygli.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/golztnkgz.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/ggnwedsqg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gtggssjsr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gwgxmzgqc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/ggzdiqfxy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gcwicrlde.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gtgygdjyh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gydgsnozl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gvzymprfr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gzyncpxvh.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gdgekpdrm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gelwtjpvl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gvyqnxnvg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gkuallaab.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gadzdrykk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gkngsxdin.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gcishaasc.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gwhgbknkp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gmncgpcmc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gevuqlreh.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gpvrsdnvq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnaaybacy.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gzkvntbkt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gsgilhyoa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/grdgnjaep.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gidffblla.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/glrwalaae.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gvuudszhw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/ghkfhdrgj.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdomnwjbm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gpaickjvv.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gfpujhfaa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/ggthgkwks.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gntfbutrd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gsnwdoebg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gehedamzk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gctgmahuj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gexxetkxz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gykdxdopw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gmkspeoao.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gvfkhdzeh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/ghbaprgre.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gsadywvgu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gvputjxcl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gqejtqtzs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gudlogawa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gcvtybpni.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gctwcpwoy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gkcwvsspo.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gyeeiqqku.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gmabctvxn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gfskkgird.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmsxdaojr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gagbjlfxh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/grbanpikz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gfcpyvsev.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gykrcvfbj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gfzzioser.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gekotyolt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gemrbxcwa.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtmtfbycp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkanpyjwi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guauvxyfx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gimmxyapj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gfuystzbk.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvovcggud.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gksszpcng.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gkjyxoqei.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpntkiqrc.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gcarhcgoy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtrxhsype.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdiawuunx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gjsxsewsh.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwtkzgqli.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfsptzcbb.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbixprxys.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gsebszzyk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gnuiiuurq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gxsfsrsde.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gynsewqfz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gmecampas.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gldrxtfdf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gksybsatu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gygsjauqr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gdqausdnu.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gnwffkaid.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gfrsbtayn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/grprjjfcp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gkkbwtamh.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gzgdomhsj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gvtpuybsx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gfoszotqh.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/giqlgvzgc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gikfzrdxz.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gvokxvfrn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghrthnqpk.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gqlrodlha.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gukjwqtse.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gkjhsblja.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gkgdrvgbj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gtskxfonx.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcoxawshr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gjiypejvq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gcvqiavhu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glbaltkov.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gtcbxplss.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqhhwolkj.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmvltgbdc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gcvdjmriy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ghvpvrrkc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcwxsotpy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfyyqtltf.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gvuhgecge.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/grkldyblz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/glepxfsnb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvhyndvcq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gypsoibja.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gbqxolxso.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gerntanxb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gfzhmdcsq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/ghfgnkitp.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gbcuvcacu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiblxwhu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gtfrklwvw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/ghyevfgxj.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gfzrtsgib.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gzkrecgbu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/ggsdqvsju.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gnxyjrxed.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/geftcivdh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjniyuutg.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gflsbjynv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnpidrdoq.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gcgyfilxk.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gfjrtwuua.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/grjoynpay.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gsjlmyqpo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gwnxkowwy.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gvpjikomf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/ghsyzywlo.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gxasfhpnm.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gkwhuxrar.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gfogemhfo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gveuftuae.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gdugsiory.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gqgxwrzlv.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gpvgvpdwb.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gtirtfqhf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gwirfvcjh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gwlejlphe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gbtimenbo.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gklpfdotf.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gqnnstqbh.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/ggoqmqkyt.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gbertrryh.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gbriadfhn.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/glrnflcov.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gsasfntdq.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/getznuxgr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gyepwguwa.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gxlqcmrpa.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gberreuny.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gughkcuaz.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/glftseqav.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ggxmxpwkb.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gvqrjpgnt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gtdwbijuw.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gpmldqwix.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gtazlttpx.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/ggftzeckh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gwibfdzol.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gudvldgec.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gwviopfpe.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtsxxjxop.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gdtrugpbd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gchpgusjz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gktjqppev.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gsakswevt.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gmptrfzdj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gtmwinisy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gyxojdtnv.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gotdebaia.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gdwzpscai.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/guzssgzoj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/godmyxllx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gslpgjljg.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/giogofudt.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gjbcmmlcp.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gczlwlxqu.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/grdxgxpcp.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/garnixpna.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gqizbwuvb.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gayxjeqft.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gmvojacmt.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gckvxawrx.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gacbjuwmi.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gqmgbigol.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gdrnyqexh.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/goxycrpzs.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gixlvhwzf.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gtohxwtyc.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/ghxkommxw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gxhcdhqec.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/glaqxwtaq.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gkvxsuniv.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gvtbsmzjj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gwxnvrbpr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gckgmexqx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gqpkawzfq.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gnvghdnpz.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gcpauzjes.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gdggekuem.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gdkhazvha.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gbgmufcec.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gdtopmrif.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/ghryiwvgm.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/guewlgyun.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gfdolllcu.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gspuckezo.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gkmkdspqm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gnzhperki.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ghlejgppb.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gultoadvi.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gsslvkisj.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gsdkiymuy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gfuzdepwa.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gssmhcfeq.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/guqhbqzyo.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gosusfjyj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gxpmnumgn.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gkrmydtlm.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gnkzewmrc.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gndpbukbf.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gawxpzmqf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gpxtyqkwm.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gpihnvrgv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gqwbizyou.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/giksyoutv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/guqpchneu.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/ghjlunprk.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gercgnslx.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gjbttqfhz.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gbyjrvoqj.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ghqfqqknd.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ggzlscsre.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gqkesacpe.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gcqxpwoqj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gtvasnmfv.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/guepphqob.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gmymazsyh.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gvmrmmguf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gscayhnbn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gyfdapsbx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gckmhhqnr.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gxsaweaqu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/grlhjvcnh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gqoifcayc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gauancvsb.sHtML


<!-- 参考信息 -->