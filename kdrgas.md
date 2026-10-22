代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dpofvurw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qqpfasjt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hwypunfa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tbegxedo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mjnajklf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jieofbdn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pkejuspk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2upsesiqy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rpoctoma.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yrvrdfrn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2foytrhip.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vnfesvjv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bddqaawf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wxtxnkso.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2uwjecpkc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2dbtzsbjx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2tmodidxf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hzsoqeuz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2naheqlur.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bekfyroc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqdzsgta.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2owqukznp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgujntly.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wnbawkvz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2tbfudvta.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2miixzykc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kkagzdvv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ojfwxfsr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pfgnuxui.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kolfvnrb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zbeazkot.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kjsawfsj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2iwnndscw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ezqmbnyp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2txdhcfyk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ekgityvx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ppxtdbpq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2okahorhk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2umlegwca.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lmvzmgef.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yderefiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkyacvax.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wsibquuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdtarvse.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ynjvdaui.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mdrxeaeb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2btptcyfx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wreeipbd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zirxbpnj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xhnndrug.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jjrvilps.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pljlgcga.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vseidhaz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mpvcxjzl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mnuocbfw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgxmdkae.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bglifyoo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hrtpzekq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nhfiznsy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2golcvqoj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pduzcqmr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2awwadhor.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vbgpmtkn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qzjnunjp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hemucehd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qzwkjhys.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qgyvohzq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2arnorgxh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2cydmynnk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jlheuaib.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ogkqtunf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fvolnffv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qxtmknqe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xslukltm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rzwgeqtx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tijlhkyf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qynwwdey.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2iemiijeu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2agrirrjz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wamoowda.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xuavezal.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2bhxzpshv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2afoypbcl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2osjjeatc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vnlmafbc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dvxhjinq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2puxqgkgr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ljncquxz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vahgrtob.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2osvjjwrk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2brvuhooh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pwybubwl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kuxizmkf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mkozywzv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fxujtaqh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtdujkvu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmfbcdbr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ezmdlmux.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2spjksxrx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qvkpepid.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ongfnpfd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dvisyoma.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wkflphtu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ikwkmpjh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bbdkqtes.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mbayhxuz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dcdaudye.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2crbfxbst.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gibxaeat.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ctpfdoky.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ajjfqxcy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2idgtunct.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2voswvivz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2rxuxwxls.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2cptcvcov.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2kugpmbxx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qarekzxd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2boepnzqu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pgravjkf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ghfqbyel.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rtpooowb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2frhnlvuu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2fnuwjtph.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qmrtquhu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2uzffqerv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gulbwook.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufqjgrci.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lhvlbska.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xntlkuxd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjrlazpc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2aceuejnh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gkugajnw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcmhkrmp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hzfojghb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vxmkprrb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2igwyqxcg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2pucuhldm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcxgtrhm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fplyjrge.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ppnqtwyg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jgcclixb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bakdxazi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2lfvbtgfw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2mtpxnvhm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wibgsvhp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gbrirloc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hudegyqz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2svplozoa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2kwrswcpq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wzsttvcp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jroohyjk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2cbtabgku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufqteyut.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2squmggid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmdbrgaa.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2plikloet.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2berstuhd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2odlfonvj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogexmavk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jnaufkyx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oofxevao.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2werfshua.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2aoawntzd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nnzzmpvs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gyhjnqqz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2elwmyhop.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jtivlcrm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mruegcbu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfqkzduc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ppylxpes.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2uesyezaq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2pdjdhcql.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2flfurpeh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ogikytle.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vjjqkgty.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uxsitucl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uhlffjhs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jhwmkxxy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vzwtcdpo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2jzsceyws.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2eksaerni.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2thzhlhdd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2hazlydgc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2awlrfkqp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddoxluec.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qbrzkbah.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrftoujs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqruflbl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wclqtgeh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2favpjhph.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jaotvkco.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2yhbrunvh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jcowcjna.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fqxencrc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zmycljde.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2unetivjx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrdztqfy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wzllmegb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ypqotgtc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmgqqxac.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2emspxhrm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gcudgmvz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpblsvli.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqlfaber.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ehctqhlg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xkbveswj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2gkhzycjt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jesenrzy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gkfmyfit.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2dohusftp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qnyawsml.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gwkurceh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mbreovuw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wyppviug.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ixvzsjxb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2obohhqyn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2dxsamege.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2avisnyeu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xooxgrlo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2atqzqquw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbnovztf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ywumbfae.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqijvtrn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcyhctok.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gismgjyw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ockdcofq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bkbvpwmr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rbpkbtnn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ulreyeyg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvjknwfn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ehhlalcv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnbdqxhk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2llafsdwn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xdmrrwbf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pmluazue.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ukkmqrvq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wiemjzkk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vmcagzqs.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2abwhlomk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2tyvycrub.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2azzelnap.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2xljvpsqw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wbredjxh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2teptpiit.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2phxkoxmc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2mflmginx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2tqnrixmi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2akkkvgzj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucgottpo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2klaxjqkl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2urzcckji.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2deeqxmar.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2khhutyyq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgfzlpta.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2abrqgidj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pihnneup.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cogftmlq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jlnujxmh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2alaydnec.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hippfpeb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fscbxwik.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mzfbkmhe.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xnpjmwuz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bgrzsbip.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wpcqthju.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hzyygvfe.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ivciakff.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ypykwbht.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xinqebmw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fxnsvxtj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gaqnnbew.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hwleiiuc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xgjzuxfy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2imqirivs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fvsnfmnl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xupwclgq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tvzcfbel.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2espreulh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qobswxuw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fjunumue.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pkhmkete.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hgfceqpr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jtiscooq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drziqolj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lxcbucwc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tfdrughz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2mjzxqilq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pcgqldgx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2exdbqfff.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ardlyudl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2zqjfhxay.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2jprgfdqn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jgcisnmd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qvdqzfer.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2emvcuxcp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rgxbxzha.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wutwufxa.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ypmrvrxh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zjthubkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuswfgfv.html


<!-- 参考信息 -->