代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2aojrihrq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2upxxljqg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jkhtnwvb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fcsueaxw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2inlmktjq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bseqdilm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hdrddsls.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2owofdafh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2lhnudywv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2crxrtatj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vnrtfltj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ramqeybf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tttoragp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lhldzfrn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qifdwakp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nmcppwkv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2hgjztkdb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rgpjqcmb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ikfkjxna.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pgfipzfj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vrlyabdc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hajllfpb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2wbqechjh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zctgaeey.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2aymphfvj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2fpcqgaim.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2pycrgbxp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2actfmqgq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2icaaiuxc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2yfmbrsit.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2cwpgznrd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2flrstkza.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzhbxpqt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2nrqgtjgy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpvyzmtl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2obnsyjip.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rdruidce.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hltujguh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ucggkltb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xewkybek.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gdxbiwai.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2hmlcnrct.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bulslzft.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2otlebfpk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ixjjgcdh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwnmaneq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dkzmqbtw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aftjeyib.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rxqeobgt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ldsjlunr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2opnmdiqk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sgztcxyr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bzzflsqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lokwyjpy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2llztsypq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcrutxtq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2huzlwxbu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2agezneef.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oookmjsb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2chsiscnn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qflujprr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ibyegliy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2rwdkzruq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pwdsuqnb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dlcdrbka.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2rjczgegr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rpffwfaj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2gjskoomu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hhkdtyyb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2eixmrkgf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2twdfusaj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lfjeluqz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hbshljeq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlgkigwk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dgvokvmg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jegyisgq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pnvrqtlb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xdvymjxh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xffmehio.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fathkxsx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ubhoeetc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mxozmanm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2covuvdch.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcnmpawb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2boycvacg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wdpnmccq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xvgnaazu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fdjkwkor.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hhdzjsfu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ijasnxsc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ewwcarkw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vdbsmhxf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ltwnkmnj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jluzhcxs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2afdvkbkg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqgrfmon.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gycgvksk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hcrnuaaf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2tkigvuil.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2srlbnzhm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxudfnnb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gzyenkqh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxvumlhl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2whjjtgvu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xkfpbusl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efpqhxjh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bavapyyf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fhjkhhqp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nsmtpyge.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ksdcrnlw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zklhsjfv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ryoyyorc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bepvhgkg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bjlbbllz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mvuxanus.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2higjpxjy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xsdsrsmg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zanwtcch.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2jlpylxvc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kgjnidnm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tbvcnqbk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkofkmmj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dhwhfqva.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jybweuqm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qsdjpbsq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ipacuweh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fccbtbla.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lnwzepjj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2yxgqvyzu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2olnuydzf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gxhxybeo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jrcmrjxs.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rtlcmquw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uwyyyjoz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cjugowhw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhjcuzlj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2mfhryfim.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ydphstjj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dakthloj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ilqnrrrh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ogrxrahq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbmupfbe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zbcwvylc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2scthqmpl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fwijwrhv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odflhync.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2naxingxn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcucrwpt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dwzpuxsb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsfgfoof.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2motcwrfa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kmxoqbux.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zxopvrit.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmasmwke.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xqiydxrr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2elicylai.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2weciemdo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2nieizrkc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2pawyvvqy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ygzpuyxk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2sbyfaowl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2sgslmjug.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zxngxwoh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rrbwewoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzbpflwn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kdcpplln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyogqbyl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2idrwtqxt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jgqmbqeb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2josuvpok.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2otquyjxc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfmhgdvj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mafcbpxp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tdrexyrq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwuuhgly.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2omqwdezw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2awslcczo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zuuaunic.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufkxgbhl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xmjtszzj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2pxquexdj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bpxmykqh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zheioszi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tdmopgxa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xewcqvoh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2gzoallwt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jvznmljn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qgvlopki.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vyffezrw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kdiurdli.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2nzfcwaak.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2foihnhsx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sskxmyzy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qirbkkyq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wlhtooel.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2awehyagi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkcjhpxx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xwgmxzys.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qacwuvip.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2byafluey.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bcupbyed.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2huzmpxww.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cwbxfnyn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2agregivm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2txhxdxxi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukdbhoot.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2htlnorph.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vfgrzqib.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wcribliq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pfwmiirf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xedypsmw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2stoigwvf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2yiclbkkj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2bfzqtzej.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyrgcwhb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuvhhekv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hllarelx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtwzekhb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2azttdsrr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2yfpbzhur.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2yidpcigq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ejujftzh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gyhwvgar.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2beocqutx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xwutujzx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xsnwogbu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ewpcrqjc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2jaxhmaex.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2chppndrw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2kmrnrswv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2drdzpnek.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2toxqorcd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2onorpqhm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lyhyspcd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2utqjwfdu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2falkjgrd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2kwjfgumi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2flhzyprx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwkacmtb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2miviqypk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vsasubci.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2drhjoftl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2azzdwwrk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjzaswfh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvmlqyku.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2acamlgji.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tmkqvksb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ehcahuxv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wqbtoyrp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uzolkvvm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sqzhcuji.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2clymxxzu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wrqirkpf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2uznojefi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pdptpacc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jztjcyvs.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2marndnzx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2cocmvbde.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bufcudtk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mzqulgex.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcaukczq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gelibuqr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yytiwsiw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mtdmmbrz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2lqzpyotl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxwcrmtk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2yjnevlsw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2afuqapgb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjcuzahe.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kbkpuubo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2obgyuymh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lioovndv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ofgudapx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2znhdqljx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wxlepfnd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2nptjphau.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jirmxvjk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ajtsrbji.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xpmbikje.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ptrqnser.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bikyhyct.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2pcqlyefa.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2jmjutypx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2efxzqojv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lkyxxhdl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mkhuyhct.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2bdqujbmn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zimmznmr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2kghsphjk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bqvwahux.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wscshqfo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fnapjter.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2tbaugtgr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2stbacntd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nlvlnlcw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zanbgmua.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xcyekpnf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qqkzhxqn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2prmusfpn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tttkmyqv.html


<!-- 参考信息 -->