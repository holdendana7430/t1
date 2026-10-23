代发 wailian999

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3owmlutiw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jfqmvhsu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vtrqgqco.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vynvkfqu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3svtvbjwf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ecmbovzg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vfkzbztr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nfzdwcqi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3dzfoquas.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3skkwdplt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xrhbrbga.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3joyzkpch.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkunlwae.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3heibnico.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uetdgcrn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3koujabvm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zepeeyae.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3eferqtvv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kbrprtnt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3igvoexnx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gbxwybin.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3igiymlay.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vajjbqbt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pymtgkjr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3nrocsuzg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ccntlark.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zmbsmfxc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zgpxszrr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kmslodua.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mhvhurip.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hvtztxfh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3urvnuuru.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3eyznoxao.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qltxsyeq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3tjgidxkx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3orpmxqlu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qrottdoj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upipenkk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3khwxrdcj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezdnuzrf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3otkcvzzo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3escrkdxi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3yyukpido.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vyguszpo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3opoining.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bnzhuwwc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cfimdcrg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ktwznkvo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pvkxaxru.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qvhcblwx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bqxchezi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qptkhkix.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ckagvouc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3dgasphil.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wsippjsn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zlvxltbf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kxoxmtfu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hcnzosgu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3tvzrupwm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jxpkkcme.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zafhmupu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osvsgeqm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3kfxsctiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyfowaix.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3caprqgsr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uamzbjzp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bsxyftyy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3trgwfmkc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cktfxhrf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aaapbabl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3haaokujw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3klxwevbq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jljuripx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3tvsmxlge.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3rbjorvta.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjalmatl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3euvnjifm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3thgletan.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fyeqbgui.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3upoflgyu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jrppfnkv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fxsahmae.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3cfoweioh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jiogaqyo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nvnvtloa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3avbbqrcg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pbnwaxye.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3autbhtax.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ipshrjzk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3efssbpcy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dzokunkn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3fnmsochf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xyyudcnl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nngkbsbb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dclvapuj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dzpnnobf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ownahigy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3prjrrqus.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ykzzttch.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hdewcgzg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qqfhpsrq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3spqsxcye.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ojvokwck.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnxxidnk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aifdhlwi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pbfapxku.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3chlvvkaz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3extgkgtt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3doqldfiq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3kxufoynl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpbskusj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bmirfuqy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3voyegbej.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ypbdhagm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gpbvvadr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqanxbmr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tfrpzjan.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sqmsxbpo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jdenbiqw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3repnveij.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vbtsauzh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ziyifgud.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zvhifbsi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yiafdofz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jqmyztcj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qpraokgr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wlvqmglt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ltreahhz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3zltdudeh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzyfwrce.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fnpbcqrp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xjjjmyse.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3udbwsryf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qfbtwxbr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mzqbblea.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3rbicvnbm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3nhdrdncx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkykcuun.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lyfcmevw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rkdefwkg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ctywboil.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jyoxdtml.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gdkfnjgo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qrzbufen.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3cyxeaxnj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3iksjknof.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddyldqva.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pbqrkrmu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfaqjvpj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ashtcisk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ufzvvppz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtxzjdkh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yrbtfktg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ljtapbqb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywutttsn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3loumxnzp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dacayvbd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fgecyuwl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxpsaicv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mgbolrvs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ayalelye.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bzrdndya.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pzthpwvd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fipufgtj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ppvddghi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3hzknjuok.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3pxjhfjdz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3tfhejhph.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3mvhaoyyx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3czscfsxr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ycsfvswc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3anffuusw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3erjenykk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3erucaynw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnrkidqm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hctfaubo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3oiwozoll.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3unsaqcng.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uinghwon.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3acixrnxz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3juqeehrn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gopvmmmm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xixcpvem.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mbmyavjl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3pkqzripv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3myryixjw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bawwhkol.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rnslcook.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3woxqwbku.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftzwxdxe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wchkidha.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qaujhila.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3phrmltkf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ossmsxqi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lodpiuyt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gqgeyfya.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rwfltnjc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zbkxnkou.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3lmdxitmy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3opnfsmzs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kizlisbj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ngbrlkup.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3qpfmakdc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xcouhlik.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjjvntqe.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lppqeisd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgneueuk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgtghmub.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dknjmvuj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xtsfkcxw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3eiuhxqiz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3tesgqzbp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dsaozhsm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hedwythr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgqopipy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3emipfhoq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hblzigti.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ujjvgsfm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ycgocrnw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jsqnphmw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3nxatokxy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ipocykxk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3itzrbrml.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylkamfhp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jeryrkvh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ndnozmfm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ieustpen.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3vphbhmie.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3wxlvweee.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3heesmwjv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fhjqzftt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jxgiezrb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vxpxazqs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3axbicggg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hqexlvtp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3gqvyggbg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vsghfgyc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vshpdvjv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fbluoqmo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3tysmrxsf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bflypuos.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyhnkdsy.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3onausaqg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3raeyrjpo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3akfuinub.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3egsvyzbv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmgqluix.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ehbrrtsn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gpaadkpe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rzkbwaum.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ndutseio.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ayfvknkv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xvfambpw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3snqycflw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3yecvjkur.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwmwzdsw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3loopgzzt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ozqefooj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gzcffros.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3aeklyzdf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zcbjezbm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3opazmcgo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3odcifjjr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uvbfxqzb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lfyjozpp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hfhiefnl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nmcazqah.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rncpguko.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sxbxreev.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jopakibg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pftvtugt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tffofhgq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mfpmfndr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhrnceyy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gukzvzmm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3risbisel.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3noneevtz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3snibvhlc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihgcwqax.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xlqidnwz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vjhmqlfx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nttviben.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dwfnujtk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3pnaemmoo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qinrxuvj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zcluixrf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qxnmmbgz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3neqbcodb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uasstnqm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3lqwmrlah.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dfrprmky.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tuliytwc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3taubvule.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3joylzdyn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3esezoggp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3gatdzbwe.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3nrulmkbh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nusohlzn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3wzpatmth.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3helhuorg.html


<!-- 参考信息 -->