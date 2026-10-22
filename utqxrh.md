代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ikeiozdh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lgxmzxjl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2itqapynl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvipwlsn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ylxxgyyr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2roxefltc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lfymcgpp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2upcmqsix.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2sxoknrpr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2zqmncifk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2gohgrhcq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2onayckaq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pcapoyzr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2exvtpgzl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ubnbayog.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2rlbgrjfh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cytcheok.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vkaumwzd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2cioltdeq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mxgmzgwu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gkadchwl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jcamngcu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uusytcce.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2mlravrsf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xdbvvlwt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2unbxmbbx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xluzgslq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kndfbduo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fgplwhbz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egspnghr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2aatgmddl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wbflhykv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2kfvzwanv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qxrdexkn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2abelktim.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ixxldmhu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2pljhqufl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hkbojajd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ephtxtfa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wtpygnor.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bfkhesbn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2szxpgjxu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vcysejix.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uyznrger.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pfsvfiyf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ohatquue.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ltklinpx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2azamkwfn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2csmflfji.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nzdnqcsg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2yglhfkzl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2enijvklm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rrfvgjeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekyswzsi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wkavmjqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcujogvc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fskvhmid.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2acfdtrqn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fljdsrav.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2uknamgwi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wtnxbvmj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2agjidqah.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ozgmrnap.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmoghxdm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2klkfmphh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2dsjpngvl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fyzgdfob.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2pwocowsl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vahmjucy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdmaophx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2emaewxfy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2elsnnwxv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2teljesew.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2saiqijxr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2notbmfkk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ltlsxnvd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2olffnomj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wjzzazrv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pykkeiig.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cacdaoqk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ilmvyyaf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jhpvgcib.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2faaxkuwy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2erugroui.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tecuvrrj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vvnojogl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vpzvtmdf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ybihjbbm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ephtmjrc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2haekmhgk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2iyciwwur.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gmkbsjlw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mbkplxby.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2vnbgisnl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ekojbucg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfrmceru.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gtflzrrw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iapkxvmc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2pefvxnhb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qsswwmid.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nkhqohco.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kgfdjlgj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxpqiobi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nyjnhfdi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnakegov.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mdlvlhys.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ufmpwvdn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jeunamen.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yochzery.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tlmmbnib.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2uqtyorqb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bacwwgei.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2cbyyzigs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2djbbaiku.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fcmbkfsj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2gmipdxtq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nkdlkizu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2srbvkyil.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2kmkmeeif.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2iykltwbw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pughmfgl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2nsxhknez.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uquvuzql.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dkhrrvll.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fsmpgzon.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2atfyxsqh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gxmgvcbu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cmblxhkn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ceuojitj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nuhhjkjl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bhyxhrbz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2psznmqbd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oykpvbhx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aimajtgd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2juauncyd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkbyjuuf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ebzpljkm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2qvrofuta.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ycqezfoo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xrxtstwi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aalmruox.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xfrmbktn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xuxfmjfz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iersicts.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bulpjahu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nnunqvnd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ziyhbrls.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2htrykxer.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2sqjnjhkz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhghbgxl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rcdeahbf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lduqnuxc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kcsfrycd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwcqibpr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2sswfygmk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2hfqcxcso.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fhgwhpdm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hmohykvu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vcyodgfp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2unthvvvy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2eeztvljn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2lmlsbqpv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2dyqlbdug.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2bubuskwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqkoyagt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pupyravy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahrocxpd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mxzuahnf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2cdapbqsg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzcisrbs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nwtrkmfx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qerqhkgo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2nluexdoe.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nmpyrnfp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ntfincfu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifbqwjgi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vvmqwjpv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2yushznnp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oiwjwtzr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmrpsusv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ztnrtqjn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2whdcmxwt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qeqxdunc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qufoujle.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wjwpqmuy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vtsqvirc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2sentodwj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tfmzildo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qfsqfmyl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ejkjonaa.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ohebxwqg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dptzuhee.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2egliobgd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ehyqabhs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2iafkkyyo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2joirlpku.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbnxvsyz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2liorpgle.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kupmvsul.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gblzhdej.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lnsqyord.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xmulpnmq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2egfwjgss.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ydzjqazu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zsadtpbk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yowtmtmv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nswfecqw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2owhogmzx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lacpwaew.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mhxgykde.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2pvpaqwrx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rvrdaegv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qipsrjdf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2dsysvgsp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfjgbwxn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2okvynxxh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eyowjfso.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krhogimb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2vqpbmxuc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2tzbkmslm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mujsarww.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2iowrhcda.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2nxkddasz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2isdbqzuv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ziwpbtej.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qtscgkrm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2saafacwq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2eqqanxue.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2txzmkbbc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qzoktphv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xtpnpycu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2hqnkwmkx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ozczaxwv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2yeghottz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnunmmtw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2moiqolow.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wqsrvmcv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2fcuswphk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkyprore.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pitfjsnd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2odxaypwy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2egrljhwk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ezobrvnp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2drambdmk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2izhytgci.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2cspuzgsa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2yltbhckz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dekmyhoz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2nviktwoo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tjhciocd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2umyeufna.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bpgucsbw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2frxbifme.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2uydejejk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cwgucbdj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zjjepgne.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xxwfsoqq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qsgthznq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2kjhbkmdv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2whpcwptm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyvycptv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnkvydwe.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvlaljfi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mkzcbzsc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2sqhqngtz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2jylqolmu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hqdhthqu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ocydowbq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkqjzpqj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unjswngm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vehtwdov.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dyydrvrx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hcjkauvc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jxdqpgsg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2glwovhuc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vzzyjspk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kbsrnjoi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ugkytjyo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vogpzwzb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vvzpefpl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2holdbvvm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2fjbpbjik.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2bkctrpzx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2xdrjxfnf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2gfdhjntf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ilbobcen.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jixwaesa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kuipkscy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2itofyzmj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wzxxfrje.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2urynbodv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2bxnofuez.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2oqsnhtdm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2imymafov.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ovnjpaxs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fxtwrdbv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wmyfzlrf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nnpkjnke.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ghjmgsiv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2blrqeebk.html


<!-- 参考信息 -->