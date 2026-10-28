代发 wailian999

[E22] 字节长度与字符长度
来源：http://hz.gzhubu.top/gttvfcfyef.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinyuanbaomall.cn/gtbngieysu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtdtfrgdlg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sysykeji.top/gtncxbpqbv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gtmoxhqgde.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtwhixtjoj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hywenlv.cn/gtprteckuy.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhoulong.xyz/gtvitsoapo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sweek.top/gthuyfrzhp.html

================================================================================
来源：http://hz.yj202588.top/gtqgcvzhqd.html

F. 文件与目录
来源：http://hz.sufxvd.cn/gtpxfupxxm.html

================================================================================
来源：http://hz.ehwqpu.com/gtuxmrskdg.html

[F01] 读取整个文件
来源：http://hz.andypj.xyz/gtztelwofk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tian-w.cn/gtbvfnmpyj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aibaodan.cn/gtpeaqqaqc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xziqi.cn/gtthhgvfsk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydjk.org.cn/gtpvsbprjj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtzqbfasjd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yanxiufei.cn/gtwibnxtth.html

Ruby: File.read("a.txt")
来源：http://hz.daria6918.cn/gtrnsknkrl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.snrcjt.cn/gtdlkyfhnz.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangkeji.top/gtifzugwof.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nanxinkj.top/gtvmcpvyjf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xylfe.cn/gtdwqubngg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gtffquklkj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gotoacloud.top/gtqhcvtopk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtkllliwww.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhongyouzk.top/gtailcoarm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hywenlv.cn/gtqbftopnf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigfzy.top/gtgcveluic.html

[F03] 写入文件（覆盖）
来源：http://hz.chenjidiqi.icu/gtyvnnghqr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhongyouzk.top/gtifjskkef.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtudtwhnyg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shangyingyoupin.top/gtrsaykrqj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gtwspxusns.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cheryme.top/gtpvekwpzg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhaomingkeji.xyz/gtrkkhcqxf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhijiandao.cn/gtztrprmnb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.mhx1999.top/gtbvwsymew.html

[F04] 追加写入文件
来源：http://hz.guannengcc.top/gthzfaytew.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yongpay.top/gtrtbabbcx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhijiandao.cn/gtpmugrebj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xinyue.icu/gtmceliusg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtfoiomczl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.wangdashe.top/gtnriynxeg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.andypj.xyz/gtsrsqiokn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cdnleiting.top/gtevytmsuu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.fengsongda.top/gtjtjgiifu.html

[F05] 判断文件或目录是否存在
来源：http://hz.xingfuxueyuan.xyz/gtvwlqtyho.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xziqi.cn/gtmbktmoek.html

PHP:  file_exists("a.txt");
来源：http://hz.xuetiantiany.cn/gtgcxljmxz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gteumgfuby.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtgeomqvma.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtouseustl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gotoacloud.top/gtibrtcqwl.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhixingplan.top/gtmxsrdcij.html

C#:   File.Exists("a.txt")
来源：http://hz.shangyingyoupin.top/gtmxusouei.html

[F06] 删除文件
来源：http://hz.52xcode.cn/gttulrbyll.html

Py:   os.remove("a.txt")
来源：http://hz.aizwys.cn/gteybripst.html

PHP:  unlink("a.txt");
来源：http://hz.ybcxt.top/gtbnapwmdz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shuidangran.top/gtlkoaoizc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yongpay.top/gtbbirtefh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtuawgcwua.html

Go:   os.Remove("a.txt")
来源：http://hz.sysykeji.top/gtolyjlgnx.html

Ruby: File.delete("a.txt")
来源：http://hz.iojbl.cn/gtipomcltn.html

C#:   File.Delete("a.txt");
来源：http://hz.dashuyun.cn/gtqdxqqnhn.html

[F07] 创建目录（含多级）
来源：http://hz.fzhhl.top/gtshjowjcj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fengsongda.top/gtgcvuvstc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zdqjudy.top/gtsjwoydvn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gtjnjaxcyx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cqqwz.cn/gtpntuyezw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.feifeiyinyue.top/gtvccjbvvh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ehwqpu.com/gtshmoonvj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hywenlv.cn/gtnvjobihj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.iojbl.cn/gtfdejpgux.html

[F08] 遍历目录
来源：http://hz.hnxiangtu.top/gtrxpfmeuc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nwbrower.top/gtcfhgmgos.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yvedp.cn/gtstczksnd.html

JS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtihvhabue.html

TS:   fs.readdirSync("dir")
来源：http://hz.daxiang520.top/gtaqholezr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yonumen.top/gtetsztukv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.quarkkingdee.top/gtgelodtyz.html

Ruby: Dir.children("dir")
来源：http://hz.quarkkingdee.top/gtarwwruxw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.smart0.xyz/gtvnmqdiya.html

[F09] 获取文件大小
来源：http://hz.gotoacloud.top/gtdwxlwakq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gtglcoxzvj.html

PHP:  filesize("a.txt");
来源：http://hz.tanke756.top/gtkrzucxng.html

JS:   fs.statSync("a.txt").size
来源：http://hz.fengsongda.top/gtdwhjvjnj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gtodgsxkyy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtblrmgcyu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jiagoushi.top/gtugawqhyt.html

Ruby: File.size("a.txt")
来源：http://hz.hysaishi.cn/gtfhokjvhr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yueranfly.top/gtqmqbdyhp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shangyingyoupin.top/gtwtqrcwsn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtxepimvfq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.wangdashe.top/gtrhruggdh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtxjdkxhyr.html

TS:   path.extname("a.txt")
来源：http://hz.xinyue.icu/gtolsvitjm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydjk.org.cn/gtssumobxz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sweek.top/gtdwfqbmwh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtobpxsyml.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.c1oappe.top/gttzrgjhjf.html

[F11] 复制与移动文件
来源：http://hz.ppjwa.cn/gtgmthmrpr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtwfxtjmqb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shangyingyoupin.top/gtlvvxwwgw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtcvlbdihz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtrcwoljhd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yueranfly.top/gtbycqdchp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.redwolf501.top/gtzeihczny.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtxcbdxywc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guowangkeji.top/gtnaizpefp.html

[F12] CSV 读写
来源：http://hz.ydjk.org.cn/gthvkjhkao.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.bjfxy.top/gtawoljfvi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nwbrower.top/gtkspbkbmd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tanke756.top/gthrdbcgra.html

TS:   // 同上
来源：http://hz.jinqigufen.top/gtjeucgmnf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.vqdsnc.cn/gthgqannjt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cdnleiting.top/gtxdsxqbpf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnxiangtu.top/gtcbymmaim.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hfpthk.cn/gtovtzbtxg.html

================================================================================
来源：http://hz.hammf.cn/gtpkeqsqvq.html

G. 面向对象
来源：http://hz.cashguo.top/gtmymqxomo.html

================================================================================
来源：http://hz.yonumen.top/gtbzcyotqb.html

[G01] 定义类
来源：http://hz.andypj.xyz/gtatootofr.html

Py:   class User: pass
来源：http://hz.fzhhl.top/gtobnfmgkj.html

PHP:  class User {}
来源：http://hz.hongshengwenyu.top/gtxagukdis.html

JS:   class User {}
来源：http://hz.tian-w.cn/gtyfpwausm.html

TS:   class User { name: string = ""; }
来源：http://hz.pycfn.com/gtohttanyg.html

Java: class User {}
来源：http://hz.zhongyouzk.top/gtutthjkbh.html

Go:   type User struct { Name string }
来源：http://hz.yanxiufei.cn/gteyctmrpe.html

Ruby: class User; end
来源：http://hz.zhijiandao.cn/gtozasbltv.html

C#:   class User {}
来源：http://hz.c1oappe.top/gtqmwtbbtm.html

[G02] 构造函数
来源：http://hz.chenlongwang.top/gtabmxgyjy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nwbrower.top/gttajrmbse.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xinyue.icu/gtyvkpaxqj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gtdgoeydyh.html

TS:   constructor(public name: string) {}
来源：http://hz.nanxinkj.top/gtijeslqdb.html

Java: User(String name) { this.name = name; }
来源：http://hz.cucudq.cn/gtooogrgbl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtazkbuzga.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinqigfzy.top/gtwjijyldh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sufxvd.cn/gtmipqovar.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gtdodnezmo.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtjqdagxba.html

PHP:  public string $name = "x";
来源：http://hz.yj202588.top/gtykxemogf.html

JS:   this.name = "x";
来源：http://hz.yueranfly.top/gtvyjmavmi.html

TS:   name: string = "x";
来源：http://hz.wangdashe.top/gtdfabpstj.html

Java: private String name;
来源：http://hz.daria6918.cn/gtygfwfkuf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinqigfzy.top/gtphoxfpae.html

Ruby: @name = "x"
来源：http://hz.guowangkeji.top/gtfsmzhrmc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.svipenyu.cn/gtnrerjvez.html

[G04] 定义方法
来源：http://hz.jinghuilouyu.cn/gtraehajdv.html

Py:   def greet(self): return self.name
来源：http://hz.andypj.xyz/gtyyhucivw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.316326.xyz/gtmrlubqkz.html

JS:   greet() { return this.name; }
来源：http://hz.xylfe.cn/gtqfkpxihb.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtweyjgfyq.html

Java: String greet() { return name; }
来源：http://hz.jinyuanbaomall.cn/gthaaasuaf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gogol.net.cn/gtryidmilh.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtjbkwaafr.html

C#:   public string Greet() => Name;
来源：http://hz.aibaodan.cn/gtjbwwnfiw.html

[G05] 继承
来源：http://hz.cucudq.cn/gtgmnycbap.html

Py:   class Admin(User): pass
来源：http://hz.shangyingyoupin.top/gtkqlhsywu.html

PHP:  class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtcbvlkmod.html

JS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtqoycboaw.html

TS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtctttmyvp.html

Java: class Admin extends User {}
来源：http://hz.gzhubu.top/gtjxukfmbh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sufxvd.cn/gtthoxbzhg.html

Ruby: class Admin < User; end
来源：http://hz.tian-w.cn/gtkeplefka.html

C#:   class Admin : User {}
来源：http://hz.shuidangran.top/gtrkabsrgj.html

[G06] 重写方法
来源：http://hz.zdqjudy.top/gtwssqocpj.html

Py:   def greet(self): return "admin"
来源：http://hz.gzhubu.top/gtbvfjgkka.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtbyicalas.html

JS:   greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtztkoktjb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gtemsovjao.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtmtsercqe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.fengsongda.top/gtysqhmtow.html

Ruby: def greet; "admin"; end
来源：http://hz.sweek.top/gtsbzycgtf.html

C#:   public override string Greet() => "admin";
来源：http://hz.tianlin.xyz/gtlhurxpoy.html

[G07] 调用父类方法
来源：http://hz.dianchejie.cn/gtstqinrcu.html

Py:   super().greet()
来源：http://hz.tanke756.top/gtulxizxop.html

PHP:  parent::greet();
来源：http://hz.bjfxy.top/gthodmesjc.html

JS:   super.greet();
来源：http://hz.svipenyu.cn/gtlfjsikob.html

TS:   super.greet();
来源：http://hz.haohaochexian.top/gtnxfsxybv.html

Java: super.greet();
来源：http://hz.feifeiyinyue.top/gtqolaqtdy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dianchejie.cn/gtnsppiolj.html

Ruby: super
来源：http://hz.jinghuilouyu.cn/gtnngfzoai.html

C#:   base.Greet();
来源：http://hz.aizwys.cn/gthljruqsf.html

[G08] 静态方法与属性
来源：http://hz.zhiwuduotai.top/gtwvaiqkhh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shzxlz.cn/gtnfodzurk.html

PHP:  public static function f() {}
来源：http://hz.jinghuilouyu.cn/gtdcsxzppa.html

JS:   static f() {}
来源：http://hz.guowangkeji.top/gtyphgrbaf.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtepqpqjls.html

Java: static void f() {}
来源：http://hz.c1oappe.top/gtupqtsnjq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuxming.cn/gtxvxiexbr.html

Ruby: def self.f; end
来源：http://hz.sweek.top/gtytltayyd.html

C#:   public static void F() {}
来源：http://hz.jinqigufen.top/gttmksxxxf.html

[G09] 接口 / 抽象类
来源：http://hz.hongshengwenyu.top/gtisgeyrlg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.c1oappe.top/gttcstgghg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangshuangyany.cn/gtvqibvxxb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pengpengdd.cyou/gtljwdoaco.html

TS:   interface Shape { area(): number; }
来源：http://hz.zdqjudy.top/gthgtxdzqv.html

Java: interface Shape { double area(); }
来源：http://hz.chenlongwang.top/gtsgkkdtfw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ehwqpu.com/gtcexizrvo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.snrcjt.cn/gtrbnzoczx.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgfzy.top/gteqavzlvw.html

[G10] 访问控制
来源：http://hz.zhiwuduotai.top/gtkoezsund.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sysykeji.top/gtfyuvitbw.html

PHP:  public / protected / private
来源：http://hz.ydjk.org.cn/gtdtgetwih.html

JS:   #private 字段；其余公开
来源：http://hz.316326.xyz/gtkczcpqxq.html

TS:   public / protected / private
来源：http://hz.meibo888.top/gtsfvgmwcw.html

Java: public / protected / private / 默认包级
来源：http://hz.svipenyu.cn/gtolpwkvtb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.iojbl.cn/gthmzdtaef.html

Ruby: public / protected / private
来源：http://hz.smart0.xyz/gtxrxamnhy.html

C#:   public / protected / private / internal
来源：http://hz.pengpengdd.cyou/gtcmdumpwa.html

[G11] getter / setter
来源：http://hz.yuanzhike.top/gtcgzqyjdq.html

Py:   @property 与 @x.setter
来源：http://hz.sufxvd.cn/gtanrnehpg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtnjijesdm.html

JS:   get name() { return this._name; }
来源：http://hz.jyoumei.cn/gtrnizktmi.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtewvblpqv.html

Java: public String getName() { return name; }
来源：http://hz.chenjidiqi.icu/gtkbyheura.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gzhubu.top/gtljqqpbgh.html

Ruby: attr_accessor :name
来源：http://hz.jiagoushi.top/gtytgzrdwq.html

C#:   public string Name { get; set; }
来源：http://hz.yuxming.cn/gttaumtjvb.html

[G12] 对象转字符串
来源：http://hz.yj20258.top/gtefzaffjt.html

Py:   def __str__(self): return self.name
来源：http://hz.svipenyu.cn/gtnqibzjwz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtormajmxl.html

JS:   toString() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtpkhcfvek.html

TS:   toString(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gtoxftupjd.html

Java: @Override public String toString() { return name; }
来源：http://hz.quarkkingdee.top/gtarojdtfz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gteqivkaje.html

Ruby: def to_s; @name; end
来源：http://hz.kuanghao11.cn/gtkkjapeta.html

C#:   public override string ToString() => Name;
来源：http://hz.zhiwuduotai.top/gtnftjyukt.html

[G13] 判断对象类型
来源：http://hz.nanxuanxn.top/gtkrefjvbf.html

Py:   isinstance(u, User)
来源：http://hz.jinghuilouyu.cn/gtcqkjwkqx.html

PHP:  $u instanceof User
来源：http://hz.hongshengwenyu.top/gtsdcdsjad.html

JS:   u instanceof User
来源：http://hz.mhx1999.top/gteaibkqby.html

TS:   u instanceof User
来源：http://hz.fzhhl.top/gthqoigjlv.html

Java: u instanceof User
来源：http://hz.chenjidiqi.icu/gtscqrqeoy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhiwuduotai.top/gtbkxhkmsf.html

Ruby: u.is_a?(User)
来源：http://hz.smart0.xyz/gtdavspksx.html

C#:   u is User
来源：http://hz.redwolf501.top/gtuwqliesq.html

[G14] 数据类 / record
来源：http://hz.dianchejie.cn/gtmlrkvfsn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhoulong.xyz/gtwcnarefc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.birdmap.top/gthssqptjf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gaohongyu789.top/gtlhmparyy.html

TS:   type User = { name: string; age: number };
来源：http://hz.jlsjyb.cn/gtiinvpjzm.html

Java: record User(String name, int age) {}
来源：http://hz.jlsjyb.cn/gtnvjgmwau.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hongshengwenyu.top/gthajmbmgu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.fengsongda.top/gttmfznrfs.html

C#:   record User(string Name, int Age);
来源：http://hz.sweek.top/gtkpewzmsw.html

[G15] 枚举
来源：http://hz.havefunace.top/gtqugfnmrv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zycfv.cn/gtwjojvywd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tanke756.top/gtezpabzop.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj202588.top/gtqhepmkxz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gtgbyktiil.html

Java: enum Color { RED, GREEN }
来源：http://hz.mhx1999.top/gtkoliondr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.snrcjt.cn/gtnlvootfa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shanyushiyangkeji.top/gtjfvtdmpv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtyvgxkorc.html

[G16] 对象转数组 / 字典
来源：http://hz.tian-w.cn/gtdtodqobn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yvedp.cn/gtxwqbhfas.html

PHP:  get_object_vars($obj);
来源：http://hz.ybcxt.top/gtroqossdj.html

JS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtdrbshzzw.html

TS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtotzyjgsz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydzc1.top/gtamugrgja.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yanxiufei.cn/gtxlswjbke.html

Ruby: obj.instance_variables
来源：http://hz.wangdashe.top/gtdfxtfcfg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigufen.top/gtsmbbzdzk.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqxcgfzmm.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gtwppzknus.html

================================================================================
来源：http://hz.ydzc1.top/gtaootiljb.html

[H01] try / catch 基础
来源：http://hz.tian-w.cn/gthtlzczqa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xuetiantiany.cn/gtzeympwfp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgufenzy.top/gtvghnfnuu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.316326.xyz/gtpvfbagor.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ybcxt.top/gtdvagjceg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydzc1.top/gtgdwquzaj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yanxiufei.cn/gtmksfliob.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtbtwjwztb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cheryme.top/gtpkmdqbbc.html

[H02] finally / ensure 收尾
来源：http://hz.daria6918.cn/gtpifsbdgf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.wangdashe.top/gtrwhdyrbu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtknxfkrfs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtcsbjroum.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtbrsujdvb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtivahcqsl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pycfn.com/gtliejdyyw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nwbrower.top/gtcyidgumn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.dashuyun.cn/gtrngrowwo.html

[H03] 主动抛出异常
来源：http://hz.zhiwuduotai.top/gtqoyitabr.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangdashe.top/gtfwfjwbby.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtubadjgcx.html

JS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gtbmmnpjct.html

TS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtnspxuhfu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtwnqlqega.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.316326.xyz/gtioyginxi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gaohongyu789.top/gtxqemdfhm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtxvilkbwz.html

[H04] 自定义异常类型
来源：http://hz.c1oappe.top/gtuuitcxhx.html

Py:   class MyError(Exception): pass
来源：http://hz.zhoulong.xyz/gtjrzutxei.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yongpay.top/gtjklwfsbp.html


<!-- 参考信息 -->