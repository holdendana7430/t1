代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vrcvifou.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gmjmrqlw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2smovhiba.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bwwudvsb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jihtfszq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2wcgpjnwn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2yefelqpv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zokawgwy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2skhiqaex.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2yugsxtfi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2iijqmhny.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2rvbfarbg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2lpleaqso.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ebiovxck.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ygirjbxz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jtrdpuzm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ellgoqkq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2msrwroxx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2maistjrh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xvvtiwdv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2nklshdgg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tatfpxdn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rabghvyy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nfayvtdx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gsjfxiue.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2reupwecx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2oqxtfliu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zlqeyoee.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zqkjujsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2squnipak.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rrihfwwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pglglrhl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2trqfsqnr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2uyyxepqs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lequqyoe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2cycaljjl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lyhjgzti.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vnjhkgcr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vqhwmvyu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tydhsyvu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kzlhhicd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbxyjohd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2adxzduon.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2oajvnuos.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wqpwyrtu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2limicwjj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ytylacma.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gcgpcada.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fqceavwy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2sblszrrk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ryhxkhpw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hgbaolyf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lkphnrzp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zlkyjvtb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ensnpqce.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eekxtqrq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2dnsxxptu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iqpiabhg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jsoxzmxz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jaucsncn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tmuevyds.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gdjcbgzx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ahmzgqbk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kkagoews.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ybaveqnn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uqjopais.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2pueemyyx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ophtwecv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cakflzcl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cyfxlkns.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2toxjrvom.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcbkkucp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2loozxoaz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hzcialdj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ucrlkyyl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfjcbpux.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnwiybgo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mryyrgvf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hofqocgu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fhdcbfxi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nozhwcox.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cisdjrlw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tovpyzos.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klbatodx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvaveclh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2azkpgmoj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2xjovyijz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qyykkfay.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2unhhswnt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2easbcyzv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2padsrwuu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2zwahujkn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rdsqxlww.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kftujkdo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2iptatvzb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ouaqjuka.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wfemhdbp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xutvdwjp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2awaruyfy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cukyjyaf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ycxxqtum.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ivqqwlas.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2lbmvdlqx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zdlhdnak.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pflvouyf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwlgllqz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vpadamsk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zcdqoqrr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zcuxenma.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xglfxlqu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cpcggyun.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dioezefl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hwiduvfr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2zuqbicwo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gzdbbkms.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2odxtadmk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2olqgpvaf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azphzgjs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2gtzjwjbn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2euegkpts.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujynwgxl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lcpfptcz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2hnqibtht.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jtmehrug.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kebeuavc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvjbqrvp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ykehzrij.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2irimkagm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2llpxcgiq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tjgtmqkn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2aibyfvnk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2psfrbnzc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2dumeimbt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2kpqjnlbl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2egavopon.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2eekgnkvm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ponawsle.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2fxuavyko.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sbolgpex.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zdmetqpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zginuzig.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2euamavff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pntjhupk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zpmvtphz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ghnsuwvj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zfrxwavn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2puxpteda.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2liiiqtqw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvdtswvr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bynezrho.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2oqxxcqnz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwmvdqdy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2fuslqtue.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2btxkpkny.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzrjqobc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vnaglhpl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ismotqql.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2snbnjirw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bmvksehs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2gxtvbpad.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vvzjhulf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kbwydeqi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2suyehfdi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cgsiqfbe.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qerefhfy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gvceuftj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2iisvlgke.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dwwtgkcy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cgbhacpy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vowepims.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vhkqeten.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jjnnhysu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ztotcinz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2drsvphwp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2verivofp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzrysieq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vfgyxxqg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2oruqifta.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rrjmznrl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2apbuhfvs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wvpvaapr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlpojyke.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xceipupj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dvzeptnk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2etqsnmdh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nfhjkzch.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eajtlbhc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrodlnek.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rszfzvpb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tlmzrlfb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxgtzesd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dxoggmim.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gckuohhj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcxcgmqv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nsqnbqpa.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rdhfzkpq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2wspcdlah.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2awtdeczi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xqeohbgj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2itpkwlfg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mzaxjvuf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lvuhxayr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dfyfcjjd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gqczhpsv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tvbnjein.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bcfjjzuk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2cgcdctvg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2wcvzjehu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2thgozntk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qiyzqktw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngdzbhlu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qntbtbvg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2bitdzpyk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2esamhmap.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifyzwihi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ztgjtxmp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2rdrhgdes.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zdpxcgbo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2sdwgcxzv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ztpcdlwq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mkchhppz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rarlwpwh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ruryuvxs.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uejkcgjz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xtxdqouf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hiphnfwt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kqmpgdvo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2jjmtuckg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iimsabzd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2yaowydlk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jqxcbghh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qzsxynsn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mgamysro.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2avadkkug.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zfozgptn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cgmvtusk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qnethkjz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bisiudoj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgikdybc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2flyyblgt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uuchbnwh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2myautrec.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2onqpmrvf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pdhrxajg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pkowkfna.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umvobbfv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wimqcmrs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vxccrixp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zfyvgcid.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gkdfbfgs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lauvepld.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2qogjuzfz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2azdfcpjw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2spkpydle.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tndaavfn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wamakkwk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2neoeaeqj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2fkeztlmn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tkrsdnka.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ajuktfip.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fevuyxta.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2zwqtifhb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2kjwuxjae.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qyppnvgn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2xalfgnpy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2znkxpozk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2squkdnzw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fbothdxk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2eyfhqexd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oquqdmuz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ldfhjbmg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dymtozai.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2yrhxwwoy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lzwcagea.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2atnhciuw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yeqhsyxm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zeboemvo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yvvnvepc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2siazycaa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2yihhrqrj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qftjaffi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bqxftmox.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kyappbrp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2kqohocrv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kbgjzzhd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2vpvigesp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jitvnsnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzksoahd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dgmyawsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frfeclvg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2vkqrtdoi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gkiwxszh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2lckncgez.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bufbfolo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eixmeicg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2udbludxe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2igpjzxuv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2anzabfgt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jogpbeul.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hwrwuwpb.html


<!-- 参考信息 -->