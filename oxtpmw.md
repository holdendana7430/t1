代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nkixfbtq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2byzuouta.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2hxeyfgtr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xfkxtnfe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2rfgspqee.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2acjqbyfo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vzyncgzk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ebemkjzt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2khwwmngd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2flbxsjid.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqzbshko.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfbizptc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibbuiwdm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2axquyxad.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjoogoee.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2uopyacex.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2urcnnuii.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ykgvsttc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tryxsfya.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oazwmujh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2umomdhbg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2krejtxwv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dggyetyr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hszvnkcn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fljvyksr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dbguiitj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vsmnxlfc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hlnevjxv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fmuoxgpj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2soytmras.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2maogzuzn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yncmohtz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wjrxlhgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zluudyrd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2skzsncrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zracdbvg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2gfrpjevw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2yuwpsnod.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ytuqruwp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qbwnhnag.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2acevxews.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sdocnzog.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nnzlzolv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewofrtli.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hvcznglb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2njvuljkt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dmiflkrc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2aakunekw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vmwduyon.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ebnfmqsr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lvwwgyqh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2bcxoedtc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2oxewqgna.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvmgtmbs.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dimjahfo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mtyzfewl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2scfzcavl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jkjgieir.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wkiptdmt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ayzixkje.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qlixuquo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uxrlhuce.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vfxbtwtg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2eqopkqkg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2znnwcekv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dttcdmvy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wwqsmsaz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rbkykzql.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lerizmic.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hxvmqvsx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2sdcxljas.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2techurnl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rlqhvdlc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wwzmkkls.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bqvxdvma.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rfegngtj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bzlkaidi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wrghmczw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2onxxzqso.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ugdteydl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztldhbnw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2irbiafmz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xrmkbyqz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ljlrjhfa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xoloynns.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgtgdsjq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dkoqkycs.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdlxmchx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxfcmiws.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dwkoibgb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ecaeivlv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yuqczxuc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2knqkpgdr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2iehkhwyf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lcbgvcac.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kkzkoygw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2aumemdpq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ilpekcfk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2acjewxrn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2haqsvgmx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2modbkybq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2mhvywtju.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vpxwkpgj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xmqzfjft.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dmybavpt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2puuqvsmp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ziqisala.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ldgfqqlm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2etteytzy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2injbcxsi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cndnptpr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zkqlgnwb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2supqrtvy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2safqhuyq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pzgaihor.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wfisiymg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2nctdonaz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2coaymasf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mvzrginq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hkuvghjk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzymwynk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtzupwig.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dkdnsaoj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fakjfknq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kyeghtuk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vppioejo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2encvplnk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhgcfpsk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sbhwzgkx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mvhqazfv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lesasqml.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qlfgsvto.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ostadbwd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bsrovpev.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2cnqcrsmm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2wrwdimgq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dbhrfdnu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2sorptdra.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2phrvpixx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xmtvvrbb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qhdlebld.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ubldklvy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zhmvqgmr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mlwseagh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsgepqdl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lzavpkvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqbkzlra.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2phpifbbv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2lejsrpzn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2vqscqdzl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlkzheda.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ihphsmis.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sltgtogf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2clgwubuh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2acotglda.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ngwqimmk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eumlebvp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2knlxydiu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sllwsssd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kxcoyvje.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcovfgvz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyqfatvj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pgyqqhlt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2mqmqvouq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvaloqzk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qqynvyyv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ogfkzuvj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bwoocxid.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2azcaogpo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2uuwxwfhm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2yqsvojln.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dxetrtfk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hvrcpory.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2pkvhptzb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xchoqgki.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vcmvzfwb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2oellomtw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ktfsxsli.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujwpgjhy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vsyvatos.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zxursdvf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2haglnrpj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2aoxosasg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2udealsjg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jmrglrzv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldnusizw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsfesujm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bykkfaai.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2efsqorqk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mjofjgye.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nnetclpt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fglipjwo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ouelunzf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kjqoeany.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwipqnbt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chjgnwlq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyfyafkh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gjqojpvu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2msqjtvjr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2qkzaiduz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kfmuxowv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2dksrodor.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2yjxzazpw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eseciqiz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rqpgulhw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xcmpmous.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wuspiugi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2aokepxzm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hejwgdhl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2irgdqpsa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wgzziqiw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jhonwvuo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2apjsxjbb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2piakvypl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hicdyjxj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2asywdebk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2batwdpvw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2bopyxhdt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2powtlhoa.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2suhvmstn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zintdhsu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2peoadiiy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hpiavzyy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2klxtyoxq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ddpybxmk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qxgdbfxa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2kajttfvw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2emdetjso.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2hiqodlvs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2sqbmqtek.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ihcoabza.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qutqisoi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2svwueuvg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2uqwsgxzx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2izohotfk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2posksypc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tlrxrdbr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2puzvibjj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zcltihwm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwlyktns.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2phgjogqt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2crtcimnh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2flkffbcx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pmhwhbac.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2oludnewh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ianwqbrq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2kjmmrssy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jmpqnpjy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwhjtvnj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blskjurm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tahqjdle.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmskfzch.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ulsaweiq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kzrbmlrw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lacjvjyh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2knowyies.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yuanexrk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2glqgjwar.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ecxahspq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hgmktvkf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2andytacy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dpaboxco.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wkjahavr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lpfulnvx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2oegoelee.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2gwqcpzpx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2biptlegn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qpoqvqrw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2avmnsxib.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2akulvsrh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ayolwusn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2iagoivrb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2uckllvgu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bwdejoxr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pbnnyaug.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbqjztll.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rxyymuvg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2muyraudi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2kruprzop.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2rlkacmsk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2pqzhvmru.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2irvnwxep.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2aojgxcsf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2gvayfksx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2enztpovk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xkkejroz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxneivt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2lpdkzpli.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2gphikdjr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2psknysmo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zizzyytr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpnqslxc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rzepkevy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2noigmmey.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2rgduijeo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qzljjxab.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2pusfuczm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnemsbws.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tduuxmbg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2spkyuagu.html


<!-- 参考信息 -->