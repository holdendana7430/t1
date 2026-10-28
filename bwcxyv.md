代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gtewssqpro.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.9152youxi.cn/gtbafmmrue.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hysaishi.cn/gtvvyjtyao.html

[F04] 追加写入文件
来源：http://hz.zhongyouzk.top/gtqkgewvlz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydzc1.top/gtrympoysy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenjidiqi.icu/gtuyywfsvw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtjxajmquq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenlongwang.top/gtinzrrikt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ybcxt.top/gtnrscdztd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nanxinkj.top/gtyvmbtram.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pengpengdd.cyou/gtajvuwpuo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.bjfxy.top/gtpvkdcguf.html

[F05] 判断文件或目录是否存在
来源：http://hz.iojbl.cn/gtmomysxfy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.havefunace.top/gttqmfksbb.html

PHP:  file_exists("a.txt");
来源：http://hz.yj20258888.top/gtmemybwgx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtkmbegeeg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgfzy.top/gtwirywkbu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtlszcakee.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hysaishi.cn/gthtqoyare.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxuanxn.top/gtcooguuyo.html

C#:   File.Exists("a.txt")
来源：http://hz.cashguo.top/gtcethzfdt.html

[F06] 删除文件
来源：http://hz.jinyuanbaomall.cn/gtimbsslnk.html

Py:   os.remove("a.txt")
来源：http://hz.iojbl.cn/gtdkcrymkf.html

PHP:  unlink("a.txt");
来源：http://hz.haohaochexian.top/gtldwmcmbz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gtueycrynf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gttysrdkud.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtmohiwhmb.html

Go:   os.Remove("a.txt")
来源：http://hz.gzhubu.top/gtonxfjhtv.html

Ruby: File.delete("a.txt")
来源：http://hz.yongpay.top/gtxdmaxhqj.html

C#:   File.Delete("a.txt");
来源：http://hz.hfpthk.cn/gtcigrlfyr.html

[F07] 创建目录（含多级）
来源：http://hz.yvedp.cn/gtwrxmmqkc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pycfn.com/gtxzfjbxjc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuxming.cn/gtcjkeylyj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuanzhike.top/gtspaogydv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guannengcc.top/gtxgnulwnn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jiagoushi.top/gtqsjpnhdw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shanyushiyangtech.top/gtgnpmeemu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.iojbl.cn/gtsizakvso.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sufxvd.cn/gtpzunvgpk.html

[F08] 遍历目录
来源：http://hz.quarkkingdee.top/gtbjdsyefb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.bjfxy.top/gtpbeddvfp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ppjwa.cn/gttpvzuzck.html

JS:   fs.readdirSync("dir")
来源：http://hz.smart0.xyz/gtwjmipbyv.html

TS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtwkjcwzzo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gtwxueqiki.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tianlin.xyz/gtpsirysuh.html

Ruby: Dir.children("dir")
来源：http://hz.cucudq.cn/gtldujumkr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ehwqpu.com/gtywdyzzeo.html

[F09] 获取文件大小
来源：http://hz.zhijiandao.cn/gtyolhrmwc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ppjwa.cn/gtreakauxu.html

PHP:  filesize("a.txt");
来源：http://hz.gzhubu.top/gtovyjpxtp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtpmmoyapb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtxraqntqs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtjfldbpcj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258888.top/gtyxhtuxku.html

Ruby: File.size("a.txt")
来源：http://hz.9152youxi.cn/gtbqtqagxp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ivvv.top/gtjiycrtbf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shanyushiyangtech.top/gtlasmkxhb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtkopqfpvy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yangfankeji.com/gtvpstewda.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtnpexjimr.html

TS:   path.extname("a.txt")
来源：http://hz.ydzc1.top/gtyzragyts.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xylfe.cn/gttjcezpff.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtdihbtmol.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtdsmefpxm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ybcxt.top/gtnmzjhbjh.html

[F11] 复制与移动文件
来源：http://hz.zhengqikj.top/gtmipxuair.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtvepsghhv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gteahudzor.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gttchukllt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtxzzedeog.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aizwys.cn/gtjtradkug.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jyoumei.cn/gtbpczwzqh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gthkzfjpav.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.birdmap.top/gtcifejcuz.html

[F12] CSV 读写
来源：http://hz.guowangkeji.top/gtvwpoetke.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.fengsongda.top/gtkokuibyy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fengsongda.top/gtjkrcdxpr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jiagoushi.top/gtvtvmfkru.html

TS:   // 同上
来源：http://hz.hfpthk.cn/gtxdemdpjv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigufen.top/gtkbewulho.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.9152youxi.cn/gtsevavbki.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gogol.net.cn/gtuyuhjjvy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.316326.xyz/gtwxmwkyno.html

================================================================================
来源：http://hz.gotoacloud.top/gtfdvqxulr.html

G. 面向对象
来源：http://hz.andypj.xyz/gtnixkfssp.html

================================================================================
来源：http://hz.guannengcc.top/gtmxatykfd.html

[G01] 定义类
来源：http://hz.gzhubu.top/gtfwckmgcx.html

Py:   class User: pass
来源：http://hz.haohaochexian.top/gttfpogzak.html

PHP:  class User {}
来源：http://hz.zhixingplan.top/gtpwwomlao.html

JS:   class User {}
来源：http://hz.yj202588.top/gtfcmqnfop.html

TS:   class User { name: string = ""; }
来源：http://hz.tianlin.xyz/gtfvhyrfjx.html

Java: class User {}
来源：http://hz.zdqjudy.top/gtekvaozju.html

Go:   type User struct { Name string }
来源：http://hz.cdnleiting.top/gtioruefnm.html

Ruby: class User; end
来源：http://hz.316326.xyz/gtyuyaqyno.html

C#:   class User {}
来源：http://hz.dashuyun.cn/gtkouxkefn.html

[G02] 构造函数
来源：http://hz.chenjidiqi.icu/gtyjiupizw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sufxvd.cn/gtbexferyi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.dianchejie.cn/gtfagfzfsa.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.birdmap.top/gtcunvzhny.html

TS:   constructor(public name: string) {}
来源：http://hz.birdmap.top/gtgczaooaq.html

Java: User(String name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtsgkivtfg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhijiandao.cn/gtuopsvtqf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenjidiqi.icu/gtxcoxkejc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.aizwys.cn/gtjlwrsxxw.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gttwfpricl.html

Py:   self.name = "x"
来源：http://hz.guowangkeji.top/gtmbhribzx.html

PHP:  public string $name = "x";
来源：http://hz.jqgfzy.top/gtppzjeymy.html

JS:   this.name = "x";
来源：http://hz.sysykeji.top/gtyuwegbfu.html

TS:   name: string = "x";
来源：http://hz.shanyushiyangkeji.top/gtrdqsosoh.html

Java: private String name;
来源：http://hz.sweek.top/gtujpufhuo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gotoacloud.top/gtvoxsuwrj.html

Ruby: @name = "x"
来源：http://hz.0kj1m.cn/gtlqmoiqcy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yanxiufei.cn/gtbvtkyitk.html

[G04] 定义方法
来源：http://hz.yj20258888.top/gtbmgrolrj.html

Py:   def greet(self): return self.name
来源：http://hz.daxiang520.top/gtlzsgbwlw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ivvv.top/gtsrtljroi.html

JS:   greet() { return this.name; }
来源：http://hz.fzhhl.top/gtgkezseby.html

TS:   greet(): string { return this.name; }
来源：http://hz.dashuyun.cn/gtenqflbuk.html

Java: String greet() { return name; }
来源：http://hz.zhijiandao.cn/gtfsprshhc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tian-w.cn/gtbwxzblvs.html

Ruby: def greet; @name; end
来源：http://hz.316326.xyz/gtppqcvrwv.html

C#:   public string Greet() => Name;
来源：http://hz.xuetiantiany.cn/gtauptglxe.html

[G05] 继承
来源：http://hz.ehwqpu.com/gtacavmcwk.html

Py:   class Admin(User): pass
来源：http://hz.yangfankeji.com/gtqfzenhik.html

PHP:  class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtwlkndomz.html

JS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtgsjfcnck.html

TS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gtqxmzxlxd.html

Java: class Admin extends User {}
来源：http://hz.guowangkeji.top/gtshmcpvuf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hysaishi.cn/gtnoagpdvw.html

Ruby: class Admin < User; end
来源：http://hz.sufxvd.cn/gtuufzwlmm.html

C#:   class Admin : User {}
来源：http://hz.ehwqpu.com/gtjscxvoyy.html

[G06] 重写方法
来源：http://hz.guannengcc.top/gtclegztct.html

Py:   def greet(self): return "admin"
来源：http://hz.zhijiandao.cn/gtsblgeqlv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtnupxbbmy.html

JS:   greet() { return "admin"; }
来源：http://hz.sweek.top/gtxtrnshdu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jyoumei.cn/gtpeshsjhu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gtvwwcmxyk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yonumen.top/gtjqqvzrlu.html

Ruby: def greet; "admin"; end
来源：http://hz.chenzaomai.com/gtxcjcsjfk.html

C#:   public override string Greet() => "admin";
来源：http://hz.jianghu66.top/gtbiozpndp.html

[G07] 调用父类方法
来源：http://hz.jqgufenzy.top/gtkaavhzyu.html

Py:   super().greet()
来源：http://hz.chenlongwang.top/gtrnqxntbi.html

PHP:  parent::greet();
来源：http://hz.hywenlv.cn/gtezsyyjuw.html

JS:   super.greet();
来源：http://hz.havefunace.top/gttiilbpyd.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtsyxmqgdi.html

Java: super.greet();
来源：http://hz.chenzaomai.com/gtgbqktvkg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tian-w.cn/gtjuerrnus.html

Ruby: super
来源：http://hz.zhaomingkeji.xyz/gttdhfamwq.html

C#:   base.Greet();
来源：http://hz.jinqigfzy.top/gtmnjnvpxj.html

[G08] 静态方法与属性
来源：http://hz.316326.xyz/gtmtgxxitt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sysykeji.top/gtfpycsqku.html

PHP:  public static function f() {}
来源：http://hz.sysykeji.top/gtrlkjaxbu.html

JS:   static f() {}
来源：http://hz.wangdashe.top/gttnlwswmx.html

TS:   static f(): void {}
来源：http://hz.jianghu66.top/gtmcmdoiqf.html

Java: static void f() {}
来源：http://hz.dashuyun.cn/gttofvoinf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangkeji.top/gtahnwpdww.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtweeaidpl.html

C#:   public static void F() {}
来源：http://hz.yonumen.top/gtccvvwhhw.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangtech.top/gtoeqekdvo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jlsjyb.cn/gtfcvtjsqn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cdnleiting.top/gtczziczjh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pycfn.com/gtjmwwcuvm.html

TS:   interface Shape { area(): number; }
来源：http://hz.tian-w.cn/gtkfdyovsh.html

Java: interface Shape { double area(); }
来源：http://hz.yuxming.cn/gtfgjqsyif.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sxryk.cn/gtpejgevdp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gzhubu.top/gtbhywjycn.html

C#:   interface IShape { double Area(); }
来源：http://hz.shanyushiyangkeji.top/gtrennhirj.html

[G10] 访问控制
来源：http://hz.yj202588.top/gtuuqzjcyw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yangfankeji.com/gtzucbsvfh.html

PHP:  public / protected / private
来源：http://hz.jqgfzy.top/gtwewnhxod.html

JS:   #private 字段；其余公开
来源：http://hz.yueranfly.top/gtgephrmvh.html

TS:   public / protected / private
来源：http://hz.daria6918.cn/gtorglwdnh.html

Java: public / protected / private / 默认包级
来源：http://hz.shangyingyoupin.top/gtlhajbtis.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gtfqaxcibi.html

Ruby: public / protected / private
来源：http://hz.andypj.xyz/gtbvyrlcbx.html

C#:   public / protected / private / internal
来源：http://hz.cqqwz.cn/gtzirtlhfq.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtkcydahrc.html

Py:   @property 与 @x.setter
来源：http://hz.vqdsnc.cn/gtvfbskmbm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtjcsbsgsb.html

JS:   get name() { return this._name; }
来源：http://hz.chenjidiqi.icu/gtiropicyz.html

TS:   get name(): string { return this._name; }
来源：http://hz.yanxiufei.cn/gtjdsjadnf.html

Java: public String getName() { return name; }
来源：http://hz.pengpengdd.cyou/gtfigqwamm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangdashe.top/gtymdflmmn.html

Ruby: attr_accessor :name
来源：http://hz.havefunace.top/gtomlpodjk.html

C#:   public string Name { get; set; }
来源：http://hz.yueranfly.top/gtnccqtawc.html

[G12] 对象转字符串
来源：http://hz.smart0.xyz/gtcuzgwxqi.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigfzy.top/gtvbkitxet.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtmxgobylf.html

JS:   toString() { return this.name; }
来源：http://hz.xuanzx.com/gthyphtwai.html

TS:   toString(): string { return this.name; }
来源：http://hz.daxiang520.top/gtnssxqdhy.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenzaomai.com/gtfhhgtmzh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.0kj1m.cn/gtwdhtkfvn.html

Ruby: def to_s; @name; end
来源：http://hz.snrcjt.cn/gtdxbsxpgg.html

C#:   public override string ToString() => Name;
来源：http://hz.jianghu66.top/gtqzuukljx.html

[G13] 判断对象类型
来源：http://hz.sufxvd.cn/gttbonzkbk.html

Py:   isinstance(u, User)
来源：http://hz.jqgfzy.top/gtihqbnubg.html

PHP:  $u instanceof User
来源：http://hz.snrcjt.cn/gtgbtppneu.html

JS:   u instanceof User
来源：http://hz.andypj.xyz/gtbvohkmmf.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtczwuwtqw.html

Java: u instanceof User
来源：http://hz.ybcxt.top/gtmyqmwmyt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenlongwang.top/gtrjlfkpie.html

Ruby: u.is_a?(User)
来源：http://hz.ydjk.org.cn/gttctdczae.html

C#:   u is User
来源：http://hz.jinghuilouyu.cn/gttjqcykds.html

[G14] 数据类 / record
来源：http://hz.daria6918.cn/gtpgywhfwv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yuxming.cn/gtkauyfymg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuetiantiany.cn/gtxkwqrrmt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgfzy.top/gtqpgvylrc.html

TS:   type User = { name: string; age: number };
来源：http://hz.ybcxt.top/gtbatszbtc.html

Java: record User(String name, int age) {}
来源：http://hz.xingfuxueyuan.xyz/gtaxefkgni.html

Go:   type User struct { Name string; Age int }
来源：http://hz.birdmap.top/gtuyymtadc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangtech.top/gtdgogfyxm.html

C#:   record User(string Name, int Age);
来源：http://hz.wangshuangyany.cn/gtvwxggcqb.html

[G15] 枚举
来源：http://hz.mhx1999.top/gtqckedhrf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hfpthk.cn/gtwebmvpqk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jqgfzy.top/gtsaviwapf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangshuangyany.cn/gttudfeubd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtsvgsetgc.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gtnkgqdrpu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinyuanbaomall.cn/gtjqjsrgve.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxuanxn.top/gtdyjnypwf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yangfankeji.com/gtoyecvegw.html

[G16] 对象转数组 / 字典
来源：http://hz.zdqjudy.top/gtxzslzvha.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhongyouzk.top/gtqgvqfjsh.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gtsqgnwhwo.html

JS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtbzmblgeu.html

TS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtorvdfzqk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.andypj.xyz/gtdvmbnxgg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nanxinkj.top/gthnpnenrn.html

Ruby: obj.instance_variables
来源：http://hz.zhengqikj.top/gtdxbkxcpg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nwbrower.top/gtsgnwgpqq.html

================================================================================
来源：http://hz.ybcxt.top/gtmukfiyur.html

H. 异常与错误处理
来源：http://hz.guowangkeji.top/gtuupnrkdr.html

================================================================================
来源：http://hz.quarkkingdee.top/gtbromtwfp.html

[H01] try / catch 基础
来源：http://hz.zhixingplan.top/gtejnygdag.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pengpengdd.cyou/gtrlswmdgl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.wangdashe.top/gtwnetetvc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.bjfxy.top/gtwyeoqpwi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangdashe.top/gtcalfdtto.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.haohaochexian.top/gtjtngxlad.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenzaomai.com/gtzimllyqp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hfpthk.cn/gtjfwsvmvg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jyoumei.cn/gtrxumtlwm.html

[H02] finally / ensure 收尾
来源：http://hz.zhijiandao.cn/gtcdgcsnsm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.iojbl.cn/gtxqemvcnn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtcrqnzxxi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtlulnyckx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gttwahtkys.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtxwpddita.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pycfn.com/gtxvykakmb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gtvgtmyume.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.9152youxi.cn/gtjlcawkuy.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gtzzmnmnkk.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhijiandao.cn/gtmwengluu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtkcrnfbfi.html

JS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtwdudrmgd.html

TS:   throw new Error("错误信息");
来源：http://hz.gotoacloud.top/gtkluhwqvd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtxzwousmo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.feifeiyinyue.top/gtbsfqbffy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cdnleiting.top/gtfsjgyopv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtqhaxffiw.html

[H04] 自定义异常类型
来源：http://hz.zhongyouzk.top/gthgltunab.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgufenzy.top/gtjoxgqcdc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtnnglplnb.html

JS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtkrgfxzza.html

TS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gtiqunvafq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guannengcc.top/gtboggekhp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sweek.top/gttjugvrwk.html

Ruby: class MyError < StandardError; end
来源：http://hz.jyoumei.cn/gthgweoipa.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtwxaprmhq.html

[H05] 捕获特定类型
来源：http://hz.zdqjudy.top/gtxkbxwhiu.html

Py:   except ValueError as e:
来源：http://hz.yj202588.top/gtkwdhsdcw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangkeji.top/gtezqeoyjp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.9152youxi.cn/gtvvdgsuaj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtfsughmpz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.havefunace.top/gtiircrscp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gogol.net.cn/gtbioxcnih.html

Ruby: rescue ArgumentError => e
来源：http://hz.nwbrower.top/gtckdjbiph.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sufxvd.cn/gtghhthqgr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guannengcc.top/gtqkpjptzb.html

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gtsjsihrof.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gaohongyu789.top/gtcprvrqdy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtltexjjjb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtkllkumbm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhoulong.xyz/gtumukknfp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yonumen.top/gtnpcgfxik.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangkeji.top/gtvaviznnj.html

C#:   obj?.A?.B ?? default
来源：http://hz.mhx1999.top/gtljmpxofm.html

[H07] 断言
来源：http://hz.zhaomingkeji.xyz/gtxjgkgsdu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxinkj.top/gttklcjllq.html

PHP:  assert($x > 0);
来源：http://hz.hnxiangtu.top/gtykciolpi.html

JS:   console.assert(x > 0);
来源：http://hz.feifeiyinyue.top/gteidauxxm.html

TS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gthjawtgdp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hysaishi.cn/gtcaciqmeo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gzhubu.top/gtpuqwxjsy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ehwqpu.com/gtdkduiapf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yuxming.cn/gtvkxjriti.html

[H08] 获取错误信息与堆栈
来源：http://hz.tanke756.top/gtmlhdcnhe.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tianlin.xyz/gtnmumuojt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xingfuxueyuan.xyz/gtlumaagqv.html


<!-- 参考信息 -->