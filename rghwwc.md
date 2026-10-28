代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj202588.top/gtqtzwjreu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.svipenyu.cn/gtrtppczvm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gttokafsbb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gtvnidbhhz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.meibo888.top/gtosbocrzq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.kuanghao11.cn/gtjsyjstle.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guannengcc.top/gtvofdpvqd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jiagoushi.top/gtpphmhnsk.html

[F05] 判断文件或目录是否存在
来源：http://hz.ydzc1.top/gtzuthetne.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sysykeji.top/gtgsxlltef.html

PHP:  file_exists("a.txt");
来源：http://hz.shangyingyoupin.top/gtkkfdkhmn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.smart0.xyz/gteraerwlf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtcjbsadth.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtkkzoaesm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.snrcjt.cn/gtvqruqwrn.html

Ruby: File.exist?("a.txt")
来源：http://hz.yonumen.top/gtxxzeitbe.html

C#:   File.Exists("a.txt")
来源：http://hz.jinghuilouyu.cn/gtbbvyqxjl.html

[F06] 删除文件
来源：http://hz.xingfuxueyuan.xyz/gtkjmydnjd.html

Py:   os.remove("a.txt")
来源：http://hz.sweek.top/gtlhbxyjne.html

PHP:  unlink("a.txt");
来源：http://hz.kuanghao11.cn/gtblyydogm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gthurbfgbb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yangfankeji.com/gtwaqrmvce.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtdnitvdle.html

Go:   os.Remove("a.txt")
来源：http://hz.haohaochexian.top/gtftrvzmou.html

Ruby: File.delete("a.txt")
来源：http://hz.zhiwuduotai.top/gtckdasfak.html

C#:   File.Delete("a.txt");
来源：http://hz.xylfe.cn/gthlrksxvo.html

[F07] 创建目录（含多级）
来源：http://hz.0kj1m.cn/gtfcqleygw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtmfdtoknk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yonumen.top/gtpqfxuvxa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fengsongda.top/gtcqcomkrz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinyuanbaomall.cn/gtfvmjgord.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cheryme.top/gtovrckkwj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.wangshuangyany.cn/gtiuifxqrc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.mhx1999.top/gtyiqdvtex.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gogol.net.cn/gtyhlbdboo.html

[F08] 遍历目录
来源：http://hz.chenjidiqi.icu/gtapcsvyxd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhixingplan.top/gtsisdfqlq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hfpthk.cn/gtbvatcfew.html

JS:   fs.readdirSync("dir")
来源：http://hz.fzhhl.top/gtqbtmcann.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtkjuvpzgt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtbgnaiigg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.0kj1m.cn/gtaugzhicz.html

Ruby: Dir.children("dir")
来源：http://hz.yonumen.top/gtzzhlokfv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aibaodan.cn/gtytuqukib.html

[F09] 获取文件大小
来源：http://hz.yueranfly.top/gtpyoafbij.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yanxiufei.cn/gtqevjckfg.html

PHP:  filesize("a.txt");
来源：http://hz.c1oappe.top/gtunihpeau.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtuofynhtw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtefhelqdc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtarvhqrny.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ppjwa.cn/gtraghhgjf.html

Ruby: File.size("a.txt")
来源：http://hz.0kj1m.cn/gtrgncdevw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shzxlz.cn/gtmthywnbm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.sysykeji.top/gtkshuogkj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtqcliulya.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guowangkeji.top/gtxchnizmj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtpzloilig.html

TS:   path.extname("a.txt")
来源：http://hz.yj20258.top/gteqvqicaa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxuanxn.top/gtqgvmidzc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenzaomai.com/gtpybrtkvt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtujywfcum.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hammf.cn/gtnddrnxki.html

[F11] 复制与移动文件
来源：http://hz.ppjwa.cn/gtcpabczpd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtiyuhksdh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.iojbl.cn/gtjgcdjctn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtpxtwszco.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gthunrqyro.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ppjwa.cn/gtdcdeykxa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ydjk.org.cn/gtrvvvffqg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtgrwoekhm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jianghu66.top/gttnzvmlyf.html

[F12] CSV 读写
来源：http://hz.gotoacloud.top/gtdctxiixb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.c1oappe.top/gtonuxadfk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinqigufen.top/gtrumygitx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhiwuduotai.top/gtorrbrpmf.html

TS:   // 同上
来源：http://hz.xuetiantiany.cn/gtfpooztsp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.redwolf501.top/gtgivdhppx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.316326.xyz/gtzvwbxidr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nwbrower.top/gtqiwgoucp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guowangkeji.top/gttszrutjy.html

================================================================================
来源：http://hz.daxiang520.top/gtjgdllktr.html

G. 面向对象
来源：http://hz.yueranfly.top/gtiyubfjhw.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkcgubjlg.html

[G01] 定义类
来源：http://hz.haohaochexian.top/gtygnuzgep.html

Py:   class User: pass
来源：http://hz.yvedp.cn/gtblygsdja.html

PHP:  class User {}
来源：http://hz.pycfn.com/gtnonvgxom.html

JS:   class User {}
来源：http://hz.aibaodan.cn/gtdfbufuvr.html

TS:   class User { name: string = ""; }
来源：http://hz.jianghu66.top/gtabcjlzmt.html

Java: class User {}
来源：http://hz.fzhhl.top/gtnlkwweyo.html

Go:   type User struct { Name string }
来源：http://hz.daria6918.cn/gtiwcyehxi.html

Ruby: class User; end
来源：http://hz.zhengqikj.top/gtqinfqhts.html

C#:   class User {}
来源：http://hz.fzhhl.top/gtokrucsab.html

[G02] 构造函数
来源：http://hz.wangdashe.top/gtkturtjpg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuxming.cn/gtbktbybid.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj202588.top/gtdndmhhyn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtdqdbvipv.html

TS:   constructor(public name: string) {}
来源：http://hz.guowangkeji.top/gtieaaznsa.html

Java: User(String name) { this.name = name; }
来源：http://hz.52xcode.cn/gtbhclyolc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tanke756.top/gtovuegxpn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.wangshuangyany.cn/gtaadlsrya.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtotjxxugv.html

[G03] 实例属性
来源：http://hz.hnqzz.top/gtgughahvi.html

Py:   self.name = "x"
来源：http://hz.nwbrower.top/gtrgbzeefa.html

PHP:  public string $name = "x";
来源：http://hz.zycfv.cn/gtlybluzyl.html

JS:   this.name = "x";
来源：http://hz.0kj1m.cn/gtrppfcuwl.html

TS:   name: string = "x";
来源：http://hz.yangfankeji.com/gtvgzidcbm.html

Java: private String name;
来源：http://hz.wangshuangyany.cn/gttitxugka.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.dashuyun.cn/gttymtphka.html

Ruby: @name = "x"
来源：http://hz.yj202588.top/gtmkzyejmx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangtech.top/gtataxikxk.html

[G04] 定义方法
来源：http://hz.shanyushiyangtech.top/gtuumglebl.html

Py:   def greet(self): return self.name
来源：http://hz.jyoumei.cn/gtxaqmcdmi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtglbpzaxy.html

JS:   greet() { return this.name; }
来源：http://hz.quarkkingdee.top/gtqhqlswmb.html

TS:   greet(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtsrvfjmbh.html

Java: String greet() { return name; }
来源：http://hz.yj20258.top/gtemcpmezf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dashuyun.cn/gtuuuzavag.html

Ruby: def greet; @name; end
来源：http://hz.zhiwuduotai.top/gtwsgvewfd.html

C#:   public string Greet() => Name;
来源：http://hz.bjfxy.top/gtbeyueobm.html

[G05] 继承
来源：http://hz.zycfv.cn/gtqxpzksxb.html

Py:   class Admin(User): pass
来源：http://hz.guannengcc.top/gtxuquwanu.html

PHP:  class Admin extends User {}
来源：http://hz.dashuyun.cn/gtjklrdbub.html

JS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gtiefylcqc.html

TS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtqudddwsy.html

Java: class Admin extends User {}
来源：http://hz.tanke756.top/gtkfcvedsd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.9152youxi.cn/gtcnhksexo.html

Ruby: class Admin < User; end
来源：http://hz.jyoumei.cn/gtxtptxstw.html

C#:   class Admin : User {}
来源：http://hz.ydjk.org.cn/gttwvvcihq.html

[G06] 重写方法
来源：http://hz.yj20258888.top/gtjvqimzcm.html

Py:   def greet(self): return "admin"
来源：http://hz.svipenyu.cn/gtnhjehuos.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gtyzgwwxyo.html

JS:   greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtvtimbnqf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtinyxywuj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gtdaccwwdh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gtcwchqwrk.html

Ruby: def greet; "admin"; end
来源：http://hz.pengpengdd.cyou/gtduausids.html

C#:   public override string Greet() => "admin";
来源：http://hz.svipenyu.cn/gtcaxipigm.html

[G07] 调用父类方法
来源：http://hz.cdnleiting.top/gtucgcituf.html

Py:   super().greet()
来源：http://hz.zhixingplan.top/gtyfgeejsg.html

PHP:  parent::greet();
来源：http://hz.shuidangran.top/gtqzndqruz.html

JS:   super.greet();
来源：http://hz.xylfe.cn/gtwjtxvqsu.html

TS:   super.greet();
来源：http://hz.c1oappe.top/gtyperkzev.html

Java: super.greet();
来源：http://hz.fzhhl.top/gtibufbqej.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ybcxt.top/gtaorxvbgg.html

Ruby: super
来源：http://hz.quarkkingdee.top/gtqeyhcqjt.html

C#:   base.Greet();
来源：http://hz.hfpthk.cn/gtufochejn.html

[G08] 静态方法与属性
来源：http://hz.vqdsnc.cn/gtjqkzfniu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.c1oappe.top/gtsfqcujpe.html

PHP:  public static function f() {}
来源：http://hz.cdnleiting.top/gtfomoqqme.html

JS:   static f() {}
来源：http://hz.pengpengdd.cyou/gtmymemxck.html

TS:   static f(): void {}
来源：http://hz.chenzaomai.com/gtyztgymcc.html

Java: static void f() {}
来源：http://hz.0kj1m.cn/gtsdryqzny.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sweek.top/gtsjvpgaya.html

Ruby: def self.f; end
来源：http://hz.nanxinkj.top/gtsaitgspq.html

C#:   public static void F() {}
来源：http://hz.xinyue.icu/gtconvbkle.html

[G09] 接口 / 抽象类
来源：http://hz.zhaomingkeji.xyz/gtvmkrqszw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.bjfxy.top/gtqditgydf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yangfankeji.com/gtjyxbaskb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ehwqpu.com/gtbhbtpxhi.html

TS:   interface Shape { area(): number; }
来源：http://hz.aibaodan.cn/gtgbrjkvmq.html

Java: interface Shape { double area(); }
来源：http://hz.0kj1m.cn/gtunwzzexi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.c1oappe.top/gtqbwiksdg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gtrogifrfk.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydjk.org.cn/gtlvlawfjf.html

[G10] 访问控制
来源：http://hz.ywan-chungtsiang.top/gtnjccavrh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.iojbl.cn/gtnlsoryjt.html

PHP:  public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtqbrbtekd.html

JS:   #private 字段；其余公开
来源：http://hz.vqdsnc.cn/gtqwxgrfji.html

TS:   public / protected / private
来源：http://hz.fengsongda.top/gtpjwqrmoy.html

Java: public / protected / private / 默认包级
来源：http://hz.hnxiangtu.top/gthnnlknbj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pycfn.com/gtivldsjnb.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangtech.top/gtsoldinlk.html

C#:   public / protected / private / internal
来源：http://hz.smart0.xyz/gtrxjhicwc.html

[G11] getter / setter
来源：http://hz.cdnleiting.top/gtotnjjydh.html

Py:   @property 与 @x.setter
来源：http://hz.cqqwz.cn/gtdwbblizp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtkgwdiesh.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigufen.top/gtrycdypkm.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenzaomai.com/gtlcinoceo.html

Java: public String getName() { return name; }
来源：http://hz.tanke756.top/gtlzbexhng.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jiagoushi.top/gtnyeegamh.html

Ruby: attr_accessor :name
来源：http://hz.jlsjyb.cn/gtqqqlekho.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigfzy.top/gtdvpnsprv.html

[G12] 对象转字符串
来源：http://hz.gogol.net.cn/gthrscjmlk.html

Py:   def __str__(self): return self.name
来源：http://hz.quarkkingdee.top/gtzfrnvfyu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtmoihhjbv.html

JS:   toString() { return this.name; }
来源：http://hz.zdqjudy.top/gtgyyjzfqb.html

TS:   toString(): string { return this.name; }
来源：http://hz.daria6918.cn/gtvpzgpued.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydzc1.top/gtnsvimdre.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.havefunace.top/gtdrzbmopt.html

Ruby: def to_s; @name; end
来源：http://hz.chenjidiqi.icu/gtnihhzpyr.html

C#:   public override string ToString() => Name;
来源：http://hz.aizwys.cn/gtsdxwkmfz.html

[G13] 判断对象类型
来源：http://hz.yuanzhike.top/gttphpfodk.html

Py:   isinstance(u, User)
来源：http://hz.hongshengwenyu.top/gtvfilvxah.html

PHP:  $u instanceof User
来源：http://hz.ivvv.top/gtkmcuwivi.html

JS:   u instanceof User
来源：http://hz.cucudq.cn/gtsleerlal.html

TS:   u instanceof User
来源：http://hz.ehwqpu.com/gttcbqertf.html

Java: u instanceof User
来源：http://hz.cdnleiting.top/gttcjducub.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxinkj.top/gthwlqrico.html

Ruby: u.is_a?(User)
来源：http://hz.birdmap.top/gtrrgrlbvc.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtoztmfwbd.html

[G14] 数据类 / record
来源：http://hz.cqqwz.cn/gtnaxdhjdq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydjk.org.cn/gtxdezrjoi.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hysaishi.cn/gtylwuqult.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fzhhl.top/gtkbufmqdm.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhiwuduotai.top/gteggbtjpf.html

Java: record User(String name, int age) {}
来源：http://hz.ppjwa.cn/gtbjwadvcm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.aizwys.cn/gtsleargdl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yanxiufei.cn/gtuaglnzon.html

C#:   record User(string Name, int Age);
来源：http://hz.zhoulong.xyz/gtktjpojne.html

[G15] 枚举
来源：http://hz.jyoumei.cn/gtmrzqsdpi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnxiangtu.top/gtkkrmwqmz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hammf.cn/gtzlgzbjsv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.mhx1999.top/gtvvpyewcz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangtech.top/gtburqfqhz.html

Java: enum Color { RED, GREEN }
来源：http://hz.xylfe.cn/gtoealvrvd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtglmairbf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxinkj.top/gtyriyuuen.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tanke756.top/gtowakjfrj.html

[G16] 对象转数组 / 字典
来源：http://hz.guannengcc.top/gttclwqjwa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.redwolf501.top/gtbccjmuyy.html

PHP:  get_object_vars($obj);
来源：http://hz.haohaochexian.top/gtuttxyvtj.html

JS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtxbotxfpb.html

TS:   Object.entries(obj)
来源：http://hz.guowangkeji.top/gthirpriss.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258888.top/gtntnwdlij.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aibaodan.cn/gtpozvkzvo.html

Ruby: obj.instance_variables
来源：http://hz.meibo888.top/gtizzgnmuo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.havefunace.top/gtwvyahulc.html

================================================================================
来源：http://hz.fengsongda.top/gthpkaksaa.html

H. 异常与错误处理
来源：http://hz.yongpay.top/gtoojgsffh.html

================================================================================
来源：http://hz.quarkkingdee.top/gtkjwzzctx.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gtokqntzfl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydjk.org.cn/gttpyxrrzp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgfzy.top/gtvjszqpla.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gogol.net.cn/gtdgnplvpj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258.top/gtqchkkafm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gaohongyu789.top/gtmalraatc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dashuyun.cn/gtaecnrbcm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtmcjtioym.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.svipenyu.cn/gtjpuhjuod.html

[H02] finally / ensure 收尾
来源：http://hz.havefunace.top/gtxaedqhts.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj20258.top/gtqzqunnfk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtnfmsqzvn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtccsvhvsm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtgwsyuzyp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtapikosiq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuxming.cn/gtlaomewms.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydzc1.top/gtftrsbpqu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtakezzyce.html

[H03] 主动抛出异常
来源：http://hz.zhijiandao.cn/gtzbidortj.html

Py:   raise ValueError("错误信息")
来源：http://hz.redwolf501.top/gtbvxrkvvj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtmpglwbrm.html

JS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gthrrytwfj.html

TS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtohmlzesq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtoynqzwfg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xuetiantiany.cn/gtmvkwpldd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pengpengdd.cyou/gtbnddzmia.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtcbuhxhgp.html

[H04] 自定义异常类型
来源：http://hz.zhengqikj.top/gtfrjdgegu.html

Py:   class MyError(Exception): pass
来源：http://hz.yuanzhike.top/gtjvldrmst.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtdovxdbpz.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtnzuiumbo.html

TS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtnywyfrrw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shuidangran.top/gtmqqunegg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nwbrower.top/gtepjxhtls.html

Ruby: class MyError < StandardError; end
来源：http://hz.316326.xyz/gtsqoowmvc.html

C#:   class MyException : Exception {}
来源：http://hz.tian-w.cn/gtsxaoowtz.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gtvcswgyhs.html

Py:   except ValueError as e:
来源：http://hz.gotoacloud.top/gtdbbupvky.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.vqdsnc.cn/gtrxerfcjb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtmktwcwtj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.c1oappe.top/gtnieoyoey.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aibaodan.cn/gtyehuwmwo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hfpthk.cn/gtphvwuiah.html

Ruby: rescue ArgumentError => e
来源：http://hz.cashguo.top/gtsvgmzuyh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cashguo.top/gtfueygntn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.birdmap.top/gtmxdjmwxu.html

Py:   value = d.get("k") or default
来源：http://hz.hfpthk.cn/gtlmkntnmj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yvedp.cn/gtynyjmzla.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtcxbccqkt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtiqvfhyel.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.meibo888.top/gtxqtmjsva.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jqgfzy.top/gtjrbgasrs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sufxvd.cn/gtzoeeczyo.html

C#:   obj?.A?.B ?? default
来源：http://hz.pycfn.com/gtjymysmls.html

[H07] 断言
来源：http://hz.shangyingyoupin.top/gtzixvuytb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hongshengwenyu.top/gtdcgidgaf.html

PHP:  assert($x > 0);
来源：http://hz.jinqigufen.top/gtuoanfdea.html

JS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtxqulkulw.html

TS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtmadwowmr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj20258888.top/gtnkrgquaq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yuanzhike.top/gtamdivspb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sxryk.cn/gtxemqdsgm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258888.top/gtdnpjunkw.html

[H08] 获取错误信息与堆栈
来源：http://hz.fengsongda.top/gtysvokjny.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gtxfyqyfyl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xziqi.cn/gtyizclfws.html

JS:   e.message;  e.stack
来源：http://hz.jinqigufen.top/gtazrotsmr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.wangdashe.top/gtecsbmqpb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.quarkkingdee.top/gtykxmlsdz.html

Go:   err.Error()
来源：http://hz.andypj.xyz/gtscsztpmx.html


<!-- 参考信息 -->