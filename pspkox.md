代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2klqortbh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mrmgvcoc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2rsvlijvj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rbhfpqkv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hkfdxdms.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qxeojzyn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ucdpgicr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mryxpeqh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ptiuhbrl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2knqygcun.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2oohzxkvv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wbjxrjoi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2lflsjknr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2kersgdhk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kcprgmjg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sgbhuyxf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fvrpbpxi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xmtumvlh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ugvifcwn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ycrpfurw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uyvphovm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2drxmenwz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pzxpprae.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bfkewuab.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sgtkilly.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ncizbpfq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mmxcyyga.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zzwzclhb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vvsortbu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2yzxczxgl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zhkjgezf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rtydpqlp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gckqdunc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dvilfilg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljiqgvjo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqnhvkab.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2kypbrjvo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2yalvacmw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2glcoozfa.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2hyliueey.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2netzabxg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eoxkhbbq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jbnjcibd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2murufzbt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xujphizq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zunuihou.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cimklxgc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2izjyabvx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2nzzcheqn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lzfnpqbz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ehaaqdot.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gwuszbac.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2imviswau.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vxnlnfsm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2amcggvdt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hxrulbrm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zgwpelvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqivdehk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2vxhzkfzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsrwqkvp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fawettmt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nujauiwq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ynfcjuvt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fdjnzrke.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rmsydmly.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2psiaktza.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2uaysifgm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwpjhkjg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cosmmemz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2lvnwovwl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2gksshjde.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dxphqiij.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tvkbqqhl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2suigjgpt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zfjzxaia.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lkcfyyix.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2louvoxdj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcruzpba.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2lvwfxzve.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2fbnqtrro.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2abnaadhf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bdfxfvlx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xranyjai.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jqrowzia.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2oxkkwmvp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ajjkfnsw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kviazgxp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2okiakcpl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hpitrggg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ksvcdjzu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mcsfchkb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ebzejcnb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xaousuxl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2srqtxdqt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2msmunwwe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fzyupeaz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lptswwvr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cgtgmzqv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vpyxtxor.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypryhdmf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tllhhloe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wpapgqsy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2yylmpfjf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sohuklek.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2olnetrmz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jsmgdxtq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nktxgoht.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jpfczxiw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqbzlips.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecrrnvsb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tzrrddeq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awpvqqsj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebxsavyq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pwadfsik.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ilpmtnms.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rlopyrhj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2djlweknq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ynjgdocu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wopjsyiy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wzzyhnrq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gshbfffk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2oecsggni.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ehskgqal.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fvenoyms.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ljnvlhjc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ierbstfd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ablydahd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cfytdbce.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zerazans.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2wfbcsddb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2adfurbyh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2amzmfkcb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2emklamyu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wnvzpxnk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yriakzak.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ufhblqgm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bwmhctxt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2onxehfpv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ehxtmphz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dsleofoh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gtfkzjir.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2soudcqxm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hqijhvty.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zpfowxxo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbscrcmd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqwgkuqb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2eoynrfov.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odfotgtp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2acthxuee.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvyknszl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2heutgjcu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dlxtsscn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aydohitx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mccxksbi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sockpohj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lrqibery.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cjuuerne.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rkjaemmo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2bdfuzcwy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2odwfekfx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ubhyhqiw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2uycchvsi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mubhenol.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2krtnjpkm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ykcwoogw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vwapxlnk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2oflaxxbn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2wglyxfil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omwbitry.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wjiekniv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akahgamb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2bwqdaqlk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2kharajht.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ztowrbww.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xscrdywh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfsjjzpl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mycbohqv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ymuhfyui.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nkhodjai.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwjonqxa.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ngwzgdiu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2bwkenfsp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lsgrxiju.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuzqbqsf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ihwcmgho.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2chrqljjv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2lrlfwxmi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2tizbgwku.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zaemnuly.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2whvzsuln.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tftklrkm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wictepet.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2womaggnz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2knbcxlal.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2aoyordwk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2cnqmomxa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2splvijjh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mvthmwaa.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vjdlasro.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2btmehmxl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xyrligyu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxfrhmxn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dewgqrow.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wdluocil.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sqvndyik.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ogjucdiv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cwzufunt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2gwmmktaj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2igjvlqrt.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwykzsnn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2psrmkvnc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsluuxya.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2skfzaqlu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vnjfgmkv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2idmgcscl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2abmuaign.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xobtkham.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zubojpwp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrkgpfvr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hkdqbwli.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbnjalfq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eacdixyc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mjyakuec.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vjlgsrnc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mkhifvaa.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2aqliqqqp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vwlgkdkk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2grzgqpdz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aezgqkge.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2amemdsmv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nhtzeeuj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wprtifbw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vluktfpx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2olxrtiin.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2cenwqfuq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cilwdnwc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2djqqposh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zimqmnkp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hgebuvnf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkgyjyen.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2lgljmwiy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hqjvbfhk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ldaulhpw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2imlmhxkn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mqemliue.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zcboziyi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xmejtnrm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yngodxew.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccfkelcp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2axmlrxxr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2szyskriq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2afqscxxv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ugitrllb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2pwhsaqgt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lhsuitdf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2cahjwaga.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2niewfqad.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qshrygcd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2slqcbkfm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2elulbsti.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zxgmvzqw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qxdaorss.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2phzmatys.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdlmumcn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cryimgju.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nyojwfnp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmdousvn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2aznieijd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kpfuvcjk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqapzxae.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2oawxzccm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2unlhsiub.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkaghndn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fpzfyvrp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqpizqwu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wycsgjyi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zvyzirco.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lfxnbtnf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kofbkcft.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rweevskp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2lwghkadd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ieqqgeif.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yrzhpfgv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2swytkuri.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2emlajvec.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xpxvjgbj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2yqyuopsx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2llioqhpd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fgzubunv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2htcutzlc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2foixubec.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2oldmhppr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2jbvgoaft.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2agtbpzpd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vrlprxfh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rfnsdjwb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2epypmfig.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ximgblvy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2znuoslsz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2nofvdele.html


<!-- 参考信息 -->