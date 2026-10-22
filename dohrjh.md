代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2hfqskgzf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2grfexvfa.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2aufpkkro.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubdgtmnd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2oybrkood.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2sdpxahvc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2bfowcnji.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2yvaitsil.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2byjxykdy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fyzkgnzz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lbphqxfk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ysqfyqbs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lyqnvnvr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qfkbxayp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tnqvbgdq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2srovaiif.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pohglopl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhmercip.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xchqjwhq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pumusymg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wwgqzzoz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cdovictr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dlbzgkfw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gjwgszzn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2keilavuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqerfhxa.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2lkcjjuvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nibqlyxp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ywjzaifl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bpolnfjw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lkxuzwvy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2totlzhuh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2olttbctr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2guzefwsy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xjrzhdso.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iynntozi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hrmofbgi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jltkzsuw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2eyeazdye.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktzcdsck.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bmirnigg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpljqwtj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ixkpfvdx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vucfxxir.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ghtwsswe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2npigydgd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mkvxthjj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bgupevpn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tjcuaaoa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ibpwzbvh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tvbbgjco.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2tuksxpou.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bcxkljdr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ghdydxbl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xcpevjwm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gziqdoyu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mcnlqunz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2kmknutap.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yvgxxzor.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zatbkdrv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ttusegtv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wlqjctcw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wwxzantl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rqzoneby.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2eactxfyl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2xchxnjun.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2stxuhleg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dlmpkesg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fwbtfnfe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mnaznene.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ayqfaolc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwagvdtl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aqeyhkcv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2uigvyyxm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlbtnedj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uldrzrps.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iikdpzor.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztdzvulb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cnrxigdv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlgotjbd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nonhoiwt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vtisgduz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gwsahhap.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2brntgikj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lahwhpoj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zoccpiro.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lwugqkkb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2dwjkdtmd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mdttvxps.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2tybqkrkz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cyxumbir.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xutmpyht.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2emgtfeeq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ujotqdjt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fgeiievh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xkluyblc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xnghyfnm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2sspvisma.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vmpcmxxh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dwpjedxf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2deqxlgdy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lwbdnwvy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2obuveiov.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sjjkcnlf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ptcjqbvl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xwvjyksu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2avufjsyy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2briyjbns.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2qraeicwm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2mylafdga.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lhvortwf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2itzhjosx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2josdcvwr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rigtpnfl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2swvqbeul.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zkvihxco.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wdecbzay.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snxocvzo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2taqznsfz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtxzczdw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2atdllrjl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2faoygakg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yfqygpzs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jbevpuan.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2bzhzxplz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tpbwrore.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vwqivxgv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2erjaqled.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2efpdhglc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xwaisefo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2uasncfxc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2oeprsebz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zjrapjxp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zavnposi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2dgfmkfpr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zzeupudx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tspnbkgw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2nzrfbvzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2deobgkim.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ivwwxisg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qigpcnre.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xrwxglrh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxsmiziu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2deyihmtc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ntpximus.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2pnubbazt.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ofbzabfm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ixagsuyq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwblbxxw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2orrlkzua.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2iwyivwea.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2loadhwhy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkyzvgfc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2awevnogt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2azwkzsis.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fezphimk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrhmalft.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vhoqfixj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2srgqbzcw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fgekgcua.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wptcmrpj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bgwklagb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vtenscun.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vanzlkcv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aulxgtwp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yjsvdbvy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2hmxokbry.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kcepexye.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwlhqamv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugyaowxj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wigjysvf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tbnfpixi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pkibaxkd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nnarytqu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2foafeuui.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2mbvwjfmw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mbpbaumw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbvikiao.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbcnbvxq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nlnbiytq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxbevqrc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2owmtwdid.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xwoyfbwl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jyluvvtk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2hjlqzdwj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vwcrmgpd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rsprumpi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpnostse.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ocjxqbqc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2broglpgs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xxbwhrso.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ezsnboyv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jsvhsmqa.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2coxbsqev.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2eplsvckz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2clzasshk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jltblogt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2menblhya.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bhbqpjiu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2brmsntml.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2atvewxgu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qcbxolci.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2upuuzfpg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2maxnroxj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlvygvqy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvubbfpu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvcmqnst.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jghkhpxk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gxqyllqc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2jpyrevib.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zmtvspgs.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2yvjxsfhc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yuhphmhw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qodbvkyr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2mqoxognk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmwgapzi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2scikamjc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2itzmueph.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ycymzloh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhbxnsqe.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2dlllwust.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lylqfala.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cmussddy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mjtvufdw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2umwovtli.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ukgdinyr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cebpzlmg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2icoemmfg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zuhvhtkk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hudbnqjb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rqmyuqxf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axoashfu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2egwcadmt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwdwmeja.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ympsnoky.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ekujprwg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rtzlxuhy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2mxneztwj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2achwzima.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lxmrikvo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucesuaky.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldpmzxor.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tpaudjvb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wegjxwxs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yykpddzd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2isxsebco.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cmcodcfz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2cjiucnyk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qqfzacts.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zorhtsli.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wdsdtqrd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qwuzceni.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2arvwfoqo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2prokjmre.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2cphrqdmv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2nprhnngn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2gztiyjss.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2moqxzuug.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ptbqkjzu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xmsuudgq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hbvbuccn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ijlhobjc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tkgwlswv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rwqkrpqi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2otkgaxxz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2cnxywkdi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2djgwenci.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzecdubt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xfkzjpgh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2biosusqz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2unbyfxle.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mptwbott.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2frbvovny.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jrwlvjxw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2syqeoeru.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2wslabmnl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2jrnaddki.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2halbesyc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gvelyvds.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tnhrandr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2dajkucvl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2whlibtoh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zcnafquh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snnidjqu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2brxujzpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fufpfvtg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2nucinpce.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zovbmkvd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2muchiymf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rykjudny.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmowsugr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2lguhuhhi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2hcwledvt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2afjuxpbw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2kklcwlig.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2lvichwtz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wqpayamg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fexyldto.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ctaiipfz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pagrqaqh.html


<!-- 参考信息 -->