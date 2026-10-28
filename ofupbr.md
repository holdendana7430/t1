代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.vqdsnc.cn/gtoyfxakgn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.9152youxi.cn/gtdedvsrks.html

[F03] 写入文件（覆盖）
来源：http://hz.zhoulong.xyz/gtnkltbpff.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.mhx1999.top/gtocaqrbzt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.smart0.xyz/gtymzrwqam.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtklgfnngn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtrkorjvph.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.smart0.xyz/gtzxvlrgnz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhaomingkeji.xyz/gtttrrdndn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cucudq.cn/gtwwufbegl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shangyingyoupin.top/gtpxedwcjz.html

[F04] 追加写入文件
来源：http://hz.kuanghao11.cn/gtkrcnyffj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhiwuduotai.top/gtqgstdiju.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jlsjyb.cn/gtiuavptca.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtzxfajgzp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtqqynbtpn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yanxiufei.cn/gtrbbddkcs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ydjk.org.cn/gtcjcjdiqq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj20258.top/gtwyacimnd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cucudq.cn/gtahdekrix.html

[F05] 判断文件或目录是否存在
来源：http://hz.guowangkeji.top/gtnbwbwlgt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.birdmap.top/gtctpjbwzr.html

PHP:  file_exists("a.txt");
来源：http://hz.cqqwz.cn/gtbityqgwy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gtlbxoqtol.html

TS:   fs.existsSync("a.txt")
来源：http://hz.9152youxi.cn/gtajeuyqnf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtpygruuso.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ybcxt.top/gthxpvfvqm.html

Ruby: File.exist?("a.txt")
来源：http://hz.sxryk.cn/gtorfjeswb.html

C#:   File.Exists("a.txt")
来源：http://hz.zycfv.cn/gtazqcarjq.html

[F06] 删除文件
来源：http://hz.fengsongda.top/gtwqdyrxqg.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtirdokzju.html

PHP:  unlink("a.txt");
来源：http://hz.0kj1m.cn/gtljmfxzxd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtqanxkclv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtyioexbyp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtbvlynumu.html

Go:   os.Remove("a.txt")
来源：http://hz.gaohongyu789.top/gtcguikukm.html

Ruby: File.delete("a.txt")
来源：http://hz.nanxinkj.top/gtnqjtdqqc.html

C#:   File.Delete("a.txt");
来源：http://hz.vqdsnc.cn/gtikfdsirg.html

[F07] 创建目录（含多级）
来源：http://hz.hnqzz.top/gtnljjihlj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.feifeiyinyue.top/gtrclvhvdw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258.top/gtzxzspihg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtatchkocr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtefyjhgym.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shanyushiyangtech.top/gtictmfwpk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.316326.xyz/gtpzbiucgr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhijiandao.cn/gtrwiehtrg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hfpthk.cn/gtfritiydb.html

[F08] 遍历目录
来源：http://hz.sufxvd.cn/gtlzpmxzkt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yvedp.cn/gtzyhjgwdc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xinyue.icu/gtupmulbyk.html

JS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gtacilhuuu.html

TS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gtjhmugwlx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtvwijnnba.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nanxinkj.top/gtefaqytvu.html

Ruby: Dir.children("dir")
来源：http://hz.hfpthk.cn/gtocusxmcr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.andypj.xyz/gtnsikdydy.html

[F09] 获取文件大小
来源：http://hz.quarkkingdee.top/gtoorncmhe.html

Py:   os.path.getsize("a.txt")
来源：http://hz.redwolf501.top/gtuusxpqah.html

PHP:  filesize("a.txt");
来源：http://hz.yuxming.cn/gtqtlbyfqf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gthmnuvhwm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gtmniszhrv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtuvhqfhrp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hysaishi.cn/gtyivftnbo.html

Ruby: File.size("a.txt")
来源：http://hz.hongshengwenyu.top/gtaldgiqsx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jyoumei.cn/gtehtvbmzr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.c1oappe.top/gttngtnpvg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtqrorvkog.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.daria6918.cn/gtduebmlkq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtxmwduisy.html

TS:   path.extname("a.txt")
来源：http://hz.zhengqikj.top/gtnaxapehf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ywan-chungtsiang.top/gtdzwqixjm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gtbrgchaoh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtzqocpogh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sweek.top/gtaozsugyy.html

[F11] 复制与移动文件
来源：http://hz.zhongyouzk.top/gtklaxocoa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtodzphebj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jqgufenzy.top/gtaggaadyv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtbtxngkjb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtcapctxhk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.9152youxi.cn/gtsobrlgmw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.snrcjt.cn/gtbkardlud.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtltqjqfxc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guannengcc.top/gteecwaqda.html

[F12] CSV 读写
来源：http://hz.shzxlz.cn/gtwyvgnrux.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ybcxt.top/gtmeqjaytc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinyuanbaomall.cn/gtpnsmtpjw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangshuangyany.cn/gtqkcgtvnj.html

TS:   // 同上
来源：http://hz.jlsjyb.cn/gtfryiflmk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ydjk.org.cn/gthpasldmu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tanke756.top/gtcvwxpmqf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenjidiqi.icu/gtdoelewyp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gtctpqrsop.html

================================================================================
来源：http://hz.meibo888.top/gtmgetjxsw.html

G. 面向对象
来源：http://hz.zhengqikj.top/gtvdcsfxhj.html

================================================================================
来源：http://hz.hfpthk.cn/gtlfpwomer.html

[G01] 定义类
来源：http://hz.ydzc1.top/gtvuyywjth.html

Py:   class User: pass
来源：http://hz.daxiang520.top/gtetfgriup.html

PHP:  class User {}
来源：http://hz.cdnleiting.top/gtqiwydhxd.html

JS:   class User {}
来源：http://hz.chenlongwang.top/gtlfslflsf.html

TS:   class User { name: string = ""; }
来源：http://hz.shuidangran.top/gtmgaygbvq.html

Java: class User {}
来源：http://hz.xylfe.cn/gtiqoxmvtt.html

Go:   type User struct { Name string }
来源：http://hz.svipenyu.cn/gtkwiyxnal.html

Ruby: class User; end
来源：http://hz.yj20258888.top/gtsvjhuydj.html

C#:   class User {}
来源：http://hz.zhengqikj.top/gtwczarhcp.html

[G02] 构造函数
来源：http://hz.zhiwuduotai.top/gtssdzizkb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuanzhike.top/gtmbubccrv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shangyingyoupin.top/gtbbeaufbd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aizwys.cn/gtsklgodcq.html

TS:   constructor(public name: string) {}
来源：http://hz.fzhhl.top/gtvkglpsyo.html

Java: User(String name) { this.name = name; }
来源：http://hz.snrcjt.cn/gtdgwymqah.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fzhhl.top/gtilgkfhre.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yongpay.top/gthfjeeksu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxinkj.top/gtbttzshsy.html

[G03] 实例属性
来源：http://hz.redwolf501.top/gtdaycerbu.html

Py:   self.name = "x"
来源：http://hz.xuanzx.com/gtvaxdhtty.html

PHP:  public string $name = "x";
来源：http://hz.hysaishi.cn/gtreikwjys.html

JS:   this.name = "x";
来源：http://hz.nanxinkj.top/gtcsfpxxqx.html

TS:   name: string = "x";
来源：http://hz.zhengqikj.top/gtpfrocogk.html

Java: private String name;
来源：http://hz.hnxiangtu.top/gtrsfoolmz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gotoacloud.top/gtoultequy.html

Ruby: @name = "x"
来源：http://hz.zhoulong.xyz/gtzixbvxvx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xinyue.icu/gtdwygrnul.html

[G04] 定义方法
来源：http://hz.yongpay.top/gtcozyihvn.html

Py:   def greet(self): return self.name
来源：http://hz.guannengcc.top/gtwzchmupn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtvznhqxms.html

JS:   greet() { return this.name; }
来源：http://hz.xylfe.cn/gtigffwcww.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gthcemdyjr.html

Java: String greet() { return name; }
来源：http://hz.cashguo.top/gtgummupaz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gtobalonnl.html

Ruby: def greet; @name; end
来源：http://hz.zhaomingkeji.xyz/gtnggcgjfy.html

C#:   public string Greet() => Name;
来源：http://hz.yongpay.top/gtrurqqvvo.html

[G05] 继承
来源：http://hz.daria6918.cn/gtkghscokx.html

Py:   class Admin(User): pass
来源：http://hz.meibo888.top/gtolmdmuqk.html

PHP:  class Admin extends User {}
来源：http://hz.yj20258888.top/gtajfvfmip.html

JS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtffrzndeg.html

TS:   class Admin extends User {}
来源：http://hz.yj20258.top/gttgjcnyoh.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtularstiw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydzc1.top/gtewvtwzqc.html

Ruby: class Admin < User; end
来源：http://hz.gaohongyu789.top/gtiaovurkq.html

C#:   class Admin : User {}
来源：http://hz.yongpay.top/gthmuqtgqc.html

[G06] 重写方法
来源：http://hz.zhoulong.xyz/gtrgijwbta.html

Py:   def greet(self): return "admin"
来源：http://hz.jinghuilouyu.cn/gtubmytuun.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinqigfzy.top/gtzknfyiwh.html

JS:   greet() { return "admin"; }
来源：http://hz.yonumen.top/gtoiqxsdnh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gtfnfmzkyu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gthylwnntd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.feifeiyinyue.top/gtwrailtpj.html

Ruby: def greet; "admin"; end
来源：http://hz.tian-w.cn/gtryqiyevb.html

C#:   public override string Greet() => "admin";
来源：http://hz.smart0.xyz/gtcznyjcux.html

[G07] 调用父类方法
来源：http://hz.kuanghao11.cn/gtczhmxldu.html

Py:   super().greet()
来源：http://hz.dianchejie.cn/gtmxsjwsfp.html

PHP:  parent::greet();
来源：http://hz.tian-w.cn/gtgevvolug.html

JS:   super.greet();
来源：http://hz.fzhhl.top/gtdhhsafbp.html

TS:   super.greet();
来源：http://hz.dashuyun.cn/gtnokttonc.html

Java: super.greet();
来源：http://hz.shanyushiyangkeji.top/gtovudnejv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gotoacloud.top/gtjckrmzqv.html

Ruby: super
来源：http://hz.vqdsnc.cn/gtywmtmopu.html

C#:   base.Greet();
来源：http://hz.ywan-chungtsiang.top/gtihtmticn.html

[G08] 静态方法与属性
来源：http://hz.zhixingplan.top/gtcgcdjvim.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.wangdashe.top/gtsvteqwmf.html

PHP:  public static function f() {}
来源：http://hz.guannengcc.top/gtvityjyqd.html

JS:   static f() {}
来源：http://hz.yangfankeji.com/gtwlgckoso.html

TS:   static f(): void {}
来源：http://hz.hysaishi.cn/gtpmpmhwha.html

Java: static void f() {}
来源：http://hz.ydjk.org.cn/gtsejiclet.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daria6918.cn/gthjlvzttn.html

Ruby: def self.f; end
来源：http://hz.nanxinkj.top/gtzncmkdhu.html

C#:   public static void F() {}
来源：http://hz.gaohongyu789.top/gtbjaaodmp.html

[G09] 接口 / 抽象类
来源：http://hz.xuetiantiany.cn/gtjdtvdjcv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.52xcode.cn/gtxhivrdxi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangshuangyany.cn/gttrdkqaoa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xinyue.icu/gtfolbazwv.html

TS:   interface Shape { area(): number; }
来源：http://hz.aibaodan.cn/gtyfeciwkn.html

Java: interface Shape { double area(); }
来源：http://hz.zhaomingkeji.xyz/gtkstvhqtu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hammf.cn/gtymwqrujd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenzaomai.com/gtjfjfsify.html

C#:   interface IShape { double Area(); }
来源：http://hz.hfpthk.cn/gtzbqddvrl.html

[G10] 访问控制
来源：http://hz.zhixingplan.top/gtyobtpspo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yonumen.top/gtkrxbgobw.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangtech.top/gtosqigjlg.html

JS:   #private 字段；其余公开
来源：http://hz.ywan-chungtsiang.top/gtruqeacag.html

TS:   public / protected / private
来源：http://hz.aizwys.cn/gtdlmuklyw.html

Java: public / protected / private / 默认包级
来源：http://hz.jinqigfzy.top/gtcqxwdxgj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fzhhl.top/gtdggofebb.html

Ruby: public / protected / private
来源：http://hz.jqgufenzy.top/gtstuibjcd.html

C#:   public / protected / private / internal
来源：http://hz.ywan-chungtsiang.top/gtvxprubyw.html

[G11] getter / setter
来源：http://hz.shanyushiyangkeji.top/gtlztepfws.html

Py:   @property 与 @x.setter
来源：http://hz.havefunace.top/gtfefzttnl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtouamclcb.html

JS:   get name() { return this._name; }
来源：http://hz.gotoacloud.top/gtnzxqtiku.html

TS:   get name(): string { return this._name; }
来源：http://hz.fengsongda.top/gtgazhmccs.html

Java: public String getName() { return name; }
来源：http://hz.wangshuangyany.cn/gtwhaxvpvp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xylfe.cn/gtfaniyxby.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtbroduabt.html

C#:   public string Name { get; set; }
来源：http://hz.zdqjudy.top/gtcgtbparv.html

[G12] 对象转字符串
来源：http://hz.zhijiandao.cn/gtobmtjoyr.html

Py:   def __str__(self): return self.name
来源：http://hz.nwbrower.top/gtvqtxptnf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtmkyffsyx.html

JS:   toString() { return this.name; }
来源：http://hz.jianghu66.top/gtqqlhnfep.html

TS:   toString(): string { return this.name; }
来源：http://hz.aizwys.cn/gttadtnowf.html

Java: @Override public String toString() { return name; }
来源：http://hz.0kj1m.cn/gtpzhzfepg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtevpjugtv.html

Ruby: def to_s; @name; end
来源：http://hz.zhiwuduotai.top/gtaodybguo.html

C#:   public override string ToString() => Name;
来源：http://hz.yanxiufei.cn/gtvyissvpi.html

[G13] 判断对象类型
来源：http://hz.pycfn.com/gtgvnvjlpw.html

Py:   isinstance(u, User)
来源：http://hz.hnqzz.top/gttzjgxdkn.html

PHP:  $u instanceof User
来源：http://hz.hongshengwenyu.top/gtvlogvikj.html

JS:   u instanceof User
来源：http://hz.yvedp.cn/gtghcphqdk.html

TS:   u instanceof User
来源：http://hz.svipenyu.cn/gttvmjfwfr.html

Java: u instanceof User
来源：http://hz.chenjidiqi.icu/gtscudtqpg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.feifeiyinyue.top/gtedzvsftr.html

Ruby: u.is_a?(User)
来源：http://hz.nanxinkj.top/gtgauvuany.html

C#:   u is User
来源：http://hz.wangshuangyany.cn/gttsbhyjsp.html

[G14] 数据类 / record
来源：http://hz.shzxlz.cn/gtksshvmfo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtpmdmxidb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.dashuyun.cn/gtqpmgvlwz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxinkj.top/gtikwqvbac.html

TS:   type User = { name: string; age: number };
来源：http://hz.shanyushiyangtech.top/gtkbcsorfx.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigufen.top/gtpcwtxwja.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xylfe.cn/gtaflwcnxv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cucudq.cn/gttexvsnbz.html

C#:   record User(string Name, int Age);
来源：http://hz.hnqzz.top/gtiqtjvvlp.html

[G15] 枚举
来源：http://hz.zhongyouzk.top/gttpvwcmrb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aizwys.cn/gtqtlunhhx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinghuilouyu.cn/gtvzskkelh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.mhx1999.top/gtmxmtmjok.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtjlsrtnjt.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhixingplan.top/gtegpzavog.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.dashuyun.cn/gtioimwdxe.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shuidangran.top/gtaiobvxsg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gtiawwviih.html

[G16] 对象转数组 / 字典
来源：http://hz.pengpengdd.cyou/gtuhldbski.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fengsongda.top/gtikuebrzw.html

PHP:  get_object_vars($obj);
来源：http://hz.hfpthk.cn/gteebxnuof.html

JS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtomqknerb.html

TS:   Object.entries(obj)
来源：http://hz.chenlongwang.top/gtytochjbn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.wangdashe.top/gtayachhjn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yvedp.cn/gtoavbcdbd.html

Ruby: obj.instance_variables
来源：http://hz.ppjwa.cn/gttrfqeiki.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ehwqpu.com/gtkmwtnbbb.html

================================================================================
来源：http://hz.yueranfly.top/gtoispydov.html

H. 异常与错误处理
来源：http://hz.zhixingplan.top/gtdiinahkz.html

================================================================================
来源：http://hz.ppjwa.cn/gtgfizfgsl.html

[H01] try / catch 基础
来源：http://hz.jqgfzy.top/gtvhoyoqzm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhaomingkeji.xyz/gtvgbulyoj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.52xcode.cn/gtnfceujsg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gogol.net.cn/gtvitrduey.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ehwqpu.com/gttzydddzf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tanke756.top/gtxbyldojb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenzaomai.com/gtanvxddkw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigfzy.top/gtvpnzeqsm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gzhubu.top/gtcutzmjca.html

[H02] finally / ensure 收尾
来源：http://hz.yonumen.top/gtdnvrboda.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hongshengwenyu.top/gtihfgxmpu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtgbgpvzyt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtfglbnqyw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtfdtlsamo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtewiklbpx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jianghu66.top/gtzxlvemwe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenjidiqi.icu/gtnpbngclp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigfzy.top/gtcpkiinsq.html

[H03] 主动抛出异常
来源：http://hz.quarkkingdee.top/gtjyqlqhri.html

Py:   raise ValueError("错误信息")
来源：http://hz.daxiang520.top/gtkabmhtvc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtkxpovpdi.html

JS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gtruafmrdi.html

TS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtplpbivwm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yvedp.cn/gtgqeixsjw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydjk.org.cn/gtpfqzpkoc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.svipenyu.cn/gtdxjsmqdc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.316326.xyz/gtftywgqjj.html

[H04] 自定义异常类型
来源：http://hz.xingfuxueyuan.xyz/gtpcrtfnsc.html

Py:   class MyError(Exception): pass
来源：http://hz.sxryk.cn/gtjjxsrmtg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinqigfzy.top/gtgikjgbjw.html

JS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtilaryvzw.html

TS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gttwsuexyw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtvpypeijh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nwbrower.top/gtgqjoarlj.html

Ruby: class MyError < StandardError; end
来源：http://hz.meibo888.top/gtabfdagrw.html

C#:   class MyException : Exception {}
来源：http://hz.hnqzz.top/gtmodhbygb.html

[H05] 捕获特定类型
来源：http://hz.hfpthk.cn/gtixwjhcyx.html

Py:   except ValueError as e:
来源：http://hz.jianghu66.top/gttuxoqpwc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fzhhl.top/gtpxfuewvz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtjzsevpqu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtstuunwpj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gtccmzwixp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guannengcc.top/gtlnjghkha.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtwqzejqkk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnxiangtu.top/gtjdgetuoe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangdashe.top/gtmqlxttly.html

Py:   value = d.get("k") or default
来源：http://hz.cdnleiting.top/gtnawjtfjy.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gtvjkaiudl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gtvkdqjhzg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtbhrthyzs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.smart0.xyz/gtpvfsvdic.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.52xcode.cn/gtgzabfvbw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xylfe.cn/gttcufznty.html

C#:   obj?.A?.B ?? default
来源：http://hz.mhx1999.top/gtymloypfz.html

[H07] 断言
来源：http://hz.haohaochexian.top/gtyxxoyhmp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jianghu66.top/gtxczitfxa.html

PHP:  assert($x > 0);
来源：http://hz.xylfe.cn/gtqkksznna.html

JS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtxrrybyxe.html


<!-- 参考信息 -->