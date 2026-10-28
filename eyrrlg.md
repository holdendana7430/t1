代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.vqdsnc.cn/gtdlsgaaok.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtpbeewufl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.feifeiyinyue.top/gtdpfbnkvc.html

Ruby: File.read("a.txt")
来源：http://hz.52xcode.cn/gteupxwjml.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.redwolf501.top/gtgryqpbtj.html

[F02] 逐行读取文件
来源：http://hz.yongpay.top/gtbmxaztsm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xuetiantiany.cn/gttpzwrvtr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aizwys.cn/gtluvqdfjl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gtewpmyyxu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtegqafpja.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gtgbotjlbs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.snrcjt.cn/gtterrhnhr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.fengsongda.top/gtdufwjhrm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj20258888.top/gteevdcabs.html

[F03] 写入文件（覆盖）
来源：http://hz.yangfankeji.com/gtlkzysefj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.feifeiyinyue.top/gtkbomkszr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cashguo.top/gtusqklofi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenjidiqi.icu/gtnnnjntww.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ivvv.top/gtyutatqts.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tianlin.xyz/gtwmbqvckr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jianghu66.top/gtvxskpdbm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ehwqpu.com/gtvvpvynhs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jqgufenzy.top/gtvzfbpled.html

[F04] 追加写入文件
来源：http://hz.jiagoushi.top/gtjyjukqxi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cashguo.top/gtbgmufbar.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.316326.xyz/gtmsxweyrc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258888.top/gtrjlwvuzf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gtmfcvysoj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.smart0.xyz/gtpxttwfnj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yangfankeji.com/gtzgvzzsgm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yanxiufei.cn/gtjcsvnxyp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.fzhhl.top/gtnpelmmun.html

[F05] 判断文件或目录是否存在
来源：http://hz.jiagoushi.top/gtnwbcywfi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xuetiantiany.cn/gtizmxieua.html

PHP:  file_exists("a.txt");
来源：http://hz.redwolf501.top/gtoxcuxmqc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhixingplan.top/gtjymezulp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgfzy.top/gtzwxsxnxq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtvyvvhmya.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aibaodan.cn/gtemukijpb.html

Ruby: File.exist?("a.txt")
来源：http://hz.cashguo.top/gtybeeitps.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtuaabqhbe.html

[F06] 删除文件
来源：http://hz.zhiwuduotai.top/gtukolyvgq.html

Py:   os.remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtmjivtqwq.html

PHP:  unlink("a.txt");
来源：http://hz.tianlin.xyz/gtppdcsngk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtnzxduqgf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yongpay.top/gtljbaokeo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtnaepbrtq.html

Go:   os.Remove("a.txt")
来源：http://hz.guowangkeji.top/gtxwnkvbmr.html

Ruby: File.delete("a.txt")
来源：http://hz.c1oappe.top/gtnxlmhmpn.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258.top/gtfoetarnp.html

[F07] 创建目录（含多级）
来源：http://hz.xingfuxueyuan.xyz/gtqhfndkit.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fzhhl.top/gtwcxmamvb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.haohaochexian.top/gtubkcqlhm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtukdwlxbd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtitunoavn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.pycfn.com/gtqlaatmba.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.iojbl.cn/gthhexhiqx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.0kj1m.cn/gtoipsnwjx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.iojbl.cn/gtkzohonar.html

[F08] 遍历目录
来源：http://hz.ywan-chungtsiang.top/gttnklappu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.0kj1m.cn/gtodxoinki.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhixingplan.top/gtraczoias.html

JS:   fs.readdirSync("dir")
来源：http://hz.snrcjt.cn/gthvddjddv.html

TS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gtlqpghgbq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtavpgqdlj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yuxming.cn/gtbosxxptf.html

Ruby: Dir.children("dir")
来源：http://hz.ywan-chungtsiang.top/gtjrgjsidb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258888.top/gtdmghacvt.html

[F09] 获取文件大小
来源：http://hz.cqqwz.cn/gtfdkrmxeh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hongshengwenyu.top/gtbejiwafd.html

PHP:  filesize("a.txt");
来源：http://hz.hfpthk.cn/gtrtscyphb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xylfe.cn/gtdttlbgtk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnqzz.top/gtwaucywqr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtygfslvyc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhongyouzk.top/gtjdpghuet.html

Ruby: File.size("a.txt")
来源：http://hz.svipenyu.cn/gtvrpgafqd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cashguo.top/gtzlkpxcku.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.redwolf501.top/gtqimsaipg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtsdipdhia.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.dianchejie.cn/gtzxvyvblu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtdnnminun.html

TS:   path.extname("a.txt")
来源：http://hz.jqgufenzy.top/gteceqsnuk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cashguo.top/gtezutzffo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtopkomtci.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shzxlz.cn/gtpovarcmj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.smart0.xyz/gtfjwkdgit.html

[F11] 复制与移动文件
来源：http://hz.andypj.xyz/gtmydzzvwg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtivtjdxqy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hfpthk.cn/gtnqtwdfff.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtteupxozm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtgcoyvdhn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cucudq.cn/gtwfwkjkyu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.meibo888.top/gtjvooujje.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtjftyuang.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuanzhike.top/gtirazjrad.html

[F12] CSV 读写
来源：http://hz.52xcode.cn/gtwwmurjyn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgfzy.top/gtujjazerv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenjidiqi.icu/gtdcqakgdv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shangyingyoupin.top/gtdfqjkxmy.html

TS:   // 同上
来源：http://hz.jlsjyb.cn/gtizqkmuap.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhaomingkeji.xyz/gtuyzizyqh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jyoumei.cn/gtmocapndk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnxiangtu.top/gtcdqebjnt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.daria6918.cn/gtkibwqsda.html

================================================================================
来源：http://hz.zhoulong.xyz/gtnycatsav.html

G. 面向对象
来源：http://hz.sweek.top/gtjzadrmxy.html

================================================================================
来源：http://hz.bjfxy.top/gtrjtyahvj.html

[G01] 定义类
来源：http://hz.haohaochexian.top/gtfokrjwls.html

Py:   class User: pass
来源：http://hz.nanxinkj.top/gtqltbipiq.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gtsmbmqhsc.html

JS:   class User {}
来源：http://hz.zycfv.cn/gtihbipexk.html

TS:   class User { name: string = ""; }
来源：http://hz.chenlongwang.top/gtukzdlmfl.html

Java: class User {}
来源：http://hz.xziqi.cn/gtkotwwvvo.html

Go:   type User struct { Name string }
来源：http://hz.pycfn.com/gtdwkbtdzx.html

Ruby: class User; end
来源：http://hz.xingfuxueyuan.xyz/gtxasljvzq.html

C#:   class User {}
来源：http://hz.cqqwz.cn/gtsbabfcon.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtqypvcugt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj202588.top/gtxormyrto.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sweek.top/gtjspmjfpj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtywbcbqgh.html

TS:   constructor(public name: string) {}
来源：http://hz.nanxuanxn.top/gtrwnufkit.html

Java: User(String name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtzmduzasi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tianlin.xyz/gtopkdpgys.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj202588.top/gtaehlsdfh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fengsongda.top/gtmljstiao.html

[G03] 实例属性
来源：http://hz.gogol.net.cn/gtbqjgtmdf.html

Py:   self.name = "x"
来源：http://hz.jinghuilouyu.cn/gtqucdiawi.html

PHP:  public string $name = "x";
来源：http://hz.xuanzx.com/gtkqtlcvwh.html

JS:   this.name = "x";
来源：http://hz.316326.xyz/gtaadwwxqg.html

TS:   name: string = "x";
来源：http://hz.pycfn.com/gteydqwsdg.html

Java: private String name;
来源：http://hz.gzhubu.top/gtyuewknoc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guannengcc.top/gtuhhkjcsc.html

Ruby: @name = "x"
来源：http://hz.dashuyun.cn/gtsgcrertt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yanxiufei.cn/gtsdvhrjpx.html

[G04] 定义方法
来源：http://hz.mhx1999.top/gtzkbxrphi.html

Py:   def greet(self): return self.name
来源：http://hz.sysykeji.top/gtgdvwncyr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtjrypbnya.html

JS:   greet() { return this.name; }
来源：http://hz.yanxiufei.cn/gtbttsggbu.html

TS:   greet(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtdepfungd.html

Java: String greet() { return name; }
来源：http://hz.jqgfzy.top/gtqffrlapp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hammf.cn/gtmkqegsws.html

Ruby: def greet; @name; end
来源：http://hz.jlsjyb.cn/gtnnstemxz.html

C#:   public string Greet() => Name;
来源：http://hz.0kj1m.cn/gtbrjeeedc.html

[G05] 继承
来源：http://hz.jlsjyb.cn/gtkobhrzii.html

Py:   class Admin(User): pass
来源：http://hz.yvedp.cn/gtqwwcfodm.html

PHP:  class Admin extends User {}
来源：http://hz.xinyue.icu/gtuusawhxc.html

JS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtrkjmaavm.html

TS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtmflzvhdq.html

Java: class Admin extends User {}
来源：http://hz.yj20258888.top/gtoviobkus.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.daria6918.cn/gtjtswlwky.html

Ruby: class Admin < User; end
来源：http://hz.wangdashe.top/gtifmwenhz.html

C#:   class Admin : User {}
来源：http://hz.quarkkingdee.top/gtyolkkzcn.html

[G06] 重写方法
来源：http://hz.zhijiandao.cn/gttvntuylo.html

Py:   def greet(self): return "admin"
来源：http://hz.dashuyun.cn/gtjpkconvl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtkgbikyja.html

JS:   greet() { return "admin"; }
来源：http://hz.cqqwz.cn/gtohvchlgq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtdorsiubs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gttilakkhn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhiwuduotai.top/gtcdyhlirn.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gtupakdnjf.html

C#:   public override string Greet() => "admin";
来源：http://hz.hammf.cn/gtvrhnatyd.html

[G07] 调用父类方法
来源：http://hz.xziqi.cn/gtdtdchmjs.html

Py:   super().greet()
来源：http://hz.kuanghao11.cn/gtenuylwgh.html

PHP:  parent::greet();
来源：http://hz.fengsongda.top/gtyeokgkei.html

JS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtcogfaxuw.html

TS:   super.greet();
来源：http://hz.chenzaomai.com/gtjqaodlvp.html

Java: super.greet();
来源：http://hz.xuetiantiany.cn/gtwioflvia.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhiwuduotai.top/gthhznybpw.html

Ruby: super
来源：http://hz.ydzc1.top/gtanlsrbim.html

C#:   base.Greet();
来源：http://hz.jinghuilouyu.cn/gtlzhyqnsy.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtqjdykubo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.redwolf501.top/gtrbkefwzy.html

PHP:  public static function f() {}
来源：http://hz.zycfv.cn/gtsehrifjp.html

JS:   static f() {}
来源：http://hz.sxryk.cn/gtzimdbtra.html

TS:   static f(): void {}
来源：http://hz.chenlongwang.top/gtpnvclmxx.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtfcrphngb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daxiang520.top/gtjkgtxris.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gtvovhhdgt.html

C#:   public static void F() {}
来源：http://hz.snrcjt.cn/gtrhxbclfl.html

[G09] 接口 / 抽象类
来源：http://hz.jinyuanbaomall.cn/gtawwnymwc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cqqwz.cn/gtowqrzprv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hongshengwenyu.top/gtmfxecbyq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gogol.net.cn/gtuwmcxctr.html

TS:   interface Shape { area(): number; }
来源：http://hz.guannengcc.top/gtzdzeirmr.html

Java: interface Shape { double area(); }
来源：http://hz.cheryme.top/gtddqzltyz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.iojbl.cn/gttikjzoys.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuanzhike.top/gtfaqtpycd.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinqigufen.top/gtptgkprpz.html

[G10] 访问控制
来源：http://hz.bjfxy.top/gtndfvaemu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ivvv.top/gtgllpadty.html

PHP:  public / protected / private
来源：http://hz.xylfe.cn/gtwuiojtyc.html

JS:   #private 字段；其余公开
来源：http://hz.dashuyun.cn/gtpmdyfrjf.html

TS:   public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtjezogrcp.html

Java: public / protected / private / 默认包级
来源：http://hz.chenjidiqi.icu/gtnoqgcxei.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sweek.top/gtijyjvspo.html

Ruby: public / protected / private
来源：http://hz.gzhubu.top/gtndpsdjcb.html

C#:   public / protected / private / internal
来源：http://hz.meibo888.top/gtsmwqlury.html

[G11] getter / setter
来源：http://hz.gzhubu.top/gtybrnezmx.html

Py:   @property 与 @x.setter
来源：http://hz.gzhubu.top/gtwnhsftbi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtxffprxwn.html

JS:   get name() { return this._name; }
来源：http://hz.sufxvd.cn/gtnmzowkve.html

TS:   get name(): string { return this._name; }
来源：http://hz.dashuyun.cn/gtocnfnvgy.html

Java: public String getName() { return name; }
来源：http://hz.wangdashe.top/gtfjbqapik.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtapymqila.html

Ruby: attr_accessor :name
来源：http://hz.yueranfly.top/gteuhfiutm.html

C#:   public string Name { get; set; }
来源：http://hz.yueranfly.top/gtxdtxwqoh.html

[G12] 对象转字符串
来源：http://hz.yvedp.cn/gtozylxqpy.html

Py:   def __str__(self): return self.name
来源：http://hz.quarkkingdee.top/gtslwskszz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtaapbbnhq.html

JS:   toString() { return this.name; }
来源：http://hz.ehwqpu.com/gthlnwsthl.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtfjqwbbmv.html

Java: @Override public String toString() { return name; }
来源：http://hz.redwolf501.top/gtqnpjsowj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ppjwa.cn/gtpsivhjqs.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtqitxhiuq.html

C#:   public override string ToString() => Name;
来源：http://hz.daxiang520.top/gtpwzbfdbn.html

[G13] 判断对象类型
来源：http://hz.sweek.top/gtjuulteer.html

Py:   isinstance(u, User)
来源：http://hz.cqqwz.cn/gtrnqvqmwn.html

PHP:  $u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtzopjqwso.html

JS:   u instanceof User
来源：http://hz.shuidangran.top/gtxsmxldwn.html

TS:   u instanceof User
来源：http://hz.ydjk.org.cn/gtawktwbus.html

Java: u instanceof User
来源：http://hz.mhx1999.top/gtcwfpcbew.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yanxiufei.cn/gtvcypdhla.html

Ruby: u.is_a?(User)
来源：http://hz.sxryk.cn/gtldayclwz.html

C#:   u is User
来源：http://hz.yanxiufei.cn/gtiwrvnxpu.html

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gttcfzpapr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sweek.top/gtwtqessep.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangtech.top/gtiilsrryc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.birdmap.top/gtixdtvxxb.html

TS:   type User = { name: string; age: number };
来源：http://hz.zdqjudy.top/gtiugttcgq.html

Java: record User(String name, int age) {}
来源：http://hz.daxiang520.top/gtfrrahdem.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gzhubu.top/gtrniazhrp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gogol.net.cn/gtxbymtexr.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtdlrywenr.html

[G15] 枚举
来源：http://hz.ybcxt.top/gtvfaqwzee.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yonumen.top/gtpuajjwov.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.svipenyu.cn/gtpcuxgqfu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj202588.top/gteybkeqlp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtmhrocjiv.html

Java: enum Color { RED, GREEN }
来源：http://hz.ivvv.top/gtxqwzzlnp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zycfv.cn/gtjjikosmr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shzxlz.cn/gtimngvrmx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtwmimydqt.html

[G16] 对象转数组 / 字典
来源：http://hz.shzxlz.cn/gtkwshfycg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.c1oappe.top/gtkfvzpzdt.html

PHP:  get_object_vars($obj);
来源：http://hz.jyoumei.cn/gtwbxcksvc.html

JS:   Object.entries(obj)
来源：http://hz.shangyingyoupin.top/gthpedczjl.html

TS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtniisberk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sweek.top/gtscmzoiml.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gthgapfnme.html

Ruby: obj.instance_variables
来源：http://hz.zhiwuduotai.top/gtwgwdwopl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hammf.cn/gtudwzbvfb.html

================================================================================
来源：http://hz.cucudq.cn/gttkjavtlt.html

H. 异常与错误处理
来源：http://hz.yj202588.top/gtpohkfbzj.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtesgfbpuc.html

[H01] try / catch 基础
来源：http://hz.cucudq.cn/gtfpmnjmmt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xingfuxueyuan.xyz/gtkkhocfly.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pengpengdd.cyou/gtitmcleqh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenzaomai.com/gtdhfsvtci.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtltcssxxw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hongshengwenyu.top/gtzngixspq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aizwys.cn/gtgvhljlyl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cucudq.cn/gtvimhqziq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nanxuanxn.top/gtsrlkgjjl.html

[H02] finally / ensure 收尾
来源：http://hz.zhiwuduotai.top/gtwglgywrb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuetiantiany.cn/gtehujgdfe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtsvtidffg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtxqjxyfod.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtbntjygpu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtgxunewqy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.0kj1m.cn/gtmfnsxxsn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cdnleiting.top/gthfyoyfib.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.bjfxy.top/gtjiobjouu.html

[H03] 主动抛出异常
来源：http://hz.vqdsnc.cn/gthoptsdaj.html

Py:   raise ValueError("错误信息")
来源：http://hz.xuetiantiany.cn/gtdgaczevg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtuivszsyj.html

JS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtmlvksnyx.html

TS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtfbcjatrv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtgxplinog.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daxiang520.top/gtlacszgjw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinghuilouyu.cn/gtnefwhgqk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtpkdlcrik.html

[H04] 自定义异常类型
来源：http://hz.pengpengdd.cyou/gtoorkldws.html

Py:   class MyError(Exception): pass
来源：http://hz.zhiwuduotai.top/gtgrsdrvxi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangtech.top/gtilsyptie.html

JS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtvfnnyqwn.html

TS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtihuoyqzi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guannengcc.top/gtlicfzdsv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.mhx1999.top/gtxyudxoqh.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenzaomai.com/gtotdhfsih.html

C#:   class MyException : Exception {}
来源：http://hz.ehwqpu.com/gtvwqeqmll.html

[H05] 捕获特定类型
来源：http://hz.svipenyu.cn/gtmnofefav.html

Py:   except ValueError as e:
来源：http://hz.jianghu66.top/gttmijbtms.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuanzhike.top/gtbhqhrreu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtvrxdvefx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gtqsddmfop.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hfpthk.cn/gtpoltkjns.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cashguo.top/gtklzzqghz.html

Ruby: rescue ArgumentError => e
来源：http://hz.shzxlz.cn/gtkkysdakm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sysykeji.top/gtrtgcdvxd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gtnwsurydt.html


<!-- 参考信息 -->