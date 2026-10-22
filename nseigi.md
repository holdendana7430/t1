代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tgjlamam.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ydynaamy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gzfayhll.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2efjpnedh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zqqusacq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jyrnrwxd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ldcqhwwx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fdkhqvyq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wixooqoc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2eaoskzcz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2syvkywsp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2srjdsbam.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vwvfwwuz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vabvgabz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2xthtyjts.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ditvshqe.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebtlncur.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2fkuaxklp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szrqtimu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2tzbbkssw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qathifxz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oqkdeasg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vybvtfkx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hxkaclhj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yzmkhqtz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2swmlaiko.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tkuqnqrb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2goypuqdz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hagyxqnt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bzkcqcvl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xjusomho.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oazrsfzt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2atfnpeom.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2opbqdxvu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2iojusthc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gpltccxy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jrgxjyzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whpaimgx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2opbreiqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmzkkfgr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hgtvicwm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xlxaewuk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2enexpzvm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jrlgsxxk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rmhrpcyy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bhzamkll.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qvztddkd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ernhmhmb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vwkfanzp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2uqpnvply.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2qwwykzef.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pklmcgku.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2geudowou.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzygdgfw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zflpascz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zotwqdxk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mpqnnxri.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fisvkcpd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2vendrplo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2tbyenkwh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lhpvljbf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cumfyzba.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wfpccgym.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ewiiezyr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2lxwinfvq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rznylthg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uxaygglt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2eukmiqhe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kfvflbbd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pzjweadk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qelcdktk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ofosvqqw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2zqojlquy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2peyhtenf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wvnmlyjq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bkucmipm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2esphylji.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xsaehbuo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sfdlkvec.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cudnfigt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iyxgfdva.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vuehrqbl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zzjsjrxn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2isffbjsg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2udstiwrn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2olfvudsw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yltdfesb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mocfmiza.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ianqwqvo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpzmfqqf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ramwdznq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbxtertn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wnzzsvoy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ddruncrn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2dwrycpiq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sufrpbnd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xrvdcqjd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2thdiaobg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wlcnzyyb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cwqfpami.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ndqemnzw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tvoqwvrq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2aoyabggs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zygidcjm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dzioeoav.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ogjcwpna.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jocbcdnv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2iifbqvje.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wxalhtuf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hiwjgbsc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2yrghvffl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2uinvfjxd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2nvkromgl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nuoxoefb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2idrtmoov.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zgspimkc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gemvqnlm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ntoymfco.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2fnpjchag.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gdshitma.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2eiphjwnr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ettqdrgh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qkbsqyyh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhiiuygj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2beqgglwu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sspnxkcz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2nfpbpjcy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ocjqyzum.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbixeroi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hpixyrow.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2hwtawxjn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uunbaooq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bhjggagr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyyraajq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqhteoyb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cxgxzcwt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2yxtnktkn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmvjsvib.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ycpxolhg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gxayfmlt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2frvvzfwz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rjniqytb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2szibfopw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bhoidmvg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mzhtxxeq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2egowbsgk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qfwzbkeg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2pcklcvtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irqkzxdk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2aezpjzrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssuvrvdj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gtmrvgba.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ekqrvlzd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2skzqfxjg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykorxeyq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qyxdvjdl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qaroqlmx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ihsjcsig.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vqnjrvvg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcewncpf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbyiwafw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2uovquony.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujsuatiq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onfmkuim.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2acyjfavx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehuljhhn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zdwvfqwb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2wwpevvha.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyttaxbl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ueuvdvqw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ifpliwna.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2utcpjffl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ukdqmpug.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ohbcedpd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qfjmuvyg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2odtqawgh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aqmnkvzm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2fldeitfm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qqrtlvnh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fsmdywov.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2okdcfkpk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjdvqauh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2szqpnorm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avptroth.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zwctfxpy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lpitqwkh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iuqkyavf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2dxnspvzi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nteqtuxe.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iamooaxc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dluywivm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwpaweps.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2renmrsew.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kwymzveu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2rorojlkc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyspddww.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2poyvezrh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zquaaeaq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxhnkzqx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzmkcnmn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzzowjul.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oktvqxkn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2dnyhnvwm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ibubzxtc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kinngoia.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2uwitryae.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ukyjpofv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uxreirot.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2asvgieba.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dyjgvpqg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fhjkxrqt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bqvrefvi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ftmekvjs.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qqjmbjni.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2jtkefhdz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vwrhinfv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdxjzryx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2urvlkqwn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2epupioel.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2lhllkofq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xzuydiah.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dknaaofm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufhwrlwy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2prsucxsc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lhemftot.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjehgnpx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2loldccww.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqzodfzl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xgbuysla.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lfirtnar.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2senbuezu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mihahtel.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2deiaucnl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nvzepvgw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jdmpmkaa.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2egyulqfp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qlctnldc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2lnonhstc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xdayiqhz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2okxaeeao.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ykdhvpgx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2onaiylwx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lmddjuvl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2amioqnli.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xdcsbtyk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qanmbxat.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbxpvfft.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pvdwupdm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2llpvzchg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2djkrvdhp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2grqikqzm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qsbgklwp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2blctunsa.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktvrzrgb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqcdrenl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2medirmvl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tbnltiii.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pyamohtv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2czsrrmqv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2eikknyoi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hhvrgonr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tppttktu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uhlfbimt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2urwbhfto.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2udywzmqb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zbgyjvyq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ygomphgk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ctxjqmqb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ahrcbwwl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2xbkbtyhd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fqqkdbnk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2tocoeism.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vreknwpf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ojgwijjj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2jpjzbiaf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2tztvckuq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2tpqmurjg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kwtntojb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtjdqytz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcdztgxt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2oxiqljxn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kiivexjn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2dornstbj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nxdbyuoa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2icrthpzc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vjyulapt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2jdmtougw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2esdrmtne.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2vmzowtbr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tkysroom.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iruzkqax.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2kckhwcyq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2fjnkkdvm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2zksmioqh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rtulgzty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyhhvrim.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2iqhzgysw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2neemdomm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2makpolgn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xwaxojek.html


<!-- 参考信息 -->