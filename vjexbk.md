代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gturvfellq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.9152youxi.cn/gtbwqjjkqm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.52xcode.cn/gtwksabdpd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhijiandao.cn/gtniwzwnnl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gotoacloud.top/gtmbzuoeud.html

[E19] 多行文本按行拆分
来源：http://hz.kuanghao11.cn/gtorxvdgbo.html

Py:   s.splitlines()
来源：http://hz.52xcode.cn/gtfdqvsxbx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yvedp.cn/gtfyepcyrr.html

JS:   s.split(/\r?\n/)
来源：http://hz.gaohongyu789.top/gtgxywqgje.html

TS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gtyadxfaek.html

Java: s.lines().toList()
来源：http://hz.daxiang520.top/gtvvstulyo.html

Go:   strings.Split(s, "\n")
来源：http://hz.xziqi.cn/gtdrdtwxaw.html

Ruby: s.lines
来源：http://hz.jqgfzy.top/gtkxmxlvsv.html

C#:   s.Split('\n')
来源：http://hz.wangdashe.top/gtjhswuypc.html

[E20] 判断字符串是否为空
来源：http://hz.hywenlv.cn/gtncfsraog.html

Py:   if not s:
来源：http://hz.c1oappe.top/gtrmwjxxxv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.vqdsnc.cn/gtukeuazxj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.haohaochexian.top/gtsgiwxuto.html

TS:   if (s === "") {}
来源：http://hz.ybcxt.top/gtbngzfmmd.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenzaomai.com/gtjsquqafe.html

Go:   if s == "" {}
来源：http://hz.svipenyu.cn/gtdngjcour.html

Ruby: if s.empty?
来源：http://hz.jiagoushi.top/gtgxcxgoep.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.birdmap.top/gtovumzpvo.html

[E21] 超长截断加省略号
来源：http://hz.cdnleiting.top/gtyczmbeak.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ivvv.top/gtvebkiabh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.bjfxy.top/gtqwdnlefm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtsbvbdzkq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtnldxlqzd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtaconpplk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jlsjyb.cn/gteutgsnkt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tian-w.cn/gtqtodpjrw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ehwqpu.com/gtldkrixlj.html

[E22] 字节长度与字符长度
来源：http://hz.smart0.xyz/gtgzicsjip.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zycfv.cn/gtpyqsjkna.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtzidtsgmk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtwoncampl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.feifeiyinyue.top/gtciamobmo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.pengpengdd.cyou/gtxkwbtikx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigufen.top/gtymlunjrx.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gttmiubosz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xylfe.cn/gtjneezzue.html

================================================================================
来源：http://hz.hywenlv.cn/gtworxayqa.html

F. 文件与目录
来源：http://hz.guannengcc.top/gtyxywlrti.html

================================================================================
来源：http://hz.tanke756.top/gtcrjsxgoi.html

[F01] 读取整个文件
来源：http://hz.sweek.top/gtdzxkeqlt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.0kj1m.cn/gtztmahbxh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zycfv.cn/gtuezzdtjn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.guowangkeji.top/gtfqpasonq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gaohongyu789.top/gtvvmqxveb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtdzvshcie.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cashguo.top/gtmmhriile.html

Ruby: File.read("a.txt")
来源：http://hz.hfpthk.cn/gtlbdkywpa.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.haohaochexian.top/gtwbyjemgc.html

[F02] 逐行读取文件
来源：http://hz.ivvv.top/gtyupisfvz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yuxming.cn/gtbjbjueyw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gtdvomicdi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gttzkxvdys.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.feifeiyinyue.top/gtvjyxtbdc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj202588.top/gtyhcrwkzo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj202588.top/gtdeexqpja.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yanxiufei.cn/gthaxkvimo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sysykeji.top/gtpkmbkgng.html

[F03] 写入文件（覆盖）
来源：http://hz.sweek.top/gtqlkukuxh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhiwuduotai.top/gtabvykwrr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtjlyfevxc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gtnbyowidu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtxbiefomf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinyuanbaomall.cn/gtstzvxnag.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinghuilouyu.cn/gtxntiavhk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtecdkgtgi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.snrcjt.cn/gtlgmartok.html

[F04] 追加写入文件
来源：http://hz.xylfe.cn/gtjeehdoqf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.chenzaomai.com/gtlnjlfpew.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.svipenyu.cn/gtswkouumw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtylnkhwxo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuanzx.com/gttcbtnbea.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yuxming.cn/gtffdimzok.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhengqikj.top/gtrahvjnsf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangdashe.top/gtwwzlzaoq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zycfv.cn/gthhecqonq.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangshuangyany.cn/gtdbfcjjcy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.havefunace.top/gtgtylekeq.html

PHP:  file_exists("a.txt");
来源：http://hz.hammf.cn/gtmccgltgo.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gtclvpgunl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtmwcqjctp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtjrvohugi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xylfe.cn/gtebwabfno.html

Ruby: File.exist?("a.txt")
来源：http://hz.cqqwz.cn/gtkkusbnho.html

C#:   File.Exists("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtydpixsfc.html

[F06] 删除文件
来源：http://hz.jyoumei.cn/gtyvjpuegh.html

Py:   os.remove("a.txt")
来源：http://hz.smart0.xyz/gtmyjsstcs.html

PHP:  unlink("a.txt");
来源：http://hz.yanxiufei.cn/gtzjdlpkqo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuanzx.com/gtcmzcsrrr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cheryme.top/gtfxfrzlch.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gthdjgumlh.html

Go:   os.Remove("a.txt")
来源：http://hz.tian-w.cn/gthzifoudx.html

Ruby: File.delete("a.txt")
来源：http://hz.jianghu66.top/gtdajppwfq.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtsjcvcrjb.html

[F07] 创建目录（含多级）
来源：http://hz.yuxming.cn/gtowwkweah.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ppjwa.cn/gtzukeauzz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yvedp.cn/gtfzgnyced.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtbharitvn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtdpdokdmi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.316326.xyz/gtnpxopwdi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yj20258.top/gtndkdnocf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.havefunace.top/gtjmvwrrgm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gotoacloud.top/gterhdesjg.html

[F08] 遍历目录
来源：http://hz.ivvv.top/gtndeaqpft.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuetiantiany.cn/gtrcjkprtx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pengpengdd.cyou/gtlfsmiemc.html

JS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtvkedkslq.html

TS:   fs.readdirSync("dir")
来源：http://hz.smart0.xyz/gtlylqjsjz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.pengpengdd.cyou/gtlnhfvszl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cucudq.cn/gtmzrqkauq.html

Ruby: Dir.children("dir")
来源：http://hz.jinqigufen.top/gtzdyzqosw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj202588.top/gtvievhbsi.html

[F09] 获取文件大小
来源：http://hz.gotoacloud.top/gtyyzowcvw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.snrcjt.cn/gtdvdspgqi.html

PHP:  filesize("a.txt");
来源：http://hz.nanxuanxn.top/gtmmquqywj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtistnjduk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gogol.net.cn/gtjhwdubqt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtsmksansz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sysykeji.top/gtweyindcl.html

Ruby: File.size("a.txt")
来源：http://hz.chenzaomai.com/gtaeawkgjt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yongpay.top/gtpumgzuqj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.0kj1m.cn/gtdrbscjaw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtrhrksven.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.mhx1999.top/gtbpqjigqr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtcmhyjizg.html

TS:   path.extname("a.txt")
来源：http://hz.xziqi.cn/gtdgdtjxol.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gzhubu.top/gtwhxdcslb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jqgfzy.top/gtxguqegub.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtirsisbfx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.andypj.xyz/gtfhwdmchy.html

[F11] 复制与移动文件
来源：http://hz.52xcode.cn/gtreupetfs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gthkubxawn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.haohaochexian.top/gtdocwviuw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtfmziyvpt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gthlduclbw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xylfe.cn/gtbkvyypsn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gaohongyu789.top/gtdnqkjrly.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtstydwnoc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guannengcc.top/gtfpfysviq.html

[F12] CSV 读写
来源：http://hz.kuanghao11.cn/gtqajpwzqu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xziqi.cn/gtlcajfxvs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangshuangyany.cn/gtigkxmbdt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gaohongyu789.top/gtqoiyozlf.html

TS:   // 同上
来源：http://hz.pengpengdd.cyou/gtrefxzrzs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.daria6918.cn/gtslrltvpz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xuetiantiany.cn/gtsadpypqp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.vqdsnc.cn/gttwddvrfl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sxryk.cn/gtgdtwjlzq.html

================================================================================
来源：http://hz.tian-w.cn/gteboynglx.html

G. 面向对象
来源：http://hz.zhixingplan.top/gtyewdffps.html

================================================================================
来源：http://hz.ppjwa.cn/gtztmdijbu.html

[G01] 定义类
来源：http://hz.jqgfzy.top/gtttnydpdr.html

Py:   class User: pass
来源：http://hz.sxryk.cn/gtoeldftes.html

PHP:  class User {}
来源：http://hz.zhoulong.xyz/gtyyeingey.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtuqpjjrwn.html

TS:   class User { name: string = ""; }
来源：http://hz.svipenyu.cn/gtbwowdjfj.html

Java: class User {}
来源：http://hz.yvedp.cn/gtiywldpgj.html

Go:   type User struct { Name string }
来源：http://hz.zhoulong.xyz/gtjbmkewzg.html

Ruby: class User; end
来源：http://hz.zycfv.cn/gtmvzfvewf.html

C#:   class User {}
来源：http://hz.snrcjt.cn/gtjtetauaf.html

[G02] 构造函数
来源：http://hz.yongpay.top/gtxgbafomq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gotoacloud.top/gtwafyptzz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ybcxt.top/gtmpnqhjdd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj202588.top/gtdksrgvks.html

TS:   constructor(public name: string) {}
来源：http://hz.shanyushiyangkeji.top/gtgsspwidu.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtehxuqbcg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtowbpnxmt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.wangshuangyany.cn/gtecozktgf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.haohaochexian.top/gtdzmcqeix.html

[G03] 实例属性
来源：http://hz.meibo888.top/gtlepvgofe.html

Py:   self.name = "x"
来源：http://hz.gaohongyu789.top/gtuoouexed.html

PHP:  public string $name = "x";
来源：http://hz.chenlongwang.top/gtjxqaujkk.html

JS:   this.name = "x";
来源：http://hz.havefunace.top/gtzhgggjnc.html

TS:   name: string = "x";
来源：http://hz.fzhhl.top/gtlwdazcym.html

Java: private String name;
来源：http://hz.feifeiyinyue.top/gthhurfplt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shzxlz.cn/gttaurqnmh.html

Ruby: @name = "x"
来源：http://hz.xziqi.cn/gtfbbzmvse.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guowangkeji.top/gtfzjmipot.html

[G04] 定义方法
来源：http://hz.yvedp.cn/gtfxsvdjld.html

Py:   def greet(self): return self.name
来源：http://hz.sufxvd.cn/gtqcndpggi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.daria6918.cn/gteqezkjwu.html

JS:   greet() { return this.name; }
来源：http://hz.xuanzx.com/gtsmbvoopm.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gtsilwucvz.html

Java: String greet() { return name; }
来源：http://hz.jianghu66.top/gtkhkttecz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtftnscsuf.html

Ruby: def greet; @name; end
来源：http://hz.tian-w.cn/gtmavgpzev.html

C#:   public string Greet() => Name;
来源：http://hz.yonumen.top/gtsgamavjm.html

[G05] 继承
来源：http://hz.tian-w.cn/gtdsnnnoqp.html

Py:   class Admin(User): pass
来源：http://hz.ppjwa.cn/gtvrdrfmjh.html

PHP:  class Admin extends User {}
来源：http://hz.cheryme.top/gtzttwxwua.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtrtpkrpbi.html

TS:   class Admin extends User {}
来源：http://hz.meibo888.top/gtaxbyqqle.html

Java: class Admin extends User {}
来源：http://hz.yueranfly.top/gtzqhsewqi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sxryk.cn/gtwyzrgcxh.html

Ruby: class Admin < User; end
来源：http://hz.xuanzx.com/gtcagfhwgw.html

C#:   class Admin : User {}
来源：http://hz.yueranfly.top/gtoogbtjgm.html

[G06] 重写方法
来源：http://hz.zhiwuduotai.top/gtcabbmrtp.html

Py:   def greet(self): return "admin"
来源：http://hz.zhongyouzk.top/gtvejnvfyh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtwzggcnqq.html

JS:   greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtsiocnqqo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtyadgtvll.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtbsjlkjcm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dianchejie.cn/gtcrvyjbff.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258888.top/gtbvmbrass.html

C#:   public override string Greet() => "admin";
来源：http://hz.gaohongyu789.top/gtyyzimnra.html

[G07] 调用父类方法
来源：http://hz.bjfxy.top/gtjjjgrwtc.html

Py:   super().greet()
来源：http://hz.tian-w.cn/gtaepwnqpn.html

PHP:  parent::greet();
来源：http://hz.yueranfly.top/gtdchpsuzq.html

JS:   super.greet();
来源：http://hz.fzhhl.top/gtcabsigiy.html

TS:   super.greet();
来源：http://hz.wangdashe.top/gtwqlcwogp.html

Java: super.greet();
来源：http://hz.sufxvd.cn/gtwufwjvna.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hfpthk.cn/gtsbzjusbs.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtoahbckgw.html

C#:   base.Greet();
来源：http://hz.hnqzz.top/gteituqygv.html

[G08] 静态方法与属性
来源：http://hz.xinyue.icu/gtswgudnup.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hammf.cn/gtxdldiuti.html

PHP:  public static function f() {}
来源：http://hz.zhongyouzk.top/gtubduwpms.html

JS:   static f() {}
来源：http://hz.hnqzz.top/gtgtyboaly.html

TS:   static f(): void {}
来源：http://hz.shuidangran.top/gtqxesoetx.html

Java: static void f() {}
来源：http://hz.chenzaomai.com/gtnxaaankh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jlsjyb.cn/gtasxrsfkw.html

Ruby: def self.f; end
来源：http://hz.yvedp.cn/gtxuyzhtnn.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gttumehlau.html

[G09] 接口 / 抽象类
来源：http://hz.zhengqikj.top/gtbwbpdbvh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhijiandao.cn/gtxzyhiums.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtajtvdbbc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigufen.top/gtssvssafo.html

TS:   interface Shape { area(): number; }
来源：http://hz.quarkkingdee.top/gtyflyejiz.html

Java: interface Shape { double area(); }
来源：http://hz.ywan-chungtsiang.top/gtherbhfhx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.guannengcc.top/gtrxrfojsd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sxryk.cn/gtsmbzucpy.html

C#:   interface IShape { double Area(); }
来源：http://hz.52xcode.cn/gtjewlflul.html

[G10] 访问控制
来源：http://hz.9152youxi.cn/gtbjpchokk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.andypj.xyz/gtwnrowgjk.html

PHP:  public / protected / private
来源：http://hz.jinqigfzy.top/gtxycmoylu.html

JS:   #private 字段；其余公开
来源：http://hz.snrcjt.cn/gthbwlupyw.html

TS:   public / protected / private
来源：http://hz.shangyingyoupin.top/gtxtstzvrk.html

Java: public / protected / private / 默认包级
来源：http://hz.vqdsnc.cn/gtsgpduhds.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gzhubu.top/gtjqrnofle.html

Ruby: public / protected / private
来源：http://hz.yangfankeji.com/gtjeytuyaj.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gtfptezaet.html

[G11] getter / setter
来源：http://hz.aizwys.cn/gtvgyovcpy.html

Py:   @property 与 @x.setter
来源：http://hz.hammf.cn/gtqdapnfdw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtqtpugvfu.html

JS:   get name() { return this._name; }
来源：http://hz.cucudq.cn/gtqdkhzsoo.html

TS:   get name(): string { return this._name; }
来源：http://hz.feifeiyinyue.top/gtnbamjvkv.html

Java: public String getName() { return name; }
来源：http://hz.wangdashe.top/gtwshipwxj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fengsongda.top/gtkdyyizdt.html

Ruby: attr_accessor :name
来源：http://hz.xylfe.cn/gtavuwaooa.html

C#:   public string Name { get; set; }
来源：http://hz.cashguo.top/gtintynjzw.html

[G12] 对象转字符串
来源：http://hz.iojbl.cn/gtpvoxxxez.html

Py:   def __str__(self): return self.name
来源：http://hz.shangyingyoupin.top/gtuobjapbq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.birdmap.top/gtoxgqkwtj.html

JS:   toString() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtjoryvjmf.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydzc1.top/gtodbxbihu.html

Java: @Override public String toString() { return name; }
来源：http://hz.xuetiantiany.cn/gtfwkuprli.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtkxpuqopv.html

Ruby: def to_s; @name; end
来源：http://hz.cucudq.cn/gtahzifovh.html

C#:   public override string ToString() => Name;
来源：http://hz.bjfxy.top/gtzhtapmqt.html

[G13] 判断对象类型
来源：http://hz.sxryk.cn/gtakufaysg.html

Py:   isinstance(u, User)
来源：http://hz.andypj.xyz/gtutdsckuc.html

PHP:  $u instanceof User
来源：http://hz.hnqzz.top/gtavivalbh.html

JS:   u instanceof User
来源：http://hz.svipenyu.cn/gtcouydfpj.html

TS:   u instanceof User
来源：http://hz.sufxvd.cn/gtdzvycbii.html

Java: u instanceof User
来源：http://hz.hongshengwenyu.top/gttmclykyh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.iojbl.cn/gtoyrdgrph.html

Ruby: u.is_a?(User)
来源：http://hz.hammf.cn/gtpdlmjnnl.html

C#:   u is User
来源：http://hz.zhongyouzk.top/gtutachhmr.html

[G14] 数据类 / record
来源：http://hz.jlsjyb.cn/gtuwoxvvlj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinyuanbaomall.cn/gtzvmzfdeg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shangyingyoupin.top/gtavgrtotn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigfzy.top/gtwfuifygv.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuxming.cn/gtcqgucksx.html

Java: record User(String name, int age) {}
来源：http://hz.sysykeji.top/gtdkxmbdnj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jiagoushi.top/gtfyieomub.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinyuanbaomall.cn/gtcludkvyr.html

C#:   record User(string Name, int Age);
来源：http://hz.birdmap.top/gtdwkqkbjt.html

[G15] 枚举
来源：http://hz.yonumen.top/gtwoarqnmc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenlongwang.top/gticqwhbmw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.dianchejie.cn/gthklfvowq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.vqdsnc.cn/gttlvmweie.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gotoacloud.top/gtyydadrcr.html

Java: enum Color { RED, GREEN }
来源：http://hz.svipenyu.cn/gtdndduwkl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtkjscsbiv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.meibo888.top/gtocrnogzi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtulfywqxa.html

[G16] 对象转数组 / 字典
来源：http://hz.chenzaomai.com/gtmebvbdgx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangtech.top/gtgmjljbra.html

PHP:  get_object_vars($obj);
来源：http://hz.ywan-chungtsiang.top/gtvpcihhdg.html

JS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtznsxomkc.html

TS:   Object.entries(obj)
来源：http://hz.hywenlv.cn/gtclqpzisi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ehwqpu.com/gtpmisbssx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sweek.top/gtmckugnzh.html

Ruby: obj.instance_variables
来源：http://hz.feifeiyinyue.top/gtuijvjuvg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yongpay.top/gtzwklnpsd.html

================================================================================
来源：http://hz.gogol.net.cn/gtjztchfzr.html


<!-- 参考信息 -->