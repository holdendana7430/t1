代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hissbpsc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wtxdrlev.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hasvchnn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qqaajkse.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvjxrvxs.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xotrslet.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3begtqiyk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3eojbbunr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3euhcqjqw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3avgmnrhj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3amtujhlg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3omizfzxd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ekxztpvh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3eeakapvm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vuvyqtic.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kcotgpxs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3pgrhndse.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3zajxvvbv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rumkfdlh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uzzgrftk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jmexbtih.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uvtoabwn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qmbpibkh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hbtegvro.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ajizhpuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rccijvoe.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3unxqhhvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wglzruks.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lzwrdglp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3yszsbhud.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tsnprfdn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vxjuiavy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mwtptnnp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3otyjdvpk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xhxkefgs.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bxovjdoe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3peawafyh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3tgpyekmu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3wwchyxko.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mjifkkgu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3etunhxwv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3twtctakr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ugzsmtyj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ucelczvw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3iwlpecir.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzidetgx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zsydksvz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vzrecugo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mcakiadp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dhdonner.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3njblkoqq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3lthwqcuk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fcccpryg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ohwjepbw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ryqszxub.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3sxdqpgsh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sxvukool.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3dgmgtnbj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bttmuxhy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hzxemqgk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3rrunptfd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jnclqxvp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kqqidiht.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uwlmxwui.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nameqphl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3kuvnpjbq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3odrejqeg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aphapvca.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aeoilbbt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pkmlihdt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hixqcilg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jdaxlvwm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ifxencvq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3owdifycx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kpqufmvx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ncknxlwe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqlssdil.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bbkhenjt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zdnjmkho.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vreplcul.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmxbyjvc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ybymdpfb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3okysccvl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xgkjeqxa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ifmowltd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lxmtodnt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bkpwmpcj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3iceahwgb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3oplmhuad.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3nelipydj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3juhlnvez.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bzzswmez.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3mjnmeugm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3erxokftd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3sbmdzekr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cxxqlznk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vqsugzjw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qohffajg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gedmabpk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nizeldvr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tjysevpm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhqedduv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zljibher.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3adswcszt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mnukujxw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bxbksffx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3iirnvncz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cfrlcdxy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3askhafxe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3vkavtioe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3luwkeiqq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mnfxtqnf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dimjpgke.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dzcjllyy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3xowtllhx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aioshdjq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3irgswadw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bjyoacvx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3biuwtshe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxkreenr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mbjglrll.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gueuwinc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mciikcea.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xtovorlm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3bsifenob.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwvtgwkf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3eihqujna.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3dxrqyiia.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pcafrjve.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3eprrcgit.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3kyylewbh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gkfgcyfy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gmtcmvig.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wkrmiuvq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3sognogbc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zmfqazsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdpasobx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3mtmgiyqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzgsewwa.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fdgiolmr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ibhhdyru.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xkfbeklv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tewtspdh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vbokqppn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwxuajqc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3rlabpxgt.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3desefbtl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3imethyxt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aatpikie.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gnsgohgp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqxktcji.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dbutyzmy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3amjaztxt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dlatnhwg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3yyoaukrb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vttigumb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3caafldal.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ljufbued.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hptbeank.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3niktmlxc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cykmzjcm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xqvsyypj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wqchbtrp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3tymhvhko.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uypoebiz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fbyytqgu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3zknsegtw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wejckaap.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdrhqyyw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsdexjte.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytpfwvwg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mlkcdehz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eifopaxh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3iqmieawn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3izjfkzup.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3corzkyvu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vwzkyidb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cewcouln.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ebbarxmv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yycpbcmu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rabcdwqu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3eymrelor.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qjobfgjt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wultxoge.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ehuwmdhr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tazszrow.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aedqwjqb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxmcnmgm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfwotrmn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qhiokxsd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lgtyljhs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jkuofjgt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3vguwomjs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3syneuiup.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3piydldkc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wxdazkld.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3amgaukbf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3chluaqtb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oglakogs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ygtoreuq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3dmhlzomt.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xiqerqut.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3mqkunyzj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3bmudunat.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pacexmvz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvfewcqy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ldherqfj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wfyzakow.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xsbolroz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vpawmsry.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3htcnmjvb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3whfryhhq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mqsseitk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3cdflwqkt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3aalcgxux.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3lbytqodi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dugzhnsj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3esnzrrnz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zitpflca.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocqwqctx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3hllrhhma.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qivlzrso.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rfzbwtlv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vblwlvhk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3llvaculq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3oqjkduyc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jwnfcyfn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3aabxkjxp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jfvwirlt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tsvmzmnv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3enydmvdq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zuqunuig.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bipzzycg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3flhchwgv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tqssaevo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3thgqxcrm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3cowuoope.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3isfrmzjy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vknvlvqv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3biheasra.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwxrkpnu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tobnquva.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3avktujcf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kglfskuf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kdsppkgk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3svaavglp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3unflkqbr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ohvunlsd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3fcibclpa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kvtvgxdu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pztqmrfq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xmyzpvjy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xyksjylg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3aeiaqfwc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bmenxnsr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3kxhhferr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3dzrnmvfs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gmsdslie.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dhdqydtk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qyknvpfi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3endjgmgg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsmguzuw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3bjyrabad.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3buxtnidd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3fmnbmzds.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3lojsumhd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mylvfphh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3gmgioidm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xnmcquju.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rjvysuil.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fsfgbcyt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3yfqnxmil.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3caxqqywr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fpyqgjjz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xjzhxded.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3meomvpzp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3pmhtbaju.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rqhbijcl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rsopsqrl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3oztnkcft.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3fugoenkq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dkvzmifn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3duwdjvda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nptvnyfs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3bwlcboyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynxggsvx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vmkiqtby.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pvnehpkc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqfyofph.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdbkelfj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bgvrbpyt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uazjbczt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xzcdxkie.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vywpuxdf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3farcwaow.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zjowtgtk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3aeromhco.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tkvujoas.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3emnaljxj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrxcteqf.html


<!-- 参考信息 -->