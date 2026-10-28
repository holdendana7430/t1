代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258888.top/gtdntgztol.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtcjxqqjoo.html

TS:   if (s === "") {}
来源：http://hz.yuxming.cn/gttufrzqtl.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj202588.top/gtlmagzggn.html

Go:   if s == "" {}
来源：http://hz.guannengcc.top/gttwhpceal.html

Ruby: if s.empty?
来源：http://hz.fengsongda.top/gtzwitqzwj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cashguo.top/gthhioxkco.html

[E21] 超长截断加省略号
来源：http://hz.pycfn.com/gtmnbhwugu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cdnleiting.top/gtfkvwvgac.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gtcraiunaf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtuhcbpjob.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zycfv.cn/gtwinjxfwz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtdmcmfgqr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nwbrower.top/gtuvvdxovl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.guowangkeji.top/gtfxdblgel.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ydzc1.top/gtgyaodzmm.html

[E22] 字节长度与字符长度
来源：http://hz.52xcode.cn/gtahssjyvd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.daxiang520.top/gtgbuxlqba.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtnqllojxc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigufen.top/gtivihnusq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.0kj1m.cn/gtcqrwxowq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.andypj.xyz/gtxrecpxmo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.havefunace.top/gtcamestog.html

Ruby: s.bytesize;  s.length
来源：http://hz.wangshuangyany.cn/gtnedqqsxf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ywan-chungtsiang.top/gtqnhmsmpx.html

================================================================================
来源：http://hz.yvedp.cn/gtcqijviyg.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gtsvrepuny.html

================================================================================
来源：http://hz.andypj.xyz/gtgtrvcsae.html

[F01] 读取整个文件
来源：http://hz.sufxvd.cn/gtbkvbhrre.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hywenlv.cn/gtyyjqyenw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hysaishi.cn/gtwhmpfvef.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj20258.top/gtqazgkvwf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.tanke756.top/gthejeeaoi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtolhxsodr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daxiang520.top/gtmcuaclkw.html

Ruby: File.read("a.txt")
来源：http://hz.ydjk.org.cn/gtkeotlpqo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.dashuyun.cn/gtjzocweyl.html

[F02] 逐行读取文件
来源：http://hz.fzhhl.top/gtisgeywdn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenjidiqi.icu/gtbtpqhhqo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yongpay.top/gtuzwhfwxq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guannengcc.top/gtkikozwxn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnxiangtu.top/gtembfjyyh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtoezhvkbr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.feifeiyinyue.top/gtjvuksepz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.vqdsnc.cn/gtzhdzuhae.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.birdmap.top/gtnlguccjg.html

[F03] 写入文件（覆盖）
来源：http://hz.meibo888.top/gtdrgntics.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xziqi.cn/gtpwvdykqv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daria6918.cn/gtyxjcvjqf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gtklcvgwwz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gttyyplqgt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangkeji.top/gthcvuruxr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sxryk.cn/gtpbighypv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydzc1.top/gtzyxdovmw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.mhx1999.top/gtujrlcmuo.html

[F04] 追加写入文件
来源：http://hz.ehwqpu.com/gtspfiwzwk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yanxiufei.cn/gtzwgyeves.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.0kj1m.cn/gtzbqdvwfz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gtmeknrqul.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtxletxvke.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tanke756.top/gtqirjtjhj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pengpengdd.cyou/gtfmtfcsin.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pengpengdd.cyou/gtylpxwphj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.wangdashe.top/gtstewuxdy.html

[F05] 判断文件或目录是否存在
来源：http://hz.fzhhl.top/gtlzzhgjfo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shuidangran.top/gtipgiabaa.html

PHP:  file_exists("a.txt");
来源：http://hz.iojbl.cn/gtlyhswkjc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cheryme.top/gtvkjtxihe.html

TS:   fs.existsSync("a.txt")
来源：http://hz.haohaochexian.top/gtfkxdhzeo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtpngdqmbm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tianlin.xyz/gtlqbnhpcb.html

Ruby: File.exist?("a.txt")
来源：http://hz.ehwqpu.com/gtdshzzwwc.html

C#:   File.Exists("a.txt")
来源：http://hz.sweek.top/gtnhrcwbkm.html

[F06] 删除文件
来源：http://hz.hnqzz.top/gtyabimoat.html

Py:   os.remove("a.txt")
来源：http://hz.hongshengwenyu.top/gtrxaerdyp.html

PHP:  unlink("a.txt");
来源：http://hz.jqgufenzy.top/gtmfuwxedg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.9152youxi.cn/gtldsktkkx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jlsjyb.cn/gtbvbxhkgd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtzlhfqjpr.html

Go:   os.Remove("a.txt")
来源：http://hz.xinyue.icu/gtttgwbnqs.html

Ruby: File.delete("a.txt")
来源：http://hz.vqdsnc.cn/gtbfvsoucp.html

C#:   File.Delete("a.txt");
来源：http://hz.xuanzx.com/gtdqtrhnlk.html

[F07] 创建目录（含多级）
来源：http://hz.shangyingyoupin.top/gtnmabftvl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pengpengdd.cyou/gtrljajqge.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtzdwvtzzw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenzaomai.com/gtgxbziore.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtkrlhbxay.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guannengcc.top/gtlaguknwb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yonumen.top/gththmjnfn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuxming.cn/gtuawybeld.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhaomingkeji.xyz/gtttxeujul.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtohntmves.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhongyouzk.top/gtvyvmrrfp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fzhhl.top/gtkvmkltae.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhongyouzk.top/gteykucztl.html

TS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtzvdzimsq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cheryme.top/gtyfipzyce.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xylfe.cn/gtukaopctv.html

Ruby: Dir.children("dir")
来源：http://hz.andypj.xyz/gtohfrznkw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nanxinkj.top/gtfrktsosh.html

[F09] 获取文件大小
来源：http://hz.sysykeji.top/gthjvtsfxp.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhiwuduotai.top/gtsxzkemix.html

PHP:  filesize("a.txt");
来源：http://hz.dianchejie.cn/gtwxrbzlcz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gtzufjiodz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangkeji.top/gtebwbxiga.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtpdkzklwl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jiagoushi.top/gttnggamnb.html

Ruby: File.size("a.txt")
来源：http://hz.hfpthk.cn/gtpcfmvdfq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pengpengdd.cyou/gttmdysbun.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xinyue.icu/gtohkhhfte.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtfhaipjds.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.mhx1999.top/gtrqviuvqi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtymghzhzu.html

TS:   path.extname("a.txt")
来源：http://hz.havefunace.top/gtitbwqskf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.52xcode.cn/gtdbitkiuf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zycfv.cn/gtdkuxtase.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtjjvqvmag.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtkvnoehap.html

[F11] 复制与移动文件
来源：http://hz.xinyue.icu/gtqrltsvee.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtzetehcem.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gtmzksqzcj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtduqetwvu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtjioamimj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.birdmap.top/gtlaxviunq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.birdmap.top/gtafipmfpl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtjrlojvgt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.haohaochexian.top/gtoocrbmqq.html

[F12] CSV 读写
来源：http://hz.ivvv.top/gtjzfinehs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhiwuduotai.top/gtqzrtoamz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jyoumei.cn/gtwkeybmav.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ivvv.top/gtwqneojpa.html

TS:   // 同上
来源：http://hz.tianlin.xyz/gtectrspwu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigufen.top/gtzdukbcje.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jyoumei.cn/gtdwwhtwej.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sweek.top/gttrnqypgr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ydjk.org.cn/gtwqusbbsh.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtsotumyks.html

G. 面向对象
来源：http://hz.hysaishi.cn/gtuxhpiueg.html

================================================================================
来源：http://hz.tian-w.cn/gtaehqrcev.html

[G01] 定义类
来源：http://hz.zhoulong.xyz/gtfghcmslc.html

Py:   class User: pass
来源：http://hz.meibo888.top/gtwroheldb.html

PHP:  class User {}
来源：http://hz.pengpengdd.cyou/gtbrvctcws.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtkbledxju.html

TS:   class User { name: string = ""; }
来源：http://hz.iojbl.cn/gtyvssevjb.html

Java: class User {}
来源：http://hz.gaohongyu789.top/gtjvwncpqr.html

Go:   type User struct { Name string }
来源：http://hz.yonumen.top/gtfjdauell.html

Ruby: class User; end
来源：http://hz.birdmap.top/gtpnujlmun.html

C#:   class User {}
来源：http://hz.cucudq.cn/gtvssjyzkz.html

[G02] 构造函数
来源：http://hz.yonumen.top/gtthofmhxt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.quarkkingdee.top/gtfwmpcxju.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhiwuduotai.top/gttnslobxu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtjqjvlzge.html

TS:   constructor(public name: string) {}
来源：http://hz.aizwys.cn/gtsigkdkdf.html

Java: User(String name) { this.name = name; }
来源：http://hz.dashuyun.cn/gtyprverag.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuetiantiany.cn/gtoyvfjutg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yongpay.top/gtrraibacs.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xziqi.cn/gtwcwpzwxp.html

[G03] 实例属性
来源：http://hz.mhx1999.top/gttzsxwgey.html

Py:   self.name = "x"
来源：http://hz.ppjwa.cn/gtmkalrkij.html

PHP:  public string $name = "x";
来源：http://hz.zhengqikj.top/gtsftkmlxf.html

JS:   this.name = "x";
来源：http://hz.daxiang520.top/gtpqunshoj.html

TS:   name: string = "x";
来源：http://hz.aibaodan.cn/gtvvxcfxhd.html

Java: private String name;
来源：http://hz.nwbrower.top/gtemlsxxtv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jqgfzy.top/gtevtuayno.html

Ruby: @name = "x"
来源：http://hz.bjfxy.top/gtnxkeempm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.mhx1999.top/gtyvtnkbmg.html

[G04] 定义方法
来源：http://hz.yj20258.top/gtpzimwtdc.html

Py:   def greet(self): return self.name
来源：http://hz.shangyingyoupin.top/gtthfobkrc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtfqpuhift.html

JS:   greet() { return this.name; }
来源：http://hz.yuanzhike.top/gtvkbvndxz.html

TS:   greet(): string { return this.name; }
来源：http://hz.birdmap.top/gtpgofwvhj.html

Java: String greet() { return name; }
来源：http://hz.gogol.net.cn/gtheyxedah.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.bjfxy.top/gtfqqixsuy.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gttpdivyku.html

C#:   public string Greet() => Name;
来源：http://hz.chenzaomai.com/gtqrnoqptx.html

[G05] 继承
来源：http://hz.yongpay.top/gtjhnszedg.html

Py:   class Admin(User): pass
来源：http://hz.zhengqikj.top/gtwppreqco.html

PHP:  class Admin extends User {}
来源：http://hz.tianlin.xyz/gtxkuhloqs.html

JS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtuwzhoutf.html

TS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtmzwpgfzw.html

Java: class Admin extends User {}
来源：http://hz.shuidangran.top/gtjezcewmq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.smart0.xyz/gtfroxeaqf.html

Ruby: class Admin < User; end
来源：http://hz.daxiang520.top/gtteftvlzd.html

C#:   class Admin : User {}
来源：http://hz.ppjwa.cn/gtpsnknucr.html

[G06] 重写方法
来源：http://hz.iojbl.cn/gtbaddyhuz.html

Py:   def greet(self): return "admin"
来源：http://hz.chenlongwang.top/gtweomszxn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.vqdsnc.cn/gtwoonpleu.html

JS:   greet() { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtaxeryajr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtfwgpojij.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtxenqjamx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhoulong.xyz/gtcxfixmuw.html

Ruby: def greet; "admin"; end
来源：http://hz.yonumen.top/gtwxgchazm.html

C#:   public override string Greet() => "admin";
来源：http://hz.aibaodan.cn/gtwccspapr.html

[G07] 调用父类方法
来源：http://hz.haohaochexian.top/gttzzyywhn.html

Py:   super().greet()
来源：http://hz.zhoulong.xyz/gtcjywmwwx.html

PHP:  parent::greet();
来源：http://hz.xinyue.icu/gtcejaiddq.html

JS:   super.greet();
来源：http://hz.52xcode.cn/gtsffvdnhc.html

TS:   super.greet();
来源：http://hz.zhongyouzk.top/gtgzysmhqi.html

Java: super.greet();
来源：http://hz.xylfe.cn/gtjordxqcm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangshuangyany.cn/gtjtpcncho.html

Ruby: super
来源：http://hz.feifeiyinyue.top/gtpvrgknge.html

C#:   base.Greet();
来源：http://hz.kuanghao11.cn/gtmpwnczti.html

[G08] 静态方法与属性
来源：http://hz.shzxlz.cn/gtbmcowcgt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.birdmap.top/gtvleoftbg.html

PHP:  public static function f() {}
来源：http://hz.zhengqikj.top/gtcmpmgcvc.html

JS:   static f() {}
来源：http://hz.nanxinkj.top/gtmnvxaxhp.html

TS:   static f(): void {}
来源：http://hz.jyoumei.cn/gtjczcsljq.html

Java: static void f() {}
来源：http://hz.yvedp.cn/gtwjiivefw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tanke756.top/gtaopkwbao.html

Ruby: def self.f; end
来源：http://hz.zhiwuduotai.top/gtribbjggf.html

C#:   public static void F() {}
来源：http://hz.316326.xyz/gtriyukslr.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258888.top/gthxhfvitr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jyoumei.cn/gtrijwmhpw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tianlin.xyz/gtopceqfpd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.9152youxi.cn/gtwvangvmo.html

TS:   interface Shape { area(): number; }
来源：http://hz.feifeiyinyue.top/gtutaieeof.html

Java: interface Shape { double area(); }
来源：http://hz.nwbrower.top/gtjrqnwosl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.redwolf501.top/gtshxfncxo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj20258888.top/gtrotsqciu.html

C#:   interface IShape { double Area(); }
来源：http://hz.yangfankeji.com/gtobinocde.html

[G10] 访问控制
来源：http://hz.gogol.net.cn/gthgypgtnt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.andypj.xyz/gtineioyxu.html

PHP:  public / protected / private
来源：http://hz.yanxiufei.cn/gttuamyhij.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtbnzdymcf.html

TS:   public / protected / private
来源：http://hz.kuanghao11.cn/gtbiwysnib.html

Java: public / protected / private / 默认包级
来源：http://hz.cqqwz.cn/gtfjfjqpel.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydzc1.top/gtyhootlym.html

Ruby: public / protected / private
来源：http://hz.iojbl.cn/gtlelorjjy.html

C#:   public / protected / private / internal
来源：http://hz.vqdsnc.cn/gtyijagqjq.html

[G11] getter / setter
来源：http://hz.jiagoushi.top/gtboxyqtpw.html

Py:   @property 与 @x.setter
来源：http://hz.xuanzx.com/gtbepnetox.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtscqgndcc.html

JS:   get name() { return this._name; }
来源：http://hz.tian-w.cn/gtgkbbhzjp.html

TS:   get name(): string { return this._name; }
来源：http://hz.snrcjt.cn/gtuqgcnldu.html

Java: public String getName() { return name; }
来源：http://hz.yj20258888.top/gtysplpdvm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cqqwz.cn/gtarbfhyug.html

Ruby: attr_accessor :name
来源：http://hz.hfpthk.cn/gtuailfflw.html

C#:   public string Name { get; set; }
来源：http://hz.chenzaomai.com/gtwbvpgovq.html

[G12] 对象转字符串
来源：http://hz.tian-w.cn/gtfcepsgeh.html

Py:   def __str__(self): return self.name
来源：http://hz.sweek.top/gtahijimyr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtpdrvruvr.html

JS:   toString() { return this.name; }
来源：http://hz.cdnleiting.top/gtbdhkyuhv.html

TS:   toString(): string { return this.name; }
来源：http://hz.jyoumei.cn/gtkamlbyyq.html

Java: @Override public String toString() { return name; }
来源：http://hz.jlsjyb.cn/gtkkxupwel.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shzxlz.cn/gtgvcxofid.html

Ruby: def to_s; @name; end
来源：http://hz.daxiang520.top/gtsybxnvaj.html

C#:   public override string ToString() => Name;
来源：http://hz.ydzc1.top/gtdlusxbow.html

[G13] 判断对象类型
来源：http://hz.ehwqpu.com/gtrmixlppa.html

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gtobzktjpu.html

PHP:  $u instanceof User
来源：http://hz.316326.xyz/gtojqsixfn.html

JS:   u instanceof User
来源：http://hz.jqgufenzy.top/gtzyhxrifv.html

TS:   u instanceof User
来源：http://hz.yj20258.top/gtlgjrsmsb.html

Java: u instanceof User
来源：http://hz.nwbrower.top/gtprclbsrt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xziqi.cn/gthkhxyjjk.html

Ruby: u.is_a?(User)
来源：http://hz.snrcjt.cn/gtxpbbodpd.html

C#:   u is User
来源：http://hz.quarkkingdee.top/gtjxxjzdbv.html

[G14] 数据类 / record
来源：http://hz.cashguo.top/gtulcyffio.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jianghu66.top/gtmufitryx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydzc1.top/gtyfsihhde.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ybcxt.top/gtenuvtlby.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangshuangyany.cn/gtkvhcmlsn.html

Java: record User(String name, int age) {}
来源：http://hz.svipenyu.cn/gtemrtjojp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.52xcode.cn/gthnkjrphj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuetiantiany.cn/gtnswskjkl.html

C#:   record User(string Name, int Age);
来源：http://hz.aibaodan.cn/gtutcacult.html

[G15] 枚举
来源：http://hz.jlsjyb.cn/gtxmzjlmkt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj202588.top/gtyasrytos.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hongshengwenyu.top/gtnzwibnyd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xylfe.cn/gtdrxopown.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtiucuehqw.html

Java: enum Color { RED, GREEN }
来源：http://hz.feifeiyinyue.top/gttkmgqopi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigfzy.top/gtkyuceocc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ivvv.top/gtgcdolhqp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhixingplan.top/gtcezfafix.html

[G16] 对象转数组 / 字典
来源：http://hz.yongpay.top/gtaxuytovs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gthgmqubsm.html

PHP:  get_object_vars($obj);
来源：http://hz.tian-w.cn/gtxnlpceag.html

JS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gtrfbbepvf.html

TS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gttcbnpotb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.vqdsnc.cn/gtzypzsiwy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.iojbl.cn/gtmtatlbxa.html

Ruby: obj.instance_variables
来源：http://hz.zhengqikj.top/gtoicgaglx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fzhhl.top/gtzwgcnipr.html

================================================================================
来源：http://hz.guannengcc.top/gtaeqnuwbr.html

H. 异常与错误处理
来源：http://hz.kuanghao11.cn/gtuaslhwma.html

================================================================================
来源：http://hz.jiagoushi.top/gtcjuexjrw.html

[H01] try / catch 基础
来源：http://hz.aibaodan.cn/gtsphsvfvu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zycfv.cn/gtehxfifve.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.andypj.xyz/gtthfcbcqh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.redwolf501.top/gtcrixobvt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.c1oappe.top/gteqlrdvyk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenlongwang.top/gtlywtpfxp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gzhubu.top/gtwwaznium.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cheryme.top/gtiatyyhsm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sysykeji.top/gtfqzcezvi.html

[H02] finally / ensure 收尾
来源：http://hz.daxiang520.top/gtsaytxmpk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigufen.top/gthpkervch.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtdbgjkqfi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtibnkduco.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtnfdkcsrf.html


<!-- 参考信息 -->