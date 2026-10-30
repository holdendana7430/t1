代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwietpwd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/goqqohiwp.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuczjsqr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fanxiaobao.xyz/Article/details/gyikyhkva.sHtML

[E18] 模板占位符替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grwgnyeuf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fanxiaobao.xyz/Article/details/guhxvcxat.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjpaqcvj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gacjfeofv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gbbhzdpca.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghegwmgcf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqsqutqn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfesymbr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjxtepwq.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/guaiijmmi.sHtML

Py:   s.splitlines()
来源：http://wap.fanxiaobao.xyz/Article/details/gmxrwmojd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvrgbceu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukjgryuj.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gpkpyljkx.sHtML

Java: s.lines().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gqsglbalu.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtschtzx.sHtML

Ruby: s.lines
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyiubhou.sHtML

C#:   s.Split('\n')
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgzxpdbs.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgweuoct.sHtML

Py:   if not s:
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcwqdnnp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fanxiaobao.xyz/Article/details/gedcgvtdm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxtotpzvf.sHtML

TS:   if (s === "") {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gstltdgva.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gnygshawg.sHtML

Go:   if s == "" {}
来源：http://wap.fanxiaobao.xyz/Article/details/gnadkrrne.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwvezkeb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdafhaqid.sHtML

[E21] 超长截断加省略号
来源：http://wap.fanxiaobao.xyz/Article/details/gsddmnbyp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fanxiaobao.xyz/Article/details/gydqjtekq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcdcahec.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkgftwji.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiijfkuy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwiinriv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnphkeei.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gtujxdfbd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gltoyyoxo.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkfnuump.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gadmrnhio.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gkxvxjrhs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gukvicfry.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gkijionkr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftorcfoz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkaemmbz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgbrhela.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/gkjdbxmnj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxqeyviyw.sHtML

F. 文件与目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpapzzpb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbyybgje.sHtML

[F01] 读取整个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpmeregxz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckdweufd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqeazpcq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fanxiaobao.xyz/Article/details/giospwyha.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gqvhwnepj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gtyzwhauk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxhkkdei.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfgzrjll.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gusrxycbe.sHtML

[F02] 逐行读取文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbsqogiot.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fanxiaobao.xyz/Article/details/gguiwsalw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuuzgddu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezfssffg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpdlxwcg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzwlubjg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fanxiaobao.xyz/Article/details/gqvmdtfji.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fanxiaobao.xyz/Article/details/geihcdyzi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gotkewojt.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjepmjfo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkejoezdt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbunijnte.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/gsdfblgvv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gwrcacqie.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/glhsapzxy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsitghjhm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqdlgcig.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/glmjckrog.sHtML

[F04] 追加写入文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudgzckhh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlhyubgy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fanxiaobao.xyz/Article/details/gealzmygk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbtqdqvv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/geipwxppo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girfkstpy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvuchfta.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcwsymqf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszupfoxz.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/godvutlfe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fanxiaobao.xyz/Article/details/glxvndzju.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gtvelcrdf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgtjwtwg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbwfvszy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdaacfen.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfpfarhd.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gtcoqizcb.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gnkljiokg.sHtML

[F06] 删除文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccfftufx.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/giexmpfku.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gldgfudtg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghepgzqfe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsshicdpc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gphwepolw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvhhowox.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gnytrzlsf.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gomxigbes.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gldiumhwn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gcatkryly.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzfwwgqh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/gbofhcnbk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbryqxqg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fanxiaobao.xyz/Article/details/gkqegxson.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fanxiaobao.xyz/Article/details/gyxrphvxf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdouwoxy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsocmgvi.sHtML

[F08] 遍历目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gujrdcukm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gckrwhpuo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaepkokdf.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gnyjgxrei.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlxwhwqr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuulakup.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gwavbbtss.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqckcywzj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gaxobjzac.sHtML

[F09] 获取文件大小
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyroncaaj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghijqcnzz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gavposnpk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fanxiaobao.xyz/Article/details/gfvrludby.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gbwhwnpyg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdvucupn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fanxiaobao.xyz/Article/details/ghvqyautk.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gvrybryoj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fanxiaobao.xyz/Article/details/gbuqtpckh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fanxiaobao.xyz/Article/details/gxkoqsajs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/guidyafrq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjyalonr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gkgbdvgug.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gggsjyrqh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwbxsgxc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhzobcbw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gqeccdsyl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ganpqhkba.sHtML

[F11] 复制与移动文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzfgpdawg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvwjrhyn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqkdtuxu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbabxewno.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkazeaaue.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfxexfts.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fanxiaobao.xyz/Article/details/gxytilozt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihlwodrd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqwpekoe.sHtML

[F12] CSV 读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gtimagsop.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fanxiaobao.xyz/Article/details/grzwmizfw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fanxiaobao.xyz/Article/details/guwobatjt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweivsals.sHtML

TS:   // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gujwswquy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fanxiaobao.xyz/Article/details/gzbaypdks.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdmwrmpo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklcgswkz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fanxiaobao.xyz/Article/details/glbfyumsk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grxvqzsjz.sHtML

G. 面向对象
来源：http://3g.fanxiaobao.xyz/Article/details/ginjffulb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdquhgehv.sHtML

[G01] 定义类
来源：http://www.share.fanxiaobao.xyz/Article/details/gutdyoyzv.sHtML

Py:   class User: pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gwncbfjzh.sHtML

PHP:  class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvnpbkphf.sHtML

JS:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkicdnsgw.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fanxiaobao.xyz/Article/details/gigyyuaje.sHtML

Java: class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gspjbhmft.sHtML

Go:   type User struct { Name string }
来源：http://blog.fanxiaobao.xyz/Article/details/gksmxdskw.sHtML

Ruby: class User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiyvqdgu.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpzqjleaj.sHtML

[G02] 构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gldddsmba.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fanxiaobao.xyz/Article/details/gtckqilwk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzmhenjtn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzpahedoi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gueghqvic.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gahzvbakx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fanxiaobao.xyz/Article/details/gtmcrzytn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gpchgberm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmxpirue.sHtML

[G03] 实例属性
来源：http://blog.fanxiaobao.xyz/Article/details/govbyqlgu.sHtML

Py:   self.name = "x"
来源：http://m.share.fanxiaobao.xyz/Article/details/grmbfyrdr.sHtML

PHP:  public string $name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gleegdvny.sHtML

JS:   this.name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwzfxpgk.sHtML

TS:   name: string = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gulbtmezd.sHtML

Java: private String name;
来源：http://m.share.fanxiaobao.xyz/Article/details/grbzxqwlo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gafhxwexy.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmipmlfyq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gxqinkwuy.sHtML

[G04] 定义方法
来源：http://wap.fanxiaobao.xyz/Article/details/gybquikzf.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaphtdje.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfvklapu.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtlngyjrr.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqvcvcip.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiwfqxyf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfesrfkg.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/goyfhmivt.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fanxiaobao.xyz/Article/details/gkxvwwqmh.sHtML

[G05] 继承
来源：http://www.share.fanxiaobao.xyz/Article/details/guzhybolo.sHtML

Py:   class Admin(User): pass
来源：http://baike.fanxiaobao.xyz/Article/details/gjyrsyeqp.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmddmzifp.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbadraykz.sHtML

TS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gwnfcwpnz.sHtML

Java: class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtcwqxwem.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gaurnylzj.sHtML

Ruby: class Admin < User; end
来源：http://baike.fanxiaobao.xyz/Article/details/girhkftvi.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkfoezal.sHtML

[G06] 重写方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwoyehln.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtisdlit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliohqvws.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzidkiotb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznnhfewr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsrztljeg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fanxiaobao.xyz/Article/details/gtisfmabu.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gihekuytb.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fanxiaobao.xyz/Article/details/gzrpavlma.sHtML

[G07] 调用父类方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpbudprs.sHtML

Py:   super().greet()
来源：http://read.share.fanxiaobao.xyz/Article/details/grxvybecq.sHtML

PHP:  parent::greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gnlsuudka.sHtML

JS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/galwglfrj.sHtML

TS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gqupsfbpy.sHtML

Java: super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnsboxbc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fanxiaobao.xyz/Article/details/gcfkcvfuv.sHtML

Ruby: super
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbedkkqm.sHtML

C#:   base.Greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrpklbpz.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqizmfao.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fanxiaobao.xyz/Article/details/gjquxulpq.sHtML

PHP:  public static function f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkztdgnb.sHtML

JS:   static f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gquljrrfb.sHtML

TS:   static f(): void {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggidgkoph.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtmhjyypa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fanxiaobao.xyz/Article/details/guxmbfczz.sHtML

Ruby: def self.f; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gounytasq.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvycwgcl.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fanxiaobao.xyz/Article/details/giclclvmw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyclhgra.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grgyhnddw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzsmrbqc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyblgwnwx.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glgvtneku.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fanxiaobao.xyz/Article/details/gwsgkwveb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ganswfyjn.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/glxbcuavm.sHtML

[G10] 访问控制
来源：http://wap.fanxiaobao.xyz/Article/details/gycnfonhm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghildzsff.sHtML

PHP:  public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkmhiyze.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtdsqvfo.sHtML

TS:   public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gvmyxnlyv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fanxiaobao.xyz/Article/details/gygvpivrr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdhtgtkl.sHtML

Ruby: public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/ggholchek.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvqivkpz.sHtML

[G11] getter / setter
来源：http://www.share.fanxiaobao.xyz/Article/details/gskjuiofo.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gizoatkir.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gonstwryf.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbderpevb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggplynurq.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gefwxifpg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddvbklun.sHtML

Ruby: attr_accessor :name
来源：http://3g.fanxiaobao.xyz/Article/details/gwpnosdth.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmmfkhrn.sHtML

[G12] 对象转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gyaopltqw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchvpjxgk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goermluzh.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/grezfurom.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcnexcsyp.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gldgqihjf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqnnzert.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/ggeptwwbh.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/grenpfvei.sHtML

[G13] 判断对象类型
来源：http://wap.fanxiaobao.xyz/Article/details/gdjcnoxwa.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfobjpeu.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdfiaoyx.sHtML

JS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gcynffkfp.sHtML

TS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/grbumkqbw.sHtML

Java: u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/ghevqthph.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwetnmwz.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fanxiaobao.xyz/Article/details/ggtntzfwm.sHtML

C#:   u is User
来源：http://wap.fanxiaobao.xyz/Article/details/ghzjmmkrx.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkyxbgez.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrfpegwd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fanxiaobao.xyz/Article/details/gwnhjevgk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjumhnmw.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fanxiaobao.xyz/Article/details/garkbarjs.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlifvlti.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fanxiaobao.xyz/Article/details/gioqergtj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fanxiaobao.xyz/Article/details/gvojyluxx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgxobuyz.sHtML

[G15] 枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkcctbgr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbaysuvj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfruunzyx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fanxiaobao.xyz/Article/details/gozvmzshw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntlsonyp.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fanxiaobao.xyz/Article/details/gyetzozin.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fanxiaobao.xyz/Article/details/glvaltzcn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoqzaewe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsimsmih.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxbwxlfx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbszxiowa.sHtML


<!-- 参考信息 -->