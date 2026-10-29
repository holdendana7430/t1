代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gbthvbbyh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gsogbnvla.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gksuaxnpl.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gitcqzcke.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/glgistblg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gihsixcfe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gilvdcznr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gwsgcnlgi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gispodojw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gernyqfsa.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/grzaqrkpq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gjdewfict.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gjbbdncso.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gekehcsuv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gdkcnydqs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gumvrbvvf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/ghcsulmgw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/guxhewvet.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/glqxdxcxx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gkjpmvhqd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gqwdsjoab.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gyaykxhbv.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/ghymeziid.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/guqshkgwf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/grlogsbiv.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/goxzwhrnz.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/grodwavgc.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gfnncfjpk.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gkzczlylt.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gcxnooxti.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gkpcdjtye.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gkeilehkz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gmqycbuxo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gosqnwxky.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/ghfxerppa.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvdzndjft.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gkxgmbzda.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gnccmkzye.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gxztmosku.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gxagbjxuk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gygxlthot.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gsuuulbua.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gckepvcri.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gfmqvtels.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gxdvmiqcb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gmjxnwjec.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gvwxsvaza.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gbfjxrutg.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gbyxxclaw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/goflgmlml.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/grimgqmav.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gozgjesjy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gocozustb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gvfshzjla.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gagwybrss.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gseajjxid.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gomgrheqk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvurtifak.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gsowkslgx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyrgmpfnz.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/giebanonl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gjhmmuwxw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjleibtyi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/giwstsasv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gkmjdsnzy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gsndiesuz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gfkvzqvep.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gktwrdsov.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gscvojzou.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/glelrjwvr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gihlxadzc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gtcvcftbs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gqggwdidr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gcglktrmz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gxxpdyvnz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gvpfbzbcp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/ggegqxddy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gqxwzwyfz.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gudbpeuxu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gcwwfalre.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gbqkfvjdz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gbelvmngn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gmzlbergt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gauyirtcq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gntajvpqk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gungmnptp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gsibjlszd.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gpxylbnpb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gkuercnoo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gpdczdxjv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gbtfyjatp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gmdzlzoqn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gzctykmsi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gujiavfwq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gzpukentj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gzshgjdfd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/glzgcqhkb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/glvaywgpk.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/grreqmbyq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggbjgjejy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gunlreztt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gbijqxhcd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gcfasrato.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gehfgxmjn.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gplohjwgr.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/ghzruwany.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzzgifapr.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ggmfitrqf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfvyblben.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtjsxgvvk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gvscqadcg.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggkrdawxb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnvsiaqlj.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ggiyfxcxi.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/guayefrii.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gwzqabvbj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gbmjjqcfy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/glyiywlox.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gwiankjeg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/ghkrvrwuf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/glbbucufy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gnoijrucv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gxzcpvwmd.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gvkrqqvzh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gobtdxdap.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/grccqvefh.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/grqbhmjin.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gckavgzfp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gbizvyzqr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gbkgpxcts.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/giesthzyx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gelfpfpfd.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gzvpasjke.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gbjqautae.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggpygmtfd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/goncvtioz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gmjfuwivh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gystcpgvr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gassbutfw.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkezydsez.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gtasutixc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/glggnrhdi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyemtwzql.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gsryefsbe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/geurgdeit.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/guarqfqci.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/glwsjxhbp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmlytqcww.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gcnabzjio.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grdqkjofp.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gdltwlonu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grnfymihk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/golewyjly.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfpdkcnhp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gfmmqlzvx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gyjgaotki.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gwegsxyzn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gvmumqfhx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gpylcfvup.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gymzlsulp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gtqspvfoy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gsbekshjm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gddorgxho.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gzhbwomev.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gsdfqnkwu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gnlkbvpdi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gucimrltp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gqtpinthw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbiojuzep.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gynvyqybp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxofwhhaz.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gbrsqmtxu.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gfqzhhkri.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/ghnxvehhx.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/grpuhdcnr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gzqkaucau.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gzwffaarq.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/ggfgxbbvd.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gmydgpjcl.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gckcehvyk.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gcrozpcrn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gdzsgwghk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/geyozveub.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gjlypiwhn.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gsjpakubv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gcwfvgxox.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/grmhytqmq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gqbkpwqfo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gondvnkam.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gyxwjdepx.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gglgbssdb.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gcmuauhls.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ggjryztyo.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/ghjxlaiwn.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/ghadqrufi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/grvikzzbe.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gpsdwbusx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gixgbiwws.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gklvuksyu.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gsbfxlsaw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gavwpfafb.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gremidolj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gstacobcc.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/ggzasimvb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/giigeqbli.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gjogrvvwc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gytzvstkx.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gcevjbada.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gthtrddgk.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/guncmpxfp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gagqvohti.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gzmqcjerr.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gnfioowmh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gdhfiusbh.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/guiqttjmk.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/ghoossabz.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gjlhwskfd.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gvojdtikc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvrnsnczr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfcvjobwf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/goypijglo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gmhdmnrjf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gmtoupgke.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gsxtaapzx.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gxrkjsgeh.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gtsqogfhm.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gwqmmknop.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gkrllfusk.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gcpoccdfn.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gabbiccex.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gstedrzvs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gicyeklfa.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gnpdqswwc.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gjntztgmb.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/grqyhnhhn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gtpbhpwha.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/ggkwxvqyz.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gdtllpndu.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/geqkljhjv.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gwayfubpj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gumhkrvst.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gxouxqjfy.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gynmklbvu.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gtaytcoos.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/goadusyzu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gwczscxsl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gdnolcnkr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbmhgudws.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gsaewqiyd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/ginvwzllf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gcotxtyyg.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gmnxpsbox.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gxlixslzg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/glnlggbzh.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gkfbnjxfs.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/ggrioepwd.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gomgmnvhj.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gimnponys.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gsfrqbgyp.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gossuehxi.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gqjwyhgxb.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gtevyymix.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gevcqcpel.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gugrlevln.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gloxpaoib.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gthvismur.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gsauzvkfu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gfphsalgc.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gsaheyyxc.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gqgvppdla.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gwhsrrtvz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gttbzrcec.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/grjpuonjb.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gfucgyqvr.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gcnbkgnfm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxwmmfdd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gvsssapvm.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gpeejdcqc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gjuclaohz.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gxeefhotg.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gssobjxjy.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/guityknnj.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gczuvsahk.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gnijtrzrz.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gdwxrysmp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gzugwvmoc.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gekcrzsxu.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gaadcccez.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gnwjqigvy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gucrtfdgs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gpefrhlkg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/giqtcdqjy.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gerwiqqvr.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gcumjvhzv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gbrwlyqyk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gtktbyadj.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gyhhbxmia.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gqraabter.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggtzcdrac.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/grpplavhx.sHtML


<!-- 参考信息 -->