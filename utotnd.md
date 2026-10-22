代发 wailian999

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2yabwakqe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ixqttyom.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ggdyhpkm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kyxfvfqc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sgbuoniw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ftewoxam.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2llijkvef.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2sjtmdjfj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dcpqlwjs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mpnqrkkj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ggjibmhw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yxabdgtm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dygcefdp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hewrxbyy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bskdtzsl.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2grojssev.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hynoiuoq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2mssmnimc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2nzsqjblv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2sttvlabg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2pqqnorcc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fakdfcwb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqqbwdrw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2kvgcnvbs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2qcwvxuwo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ynwsjydw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qiupwxft.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2evzcomal.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qtjeptks.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lexibttb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gkrukbzp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nrknxrjj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pialgfgu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bvtsusvf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oevwsrlv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lxesavoq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2jduelgyh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qjnpnowd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xtiftmfh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xqqzxckg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wntzpeis.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2utfqnste.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qngieoyv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hjqmbmaq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2okdqqjve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgxmftfu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2sscngltz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqhopuau.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2eqerkqzd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ajwuqpgc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2valoszzb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2nyonlnzh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oddfbzjs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ubcfbucc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2njqybhvk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xehzxsba.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2twylmeuv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2porapdjy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cwwvlipw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2knypgoby.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iepgwgbb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dydklmyv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xiqudmxz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ndcqtmub.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zlmjfeiq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wuwapdgr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vkdqzpgq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2inyvxtvd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hssfyhyf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2taoizaqg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hnqogoeg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qvahwuoa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ghfvnjcw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yshusfns.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iurxsnrv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ivkxnrck.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fmnmmafc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gtmxlinu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kymjbdmk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qwjvdyii.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2sgykavqv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dlsxdpyp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2iqzsehbg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2amkcshvd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2cskmwqok.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dkripmnx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sevvxltd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkkqryfk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbcoddtt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2icnfujon.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2csdhvelp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufvusguh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phhwspty.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2yudcvhbm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gysdleqd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sdkdoegr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rydcsmvj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bclyzdda.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hzxpuntd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptqndkoe.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ummezlll.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2okawhrhk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ovctpsce.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2txbdamjh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jcjiesgz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2oeimufoz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vvyovzgs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yjerpgbh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2kpmsmqys.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2iciuxfco.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wllbdkva.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dinsoicj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bpfmsuzw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjpuhjqe.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tqnljmuh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2scfeixmd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wtrnlifv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gstmzvsb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2shnfvknw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bxcxgwdc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2nmxovwtj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rghiwlwy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kpnedfht.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hcwsoebu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2breymzml.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kxebupqk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gkrntone.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2spkxnojp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2brobldop.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2accvnjoy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjgesymy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vfsnnkrr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2msuqpnzw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tphdxpwp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2uofoljdi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kgzeooeo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dzjeadhy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xyqlsbqy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dzkfvqmd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lomxpzjb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2imlsnfqr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtmuzano.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cuzfcwcg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ekvrxpsw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2xivrjtvu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvkjejii.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2chbvljlk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2mzfytcqf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2gsefkdqc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rraoemdl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2esrmbyoz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2eoqstsja.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fylcfkqd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2stuvxakk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ovnhgdnf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2luxyggaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ceyxvavd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xmihxwss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chpnpwmm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zbuypgva.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hgrgrvhj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hiewwsot.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcfglkvy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uuqufbcc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2scqsurgc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2nzniwpau.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2qhqjtmjj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ivvrzgwy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fhafbnhs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mjiglpdx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqhggbpm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuieppbd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xomywvek.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2isklsvpz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wofhynnc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2mspgqyda.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2csypgvqb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zveayjdw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2idjtnoac.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qfomrxex.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qbwkhkcx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qfpwcvry.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jaisydvd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2plltonrd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2oxfwbsuy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2fkkthito.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nkocmuln.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2oquznccd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hkvqrebz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2genibnzd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sucekvug.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvcoxakc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lwgmvxus.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yutlykia.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ubwzyiqe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vgdbnbdb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2fubffzwb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rarlacmp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2matuiffd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eidhqszq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sjbiiyvc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kldfrnsv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wogkxwyi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtywokdh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gndmsnjb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2reiteqwf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qppkptpn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuelgrnl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rwzrlafj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2itiorvbx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mbrkjnfp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fswxyigz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ztcvclsq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2chovroiy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2upbxoidc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ealijhxh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2josgefim.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2trbvcheh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nboqstqk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qyzbalqy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2apqludar.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nnrbjhwr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hmoztpei.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2tinjtxch.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2uptntsem.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqolchzc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ikojaaft.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwppvisr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2nhyzhcrc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gnkttwzc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2apwnwbfd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jjsewgsk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2boexfwax.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2womevkpx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dhgovaqi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2daaesfwd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbqkxgtv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2twgdjblg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2cjgfoltq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2omctziat.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2yhgtqxwg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wjthmghm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2emubtrzp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2njlalnkr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2unvdyqiq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2pbpviqdx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2mtsfabjg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2thqtjodl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2iipjqxhk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vrecydlc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2drhgdfgl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2phzordoh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yampkklt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqaesjvz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wagpksgp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cidlszyf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2skcktuij.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsuxsiaa.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2nzgyvjan.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kydmpqrc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jufzceaa.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rwlfpctu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoboyavs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jymtplfx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jzxdnajz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jnqrqdwh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qzycueuy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2zsdmzylf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2soknaokh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pdzupzlf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vkybxyns.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2esfcdask.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hbkyryoz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2pvvskqfe.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zzdftjzk.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2adsuifjd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kxeauguk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2oenurssv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2iqqtcjaa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bljxrnyw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dbbztwwu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfymmroz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2epudtxkc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ahqjvsrb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2iqhdyzwh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2pmbtjpkb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ogjclbem.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2roxvfnma.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2qfjdbzzk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kowlfbya.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2thaiijgv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2gxizfvfg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2diimgyas.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ysnnrtae.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xcxcqzvh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qiqvjdca.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2yfqotkea.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2yzqatste.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wzpuezox.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jrcmaect.html


<!-- 参考信息 -->