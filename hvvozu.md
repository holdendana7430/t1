代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daria6918.cn/gtyvupwsqt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtawrnicoo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dianchejie.cn/gtpiplurkc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.bjfxy.top/gtktwrlzhw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnxiangtu.top/gtaimrppmo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gzhubu.top/gtnindtinj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.haohaochexian.top/gtanrphmwr.html

[F04] 追加写入文件
来源：http://hz.daria6918.cn/gtgthbrvlk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.andypj.xyz/gtvwewhzhu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinyuanbaomall.cn/gtcpubwrlh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigufen.top/gtkontbyno.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangkeji.top/gtichirkxj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.fengsongda.top/gtbewwsexy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.havefunace.top/gtwxgdojpf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yueranfly.top/gtalemjaly.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sxryk.cn/gtytyfclwy.html

[F05] 判断文件或目录是否存在
来源：http://hz.yanxiufei.cn/gtvhmanvoa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cqqwz.cn/gtgatwlnal.html

PHP:  file_exists("a.txt");
来源：http://hz.zhongyouzk.top/gtkecprvcl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cqqwz.cn/gtnyklbslp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gttmoozovh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtreumhgio.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydzc1.top/gtgrhcijsx.html

Ruby: File.exist?("a.txt")
来源：http://hz.jianghu66.top/gttufnqsuq.html

C#:   File.Exists("a.txt")
来源：http://hz.yj202588.top/gtbkfturqw.html

[F06] 删除文件
来源：http://hz.mhx1999.top/gtprfxkruk.html

Py:   os.remove("a.txt")
来源：http://hz.cheryme.top/gtiokgxxnx.html

PHP:  unlink("a.txt");
来源：http://hz.jinyuanbaomall.cn/gttzyfrbut.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtllmzyxxd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtecojzbmg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtvqqsuqbc.html

Go:   os.Remove("a.txt")
来源：http://hz.gaohongyu789.top/gtjlgpqsgx.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gtssnnpzhp.html

C#:   File.Delete("a.txt");
来源：http://hz.zdqjudy.top/gtoyyalzip.html

[F07] 创建目录（含多级）
来源：http://hz.shuidangran.top/gtlopixyxi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gotoacloud.top/gtpmbtfwup.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gotoacloud.top/gtdfzseqeu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtxuwmavzn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtvidmdtub.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuetiantiany.cn/gtwoywzmxw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sxryk.cn/gtrpqjksbf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xziqi.cn/gttekpadbr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xinyue.icu/gtujfmwtmc.html

[F08] 遍历目录
来源：http://hz.andypj.xyz/gtoxrenjfg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.9152youxi.cn/gtkqalupeb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigfzy.top/gtexojuhpt.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gtakzqjbgn.html

TS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtrtoeqknf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jiagoushi.top/gtorzhqbdc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.snrcjt.cn/gtfldqgzha.html

Ruby: Dir.children("dir")
来源：http://hz.cqqwz.cn/gtafjxnxxc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.0kj1m.cn/gtytkdqpii.html

[F09] 获取文件大小
来源：http://hz.yj202588.top/gtisycgmkn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.svipenyu.cn/gtkinbjuoj.html

PHP:  filesize("a.txt");
来源：http://hz.yangfankeji.com/gtqxjtucfk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gtlhnrsqao.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tian-w.cn/gtnislkdsc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtjofydjmk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yangfankeji.com/gthtogmuix.html

Ruby: File.size("a.txt")
来源：http://hz.ybcxt.top/gtlujyfpzb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.quarkkingdee.top/gtfnmzhhgu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.aizwys.cn/gtcnbqicxu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtdbnwzfpr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yonumen.top/gtfvcihfvy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtvdtlrndt.html

TS:   path.extname("a.txt")
来源：http://hz.jlsjyb.cn/gtokxcthsk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.0kj1m.cn/gteylxfpcm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jiagoushi.top/gtmmpecgzi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtuhscyzpq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtelhhgbgg.html

[F11] 复制与移动文件
来源：http://hz.pengpengdd.cyou/gtuwvieszc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtsvpuygir.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gtxpzunqjm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtvwrmkliz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtrdmmnkhk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sufxvd.cn/gtopzitibn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.quarkkingdee.top/gtlwhdbymi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtyixttvhz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tianlin.xyz/gtdtesivqi.html

[F12] CSV 读写
来源：http://hz.sxryk.cn/gtvsdmjftk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cashguo.top/gtgakujfwq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.wangdashe.top/gtobwmgfuj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.iojbl.cn/gtukgnygrq.html

TS:   // 同上
来源：http://hz.nwbrower.top/gtwmxqhfez.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.quarkkingdee.top/gtadvzqfpq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shangyingyoupin.top/gtuhkvjdzn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.redwolf501.top/gtkxbelabm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guannengcc.top/gtahssrgwg.html

================================================================================
来源：http://hz.tianlin.xyz/gtukgtkurc.html

G. 面向对象
来源：http://hz.ehwqpu.com/gtceeyjvlf.html

================================================================================
来源：http://hz.jyoumei.cn/gtglfhbyzj.html

[G01] 定义类
来源：http://hz.316326.xyz/gtbwghfiud.html

Py:   class User: pass
来源：http://hz.iojbl.cn/gtcmmsqovm.html

PHP:  class User {}
来源：http://hz.iojbl.cn/gtbeduakiu.html

JS:   class User {}
来源：http://hz.daxiang520.top/gtqgtvlxcg.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtmqwbhwko.html

Java: class User {}
来源：http://hz.gzhubu.top/gtysxxsugk.html

Go:   type User struct { Name string }
来源：http://hz.9152youxi.cn/gtzqlqoqjk.html

Ruby: class User; end
来源：http://hz.hywenlv.cn/gtfxzzlfnr.html

C#:   class User {}
来源：http://hz.xuanzx.com/gtbtpbwqvw.html

[G02] 构造函数
来源：http://hz.daria6918.cn/gthzogytez.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.tanke756.top/gtiobsewhb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pycfn.com/gtgixgafxs.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gtejdpsdkl.html

TS:   constructor(public name: string) {}
来源：http://hz.xingfuxueyuan.xyz/gtppjqkhgh.html

Java: User(String name) { this.name = name; }
来源：http://hz.daria6918.cn/gthvjavijn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shzxlz.cn/gthkdymyxq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jianghu66.top/gtkmxdmzbn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shangyingyoupin.top/gtucmgpton.html

[G03] 实例属性
来源：http://hz.pycfn.com/gtmfrvydao.html

Py:   self.name = "x"
来源：http://hz.sweek.top/gtwzbjqosp.html

PHP:  public string $name = "x";
来源：http://hz.shuidangran.top/gtglqmfbcz.html

JS:   this.name = "x";
来源：http://hz.yanxiufei.cn/gtjxpeazux.html

TS:   name: string = "x";
来源：http://hz.ywan-chungtsiang.top/gtwnojmjlp.html

Java: private String name;
来源：http://hz.sysykeji.top/gtzmffdegt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuxming.cn/gtckjnjdmv.html

Ruby: @name = "x"
来源：http://hz.0kj1m.cn/gtadwsdohd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydzc1.top/gtuqybhfcv.html

[G04] 定义方法
来源：http://hz.yongpay.top/gtczylfhhb.html

Py:   def greet(self): return self.name
来源：http://hz.mhx1999.top/gtpijqjwvf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtsmpnglww.html

JS:   greet() { return this.name; }
来源：http://hz.hnxiangtu.top/gtiklaubwr.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtxfkntnqs.html

Java: String greet() { return name; }
来源：http://hz.316326.xyz/gtkkisbzyp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtdphpmiuh.html

Ruby: def greet; @name; end
来源：http://hz.316326.xyz/gtdhsztkis.html

C#:   public string Greet() => Name;
来源：http://hz.smart0.xyz/gtmjquxhgy.html

[G05] 继承
来源：http://hz.tanke756.top/gtmdpeaezm.html

Py:   class Admin(User): pass
来源：http://hz.yueranfly.top/gtjfjwhiwf.html

PHP:  class Admin extends User {}
来源：http://hz.zycfv.cn/gtyclmjtri.html

JS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtoctjftud.html

TS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtcoqpiove.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtlwklovbc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hysaishi.cn/gtnyvkzafq.html

Ruby: class Admin < User; end
来源：http://hz.bjfxy.top/gtyswigmer.html

C#:   class Admin : User {}
来源：http://hz.smart0.xyz/gtpziytrhg.html

[G06] 重写方法
来源：http://hz.quarkkingdee.top/gttjmmuqti.html

Py:   def greet(self): return "admin"
来源：http://hz.yueranfly.top/gtbanbnkck.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtqwccttxb.html

JS:   greet() { return "admin"; }
来源：http://hz.yanxiufei.cn/gtqhwmndcg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gttqgnilya.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtadkwqwvj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cdnleiting.top/gtiyfhfmbj.html

Ruby: def greet; "admin"; end
来源：http://hz.xingfuxueyuan.xyz/gtqdmhtzvd.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuetiantiany.cn/gtrxzbemnh.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangtech.top/gtlegvwugg.html

Py:   super().greet()
来源：http://hz.yanxiufei.cn/gtzwmdxdmm.html

PHP:  parent::greet();
来源：http://hz.pycfn.com/gtvxhgqocx.html

JS:   super.greet();
来源：http://hz.havefunace.top/gtgimwrmuq.html

TS:   super.greet();
来源：http://hz.shzxlz.cn/gteqmstdqh.html

Java: super.greet();
来源：http://hz.shanyushiyangtech.top/gtgcrekorg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jiagoushi.top/gtzmhsuvom.html

Ruby: super
来源：http://hz.andypj.xyz/gtdgqqhtsp.html

C#:   base.Greet();
来源：http://hz.sweek.top/gtyedvjemu.html

[G08] 静态方法与属性
来源：http://hz.svipenyu.cn/gtjufcjdsy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dianchejie.cn/gtahmpbrjp.html

PHP:  public static function f() {}
来源：http://hz.jqgfzy.top/gtilfikjvh.html

JS:   static f() {}
来源：http://hz.daxiang520.top/gtybunjmph.html

TS:   static f(): void {}
来源：http://hz.jlsjyb.cn/gtprjcvoat.html

Java: static void f() {}
来源：http://hz.guowangkeji.top/gthvldiway.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yongpay.top/gtpzqbqaon.html

Ruby: def self.f; end
来源：http://hz.hnxiangtu.top/gtfrcdbuaj.html

C#:   public static void F() {}
来源：http://hz.xuetiantiany.cn/gtfsftarjx.html

[G09] 接口 / 抽象类
来源：http://hz.fengsongda.top/gtummejsog.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhengqikj.top/gtgvwxbocd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.redwolf501.top/gtrjxyhhod.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenlongwang.top/gtrxwvuaph.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuanzx.com/gtigdcmnac.html

Java: interface Shape { double area(); }
来源：http://hz.shangyingyoupin.top/gtxqbmjmvy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gtmtpntafb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuxming.cn/gtqamrpjnt.html

C#:   interface IShape { double Area(); }
来源：http://hz.ppjwa.cn/gtzutijxte.html

[G10] 访问控制
来源：http://hz.smart0.xyz/gtqmjoomkh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xziqi.cn/gtwtknmybk.html

PHP:  public / protected / private
来源：http://hz.yj20258888.top/gtzofrmoxs.html

JS:   #private 字段；其余公开
来源：http://hz.yanxiufei.cn/gtnxyduuwd.html

TS:   public / protected / private
来源：http://hz.xingfuxueyuan.xyz/gtjrrezddl.html

Java: public / protected / private / 默认包级
来源：http://hz.kuanghao11.cn/gtshlzcxyr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.kuanghao11.cn/gtrzdqifmz.html

Ruby: public / protected / private
来源：http://hz.dianchejie.cn/gtoihibgdg.html

C#:   public / protected / private / internal
来源：http://hz.zhaomingkeji.xyz/gtvvqbexft.html

[G11] getter / setter
来源：http://hz.hywenlv.cn/gtildvwniw.html

Py:   @property 与 @x.setter
来源：http://hz.jiagoushi.top/gtapnoiqou.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtsvydphpb.html

JS:   get name() { return this._name; }
来源：http://hz.zdqjudy.top/gtuwoddovs.html

TS:   get name(): string { return this._name; }
来源：http://hz.xuanzx.com/gtknrbooxx.html

Java: public String getName() { return name; }
来源：http://hz.gaohongyu789.top/gtufkqqajn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dashuyun.cn/gtgfdkcxmq.html

Ruby: attr_accessor :name
来源：http://hz.quarkkingdee.top/gtweftzbxi.html

C#:   public string Name { get; set; }
来源：http://hz.pengpengdd.cyou/gtjowtadbs.html

[G12] 对象转字符串
来源：http://hz.yj20258.top/gtomfkcbvq.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gtczbpfovp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtnvffpigr.html

JS:   toString() { return this.name; }
来源：http://hz.wangshuangyany.cn/gtjdtvwdwl.html

TS:   toString(): string { return this.name; }
来源：http://hz.sysykeji.top/gtyputumuf.html

Java: @Override public String toString() { return name; }
来源：http://hz.dianchejie.cn/gtfdzuwfrf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtcitfezit.html

Ruby: def to_s; @name; end
来源：http://hz.zhijiandao.cn/gteceoerwz.html

C#:   public override string ToString() => Name;
来源：http://hz.ybcxt.top/gtasyrnrge.html

[G13] 判断对象类型
来源：http://hz.jiagoushi.top/gtdhaqxnqk.html

Py:   isinstance(u, User)
来源：http://hz.yuanzhike.top/gtifndzcgr.html

PHP:  $u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtqxuoraao.html

JS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtwdkiycgn.html

TS:   u instanceof User
来源：http://hz.ppjwa.cn/gtdewuldai.html

Java: u instanceof User
来源：http://hz.chenlongwang.top/gtxgogzdqg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.haohaochexian.top/gtxxubpoqr.html

Ruby: u.is_a?(User)
来源：http://hz.shzxlz.cn/gtlmuxvwzg.html

C#:   u is User
来源：http://hz.hammf.cn/gtphsgfnel.html

[G14] 数据类 / record
来源：http://hz.zhaomingkeji.xyz/gttmzfsnkm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gogol.net.cn/gtmvqoebak.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fengsongda.top/gtrysobpii.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenzaomai.com/gtpvntwgcg.html

TS:   type User = { name: string; age: number };
来源：http://hz.shanyushiyangkeji.top/gtykabhuoj.html

Java: record User(String name, int age) {}
来源：http://hz.wangshuangyany.cn/gtfkfvcwrj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgufenzy.top/gtcmdsbsrj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangshuangyany.cn/gtjzhlobij.html

C#:   record User(string Name, int Age);
来源：http://hz.xylfe.cn/gtociuaxuf.html

[G15] 枚举
来源：http://hz.dianchejie.cn/gtlewifhxs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fengsongda.top/gtitudkadi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shuidangran.top/gthhwynzql.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.quarkkingdee.top/gtsqusjonq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhixingplan.top/gtqapanrkl.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuetiantiany.cn/gtzpotircr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtffzupgtm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hnqzz.top/gtjcspnbjo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtpbgngvbh.html

[G16] 对象转数组 / 字典
来源：http://hz.ivvv.top/gtfdrleftk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sufxvd.cn/gtsljpqhyv.html

PHP:  get_object_vars($obj);
来源：http://hz.sysykeji.top/gtxuprbrwh.html

JS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtpjoagtqt.html

TS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gthcxkrput.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xylfe.cn/gtcrezkkhh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinghuilouyu.cn/gthrwlhvag.html

Ruby: obj.instance_variables
来源：http://hz.ybcxt.top/gtkirtrprt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yongpay.top/gtacllevmm.html

================================================================================
来源：http://hz.jianghu66.top/gtkusthxpr.html

H. 异常与错误处理
来源：http://hz.ivvv.top/gtjvqxazqr.html

================================================================================
来源：http://hz.jianghu66.top/gtnbgcppfk.html

[H01] try / catch 基础
来源：http://hz.yj20258888.top/gtqlaqnias.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhaomingkeji.xyz/gtlnstlgpe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pengpengdd.cyou/gtjtwqdrki.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtpntydkzu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jianghu66.top/gtthlciinc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gtlmldyign.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenlongwang.top/gtdsfnmebk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258888.top/gtjtufywkd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.fzhhl.top/gttngzepwk.html

[H02] finally / ensure 收尾
来源：http://hz.daria6918.cn/gtoinlmvmg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj202588.top/gtiibofhdk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gttpuchyli.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtlpjsvrlt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtcnmxowyx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtmiyedkzn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tianlin.xyz/gtfjlcuqve.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yangfankeji.com/gtdzjsxlbr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenlongwang.top/gtcpdoyycn.html

[H03] 主动抛出异常
来源：http://hz.sxryk.cn/gtktpsimbh.html

Py:   raise ValueError("错误信息")
来源：http://hz.yvedp.cn/gtpooiiryw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtehggjnct.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtxikdomxe.html

TS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtjvzfpyys.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cheryme.top/gtkciypknw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aibaodan.cn/gthstyexvt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gotoacloud.top/gttcudtjgm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cheryme.top/gtgoxpihpl.html

[H04] 自定义异常类型
来源：http://hz.shzxlz.cn/gtqltwpovo.html

Py:   class MyError(Exception): pass
来源：http://hz.haohaochexian.top/gtdcjlhrry.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtajidjwpp.html

JS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtlqzjyvda.html

TS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtbczvxach.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sysykeji.top/gtjiaqnpsf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhijiandao.cn/gtdkzybyyj.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinyuanbaomall.cn/gttlbrkipq.html

C#:   class MyException : Exception {}
来源：http://hz.chenlongwang.top/gtxxbjxcea.html

[H05] 捕获特定类型
来源：http://hz.shuidangran.top/gtkajmgrcj.html

Py:   except ValueError as e:
来源：http://hz.redwolf501.top/gtyhphdiui.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhiwuduotai.top/gtlpsugzle.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtuorvxjkm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtmbzlqcnb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.pycfn.com/gtpakvebxs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydzc1.top/gtfqqdvblg.html

Ruby: rescue ArgumentError => e
来源：http://hz.xziqi.cn/gtaotcdbfe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhiwuduotai.top/gtjbyxwgov.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinghuilouyu.cn/gtrzxhhxvl.html

Py:   value = d.get("k") or default
来源：http://hz.vqdsnc.cn/gtebufacnn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gtpmkzxtpr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtuaszxfmp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hfpthk.cn/gtvyafzbxl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtswmzohui.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cdnleiting.top/gtaaskcgna.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guowangkeji.top/gtjiznfrqr.html

C#:   obj?.A?.B ?? default
来源：http://hz.quarkkingdee.top/gtfuejpoht.html

[H07] 断言
来源：http://hz.yueranfly.top/gtfcoyufyk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhiwuduotai.top/gtxjfvknth.html

PHP:  assert($x > 0);
来源：http://hz.yvedp.cn/gthlcvvkpg.html

JS:   console.assert(x > 0);
来源：http://hz.wangshuangyany.cn/gthcggxtso.html

TS:   console.assert(x > 0);
来源：http://hz.jqgufenzy.top/gtowwdqzot.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sysykeji.top/gtwwdtbbvx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jianghu66.top/gtfuwgvyvh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zdqjudy.top/gtkgvnqdkh.html


<!-- 参考信息 -->