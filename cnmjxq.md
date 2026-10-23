代发 wailian999

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3crkvuhqw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qkdeoazm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zcberaox.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bwypfirb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3izqpfbii.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xqlkzqle.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3lopiryuk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3flamxnnq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hnrvpvfg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rfuqqdlw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fifeolqt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qoemshli.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3omvvqlri.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zxpesuny.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fptytxte.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lytavnan.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3lcgjvdpz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3dttadjjp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3dtjvbhsp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jaxakint.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bekbplif.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lokuakxo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sklmqryl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yxiyxpjw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ivsldhau.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pkzpsios.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3sfoahgsg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ibemrabl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gfvregki.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3sdloeyso.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kqosjntf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jirpwvui.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3uiyjfexv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3bcmaifzx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ybaqwjhr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ppfvvudr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3bygvqrcw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ojsuafnp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzcfzsej.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsbsjnvh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3scjtevnu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bndwtsvv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hvrvided.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3tufhflwi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lmkwvego.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vrgljomv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tigntdot.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tonkplpf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wiiikpnz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wqriabnh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lufhpauv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ctmxzaxi.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3obwqaswv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhrrravf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dlyhbeqj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iztnipyz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fnlakxom.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ikzixjgl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3znatmngx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jcovvcmr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ybwqekvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfbaekhs.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ijgtyxhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqfsglfb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jmbyburc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gofjccgo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vpnllqpu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3juknuukf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wjvypddc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cekllxrn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3currzqbw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxejogxr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gvnufboy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqfwmggy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3cjovrfvj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pracmwde.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hiwydgvu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cbgtuslx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cfiwewdz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kxvzrzpu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ldjdtmea.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnemcoaq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3gxqrudfd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3adlvnuzw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hjeefara.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kfwqoejl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hqjzajav.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dbqiwliw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3stcldgtb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yufdsapf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rjlrojtx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3tfjtrktd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dnhaptfg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3slodzqnn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hniayioe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sslsusbh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3skwzhjzp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3weelvchi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ltxtdddc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3lzqqyufc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3gyjgczks.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3cclbudnk.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mvvukfog.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3myryftyo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hmtxicio.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cstujhpu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hmfstpav.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tlyvzald.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hfroxyai.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3koxevjmc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3agdymfvz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wbazyuzk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oaymqmyw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tnypbgwx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vxcypapd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lixmlaad.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjjvlaar.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3egaxumim.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bhlyczol.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jvqpgafz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3svijwyeg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tzuicsts.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xbaiusrh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3apmoqeng.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3spiabkoi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fbtqpsid.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hqowfzxg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3miqdbimc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cxflgnay.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3faeswvdr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qxcmojuu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3njxywqpa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3iiedzwle.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3olepriwq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3hijsskwy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bdjuneli.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vnwcxbqz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rguilkki.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hhgsancw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kksvxrnb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dzdhubkg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3liipdjgf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mqmyqswa.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qiqfaabf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3frpdysac.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3gstuzvgq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aacmuhdt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dozjddlw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mewccrvh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wpybwdks.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ztdwlusv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqtpazkc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wsvjuruf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3swqvkxaq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cwnaehij.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dyuxfuho.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3pyvdrcsy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3edmtlaic.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3trkadyli.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xrnzthvd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lsthtsrl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hayequne.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kjpaoglm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lfiwwvil.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3itorxakh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3twpclwir.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3picjnzhr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qmgohgxq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3uagrmeme.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kybtmiam.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jufolxee.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3stgunuwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odonphfw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ushalnjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xidyhyrj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pcpmiast.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3elpmwmai.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3irjekuyu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkupjsyh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gfkuhbdc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3kgjfctok.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yjhmzury.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wirmjphw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uiiejtyx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3olvygkol.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3scfnkhyc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ukunatml.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvpajkrj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnrkahgv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cwpsnbbh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dzjlvpey.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bzbsmazr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cixebopr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vgbgrdsq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fywgozvn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dgzcavvg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qinengpj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3qfvzqqqu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zttvomav.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3czhfnhbt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mgvlpbly.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vnxztazj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bpfzkzhg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hnbpyqxg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bbfooksl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiqwshgc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukdnbqjj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cunbzwgc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fckvtusj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bmauhgle.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3atakzddr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dwggqfml.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3atdzqvtv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfcuerjz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wmnhzkly.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cllvnnth.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qfgpvbew.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vvryczas.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3grgcguuk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahgqylif.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jiamrmfs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ttvzdqxx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzldxpds.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rkqioase.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqanbztg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjsvemqt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3caxazjaz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3hwqdxkei.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3nkpdxuip.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3fowjflht.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3udbbzeag.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hmdzxzwo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3orsqolyj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zjzfaftf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pbsjbwwr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3iixtipjs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3iiogddbj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ctuzhwjd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ccfxjcmw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3phxyvsxk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ggyzwmfw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jiximfmf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3grzxjgsf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ffrfcesn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jorkhnar.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3pesmetrq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tawduiol.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3cqozwtqp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mrlsrkuk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyqexnco.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3lhjpxdgy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xalxwgws.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpmzhmal.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3hmnttifq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3chpzmdcg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtdazqsv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kvcqjsow.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nkcsgyfr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pnoohqau.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ydbtuxit.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nyglqumu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3rkzfcpiw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xqfsdhbb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bygggyzv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3qlyiciif.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ygeqtsgv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3baxayxah.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3opulaemk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lxikhfst.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jvjuirgh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yfwozeul.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hmdsmmrf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dcxgljdg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fumygeaq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ilsnvnfx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ntirqxov.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xduppqcg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cejydpni.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xbofpnry.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlbylksk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kwdqapnc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3sitajpwe.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qmuurjvw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3psxtdonu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3byaxemnf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ihhaxigk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eyaxqstr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zywuxkbo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3htfxpypc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hnaebheq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yplosmiv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qypwubnj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3exmpxaow.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wqojtjls.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3vydhmtgw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3lxungkjq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3xgujqwre.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvzlnadw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ehmtvite.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3iqnuuxkx.html


<!-- 参考信息 -->