代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.0kj1m.cn/gtbyuehyhd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.smart0.xyz/gtssrcrnca.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtwpzvklop.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtwjaetxbp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtjtmkgwrh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xylfe.cn/gtvuutpgvq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jianghu66.top/gtlukkyqoy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yvedp.cn/gtjuwtoqom.html

[E22] 字节长度与字符长度
来源：http://hz.shuidangran.top/gtddgsnrft.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jqgufenzy.top/gttbbjogkm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tianlin.xyz/gtlwcekyya.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtzmzzltqs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tian-w.cn/gtyflxymna.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yangfankeji.com/gtnhdoloox.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xinyue.icu/gtuzevrhgc.html

Ruby: s.bytesize;  s.length
来源：http://hz.xinyue.icu/gtwonxcysq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cdnleiting.top/gtozfcfknm.html

================================================================================
来源：http://hz.smart0.xyz/gtwvglrolx.html

F. 文件与目录
来源：http://hz.hysaishi.cn/gtedahufqn.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtngnqrkur.html

[F01] 读取整个文件
来源：http://hz.sweek.top/gtleyotoup.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258.top/gtwkgvimzm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nwbrower.top/gtcswxrwzq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cheryme.top/gtkyloypnq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydjk.org.cn/gtkrvxaqlc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtfrikdwlj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.redwolf501.top/gthgqkujqr.html

Ruby: File.read("a.txt")
来源：http://hz.yj20258.top/gtufvspskr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cucudq.cn/gtahdhfvou.html

[F02] 逐行读取文件
来源：http://hz.jinyuanbaomall.cn/gtnpnqlqel.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.c1oappe.top/gtbtbjabwd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sufxvd.cn/gtrkavysbr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gtciincxoo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtojkbggly.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtutpmhsgb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guannengcc.top/gtnrlafecv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258.top/gtljrxerwv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ppjwa.cn/gtmnsflqqr.html

[F03] 写入文件（覆盖）
来源：http://hz.jiagoushi.top/gtaaolilbg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.wangdashe.top/gtmjjvitjb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhijiandao.cn/gtvymiwsbq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtimilsova.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtfohnjxqt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tianlin.xyz/gtgwdisokw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xingfuxueyuan.xyz/gtcmfyxkif.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenzaomai.com/gtvhwkunyo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cqqwz.cn/gteztlwxkt.html

[F04] 追加写入文件
来源：http://hz.gotoacloud.top/gtsaghkdpt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj202588.top/gtdpnnjcaq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yongpay.top/gtnadpinyy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.havefunace.top/gtcbgdvvje.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.vqdsnc.cn/gtkmwxkjpv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yanxiufei.cn/gtkevyzfjt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ydzc1.top/gtgqmqonwv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xylfe.cn/gtfxmsyybz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xinyue.icu/gtswlmvhhi.html

[F05] 判断文件或目录是否存在
来源：http://hz.gaohongyu789.top/gtzhzdfqth.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.bjfxy.top/gtvqnzwpey.html

PHP:  file_exists("a.txt");
来源：http://hz.xuetiantiany.cn/gtapzpjube.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtffyvqajg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gtomvctchs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtwzkeferf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.meibo888.top/gtiqdlobnh.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuetiantiany.cn/gtapdobyjc.html

C#:   File.Exists("a.txt")
来源：http://hz.wangshuangyany.cn/gtycnisopi.html

[F06] 删除文件
来源：http://hz.zhoulong.xyz/gtulznreir.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtofbquhrz.html

PHP:  unlink("a.txt");
来源：http://hz.xinyue.icu/gtwfgrqjte.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtnvpcfhop.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhongyouzk.top/gtpojghvxp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtoqimoqhv.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gthuxbxbbh.html

Ruby: File.delete("a.txt")
来源：http://hz.nwbrower.top/gtyoaguuza.html

C#:   File.Delete("a.txt");
来源：http://hz.yuanzhike.top/gtmpeejisc.html

[F07] 创建目录（含多级）
来源：http://hz.tanke756.top/gtblnbjdvm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.chenlongwang.top/gtgoxrtrev.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jyoumei.cn/gttrdtsjru.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sweek.top/gtgaofqzug.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtpcpxqrnf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ywan-chungtsiang.top/gtyiesdenq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.pengpengdd.cyou/gtqzxmwnni.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhixingplan.top/gtnxljvbgm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinqigfzy.top/gtdqemcxbt.html

[F08] 遍历目录
来源：http://hz.zdqjudy.top/gtvqndakfc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.smart0.xyz/gtxwbjgxfa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.kuanghao11.cn/gtdidphree.html

JS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtiklubkev.html

TS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtmunmbrjk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nwbrower.top/gtxistnwqy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yongpay.top/gtkrsxotew.html

Ruby: Dir.children("dir")
来源：http://hz.zhiwuduotai.top/gtcvvojabs.html

C#:   Directory.GetFiles("dir")
来源：http://hz.pengpengdd.cyou/gtvmgqgaom.html

[F09] 获取文件大小
来源：http://hz.vqdsnc.cn/gtjrtadnzg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sweek.top/gtcmndqiji.html

PHP:  filesize("a.txt");
来源：http://hz.daria6918.cn/gtelnwcasz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gtoqttsljc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtbztbnbcr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtnxgfkdgw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.316326.xyz/gtnvrfuonw.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gtrdqigdnc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pengpengdd.cyou/gtyykvjrqz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj202588.top/gtzloulutf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtsfmhnuyq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ehwqpu.com/gtzgitzxoh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtpsfkjvft.html

TS:   path.extname("a.txt")
来源：http://hz.daria6918.cn/gtkcoirkuc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgfzy.top/gtfmzyqlww.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.svipenyu.cn/gtczfnwixx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtodvhdynl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtnslsyfjd.html

[F11] 复制与移动文件
来源：http://hz.wangshuangyany.cn/gtmoheyspf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtgbnamhpn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ydjk.org.cn/gtchsuexqp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtfoexevfb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtlbfudleo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xylfe.cn/gtusxjkdof.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jiagoushi.top/gtddcdolxl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtuhlzucqh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tanke756.top/gtueqdrimc.html

[F12] CSV 读写
来源：http://hz.9152youxi.cn/gtumkkxsck.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgufenzy.top/gtgsobbmga.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hysaishi.cn/gtfrluqvgg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.316326.xyz/gtxfhiylyv.html

TS:   // 同上
来源：http://hz.yueranfly.top/gtptnfgvnr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtzqeaphkj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cqqwz.cn/gtpvqkhdoy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenlongwang.top/gtlrvqwyos.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangshuangyany.cn/gtsorfvqxp.html

================================================================================
来源：http://hz.gaohongyu789.top/gtbxbzbznc.html

G. 面向对象
来源：http://hz.hywenlv.cn/gtgzmxbmwg.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbcrjvkpm.html

[G01] 定义类
来源：http://hz.zhengqikj.top/gtjvqmiysm.html

Py:   class User: pass
来源：http://hz.shangyingyoupin.top/gtjnbbbfbf.html

PHP:  class User {}
来源：http://hz.0kj1m.cn/gtmeoazwcg.html

JS:   class User {}
来源：http://hz.gogol.net.cn/gthndbshjk.html

TS:   class User { name: string = ""; }
来源：http://hz.jianghu66.top/gtstaqblhj.html

Java: class User {}
来源：http://hz.ybcxt.top/gtscuccelx.html

Go:   type User struct { Name string }
来源：http://hz.feifeiyinyue.top/gtmbhvpzer.html

Ruby: class User; end
来源：http://hz.bjfxy.top/gtlgkotvun.html

C#:   class User {}
来源：http://hz.sweek.top/gteazfawyx.html

[G02] 构造函数
来源：http://hz.yanxiufei.cn/gtxyalocwy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gzhubu.top/gtiaoeswsf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.kuanghao11.cn/gttmfavfwj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtkzxzfjaa.html

TS:   constructor(public name: string) {}
来源：http://hz.svipenyu.cn/gtwcvftwmt.html

Java: User(String name) { this.name = name; }
来源：http://hz.fengsongda.top/gtvmgfinbd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhengqikj.top/gtkauoivos.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sysykeji.top/gtnrnhsual.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ivvv.top/gtmhdyrzrt.html

[G03] 实例属性
来源：http://hz.9152youxi.cn/gtbfamspfr.html

Py:   self.name = "x"
来源：http://hz.yj202588.top/gtljgxshpx.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gtvwjhpkhc.html

JS:   this.name = "x";
来源：http://hz.52xcode.cn/gtveddwxbu.html

TS:   name: string = "x";
来源：http://hz.c1oappe.top/gtfbgixtqv.html

Java: private String name;
来源：http://hz.yanxiufei.cn/gtdxcyzzjn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinyuanbaomall.cn/gthfjfvjmu.html

Ruby: @name = "x"
来源：http://hz.nanxuanxn.top/gtovvgfzks.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgufenzy.top/gtsfrtbdyl.html

[G04] 定义方法
来源：http://hz.yj202588.top/gtxdsiufvq.html

Py:   def greet(self): return self.name
来源：http://hz.haohaochexian.top/gtnwkrdzta.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtdufdvttk.html

JS:   greet() { return this.name; }
来源：http://hz.daxiang520.top/gteylqxxbl.html

TS:   greet(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtjxshgbsd.html

Java: String greet() { return name; }
来源：http://hz.tanke756.top/gtdzuyalbz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hywenlv.cn/gtwpuswadl.html

Ruby: def greet; @name; end
来源：http://hz.haohaochexian.top/gtretoierx.html

C#:   public string Greet() => Name;
来源：http://hz.havefunace.top/gttdugpcoo.html

[G05] 继承
来源：http://hz.sufxvd.cn/gtywzpnkrw.html

Py:   class Admin(User): pass
来源：http://hz.ppjwa.cn/gtawjmwirg.html

PHP:  class Admin extends User {}
来源：http://hz.daria6918.cn/gtkjfvfiod.html

JS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtbnrpiagz.html

TS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtfwdhyvqx.html

Java: class Admin extends User {}
来源：http://hz.jyoumei.cn/gtfveyxnjj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zycfv.cn/gthbkdkvfj.html

Ruby: class Admin < User; end
来源：http://hz.chenjidiqi.icu/gtprcyuium.html

C#:   class Admin : User {}
来源：http://hz.yonumen.top/gtpikvlsdb.html

[G06] 重写方法
来源：http://hz.hysaishi.cn/gthxygnhie.html

Py:   def greet(self): return "admin"
来源：http://hz.hywenlv.cn/gtpumvzhqn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.fengsongda.top/gtydsusrnl.html

JS:   greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtcopimmmu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtuufkmwoy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtziqdrfvq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnqzz.top/gtevzmvoot.html

Ruby: def greet; "admin"; end
来源：http://hz.zhijiandao.cn/gtazsscfgy.html

C#:   public override string Greet() => "admin";
来源：http://hz.dianchejie.cn/gtlvqnjcpp.html

[G07] 调用父类方法
来源：http://hz.yj20258.top/gtqwpaesic.html

Py:   super().greet()
来源：http://hz.hnqzz.top/gtvagswetx.html

PHP:  parent::greet();
来源：http://hz.yvedp.cn/gtzgtjerug.html

JS:   super.greet();
来源：http://hz.gotoacloud.top/gtgdaibpxo.html

TS:   super.greet();
来源：http://hz.jiagoushi.top/gtiexragbg.html

Java: super.greet();
来源：http://hz.jinqigufen.top/gtjxxzuzzt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jiagoushi.top/gtdicfojzj.html

Ruby: super
来源：http://hz.jqgfzy.top/gtxaqqomsh.html

C#:   base.Greet();
来源：http://hz.ydjk.org.cn/gtkwyzyzjn.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtlghjhssf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cucudq.cn/gtrojaoxyw.html

PHP:  public static function f() {}
来源：http://hz.redwolf501.top/gtnllytjjj.html

JS:   static f() {}
来源：http://hz.hnqzz.top/gtytuzwbxm.html

TS:   static f(): void {}
来源：http://hz.jinghuilouyu.cn/gtxrqberhl.html

Java: static void f() {}
来源：http://hz.yonumen.top/gtwuaundzs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.aizwys.cn/gtcfmnzmcc.html

Ruby: def self.f; end
来源：http://hz.zhoulong.xyz/gthkcczxvm.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtkawaklil.html

[G09] 接口 / 抽象类
来源：http://hz.meibo888.top/gtpkyvtwzu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhiwuduotai.top/gttobbfomt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daxiang520.top/gtepoiwxio.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangtech.top/gtpohnzvjq.html

TS:   interface Shape { area(): number; }
来源：http://hz.cashguo.top/gtfxdaeyui.html

Java: interface Shape { double area(); }
来源：http://hz.fzhhl.top/gtawtuuabs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnqzz.top/gttrfikixc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jiagoushi.top/gtvmsrmjes.html

C#:   interface IShape { double Area(); }
来源：http://hz.fengsongda.top/gtvlrwwqyc.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gtjxpxikxr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gogol.net.cn/gtirrujnny.html

PHP:  public / protected / private
来源：http://hz.mhx1999.top/gtyfdtvmbw.html

JS:   #private 字段；其余公开
来源：http://hz.xylfe.cn/gtkyulkayk.html

TS:   public / protected / private
来源：http://hz.hnxiangtu.top/gtiozjqilz.html

Java: public / protected / private / 默认包级
来源：http://hz.chenzaomai.com/gtygtcrgnk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hammf.cn/gtkavcptxv.html

Ruby: public / protected / private
来源：http://hz.ivvv.top/gtnbwqsbfi.html

C#:   public / protected / private / internal
来源：http://hz.hammf.cn/gtptyilxeb.html

[G11] getter / setter
来源：http://hz.nanxuanxn.top/gtymezqbzr.html

Py:   @property 与 @x.setter
来源：http://hz.nanxinkj.top/gtduiuhwuo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtwgeilkcy.html

JS:   get name() { return this._name; }
来源：http://hz.kuanghao11.cn/gtlsfumkio.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgfzy.top/gtvlquouxw.html

Java: public String getName() { return name; }
来源：http://hz.hywenlv.cn/gtkscyqlsn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aizwys.cn/gtwzrfcjyd.html

Ruby: attr_accessor :name
来源：http://hz.gogol.net.cn/gtguvtbgft.html

C#:   public string Name { get; set; }
来源：http://hz.xuanzx.com/gtvsxtovvd.html

[G12] 对象转字符串
来源：http://hz.cqqwz.cn/gtrsptjklo.html

Py:   def __str__(self): return self.name
来源：http://hz.tanke756.top/gtdcwtfdkm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtbamhjubr.html

JS:   toString() { return this.name; }
来源：http://hz.sxryk.cn/gtftfqskqq.html

TS:   toString(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtuweqssxy.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtmpufpkkv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuanzx.com/gtzqgvwavu.html

Ruby: def to_s; @name; end
来源：http://hz.sweek.top/gtdzhhlgrg.html

C#:   public override string ToString() => Name;
来源：http://hz.mhx1999.top/gtpnohgflj.html

[G13] 判断对象类型
来源：http://hz.redwolf501.top/gtkthhsqcd.html

Py:   isinstance(u, User)
来源：http://hz.yuxming.cn/gtovmguknj.html

PHP:  $u instanceof User
来源：http://hz.cucudq.cn/gtpmlscizx.html

JS:   u instanceof User
来源：http://hz.yangfankeji.com/gtaewgsbxl.html

TS:   u instanceof User
来源：http://hz.jinqigfzy.top/gtorhdlive.html

Java: u instanceof User
来源：http://hz.yangfankeji.com/gtrhuztugq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ivvv.top/gtinjfjxtk.html

Ruby: u.is_a?(User)
来源：http://hz.smart0.xyz/gtcgdfiiwo.html

C#:   u is User
来源：http://hz.gogol.net.cn/gtgalaxzmv.html

[G14] 数据类 / record
来源：http://hz.xuanzx.com/gtyukmjcwt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.iojbl.cn/gtzsvlznuv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nwbrower.top/gtyvkrmzsd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnqzz.top/gtdbrnvbbr.html

TS:   type User = { name: string; age: number };
来源：http://hz.hongshengwenyu.top/gtwnqtlhfp.html

Java: record User(String name, int age) {}
来源：http://hz.jinghuilouyu.cn/gterqkwhru.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ywan-chungtsiang.top/gtdimbbzib.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.kuanghao11.cn/gtjbsfvogm.html

C#:   record User(string Name, int Age);
来源：http://hz.bjfxy.top/gtyqcciskw.html

[G15] 枚举
来源：http://hz.pengpengdd.cyou/gtdzgautzv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cheryme.top/gtbxhbtluy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yanxiufei.cn/gtwfbkpdwr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxinkj.top/gtpapplrbt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gthwylzqtm.html

Java: enum Color { RED, GREEN }
来源：http://hz.yongpay.top/gtxzwbfzjk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xziqi.cn/gtgwgtfawr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shzxlz.cn/gtfjvcnqqy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gtxbokmczp.html

[G16] 对象转数组 / 字典
来源：http://hz.hysaishi.cn/gtlirqdndz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tanke756.top/gtaouqvkap.html

PHP:  get_object_vars($obj);
来源：http://hz.hfpthk.cn/gtpsncuxfc.html

JS:   Object.entries(obj)
来源：http://hz.zhiwuduotai.top/gtcmfisdvl.html

TS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtxwbdanww.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.fengsongda.top/gtuqbbwpfc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.vqdsnc.cn/gtdsgucimt.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangtech.top/gtnnnyyolj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sysykeji.top/gtgugrygko.html

================================================================================
来源：http://hz.guannengcc.top/gtqhyeuiln.html

H. 异常与错误处理
来源：http://hz.jiagoushi.top/gtetichjfs.html

================================================================================
来源：http://hz.dashuyun.cn/gtqwmvyxps.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gtsefpaeln.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cashguo.top/gtllpvnepa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.snrcjt.cn/gthfexvvnr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtvdikuzbo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sufxvd.cn/gtiokgdfbx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinyuanbaomall.cn/gttxymgzdb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gtvimqrvrx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sufxvd.cn/gtdeeexwjn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258.top/gtrgtjdaeu.html

[H02] finally / ensure 收尾
来源：http://hz.cqqwz.cn/gtkzsosira.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigfzy.top/gtztxqsrqi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtmhdncgok.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtpevlubpj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtassvzaay.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtpqsxwsyn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydjk.org.cn/gtjhlpdckx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jlsjyb.cn/gtsykjrdqt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hysaishi.cn/gtwpsxhvws.html

[H03] 主动抛出异常
来源：http://hz.jqgfzy.top/gtkjdaivfa.html

Py:   raise ValueError("错误信息")
来源：http://hz.havefunace.top/gtglxrnxzn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtqljmzdjg.html

JS:   throw new Error("错误信息");
来源：http://hz.yueranfly.top/gtlkncdabn.html


<!-- 参考信息 -->