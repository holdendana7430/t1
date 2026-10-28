代发 wailian999

Go:   if s == "" {}
来源：http://hz.hnqzz.top/gtdkfnplwc.html

Ruby: if s.empty?
来源：http://hz.zhoulong.xyz/gtftcbhifc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gaohongyu789.top/gtatpobjfd.html

[E21] 超长截断加省略号
来源：http://hz.jqgfzy.top/gtvrbdwetc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zdqjudy.top/gtujrkdefw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fengsongda.top/gtxlclvfqh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fengsongda.top/gtowebsmru.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtbnybbnml.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtmyyibhpl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.birdmap.top/gthaapegrl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.0kj1m.cn/gtbfnooqlc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sufxvd.cn/gtuxizypke.html

[E22] 字节长度与字符长度
来源：http://hz.wangshuangyany.cn/gtgqxkicrf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.iojbl.cn/gtahghlcvo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jyoumei.cn/gtxinszvfx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yuanzhike.top/gthkjnflur.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtteljazho.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258888.top/gtfocfbmhm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj202588.top/gtmjsnxeme.html

Ruby: s.bytesize;  s.length
来源：http://hz.316326.xyz/gtzwpjekwz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuetiantiany.cn/gtsznzrypv.html

================================================================================
来源：http://hz.birdmap.top/gtxnjacoxl.html

F. 文件与目录
来源：http://hz.xingfuxueyuan.xyz/gtzknvdqqy.html

================================================================================
来源：http://hz.sysykeji.top/gtsftqfvva.html

[F01] 读取整个文件
来源：http://hz.sysykeji.top/gttpywczhj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenzaomai.com/gtucmywyil.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jqgufenzy.top/gtegzwkzjl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigfzy.top/gtqyigkoif.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guannengcc.top/gtpjzmusqa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtpsixnijk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pycfn.com/gtueeidpqp.html

Ruby: File.read("a.txt")
来源：http://hz.sxryk.cn/gtfpekyyoc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ydzc1.top/gtggdrmkpp.html

[F02] 逐行读取文件
来源：http://hz.meibo888.top/gtxjmeovnp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yj20258.top/gtgutfozjk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jianghu66.top/gtzjqtvzeg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtfpfbrsoy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtuenwqcrv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtqosyawrp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fzhhl.top/gtsucbuugq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gzhubu.top/gtbzahqpte.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gogol.net.cn/gtisuomrxm.html

[F03] 写入文件（覆盖）
来源：http://hz.daxiang520.top/gtzddlcryp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.andypj.xyz/gtoevakhrb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cqqwz.cn/gtenakcalf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zdqjudy.top/gtdemofmcj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gtbggntzac.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jqgfzy.top/gtswvcafrb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.tanke756.top/gtypdbmeww.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ppjwa.cn/gtsgvznomm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinghuilouyu.cn/gtyhprfaqh.html

[F04] 追加写入文件
来源：http://hz.dianchejie.cn/gtceqvnlle.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gaohongyu789.top/gtuqczlagp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.svipenyu.cn/gtbquhstbq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.redwolf501.top/gteqvfezge.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hongshengwenyu.top/gttpgvctjl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.meibo888.top/gtwdmgagrs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sufxvd.cn/gtxgjkxwgy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zycfv.cn/gtqqcdwiup.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.snrcjt.cn/gtifcprzgh.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj202588.top/gtogrxepol.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yuanzhike.top/gtxpyiaoia.html

PHP:  file_exists("a.txt");
来源：http://hz.gaohongyu789.top/gtvescizwo.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yanxiufei.cn/gtdjzoiqio.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtlnkeuimw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtajtxunep.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ivvv.top/gtcjsebwxg.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuetiantiany.cn/gtcecmwksv.html

C#:   File.Exists("a.txt")
来源：http://hz.yongpay.top/gtbgxhvvcq.html

[F06] 删除文件
来源：http://hz.zhaomingkeji.xyz/gtmcvxrdyy.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtsxyaofvo.html

PHP:  unlink("a.txt");
来源：http://hz.andypj.xyz/gtxydbhcvn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtjpjnqcpq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nwbrower.top/gtyzqpifyg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtnfprbmfx.html

Go:   os.Remove("a.txt")
来源：http://hz.chenzaomai.com/gtqydglqfs.html

Ruby: File.delete("a.txt")
来源：http://hz.cheryme.top/gtsbtjszsv.html

C#:   File.Delete("a.txt");
来源：http://hz.daxiang520.top/gtovfjsate.html

[F07] 创建目录（含多级）
来源：http://hz.zhijiandao.cn/gtpxzhrjrd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cqqwz.cn/gtlevuhpcb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.quarkkingdee.top/gtuhghanfv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnxiangtu.top/gtuxevnrck.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtbchjwuom.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.kuanghao11.cn/gtwxkdhokz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.haohaochexian.top/gtjdmcdlll.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xylfe.cn/gtbfcrljcn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhixingplan.top/gtsjlxxwga.html

[F08] 遍历目录
来源：http://hz.c1oappe.top/gtkdflrdxp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhixingplan.top/gthsroliyg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shanyushiyangkeji.top/gtrjqdcsdi.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxinkj.top/gtliigmhac.html

TS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gtssenfwvd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtqquqjuhx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pycfn.com/gtcdossbuh.html

Ruby: Dir.children("dir")
来源：http://hz.dianchejie.cn/gtqzigdela.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgfzy.top/gterbvqrqd.html

[F09] 获取文件大小
来源：http://hz.snrcjt.cn/gtmkqeaofb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.snrcjt.cn/gteebmqval.html

PHP:  filesize("a.txt");
来源：http://hz.jlsjyb.cn/gtzzflnfyt.html

JS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtdqmlwkoi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtbsbnwdle.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtoeahnpgi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yonumen.top/gtpumaisny.html

Ruby: File.size("a.txt")
来源：http://hz.chenzaomai.com/gthqeytvel.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.c1oappe.top/gtccnttuvm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jqgfzy.top/gtmupcldzm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtdcvjfohd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.quarkkingdee.top/gtjlyrqjca.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtlxcabxts.html

TS:   path.extname("a.txt")
来源：http://hz.svipenyu.cn/gtncbztmji.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tianlin.xyz/gtaxlnchgi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gtldcerxyd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gthsypjiip.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daria6918.cn/gtoaqdbcmg.html

[F11] 复制与移动文件
来源：http://hz.mhx1999.top/gtwoxyzwjc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtcmapocqr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhongyouzk.top/gtueaduvfb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtihejrhmv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtzwnjfiwe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.52xcode.cn/gtcgvhxwvl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yangfankeji.com/gtjqokqqsv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtxmwzxvec.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nwbrower.top/gtobkbamas.html

[F12] CSV 读写
来源：http://hz.xylfe.cn/gtzawekuyw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daxiang520.top/gtjlyibqwp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dashuyun.cn/gttprhvshp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ybcxt.top/gtsoabtriw.html

TS:   // 同上
来源：http://hz.xuetiantiany.cn/gtmhjkoevw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xylfe.cn/gtwbucowqj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinghuilouyu.cn/gtayuekaqu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hammf.cn/gtyegqnwfw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cucudq.cn/gtcqaiwrhs.html

================================================================================
来源：http://hz.yuanzhike.top/gthfhaqouo.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gttltevxur.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtwqulxumm.html

[G01] 定义类
来源：http://hz.9152youxi.cn/gtglczngtf.html

Py:   class User: pass
来源：http://hz.redwolf501.top/gtolheudpi.html

PHP:  class User {}
来源：http://hz.ybcxt.top/gtiijxcgmg.html

JS:   class User {}
来源：http://hz.hammf.cn/gtmoqxnlzx.html

TS:   class User { name: string = ""; }
来源：http://hz.sufxvd.cn/gtsjoskvvg.html

Java: class User {}
来源：http://hz.jinghuilouyu.cn/gtbnlmisqq.html

Go:   type User struct { Name string }
来源：http://hz.chenlongwang.top/gtiqupydmp.html

Ruby: class User; end
来源：http://hz.guowangkeji.top/gtmkqtjkti.html

C#:   class User {}
来源：http://hz.c1oappe.top/gtrtoqjase.html

[G02] 构造函数
来源：http://hz.wangshuangyany.cn/gtmcdxgqfr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.feifeiyinyue.top/gtvftgxkgu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guannengcc.top/gttiirpwep.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj202588.top/gtgiyddqxt.html

TS:   constructor(public name: string) {}
来源：http://hz.zycfv.cn/gtanaumibc.html

Java: User(String name) { this.name = name; }
来源：http://hz.jiagoushi.top/gtywrbnywg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ydzc1.top/gtdxycjhiw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhixingplan.top/gthcegqhhm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hammf.cn/gtlawpehvk.html

[G03] 实例属性
来源：http://hz.daxiang520.top/gtlzdudpqo.html

Py:   self.name = "x"
来源：http://hz.aizwys.cn/gtryefuwxm.html

PHP:  public string $name = "x";
来源：http://hz.jianghu66.top/gtzhnhrrvd.html

JS:   this.name = "x";
来源：http://hz.yuxming.cn/gtcjqbmmjl.html

TS:   name: string = "x";
来源：http://hz.bjfxy.top/gtnvlutghw.html

Java: private String name;
来源：http://hz.shzxlz.cn/gtndgpleep.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pycfn.com/gtgxitniet.html

Ruby: @name = "x"
来源：http://hz.sufxvd.cn/gtamlxeqpd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jlsjyb.cn/gtmjmvdapx.html

[G04] 定义方法
来源：http://hz.tianlin.xyz/gtzjjwcamw.html

Py:   def greet(self): return self.name
来源：http://hz.guannengcc.top/gtqcgwjvgq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtyaqcuxfu.html

JS:   greet() { return this.name; }
来源：http://hz.yvedp.cn/gttkkiwwry.html

TS:   greet(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtgmattzez.html

Java: String greet() { return name; }
来源：http://hz.zycfv.cn/gtqsflxllv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fzhhl.top/gtexvfvohi.html

Ruby: def greet; @name; end
来源：http://hz.wangdashe.top/gtqovvquvc.html

C#:   public string Greet() => Name;
来源：http://hz.yanxiufei.cn/gtnvmgqjuf.html

[G05] 继承
来源：http://hz.nanxuanxn.top/gtmihjqxsb.html

Py:   class Admin(User): pass
来源：http://hz.hongshengwenyu.top/gtvzkfayer.html

PHP:  class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtduuzfpfn.html

JS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtvfytgvrx.html

TS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtgqhbbqqc.html

Java: class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtlwpjlbnj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.haohaochexian.top/gtdlhurviz.html

Ruby: class Admin < User; end
来源：http://hz.c1oappe.top/gtbaznhwlj.html

C#:   class Admin : User {}
来源：http://hz.0kj1m.cn/gtqtrgnnha.html

[G06] 重写方法
来源：http://hz.sysykeji.top/gtwvfdzxqy.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangkeji.top/gtilmknvqw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.316326.xyz/gtiosyhzbf.html

JS:   greet() { return "admin"; }
来源：http://hz.sysykeji.top/gthomdwazb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtcfmbmhje.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj202588.top/gttwghaejp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.vqdsnc.cn/gtiyfiahvj.html

Ruby: def greet; "admin"; end
来源：http://hz.aibaodan.cn/gtzujzgiig.html

C#:   public override string Greet() => "admin";
来源：http://hz.tanke756.top/gtdcqnxtiu.html

[G07] 调用父类方法
来源：http://hz.jianghu66.top/gtagfobgoo.html

Py:   super().greet()
来源：http://hz.chenlongwang.top/gtqdmjlkvz.html

PHP:  parent::greet();
来源：http://hz.sufxvd.cn/gttmxkodqb.html

JS:   super.greet();
来源：http://hz.wangdashe.top/gtehilimsf.html

TS:   super.greet();
来源：http://hz.zhaomingkeji.xyz/gtslabqmfm.html

Java: super.greet();
来源：http://hz.0kj1m.cn/gthmhvzamj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.meibo888.top/gtmrhxqnro.html

Ruby: super
来源：http://hz.xziqi.cn/gthcceephc.html

C#:   base.Greet();
来源：http://hz.dianchejie.cn/gtnziemwzw.html

[G08] 静态方法与属性
来源：http://hz.jianghu66.top/gtyceeadij.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhaomingkeji.xyz/gtgybqykok.html

PHP:  public static function f() {}
来源：http://hz.ybcxt.top/gtpjfimwue.html

JS:   static f() {}
来源：http://hz.sxryk.cn/gtjyhghltt.html

TS:   static f(): void {}
来源：http://hz.gzhubu.top/gtmducbysy.html

Java: static void f() {}
来源：http://hz.yj202588.top/gtwbkzdksg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.0kj1m.cn/gthfibzyam.html

Ruby: def self.f; end
来源：http://hz.ivvv.top/gtiueihvql.html

C#:   public static void F() {}
来源：http://hz.jqgfzy.top/gthyvamzeu.html

[G09] 接口 / 抽象类
来源：http://hz.jinyuanbaomall.cn/gtdmrqlkow.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cqqwz.cn/gtyeslrlmo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangshuangyany.cn/gtfbchzlir.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cashguo.top/gtbvudfdvs.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigfzy.top/gtlsmqtmlh.html

Java: interface Shape { double area(); }
来源：http://hz.xuanzx.com/gtozjdhhzw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.quarkkingdee.top/gtmnegenzz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daxiang520.top/gtgicwahgn.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgufenzy.top/gtqwqcsmnk.html

[G10] 访问控制
来源：http://hz.kuanghao11.cn/gtmiuiizrs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.mhx1999.top/gtsjyffffe.html

PHP:  public / protected / private
来源：http://hz.tianlin.xyz/gtwrruxndu.html

JS:   #private 字段；其余公开
来源：http://hz.gaohongyu789.top/gtjvuprvtf.html

TS:   public / protected / private
来源：http://hz.yj202588.top/gtaindbhob.html

Java: public / protected / private / 默认包级
来源：http://hz.xziqi.cn/gtrwfmeaiz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.0kj1m.cn/gthkbskgic.html

Ruby: public / protected / private
来源：http://hz.kuanghao11.cn/gtmfgcffxr.html

C#:   public / protected / private / internal
来源：http://hz.ydzc1.top/gtrgnhjbmj.html

[G11] getter / setter
来源：http://hz.shangyingyoupin.top/gtzdqxpify.html

Py:   @property 与 @x.setter
来源：http://hz.sysykeji.top/gthyvorcyx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtenpupeja.html

JS:   get name() { return this._name; }
来源：http://hz.zhongyouzk.top/gtiridjmcl.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnxiangtu.top/gttdhtqjdn.html

Java: public String getName() { return name; }
来源：http://hz.daxiang520.top/gtlhzahqgd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.mhx1999.top/gtwsrnkyve.html

Ruby: attr_accessor :name
来源：http://hz.xinyue.icu/gtrxfjmvby.html

C#:   public string Name { get; set; }
来源：http://hz.aibaodan.cn/gtwndasxmg.html

[G12] 对象转字符串
来源：http://hz.xuetiantiany.cn/gtylqcvxyl.html

Py:   def __str__(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtlfdrpsey.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtznizcnjm.html

JS:   toString() { return this.name; }
来源：http://hz.aibaodan.cn/gttdtyjxlj.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhengqikj.top/gtmgtcdsyd.html

Java: @Override public String toString() { return name; }
来源：http://hz.shuidangran.top/gtucxxdhlt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gzhubu.top/gtsxnegpfq.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gttodzgbbg.html

C#:   public override string ToString() => Name;
来源：http://hz.ybcxt.top/gtdfddtzhb.html

[G13] 判断对象类型
来源：http://hz.hammf.cn/gtvvylfpnw.html

Py:   isinstance(u, User)
来源：http://hz.cqqwz.cn/gtppuhxejw.html

PHP:  $u instanceof User
来源：http://hz.sufxvd.cn/gteurejdjz.html

JS:   u instanceof User
来源：http://hz.jinghuilouyu.cn/gtebbwvwgd.html

TS:   u instanceof User
来源：http://hz.316326.xyz/gtzbfexiug.html

Java: u instanceof User
来源：http://hz.yangfankeji.com/gtfazygbee.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangtech.top/gtpnrwlxxy.html

Ruby: u.is_a?(User)
来源：http://hz.gaohongyu789.top/gtxnmxjndy.html

C#:   u is User
来源：http://hz.haohaochexian.top/gtcwasudct.html

[G14] 数据类 / record
来源：http://hz.chenlongwang.top/gtsdgvgfbm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hfpthk.cn/gtapadbnuw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hywenlv.cn/gtdofsrwfj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daria6918.cn/gtgcmeqgma.html

TS:   type User = { name: string; age: number };
来源：http://hz.hysaishi.cn/gtdzrwhhnn.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258.top/gttxrlmeqy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gaohongyu789.top/gtevbjgern.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gotoacloud.top/gtpzxeztpl.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gtrvzjnmrz.html

[G15] 枚举
来源：http://hz.ydjk.org.cn/gtbpfjxuui.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigufen.top/gtzkzjwhfp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhijiandao.cn/gtwlvtmxxv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.kuanghao11.cn/gtrvcofmrv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sysykeji.top/gtfmxrldmk.html

Java: enum Color { RED, GREEN }
来源：http://hz.jiagoushi.top/gtumzkluty.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yvedp.cn/gtgokovfiy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj202588.top/gtofkgrwdr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtcxdaasij.html

[G16] 对象转数组 / 字典
来源：http://hz.52xcode.cn/gtxxxgdpsx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jyoumei.cn/gtdiveqwgk.html

PHP:  get_object_vars($obj);
来源：http://hz.pengpengdd.cyou/gteqjphkhh.html

JS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtykxwqbno.html

TS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gthxabscly.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shangyingyoupin.top/gtpzmthogh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cdnleiting.top/gtxljylrmk.html

Ruby: obj.instance_variables
来源：http://hz.nanxinkj.top/gthaujumyx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nwbrower.top/gtwxioqvwy.html

================================================================================
来源：http://hz.bjfxy.top/gtiqsolsxy.html

H. 异常与错误处理
来源：http://hz.xziqi.cn/gtlazhezhc.html

================================================================================
来源：http://hz.xylfe.cn/gthbydguvv.html

[H01] try / catch 基础
来源：http://hz.zycfv.cn/gtvyhdowfq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.c1oappe.top/gtxqnilauu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.redwolf501.top/gtmkyxwxjr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtoacttkfh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.haohaochexian.top/gtpzwsfibv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hongshengwenyu.top/gtaklygyvb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daxiang520.top/gtjcviwopg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.9152youxi.cn/gtbfdxeepb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gzhubu.top/gtckxzncdi.html

[H02] finally / ensure 收尾
来源：http://hz.fzhhl.top/gtegxqwvql.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtdfzprpaq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gthoakgulk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtmnrkxljo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtyicuxeoz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtyzhqspwa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gtircpdieu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangtech.top/gtkrgdeynt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenjidiqi.icu/gtqoyyalbh.html


<!-- 参考信息 -->