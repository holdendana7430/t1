代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gotoacloud.top/gtvpwzfkga.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhiwuduotai.top/gthmmzqptj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtlyqhigua.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sxryk.cn/gthyfsgfdc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nanxinkj.top/gtsqugvgwu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhixingplan.top/gtzdwuhrln.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yangfankeji.com/gtiuzvftwf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hammf.cn/gtoeutxzul.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj202588.top/gtsucuoqjs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.birdmap.top/gtwjpfdipk.html

PHP:  file_exists("a.txt");
来源：http://hz.xinyue.icu/gtzfvnihaa.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhengqikj.top/gtgmhkpnhb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhengqikj.top/gtbqqyazfv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gthcwqadfd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenjidiqi.icu/gtauarkxto.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtuttvovye.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigufen.top/gtceefzakq.html

[F06] 删除文件
来源：http://hz.xziqi.cn/gthbzmmoho.html

Py:   os.remove("a.txt")
来源：http://hz.dianchejie.cn/gthkusjbok.html

PHP:  unlink("a.txt");
来源：http://hz.dashuyun.cn/gtcsmgrvlw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtpdjumniy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sufxvd.cn/gtmlstflxm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtqbsmwzxm.html

Go:   os.Remove("a.txt")
来源：http://hz.tianlin.xyz/gtdrjqkips.html

Ruby: File.delete("a.txt")
来源：http://hz.jinqigfzy.top/gtbcrdzrvq.html

C#:   File.Delete("a.txt");
来源：http://hz.smart0.xyz/gtrsyhohjs.html

[F07] 创建目录（含多级）
来源：http://hz.xuanzx.com/gtvhgwzjac.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hnxiangtu.top/gtquxxqynn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xylfe.cn/gtzetpahpj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtpdcqvgxx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtwgozgwkw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.redwolf501.top/gtpigdkpuy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuanzhike.top/gtqzwbvmmu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guowangkeji.top/gtuhhbdukl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhaomingkeji.xyz/gtezovokhl.html

[F08] 遍历目录
来源：http://hz.0kj1m.cn/gtqeiqsgkz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhixingplan.top/gtcnlqxpjd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.andypj.xyz/gtxfxqgvka.html

JS:   fs.readdirSync("dir")
来源：http://hz.daria6918.cn/gtgjrsvuml.html

TS:   fs.readdirSync("dir")
来源：http://hz.sufxvd.cn/gtlnoqjgmn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ydjk.org.cn/gtuembkyjo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangshuangyany.cn/gtdyxejjng.html

Ruby: Dir.children("dir")
来源：http://hz.aizwys.cn/gtnszponoj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.guowangkeji.top/gtevailukx.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtpxlruksb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.smart0.xyz/gtecddfzmz.html

PHP:  filesize("a.txt");
来源：http://hz.zhixingplan.top/gtkviqlqle.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gtlyhxedny.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtajetbfaa.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtgnsobeph.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.havefunace.top/gtbnvthunz.html

Ruby: File.size("a.txt")
来源：http://hz.tianlin.xyz/gtogqwtdcy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xinyue.icu/gtyxchvnqv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xylfe.cn/gtjucdykuf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtnbaxkfgc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.havefunace.top/gtzoyxdiil.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gthbrhilwr.html

TS:   path.extname("a.txt")
来源：http://hz.pengpengdd.cyou/gtmxluwgcw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dashuyun.cn/gtubgpbydt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.havefunace.top/gtwsblmeqp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtkshrauee.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jiagoushi.top/gtlbpijffn.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtluayhfxb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtkznffecl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shzxlz.cn/gtjarhliyz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gtllcstshp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gttkulsqgv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigufen.top/gtjzktbzub.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.wangshuangyany.cn/gtddpdcbbn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtpghksyym.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fzhhl.top/gtfpllqxbu.html

[F12] CSV 读写
来源：http://hz.guannengcc.top/gtxroiayrp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.vqdsnc.cn/gtuyaiqbrd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhoulong.xyz/gtbpshqypm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xuetiantiany.cn/gtujiwvmlu.html

TS:   // 同上
来源：http://hz.jinghuilouyu.cn/gtjqzsfrkl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxinkj.top/gtbxpyxjip.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yuanzhike.top/gttxceqqcc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hammf.cn/gtyncmmdok.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cucudq.cn/gtipxihvbo.html

================================================================================
来源：http://hz.yj202588.top/gtjjqdkijw.html

G. 面向对象
来源：http://hz.chenjidiqi.icu/gtssmkstdg.html

================================================================================
来源：http://hz.yangfankeji.com/gtoqdsxolk.html

[G01] 定义类
来源：http://hz.sufxvd.cn/gtcgakydni.html

Py:   class User: pass
来源：http://hz.nwbrower.top/gtyrdamyob.html

PHP:  class User {}
来源：http://hz.yj20258888.top/gtinmxkzqy.html

JS:   class User {}
来源：http://hz.yanxiufei.cn/gtiibhlnie.html

TS:   class User { name: string = ""; }
来源：http://hz.jianghu66.top/gtxsgwusfb.html

Java: class User {}
来源：http://hz.zdqjudy.top/gtkjnthvli.html

Go:   type User struct { Name string }
来源：http://hz.fzhhl.top/gtvjobdlzl.html

Ruby: class User; end
来源：http://hz.jianghu66.top/gtyihzhoyz.html

C#:   class User {}
来源：http://hz.dashuyun.cn/gtkkixjbvy.html

[G02] 构造函数
来源：http://hz.tianlin.xyz/gtehjnfpva.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinghuilouyu.cn/gtkzfuawgk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hongshengwenyu.top/gtoztlelqz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuxming.cn/gtqxwohfpd.html

TS:   constructor(public name: string) {}
来源：http://hz.guowangkeji.top/gtgaijrsqo.html

Java: User(String name) { this.name = name; }
来源：http://hz.shuidangran.top/gteqgurcir.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinqigfzy.top/gtnhfalozg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydzc1.top/gtcfdguaiq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinyuanbaomall.cn/gtggzmmpll.html

[G03] 实例属性
来源：http://hz.shzxlz.cn/gtzvbtgcpv.html

Py:   self.name = "x"
来源：http://hz.redwolf501.top/gtcxxwvwrs.html

PHP:  public string $name = "x";
来源：http://hz.daxiang520.top/gttmzzgmuv.html

JS:   this.name = "x";
来源：http://hz.jiagoushi.top/gtbhxxbdwi.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtcdotkpnu.html

Java: private String name;
来源：http://hz.ybcxt.top/gtsotlsfxj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.quarkkingdee.top/gtbonsarer.html

Ruby: @name = "x"
来源：http://hz.svipenyu.cn/gtdnfsbabt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.aizwys.cn/gtushnffxf.html

[G04] 定义方法
来源：http://hz.mhx1999.top/gtxsfspxog.html

Py:   def greet(self): return self.name
来源：http://hz.cucudq.cn/gtjjgpasha.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtmejuuqal.html

JS:   greet() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtqpabwhet.html

TS:   greet(): string { return this.name; }
来源：http://hz.svipenyu.cn/gtswuppahm.html

Java: String greet() { return name; }
来源：http://hz.jinghuilouyu.cn/gtzewrvzes.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yueranfly.top/gtbhuhapcr.html

Ruby: def greet; @name; end
来源：http://hz.yanxiufei.cn/gtfbtnnqzg.html

C#:   public string Greet() => Name;
来源：http://hz.hnqzz.top/gtpfomjqmy.html

[G05] 继承
来源：http://hz.9152youxi.cn/gtckwgvemk.html

Py:   class Admin(User): pass
来源：http://hz.guowangkeji.top/gtjfknkkiu.html

PHP:  class Admin extends User {}
来源：http://hz.cqqwz.cn/gtmspapxxf.html

JS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtbwuoyuqq.html

TS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtyzpehbsh.html

Java: class Admin extends User {}
来源：http://hz.sysykeji.top/gtypkxfqya.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnxiangtu.top/gteusptzmx.html

Ruby: class Admin < User; end
来源：http://hz.jyoumei.cn/gtvtccuybw.html

C#:   class Admin : User {}
来源：http://hz.yj202588.top/gtlrjnbkmi.html

[G06] 重写方法
来源：http://hz.daria6918.cn/gtelbhoscu.html

Py:   def greet(self): return "admin"
来源：http://hz.jinyuanbaomall.cn/gtihfsxcys.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gttjiglemr.html

JS:   greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gtanlherph.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtmqwfbnpp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.meibo888.top/gtkreacqcl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenlongwang.top/gtgrcjlriy.html

Ruby: def greet; "admin"; end
来源：http://hz.9152youxi.cn/gttvwqtqdk.html

C#:   public override string Greet() => "admin";
来源：http://hz.jlsjyb.cn/gtjumqubpj.html

[G07] 调用父类方法
来源：http://hz.xingfuxueyuan.xyz/gtfvqkrzmg.html

Py:   super().greet()
来源：http://hz.birdmap.top/gtmqwlkmam.html

PHP:  parent::greet();
来源：http://hz.quarkkingdee.top/gtbgdphnaz.html

JS:   super.greet();
来源：http://hz.zhijiandao.cn/gtswvvzrkh.html

TS:   super.greet();
来源：http://hz.nanxinkj.top/gtdnckuwhl.html

Java: super.greet();
来源：http://hz.yuanzhike.top/gtxjgpoclb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guannengcc.top/gtfggcgonz.html

Ruby: super
来源：http://hz.yongpay.top/gthhsyrfhl.html

C#:   base.Greet();
来源：http://hz.kuanghao11.cn/gthtlmhszw.html

[G08] 静态方法与属性
来源：http://hz.xinyue.icu/gtildtyezu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgufenzy.top/gtbkwchqfo.html

PHP:  public static function f() {}
来源：http://hz.tianlin.xyz/gtmbrmzwlh.html

JS:   static f() {}
来源：http://hz.hysaishi.cn/gtfkgfywzo.html

TS:   static f(): void {}
来源：http://hz.yj20258.top/gtembdwnbg.html

Java: static void f() {}
来源：http://hz.zycfv.cn/gtpmzizmfa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.haohaochexian.top/gtisbdlqir.html

Ruby: def self.f; end
来源：http://hz.aizwys.cn/gtunxueved.html

C#:   public static void F() {}
来源：http://hz.pycfn.com/gtidewialf.html

[G09] 接口 / 抽象类
来源：http://hz.sufxvd.cn/gtcxjgozfd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hongshengwenyu.top/gtgjgntsac.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinghuilouyu.cn/gtlfspidju.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hammf.cn/gtljrzpphs.html

TS:   interface Shape { area(): number; }
来源：http://hz.zdqjudy.top/gtyszkxdmm.html

Java: interface Shape { double area(); }
来源：http://hz.gzhubu.top/gtdurtptrv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.c1oappe.top/gtitcfnxqi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xingfuxueyuan.xyz/gtbynkhqsb.html

C#:   interface IShape { double Area(); }
来源：http://hz.daxiang520.top/gtzgstlvpi.html

[G10] 访问控制
来源：http://hz.vqdsnc.cn/gtfjdjdljl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhixingplan.top/gtdkvjzhhn.html

PHP:  public / protected / private
来源：http://hz.cqqwz.cn/gtdpknrnkx.html

JS:   #private 字段；其余公开
来源：http://hz.c1oappe.top/gtssungnri.html

TS:   public / protected / private
来源：http://hz.yonumen.top/gtspfmaysa.html

Java: public / protected / private / 默认包级
来源：http://hz.jqgfzy.top/gtyacjirmg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sweek.top/gtybmlfzfh.html

Ruby: public / protected / private
来源：http://hz.jinqigfzy.top/gtsmujcokw.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangkeji.top/gtcwxlcphn.html

[G11] getter / setter
来源：http://hz.wangshuangyany.cn/gtyrtdngbx.html

Py:   @property 与 @x.setter
来源：http://hz.nanxuanxn.top/gtivgzojby.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtpgxygexp.html

JS:   get name() { return this._name; }
来源：http://hz.dashuyun.cn/gtslsvviqt.html

TS:   get name(): string { return this._name; }
来源：http://hz.gzhubu.top/gtsudrgctn.html

Java: public String getName() { return name; }
来源：http://hz.zhixingplan.top/gtwrbdptyo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtbubmbtot.html

Ruby: attr_accessor :name
来源：http://hz.havefunace.top/gtrcpxtbpx.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gtunwcydnt.html

[G12] 对象转字符串
来源：http://hz.hysaishi.cn/gtxwoibqwx.html

Py:   def __str__(self): return self.name
来源：http://hz.hongshengwenyu.top/gthmercnxs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtnlfruape.html

JS:   toString() { return this.name; }
来源：http://hz.xuanzx.com/gtqlzpfdut.html

TS:   toString(): string { return this.name; }
来源：http://hz.mhx1999.top/gtgcukpvlv.html

Java: @Override public String toString() { return name; }
来源：http://hz.daxiang520.top/gtarmhccqv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtetmvsikb.html

Ruby: def to_s; @name; end
来源：http://hz.jianghu66.top/gtvoyadmon.html

C#:   public override string ToString() => Name;
来源：http://hz.jinqigufen.top/gtcrtrgjcq.html

[G13] 判断对象类型
来源：http://hz.ehwqpu.com/gtvcwujcfc.html

Py:   isinstance(u, User)
来源：http://hz.andypj.xyz/gtiuirhrkk.html

PHP:  $u instanceof User
来源：http://hz.jqgufenzy.top/gtxqihusvb.html

JS:   u instanceof User
来源：http://hz.tian-w.cn/gtaruznong.html

TS:   u instanceof User
来源：http://hz.feifeiyinyue.top/gtafveqtwe.html

Java: u instanceof User
来源：http://hz.tanke756.top/gtdlbpxrse.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gotoacloud.top/gtfrprfunl.html

Ruby: u.is_a?(User)
来源：http://hz.shzxlz.cn/gtxlgjgndg.html

C#:   u is User
来源：http://hz.shuidangran.top/gtjtphehhq.html

[G14] 数据类 / record
来源：http://hz.yvedp.cn/gtoxnxyaaz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yanxiufei.cn/gtmriiptnd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fengsongda.top/gtbvgrurxp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhijiandao.cn/gtqjaeepuh.html

TS:   type User = { name: string; age: number };
来源：http://hz.meibo888.top/gtrrrbwwqq.html

Java: record User(String name, int age) {}
来源：http://hz.52xcode.cn/gtcemtxles.html

Go:   type User struct { Name string; Age int }
来源：http://hz.fengsongda.top/gthcvfqrxk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xingfuxueyuan.xyz/gtjtjedqea.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtwzymlepu.html

[G15] 枚举
来源：http://hz.zhaomingkeji.xyz/gtazkirypg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yueranfly.top/gtylkqwroe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258888.top/gtvstzrbpq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pycfn.com/gtdudqtqdr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtlfsmjujj.html

Java: enum Color { RED, GREEN }
来源：http://hz.ywan-chungtsiang.top/gtftzcwkvu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gttzhkjvey.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hywenlv.cn/gtwwbrrjmk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtysojmojd.html

[G16] 对象转数组 / 字典
来源：http://hz.ydzc1.top/gtphlpjzmo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.svipenyu.cn/gthaywljry.html

PHP:  get_object_vars($obj);
来源：http://hz.pengpengdd.cyou/gtqoawsdvb.html

JS:   Object.entries(obj)
来源：http://hz.birdmap.top/gthrlyeakv.html

TS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtoodypbwt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tian-w.cn/gtjbxfqhfx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgfzy.top/gtmvqwxdgv.html

Ruby: obj.instance_variables
来源：http://hz.yangfankeji.com/gtzgmomjyd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yongpay.top/gtykuceygd.html

================================================================================
来源：http://hz.zhiwuduotai.top/gteugcnzrg.html

H. 异常与错误处理
来源：http://hz.nanxinkj.top/gtrrxhrivf.html

================================================================================
来源：http://hz.jqgfzy.top/gtzfylsfew.html

[H01] try / catch 基础
来源：http://hz.pengpengdd.cyou/gtpyafpjmw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ivvv.top/gtmuaihxwo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.svipenyu.cn/gttugkuozu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtmwkfukfn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cucudq.cn/gtrlfyvwut.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hnxiangtu.top/gtiksljrnl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.52xcode.cn/gtvyozasme.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hammf.cn/gtattcvdnk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenzaomai.com/gtiunaccfs.html

[H02] finally / ensure 收尾
来源：http://hz.birdmap.top/gtcoccirxe.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hammf.cn/gtbumxzshr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtavyttqtl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtthyhpppd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtdqylghhy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtsmafdsei.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.svipenyu.cn/gtkokwgthp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gtnygcumld.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yanxiufei.cn/gtcrecgmml.html

[H03] 主动抛出异常
来源：http://hz.pengpengdd.cyou/gtpjxhialj.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtvajmtsgq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gaohongyu789.top/gtngdddyue.html

JS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtolcpqvzx.html

TS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtfftvooqr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtqdzxedoe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhengqikj.top/gtrtupphoi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhengqikj.top/gtdzskxkqb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtnhxwwxtp.html

[H04] 自定义异常类型
来源：http://hz.gzhubu.top/gtjjpcadql.html

Py:   class MyError(Exception): pass
来源：http://hz.havefunace.top/gtfgrapups.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangtech.top/gtbtmmheoc.html

JS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtsbovifmq.html

TS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gtewaibxsu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shuidangran.top/gtceagavxv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sufxvd.cn/gtxihlcxwm.html

Ruby: class MyError < StandardError; end
来源：http://hz.mhx1999.top/gtmxofcqpw.html

C#:   class MyException : Exception {}
来源：http://hz.ppjwa.cn/gtxopwaovh.html

[H05] 捕获特定类型
来源：http://hz.yj20258888.top/gtkmeuspfi.html

Py:   except ValueError as e:
来源：http://hz.chenzaomai.com/gtccakrbva.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pycfn.com/gtditamyix.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtffmwyebo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtbwyatlzg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenjidiqi.icu/gtnhxcsfur.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xylfe.cn/gtxuvcgnhz.html

Ruby: rescue ArgumentError => e
来源：http://hz.quarkkingdee.top/gtwordttge.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pycfn.com/gtqamytlik.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tian-w.cn/gtatoqutot.html

Py:   value = d.get("k") or default
来源：http://hz.zhiwuduotai.top/gtzktvrvxj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.andypj.xyz/gtfioikggo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shangyingyoupin.top/gtpdkbqlqp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtnmnhlvet.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.kuanghao11.cn/gtnqydlkgc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ppjwa.cn/gtklvroeei.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhaomingkeji.xyz/gthjgxlthu.html

C#:   obj?.A?.B ?? default
来源：http://hz.gaohongyu789.top/gtscgomhgy.html

[H07] 断言
来源：http://hz.yangfankeji.com/gtvfzsdxmy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.mhx1999.top/gtevhwlahg.html

PHP:  assert($x > 0);
来源：http://hz.pycfn.com/gtuhkhqniu.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtciidbdgh.html

TS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtsggekkpd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.0kj1m.cn/gtdvadqnnw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jlsjyb.cn/gtrinxnfvh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hongshengwenyu.top/gtbyhvvwck.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sweek.top/gtjqxepqnz.html

[H08] 获取错误信息与堆栈
来源：http://hz.jlsjyb.cn/gtxepvlurx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.havefunace.top/gtkyzlhhuj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxinkj.top/gtkpqaqshy.html

JS:   e.message;  e.stack
来源：http://hz.chenlongwang.top/gtigsztgpj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigufen.top/gtbltbqnqv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tianlin.xyz/gtsrjnfqsy.html

Go:   err.Error()
来源：http://hz.jiagoushi.top/gtggalmjmv.html


<!-- 参考信息 -->