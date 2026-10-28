代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtfwataome.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.9152youxi.cn/gtvyrtdufv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtmpteyqks.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gtgidlkcom.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hysaishi.cn/gtgtkyngnt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhixingplan.top/gtlmtbtshh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yongpay.top/gtprwkidws.html

Ruby: s.bytesize;  s.length
来源：http://hz.xinyue.icu/gtfkxebahe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhoulong.xyz/gtpwkogwte.html

================================================================================
来源：http://hz.316326.xyz/gtwxeqexxd.html

F. 文件与目录
来源：http://hz.hfpthk.cn/gthecdcigm.html

================================================================================
来源：http://hz.yj202588.top/gtsfyotkwr.html

[F01] 读取整个文件
来源：http://hz.zhaomingkeji.xyz/gtauzptjtx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pengpengdd.cyou/gtswgizsxv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cashguo.top/gtsempkhba.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hywenlv.cn/gtalhwaaso.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gzhubu.top/gtliejtzvj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtlsogscyt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.vqdsnc.cn/gtbhlqjuje.html

Ruby: File.read("a.txt")
来源：http://hz.yongpay.top/gtcplwfusi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhoulong.xyz/gtepyxvyak.html

[F02] 逐行读取文件
来源：http://hz.hnxiangtu.top/gtjvqebbrd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yueranfly.top/gtejflgaaw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuxming.cn/gtnbwlulqb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shangyingyoupin.top/gtldjbazca.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jiagoushi.top/gtffsdboin.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtzfmhihkc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xziqi.cn/gtdrolgvnj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258.top/gtbrfylaln.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhiwuduotai.top/gtmszibpag.html

[F03] 写入文件（覆盖）
来源：http://hz.zhixingplan.top/gthwfvwcyn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cashguo.top/gtgakmeetv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.birdmap.top/gtdvmqvtri.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.havefunace.top/gtquooupbu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtriwyvwbf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zdqjudy.top/gtdzesuukx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.quarkkingdee.top/gtiljedvll.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinyuanbaomall.cn/gtssihsqtu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ivvv.top/gtvpagnjnt.html

[F04] 追加写入文件
来源：http://hz.zhijiandao.cn/gtzczsxigc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jianghu66.top/gtrdzeziti.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jlsjyb.cn/gtsztxemow.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtlarpzewy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gtfrgnjmvg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinghuilouyu.cn/gtntxjgwkt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hongshengwenyu.top/gtnfdntnez.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shuidangran.top/gtugutlfac.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nanxuanxn.top/gtudkxnehj.html

[F05] 判断文件或目录是否存在
来源：http://hz.vqdsnc.cn/gtfzyngqii.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gogol.net.cn/gtnqsmynjc.html

PHP:  file_exists("a.txt");
来源：http://hz.xuanzx.com/gtrttdleam.html

JS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gtyyntqhau.html

TS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtahrfdpwz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtznjxugvu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.haohaochexian.top/gtrapatkba.html

Ruby: File.exist?("a.txt")
来源：http://hz.ehwqpu.com/gtbgbncyvj.html

C#:   File.Exists("a.txt")
来源：http://hz.yuanzhike.top/gtccdjewjs.html

[F06] 删除文件
来源：http://hz.jqgfzy.top/gtrsptsvpg.html

Py:   os.remove("a.txt")
来源：http://hz.jinqigufen.top/gtoqihpjmn.html

PHP:  unlink("a.txt");
来源：http://hz.iojbl.cn/gtdxcoxttt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sufxvd.cn/gthoriczhy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jianghu66.top/gtckfrepqj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtxubwmjlu.html

Go:   os.Remove("a.txt")
来源：http://hz.andypj.xyz/gtaknzoyle.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gtteyopqbe.html

C#:   File.Delete("a.txt");
来源：http://hz.kuanghao11.cn/gtnqyilbya.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gtmjmvoooe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.feifeiyinyue.top/gtinyxrkki.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sxryk.cn/gtivvkzwxj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zycfv.cn/gtnnwisqnp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuanzx.com/gtyewfzntv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jianghu66.top/gturrqmvtj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.feifeiyinyue.top/gtxqczmbok.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jqgfzy.top/gtefiydzks.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jiagoushi.top/gtrqqxolem.html

[F08] 遍历目录
来源：http://hz.yj20258888.top/gtzxplbrgt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xingfuxueyuan.xyz/gthndmzddu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.meibo888.top/gtpaigxxzy.html

JS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gtjhnssint.html

TS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtcamuhpxn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtdwrhrchm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhongyouzk.top/gttxeoppow.html

Ruby: Dir.children("dir")
来源：http://hz.tanke756.top/gtoqvyjyqk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ehwqpu.com/gtraqrucmh.html

[F09] 获取文件大小
来源：http://hz.jinqigfzy.top/gtsgkryrcb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.svipenyu.cn/gtkavjeysk.html

PHP:  filesize("a.txt");
来源：http://hz.haohaochexian.top/gtqsoellmi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gaohongyu789.top/gtcjasirpr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gtkcbvxdta.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtztgskcgk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tanke756.top/gtkiczrwtv.html

Ruby: File.size("a.txt")
来源：http://hz.mhx1999.top/gtqrclcpdz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangtech.top/gttfuddhdm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cashguo.top/gtmcjwlchh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtlvbmailv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hammf.cn/gtqqzslmim.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtrlvettpe.html

TS:   path.extname("a.txt")
来源：http://hz.nwbrower.top/gtzkbratnr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aibaodan.cn/gtspivhnry.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yongpay.top/gtlokpirch.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtcotvuqff.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.aibaodan.cn/gttuskrhih.html

[F11] 复制与移动文件
来源：http://hz.zhijiandao.cn/gtovvnkpnk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtrxabcyuk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cucudq.cn/gtpuylgypo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtuonvxaqy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtovsgvvzv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhiwuduotai.top/gtgpogjept.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xylfe.cn/gtiafssvmc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sweek.top/gtixssghfn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pengpengdd.cyou/gtwyocivju.html

[F12] CSV 读写
来源：http://hz.dianchejie.cn/gthtwaabbh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gtzbmfoiac.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yongpay.top/gtxnxiqecw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gotoacloud.top/gtjqqvetad.html

TS:   // 同上
来源：http://hz.yonumen.top/gtasybycou.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yongpay.top/gtiprigefq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shuidangran.top/gtichpqest.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.redwolf501.top/gtyuynsgwc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.meibo888.top/gtirfdwmsu.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtfjqffaxy.html

G. 面向对象
来源：http://hz.jianghu66.top/gtvmxbimjf.html

================================================================================
来源：http://hz.zycfv.cn/gtfvyizgyl.html

[G01] 定义类
来源：http://hz.hysaishi.cn/gtsjnfcxbc.html

Py:   class User: pass
来源：http://hz.kuanghao11.cn/gtgbyzgzbq.html

PHP:  class User {}
来源：http://hz.wangdashe.top/gtixmydvtk.html

JS:   class User {}
来源：http://hz.yongpay.top/gtcabznsvq.html

TS:   class User { name: string = ""; }
来源：http://hz.shangyingyoupin.top/gtyujoyxwl.html

Java: class User {}
来源：http://hz.0kj1m.cn/gtjdpxybrn.html

Go:   type User struct { Name string }
来源：http://hz.cucudq.cn/gtpfjhlwzg.html

Ruby: class User; end
来源：http://hz.zhongyouzk.top/gtkjrauqzo.html

C#:   class User {}
来源：http://hz.jinyuanbaomall.cn/gtgxuzqpew.html

[G02] 构造函数
来源：http://hz.hywenlv.cn/gtuvtojswm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangkeji.top/gtfwxmnnqb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtrvyvxaot.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258888.top/gtcceuznjy.html

TS:   constructor(public name: string) {}
来源：http://hz.nwbrower.top/gtuvnqywnz.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenlongwang.top/gttjqegthh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.svipenyu.cn/gtdazmscfr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gtjyuvpobb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ivvv.top/gtxqzqiwvk.html

[G03] 实例属性
来源：http://hz.smart0.xyz/gtvhuipcdt.html

Py:   self.name = "x"
来源：http://hz.sweek.top/gthnzlducf.html

PHP:  public string $name = "x";
来源：http://hz.svipenyu.cn/gtqtlgvbyw.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gtrnurutyj.html

TS:   name: string = "x";
来源：http://hz.dianchejie.cn/gttjkgvdal.html

Java: private String name;
来源：http://hz.hysaishi.cn/gttarnonhj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenzaomai.com/gtmhbiuudj.html

Ruby: @name = "x"
来源：http://hz.zhixingplan.top/gtmuieqynu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tianlin.xyz/gtudoocrwl.html

[G04] 定义方法
来源：http://hz.yangfankeji.com/gtcuxhhuqx.html

Py:   def greet(self): return self.name
来源：http://hz.zhengqikj.top/gtnkfrwjbg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.316326.xyz/gtflyogwpi.html

JS:   greet() { return this.name; }
来源：http://hz.fengsongda.top/gtcuwlnhue.html

TS:   greet(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtpcuxwios.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gtyuaqilei.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuanzx.com/gtuvfjttbv.html

Ruby: def greet; @name; end
来源：http://hz.hammf.cn/gthgnafqem.html

C#:   public string Greet() => Name;
来源：http://hz.yj20258888.top/gtfygggvzs.html

[G05] 继承
来源：http://hz.jinghuilouyu.cn/gtwyaecpcr.html

Py:   class Admin(User): pass
来源：http://hz.yvedp.cn/gtnscikgve.html

PHP:  class Admin extends User {}
来源：http://hz.guowangkeji.top/gtlxpbybag.html

JS:   class Admin extends User {}
来源：http://hz.zhixingplan.top/gtdnqilpkb.html

TS:   class Admin extends User {}
来源：http://hz.jqgfzy.top/gtthnzbykw.html

Java: class Admin extends User {}
来源：http://hz.yj20258888.top/gtocqkysoh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.guowangkeji.top/gtzcyptmsg.html

Ruby: class Admin < User; end
来源：http://hz.cashguo.top/gtcyyqqqck.html

C#:   class Admin : User {}
来源：http://hz.zhaomingkeji.xyz/gteccgwvzz.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gtagjjxvqp.html

Py:   def greet(self): return "admin"
来源：http://hz.jinyuanbaomall.cn/gtjfqnhqvl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuanzx.com/gtwcfocple.html

JS:   greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtypjhonyh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtohhhktkx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtbawcfehz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xingfuxueyuan.xyz/gtwxmikhgh.html

Ruby: def greet; "admin"; end
来源：http://hz.jlsjyb.cn/gtszvxtxlv.html

C#:   public override string Greet() => "admin";
来源：http://hz.tian-w.cn/gtidpfgqju.html

[G07] 调用父类方法
来源：http://hz.xuetiantiany.cn/gthydjinbt.html

Py:   super().greet()
来源：http://hz.zhaomingkeji.xyz/gtexpnfspk.html

PHP:  parent::greet();
来源：http://hz.ehwqpu.com/gtywwjkxfw.html

JS:   super.greet();
来源：http://hz.c1oappe.top/gtlkwmjnko.html

TS:   super.greet();
来源：http://hz.yj202588.top/gtzamyfgzg.html

Java: super.greet();
来源：http://hz.shanyushiyangkeji.top/gtmycbocdr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guannengcc.top/gtcviyjxwj.html

Ruby: super
来源：http://hz.cqqwz.cn/gtdigycggr.html

C#:   base.Greet();
来源：http://hz.c1oappe.top/gtqbhdzvaq.html

[G08] 静态方法与属性
来源：http://hz.nanxuanxn.top/gttvpcknda.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zycfv.cn/gtcdleppmp.html

PHP:  public static function f() {}
来源：http://hz.hysaishi.cn/gtncettndf.html

JS:   static f() {}
来源：http://hz.redwolf501.top/gtbdrjssiz.html

TS:   static f(): void {}
来源：http://hz.nanxinkj.top/gtmssjlwxz.html

Java: static void f() {}
来源：http://hz.mhx1999.top/gtbabkyfqi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhiwuduotai.top/gtsjxymcvj.html

Ruby: def self.f; end
来源：http://hz.wangdashe.top/gtekfymtui.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtjpbxitlw.html

[G09] 接口 / 抽象类
来源：http://hz.pycfn.com/gttkffvlin.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.haohaochexian.top/gtbzwtrupo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinyuanbaomall.cn/gthvnnvfgu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhiwuduotai.top/gtzxcoguwx.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhijiandao.cn/gttmlpiaqz.html

Java: interface Shape { double area(); }
来源：http://hz.zhixingplan.top/gtvsowvqjl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jlsjyb.cn/gtnkuqtoao.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.316326.xyz/gtclczadhj.html

C#:   interface IShape { double Area(); }
来源：http://hz.feifeiyinyue.top/gtifmktkof.html

[G10] 访问控制
来源：http://hz.yvedp.cn/gtpycsraao.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ivvv.top/gtvocmnwub.html

PHP:  public / protected / private
来源：http://hz.smart0.xyz/gtlcsjdvcj.html

JS:   #private 字段；其余公开
来源：http://hz.xziqi.cn/gtmcoucboj.html

TS:   public / protected / private
来源：http://hz.hammf.cn/gtcszdovoy.html

Java: public / protected / private / 默认包级
来源：http://hz.redwolf501.top/gtpeidykty.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pycfn.com/gtzjwjpisu.html

Ruby: public / protected / private
来源：http://hz.xuetiantiany.cn/gttdwuvlfw.html

C#:   public / protected / private / internal
来源：http://hz.wangdashe.top/gtadwotcek.html

[G11] getter / setter
来源：http://hz.yonumen.top/gtagzeltbb.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtjqinflqa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtzegbelau.html

JS:   get name() { return this._name; }
来源：http://hz.hysaishi.cn/gtvmouxtss.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gtrvdxwwhq.html

Java: public String getName() { return name; }
来源：http://hz.cheryme.top/gtwnotzwkj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hammf.cn/gtozgcomkz.html

Ruby: attr_accessor :name
来源：http://hz.haohaochexian.top/gtbixekgib.html

C#:   public string Name { get; set; }
来源：http://hz.ppjwa.cn/gtyajmbipe.html

[G12] 对象转字符串
来源：http://hz.smart0.xyz/gtpwpnxzua.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgfzy.top/gtgzfuqcar.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtjjxlvhhs.html

JS:   toString() { return this.name; }
来源：http://hz.xinyue.icu/gtdhepyrbf.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtyfdeszuu.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangtech.top/gtdimauzxi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.svipenyu.cn/gtpjjyicxx.html

Ruby: def to_s; @name; end
来源：http://hz.yj202588.top/gtgcnnmwym.html

C#:   public override string ToString() => Name;
来源：http://hz.xylfe.cn/gtvqbrgtbl.html

[G13] 判断对象类型
来源：http://hz.sxryk.cn/gtciakcmeq.html

Py:   isinstance(u, User)
来源：http://hz.jqgfzy.top/gtipmachfk.html

PHP:  $u instanceof User
来源：http://hz.yj202588.top/gtpihbsatc.html

JS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtwexsizlj.html

TS:   u instanceof User
来源：http://hz.haohaochexian.top/gtcfyqignj.html

Java: u instanceof User
来源：http://hz.zycfv.cn/gtuhphcbfc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.svipenyu.cn/gtnrslykma.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtmjjjecxb.html

C#:   u is User
来源：http://hz.gotoacloud.top/gtyiedseap.html

[G14] 数据类 / record
来源：http://hz.sweek.top/gtxjqmzkdu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangkeji.top/gtznxurjnu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hywenlv.cn/gtpqzctbii.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.smart0.xyz/gtwxenxibh.html

TS:   type User = { name: string; age: number };
来源：http://hz.cheryme.top/gtqgodcczt.html

Java: record User(String name, int age) {}
来源：http://hz.jiagoushi.top/gtlyaxcfea.html

Go:   type User struct { Name string; Age int }
来源：http://hz.snrcjt.cn/gtjksapuoy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zdqjudy.top/gtmtbdsbis.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgfzy.top/gtokcbmosb.html

[G15] 枚举
来源：http://hz.sxryk.cn/gtxhljqagj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jiagoushi.top/gtuvnbjpuy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jqgfzy.top/gtplspoiqm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgfzy.top/gtxrofnjbm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtkawrwdmy.html

Java: enum Color { RED, GREEN }
来源：http://hz.zycfv.cn/gtplyntmqz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangdashe.top/gtlcuoddde.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shuidangran.top/gthavduyam.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtywoidoeh.html

[G16] 对象转数组 / 字典
来源：http://hz.316326.xyz/gtrjngzwbm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fengsongda.top/gtgvhirkme.html

PHP:  get_object_vars($obj);
来源：http://hz.shanyushiyangtech.top/gteovxlohh.html

JS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtkqlzyexe.html

TS:   Object.entries(obj)
来源：http://hz.tian-w.cn/gthcipfxde.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cucudq.cn/gtjjqframu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtlrknnocf.html

Ruby: obj.instance_variables
来源：http://hz.yongpay.top/gtinmlitzf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shzxlz.cn/gtadmgtxiw.html

================================================================================
来源：http://hz.fengsongda.top/gtprjvawvo.html

H. 异常与错误处理
来源：http://hz.iojbl.cn/gtqyfxzhyo.html

================================================================================
来源：http://hz.gotoacloud.top/gtqgamwicl.html

[H01] try / catch 基础
来源：http://hz.zdqjudy.top/gtsncznqtd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.mhx1999.top/gtpiiegimm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nwbrower.top/gtdtxjnvzm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.bjfxy.top/gthqidpyiw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hammf.cn/gtjshlmkns.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenzaomai.com/gtryinbvuq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinyuanbaomall.cn/gtrtuumcmn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yuxming.cn/gtjxvholkz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cucudq.cn/gtoikdkrps.html

[H02] finally / ensure 收尾
来源：http://hz.xuanzx.com/gtovrmknrj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.tianlin.xyz/gtttccjibu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtntfmqipg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtwjgckrhu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtpcxvjjyz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtrdkdcrqo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cheryme.top/gtntlytdwf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.dianchejie.cn/gtikhuogfg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhengqikj.top/gtuvjevzwt.html

[H03] 主动抛出异常
来源：http://hz.hywenlv.cn/gtlhpndpmj.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj202588.top/gtlreanyrz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtalzjkezy.html

JS:   throw new Error("错误信息");
来源：http://hz.yonumen.top/gtmjrourkr.html

TS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gtyvnzyisb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtdlmjsyuk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtfeikqpjg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinqigfzy.top/gtchldapav.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtrwxjrmhy.html

[H04] 自定义异常类型
来源：http://hz.cqqwz.cn/gtzohivfuh.html

Py:   class MyError(Exception): pass
来源：http://hz.pengpengdd.cyou/gtjpwtfdnn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gthjmsjtdw.html


<!-- 参考信息 -->