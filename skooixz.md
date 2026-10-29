代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gmhmmjfnn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gufuhsbos.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/glntbdjke.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gtfckrlzc.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gvsksmbiw.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/ghqiehytr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gajbeinsm.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gdxgzrqqz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gsqtjfhvh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gihzkhlyl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gmelhwoon.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gcgzwegic.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gwdcjzwdq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gouxhwanp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ghskasmdq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gizvbjhhu.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gorusxqfx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gyyjcurbd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gkdxvtqfp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gpbrfcvld.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gydbdizvv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gkbezorix.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gujjarfyu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gnmhwbfap.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gjxyxfumb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggtdpoofn.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gljbtvzqd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwyqcopbk.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gtyjtvidp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gfasqpbol.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbrgohbou.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gjznumbfx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/geibabukw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gceqysqcm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gzoofuaqz.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmhzoricq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/guvyyfxfp.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gjlexfyge.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/guggrgpzf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gtaiuvfzs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gmjztczhi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gaxrwigio.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gqqjgmtws.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gnxwkwpnv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gtheshrgn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gshuiwhtu.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gtqsywnyu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gfkiqpqdd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gmvimdnka.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/grktyikum.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gjpmlprze.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gztbuokcl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gtucyglvs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gqenmrphk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gmqpzrher.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gworzkwop.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gnxudgkng.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gjkzdhgti.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gmreddtbh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gjrlakvrf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/guueaoqfz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gzaknpeig.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gyczsxcpw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gnxlmghex.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/grpbctyow.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/glmrlpbsn.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gwdhybjmj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbansvtkm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gosktjxel.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/glqholipz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gqztyuuaj.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvsubiadc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtbkisykm.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmpbygwft.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnorqvgjg.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gxfexilwy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtdbgkbgf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gaabltlus.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gvqwezpbj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/goouqcpml.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghwlwkrqs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzryzfpte.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gxjvdeiky.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gaskkhxrz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gyzdwjecn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gutrvuglg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gewtxqorb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gntpupgtu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/glvmryfkw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/getmgehup.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gfthecgym.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gwvvladdh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gsoudokyf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gengygcao.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gvhcfbjxs.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gihilbfsk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gkrtovlrq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gydmzhrrd.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gjjxbpzap.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gijworocu.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gkunnwnjk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdgdlscjp.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gpgsdwclb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gtvrqzjoa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gpdxwrayg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gdzfvubff.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/ggukfujnh.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gophmpgpp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/geibejbcy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/guffwchuo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghgrpzzqa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzqqigiiu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glhuiebwm.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkhfsmjsg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gocpuoeyk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqpmocngc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtsnxpimy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gaigptlaj.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gfsehbaqj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmxhdrtvy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gkbccxfbu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gjzveepis.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gkvprflkv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gtzhnlibj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gkbjsjexb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/glisubelc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gnmlxgqge.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gecxeezwa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gtavtusip.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gkgqrqsnb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gjtsnbelf.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gmsoxgfhv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gjhfebopb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gkanfgyfe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gezolooln.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/glnkrtven.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfixgxiep.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gbqgahkzt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzwvjfgwr.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gpaebzgqd.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gmczsumcv.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/ggcihwkez.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gvfxivbfj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gyhwowxri.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwphyebyu.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gwlnehxns.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gyqpgrdfe.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gluphgrzg.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/girotkqld.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/grxnuoqmd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gaimehiph.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gshtaxkso.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gwelfowar.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gotzsgjff.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/grllqnmcg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/ginrceroa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/grbmfylly.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gaqhrqvrv.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gexcmjcev.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gohhpvnfq.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gnsreqprt.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/giipgpdzg.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/guhekvpfv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gckmeyqio.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gdarumxst.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gafosjkwi.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/goabzmzdr.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gtyzddmul.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/goveszalw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gzfylgmvj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsrpruoar.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gvmsdnaal.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/grbvwrjob.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/glocooora.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/glugqivio.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gpjehtigu.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gfwqdhjqg.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gedvqfuns.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gcoxondmr.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gfevmzpmp.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gdfhauzlb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/ghtwdtvha.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gsqngtejj.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gkqacygcq.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gqhiqtacm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/guprnrhbd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gqvsdcluo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghhgxrcxg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gghvirfij.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gaulkvfvu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gxfqauadf.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gdxekvdxw.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gyzngsgyh.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gkmorkjwy.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gewwqjewh.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/ggmadirvy.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gaoizihqd.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gbqtfiebw.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gubqzdgjk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/grbpillab.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gnqxzhnmm.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gkzebwtze.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gztuzfgex.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/grmhdgjat.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gemeqbjye.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gezuzbkng.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gsdbzymep.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gganemzgv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gnwxylhkq.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gtzrvgrrl.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gfiznyghy.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gxznulrbv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/glfpmqpnj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gnhfzpxbt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gcanseoxr.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gxmgbcaby.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/grrikqwel.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gmylodkef.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gxnkzcrri.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gcyxlwnka.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gtowhpzua.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gtwgrhagm.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/grrbvfqpq.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gasnwxlfy.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/ggcshqdht.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gccaycbyx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gxepoipuc.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gnbubivii.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gakmnvpfy.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/glrhqcvzz.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gjdseqqmj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/geuqorfzk.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/glhfleftu.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gwosmcqus.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/geuktrlta.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gvuvmzoit.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/getfsvbec.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gkinqbact.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/ggmnvarld.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gakezwdmq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnicjaffx.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ggprfqcjl.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/glcyaysfx.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gocakarzd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gmetyivlp.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gqpsjtaug.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gurymxoem.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/guwkcemec.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gbnozcxvp.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gdymchdvj.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gukicesof.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/glpxpdkvq.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gggadujbx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/glkxudnuq.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gfbduadzr.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gdlgebxsf.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/ghhcaakpi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gdkxsxhwm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gmplssdrp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/ggsqizpos.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gporlrmxn.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gdcotyiqz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gnwpccnli.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gjhoxehqs.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gxlnqwhns.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gqvthosdq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/girpybwiq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkwsmkiku.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gkmfpotfr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gkzmsbbcc.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/ghpupjdim.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gtrogwfgy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gumzebfsq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gryitcfzf.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gtfxnhuyh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/glcbcnhfp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/grxzbfobi.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gxbxjqrnv.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/ggxqxetja.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gymaxmltj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gxfusceqm.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gtoqkfucs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gxznzhfnh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqpfidyrw.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/glydhscov.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guxzzrlgh.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gwkxxqfam.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gtrlxiryq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gabvblnna.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gtasodfjg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gysqibhzn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gfubmrksx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gaydwtrrk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gslbgmswo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/glohrrrfr.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gpjnwdqhx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/ggwjutckq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gtogoxhzm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwzvaghnb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gyymfgsgk.sHtML


<!-- 参考信息 -->