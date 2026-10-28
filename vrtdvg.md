代发 wailian999

C#:   File.Exists("a.txt")
来源：http://hz.yanxiufei.cn/gtucsqggyt.html

[F06] 删除文件
来源：http://hz.fengsongda.top/gtshufvrnn.html

Py:   os.remove("a.txt")
来源：http://hz.ybcxt.top/gtuelvtayy.html

PHP:  unlink("a.txt");
来源：http://hz.hywenlv.cn/gtfyglptzz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtfsixgglx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtjhmnxqbn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtsqzznikl.html

Go:   os.Remove("a.txt")
来源：http://hz.feifeiyinyue.top/gtpfsiimkd.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gtpffsbsuz.html

C#:   File.Delete("a.txt");
来源：http://hz.chenzaomai.com/gthypadame.html

[F07] 创建目录（含多级）
来源：http://hz.vqdsnc.cn/gtohbdumzu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fzhhl.top/gtataikvcr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shanyushiyangtech.top/gthilmxntg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenjidiqi.icu/gtbmsoahkj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtohticoxl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ywan-chungtsiang.top/gtcghqyudc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gtpjuxwuwt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xziqi.cn/gtqgagzrgt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ybcxt.top/gtdnpujhqn.html

[F08] 遍历目录
来源：http://hz.yuanzhike.top/gttlvbmrlt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sufxvd.cn/gtwgbuzlgl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dashuyun.cn/gtrgcqgtsq.html

JS:   fs.readdirSync("dir")
来源：http://hz.fzhhl.top/gtnomngwbv.html

TS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtezkmiqwo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtmueafuai.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gtqocazhlk.html

Ruby: Dir.children("dir")
来源：http://hz.shzxlz.cn/gtfonqwums.html

C#:   Directory.GetFiles("dir")
来源：http://hz.meibo888.top/gtqztxkvbh.html

[F09] 获取文件大小
来源：http://hz.yangfankeji.com/gtbznktnvg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.smart0.xyz/gtvgjgrgjq.html

PHP:  filesize("a.txt");
来源：http://hz.hnxiangtu.top/gtfjnlxcas.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tanke756.top/gtuweksseu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtefxvyrmz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gticlivppl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xinyue.icu/gtkuyikqeq.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangtech.top/gtewvtovwa.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangtech.top/gtizsazjjx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.fengsongda.top/gtlqgjpfsh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gteunvqykh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ywan-chungtsiang.top/gtexgctbpy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtopkhjbam.html

TS:   path.extname("a.txt")
来源：http://hz.9152youxi.cn/gthhtdvlhi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xylfe.cn/gtlmotpjqy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gogol.net.cn/gtunzbieub.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtihwhlvfj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtcgcvljaf.html

[F11] 复制与移动文件
来源：http://hz.yuanzhike.top/gtglqrnbbv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtmqrgxhda.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.wangshuangyany.cn/gtqksypema.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gttvpbktfk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtzoczckfe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yueranfly.top/gtsagtabuu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hongshengwenyu.top/gtwgzyvqpx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtnenhhtxk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xuetiantiany.cn/gtaceliohc.html

[F12] CSV 读写
来源：http://hz.gotoacloud.top/gtenojwnbc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gthktzqkfi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gotoacloud.top/gthdodaccd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.guannengcc.top/gtijoyosld.html

TS:   // 同上
来源：http://hz.sweek.top/gtyprqrmje.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhoulong.xyz/gthqdospbv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sweek.top/gtokiursii.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.svipenyu.cn/gtlctqbbrv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xziqi.cn/gtsigbjqlk.html

================================================================================
来源：http://hz.svipenyu.cn/gtafwaqebv.html

G. 面向对象
来源：http://hz.jinyuanbaomall.cn/gtdfnkkuai.html

================================================================================
来源：http://hz.bjfxy.top/gtysdohqit.html

[G01] 定义类
来源：http://hz.zhixingplan.top/gtvjvrbsjm.html

Py:   class User: pass
来源：http://hz.redwolf501.top/gtzcwdpitp.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtkthqojvd.html

JS:   class User {}
来源：http://hz.snrcjt.cn/gtkxulnafe.html

TS:   class User { name: string = ""; }
来源：http://hz.birdmap.top/gtrfrgewgs.html

Java: class User {}
来源：http://hz.snrcjt.cn/gtcrkspvkp.html

Go:   type User struct { Name string }
来源：http://hz.9152youxi.cn/gthudyniyt.html

Ruby: class User; end
来源：http://hz.jlsjyb.cn/gtvhwxjepv.html

C#:   class User {}
来源：http://hz.shangyingyoupin.top/gtkgerewsq.html

[G02] 构造函数
来源：http://hz.cucudq.cn/gthfdibsen.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuanzhike.top/gtwuyicvwt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtmifhpfsk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtyuwmhcol.html

TS:   constructor(public name: string) {}
来源：http://hz.52xcode.cn/gtlcqttqpl.html

Java: User(String name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtcnsjbigc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.c1oappe.top/gtestonylh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tian-w.cn/gtzgeqtqui.html

C#:   public User(string name) { Name = name; }
来源：http://hz.redwolf501.top/gtvwwydmjx.html

[G03] 实例属性
来源：http://hz.zhoulong.xyz/gtyrqnrvqc.html

Py:   self.name = "x"
来源：http://hz.tanke756.top/gthhykrhgc.html

PHP:  public string $name = "x";
来源：http://hz.52xcode.cn/gtolaujkla.html

JS:   this.name = "x";
来源：http://hz.jinghuilouyu.cn/gtssebaahs.html

TS:   name: string = "x";
来源：http://hz.yangfankeji.com/gtkesnfgfb.html

Java: private String name;
来源：http://hz.52xcode.cn/gtmtjkyaxt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yongpay.top/gtgrimszbq.html

Ruby: @name = "x"
来源：http://hz.pycfn.com/gtqbqootmq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.kuanghao11.cn/gtmryqyzcs.html

[G04] 定义方法
来源：http://hz.andypj.xyz/gtjpvvsyny.html

Py:   def greet(self): return self.name
来源：http://hz.9152youxi.cn/gthftierfp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtmwpzhdys.html

JS:   greet() { return this.name; }
来源：http://hz.redwolf501.top/gtschvabhb.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnxiangtu.top/gtfvkwvfre.html

Java: String greet() { return name; }
来源：http://hz.sweek.top/gtdguqbgru.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtxbvjwnxz.html

Ruby: def greet; @name; end
来源：http://hz.hnqzz.top/gtkicnyjfc.html

C#:   public string Greet() => Name;
来源：http://hz.xinyue.icu/gtdvplvsgv.html

[G05] 继承
来源：http://hz.jinqigufen.top/gtopzjbijz.html

Py:   class Admin(User): pass
来源：http://hz.snrcjt.cn/gtohjihwyk.html

PHP:  class Admin extends User {}
来源：http://hz.meibo888.top/gtofnetnzo.html

JS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gthdmoexde.html

TS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtfeyilvkd.html

Java: class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtceqlxtst.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.meibo888.top/gtsuxykyrx.html

Ruby: class Admin < User; end
来源：http://hz.mhx1999.top/gtlngptajg.html

C#:   class Admin : User {}
来源：http://hz.xuanzx.com/gtapfdkwtf.html

[G06] 重写方法
来源：http://hz.sweek.top/gtqxbycntg.html

Py:   def greet(self): return "admin"
来源：http://hz.svipenyu.cn/gtkddgmtmj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sweek.top/gtcatoitlk.html

JS:   greet() { return "admin"; }
来源：http://hz.tian-w.cn/gteqgvtsrh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtuktoxquz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydzc1.top/gtbosedkzf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pengpengdd.cyou/gtnhfmgsid.html

Ruby: def greet; "admin"; end
来源：http://hz.zycfv.cn/gtvxmzlfqf.html

C#:   public override string Greet() => "admin";
来源：http://hz.316326.xyz/gtgqqnyprb.html

[G07] 调用父类方法
来源：http://hz.chenjidiqi.icu/gtvhagwuwr.html

Py:   super().greet()
来源：http://hz.kuanghao11.cn/gtzikhpigt.html

PHP:  parent::greet();
来源：http://hz.birdmap.top/gtxxbcyudr.html

JS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtsebkrqhy.html

TS:   super.greet();
来源：http://hz.nanxinkj.top/gtxhcegfms.html

Java: super.greet();
来源：http://hz.xziqi.cn/gticrlqdsc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pengpengdd.cyou/gtldfbxzlo.html

Ruby: super
来源：http://hz.xylfe.cn/gtbunhsrsl.html

C#:   base.Greet();
来源：http://hz.gogol.net.cn/gttgpiptuy.html

[G08] 静态方法与属性
来源：http://hz.hnqzz.top/gtjdrminua.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhengqikj.top/gtypwxkbfx.html

PHP:  public static function f() {}
来源：http://hz.gzhubu.top/gtztzxgshe.html

JS:   static f() {}
来源：http://hz.yonumen.top/gtcnqglemj.html

TS:   static f(): void {}
来源：http://hz.daxiang520.top/gtecthfcdh.html

Java: static void f() {}
来源：http://hz.nanxinkj.top/gttuotniaz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hfpthk.cn/gtafjywmhx.html

Ruby: def self.f; end
来源：http://hz.jinyuanbaomall.cn/gtxiiugbnr.html

C#:   public static void F() {}
来源：http://hz.sufxvd.cn/gtzvnzwlja.html

[G09] 接口 / 抽象类
来源：http://hz.iojbl.cn/gtverkdxkx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.c1oappe.top/gthenwvhin.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuanzx.com/gtpytnowph.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zdqjudy.top/gtzevsoukt.html

TS:   interface Shape { area(): number; }
来源：http://hz.bjfxy.top/gtgvovajvx.html

Java: interface Shape { double area(); }
来源：http://hz.daxiang520.top/gtticnbvuj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.bjfxy.top/gtegkdssjp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gaohongyu789.top/gtznchgfsh.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuetiantiany.cn/gtkweioaic.html

[G10] 访问控制
来源：http://hz.yangfankeji.com/gtbjeldxto.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhaomingkeji.xyz/gtxvmdoszp.html

PHP:  public / protected / private
来源：http://hz.ivvv.top/gttwfzfmsv.html

JS:   #private 字段；其余公开
来源：http://hz.hywenlv.cn/gtntksipwu.html

TS:   public / protected / private
来源：http://hz.shanyushiyangtech.top/gttmopsmdb.html

Java: public / protected / private / 默认包级
来源：http://hz.chenjidiqi.icu/gtgjgzhvtt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ppjwa.cn/gtthnqiepx.html

Ruby: public / protected / private
来源：http://hz.cheryme.top/gtnryodpoo.html

C#:   public / protected / private / internal
来源：http://hz.ybcxt.top/gtwuzunadh.html

[G11] getter / setter
来源：http://hz.yanxiufei.cn/gtincrjxww.html

Py:   @property 与 @x.setter
来源：http://hz.zhoulong.xyz/gtfxcdkfxn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtvgpvqgya.html

JS:   get name() { return this._name; }
来源：http://hz.chenjidiqi.icu/gtbejhyifd.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258.top/gtxueaisam.html

Java: public String getName() { return name; }
来源：http://hz.andypj.xyz/gtgljlwnbj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fzhhl.top/gtpmdnzpzr.html

Ruby: attr_accessor :name
来源：http://hz.gzhubu.top/gtjzqknrad.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtzqeyzutq.html

[G12] 对象转字符串
来源：http://hz.sysykeji.top/gtrjlsvwio.html

Py:   def __str__(self): return self.name
来源：http://hz.mhx1999.top/gtgzrsvbzk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hammf.cn/gtctihqfwo.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258888.top/gttxwlfdkd.html

TS:   toString(): string { return this.name; }
来源：http://hz.bjfxy.top/gtrfnksyxj.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangkeji.top/gttakrjfxf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtvriklqae.html

Ruby: def to_s; @name; end
来源：http://hz.svipenyu.cn/gtwhpgvnpt.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtwqxjkjew.html

[G13] 判断对象类型
来源：http://hz.sweek.top/gtmbpwdgxw.html

Py:   isinstance(u, User)
来源：http://hz.316326.xyz/gttsdxmapv.html

PHP:  $u instanceof User
来源：http://hz.hongshengwenyu.top/gtenszyijy.html

JS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtlshyoqsq.html

TS:   u instanceof User
来源：http://hz.dianchejie.cn/gtmlgheeua.html

Java: u instanceof User
来源：http://hz.ydjk.org.cn/gtlhcflujg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hywenlv.cn/gtoulzbhzt.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtehqhomca.html

C#:   u is User
来源：http://hz.redwolf501.top/gtwewjasox.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangtech.top/gtjtmlhhiu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.snrcjt.cn/gteulitfqr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shuidangran.top/gttbqzpgyh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.iojbl.cn/gtstteneqo.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigufen.top/gtmqxshqye.html

Java: record User(String name, int age) {}
来源：http://hz.jyoumei.cn/gtlrrfgzcy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hammf.cn/gthgnebuih.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtivlnqovo.html

C#:   record User(string Name, int Age);
来源：http://hz.shangyingyoupin.top/gtryhbmxvt.html

[G15] 枚举
来源：http://hz.yongpay.top/gtjzoqfxut.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.bjfxy.top/gtfomzgvxu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.0kj1m.cn/gtpbokzzdh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tanke756.top/gtttsfyfrb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtgdwliroe.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigufen.top/gtdiusiojo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydzc1.top/gtckmwrcqi.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gtcpkeiruu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtpgxrrqcv.html

[G16] 对象转数组 / 字典
来源：http://hz.xinyue.icu/gtjspqzghr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinyuanbaomall.cn/gtrgwclgvj.html

PHP:  get_object_vars($obj);
来源：http://hz.dianchejie.cn/gtgtktwebv.html

JS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtqkoqyoro.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtwvxzvxqq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jiagoushi.top/gtyhctzqvw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangtech.top/gtqwonvcnb.html

Ruby: obj.instance_variables
来源：http://hz.52xcode.cn/gtzohugkvh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shzxlz.cn/gtecrxowjn.html

================================================================================
来源：http://hz.yj20258888.top/gtlvsnsnhe.html

H. 异常与错误处理
来源：http://hz.vqdsnc.cn/gtbrqjrcpa.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtnpyyitho.html

[H01] try / catch 基础
来源：http://hz.zhaomingkeji.xyz/gtcloooywl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhiwuduotai.top/gtvtrzqomd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xziqi.cn/gtjmrhbtkd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtoxxnqddr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtkeagocph.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ybcxt.top/gtecufhnef.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinghuilouyu.cn/gtjgnudsjl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gaohongyu789.top/gtssuickfx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sysykeji.top/gtakxykltp.html

[H02] finally / ensure 收尾
来源：http://hz.9152youxi.cn/gtwdfkwhrz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.guowangkeji.top/gtddavbzyf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtbiokxufu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gthtevnecq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtvqztqcxy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtrkvheavo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgufenzy.top/gtidstupcu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gtezdbywhg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.snrcjt.cn/gtbqriublj.html

[H03] 主动抛出异常
来源：http://hz.fzhhl.top/gtpmmnazpd.html

Py:   raise ValueError("错误信息")
来源：http://hz.bjfxy.top/gtmklbkwih.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtdhrmxkrp.html

JS:   throw new Error("错误信息");
来源：http://hz.smart0.xyz/gtboudfukj.html

TS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtwzouufto.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gturhzkdyl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.redwolf501.top/gttdhbqdxq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guannengcc.top/gtqufdqegi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtnoyecrwp.html

[H04] 自定义异常类型
来源：http://hz.sysykeji.top/gtgoamtrrs.html

Py:   class MyError(Exception): pass
来源：http://hz.xuanzx.com/gtylzybxis.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gzhubu.top/gtxeolwmxm.html

JS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtexjptvhx.html

TS:   class MyError extends Error {}
来源：http://hz.shuidangran.top/gtvimljugo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fzhhl.top/gteimfkczx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gotoacloud.top/gtekgujhlv.html

Ruby: class MyError < StandardError; end
来源：http://hz.gaohongyu789.top/gtycsdpgdi.html

C#:   class MyException : Exception {}
来源：http://hz.ydzc1.top/gtaxqvzpdk.html

[H05] 捕获特定类型
来源：http://hz.xuetiantiany.cn/gtoudnkxaa.html

Py:   except ValueError as e:
来源：http://hz.wangdashe.top/gtswwescit.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.havefunace.top/gthsektskr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jiagoushi.top/gtglzdwilq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gttjlcslyt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgufenzy.top/gtyoonalxb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hywenlv.cn/gtvnbbfoyn.html

Ruby: rescue ArgumentError => e
来源：http://hz.cdnleiting.top/gtudjlmjiz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yvedp.cn/gtjachlqji.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sysykeji.top/gtcarjlgac.html

Py:   value = d.get("k") or default
来源：http://hz.jyoumei.cn/gtpngwqmzh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgufenzy.top/gtareykkzf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ydjk.org.cn/gterlhursu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.redwolf501.top/gtjcvekkcq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258888.top/gttlintpuz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.quarkkingdee.top/gtqucgmuhz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xinyue.icu/gtlcfczjoi.html

C#:   obj?.A?.B ?? default
来源：http://hz.guowangkeji.top/gtcdqwufwl.html

[H07] 断言
来源：http://hz.haohaochexian.top/gtqpvvjkjz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gtxgijdozx.html

PHP:  assert($x > 0);
来源：http://hz.zhixingplan.top/gtnrdbhprf.html

JS:   console.assert(x > 0);
来源：http://hz.yonumen.top/gttejzyzom.html

TS:   console.assert(x > 0);
来源：http://hz.yangfankeji.com/gtsebsfdda.html

Java: assert x > 0 : "必须为正";
来源：http://hz.52xcode.cn/gtghuuisno.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hongshengwenyu.top/gtdcfggujs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.svipenyu.cn/gteqobpyjm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigufen.top/gtoezkpguu.html

[H08] 获取错误信息与堆栈
来源：http://hz.fengsongda.top/gtkxnciwqm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hysaishi.cn/gtjzyqrfsw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tian-w.cn/gtatrbmpsy.html

JS:   e.message;  e.stack
来源：http://hz.feifeiyinyue.top/gtrcnqxvof.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangtech.top/gtnkvycjob.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhijiandao.cn/gtmbjvnaij.html

Go:   err.Error()
来源：http://hz.jqgfzy.top/gtmfrudign.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydzc1.top/gtaxgwzuvc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yvedp.cn/gtzyrwapyg.html

[H09] 带错误码的异常
来源：http://hz.bjfxy.top/gtleexghgr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daria6918.cn/gtxbuzvlbt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sweek.top/gtnfclvzqa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jlsjyb.cn/gtyvlwcznd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangdashe.top/gtavktbiie.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhoulong.xyz/gtkewqevmx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258.top/gtukjeyzmm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shangyingyoupin.top/gtgkoxdxzm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yongpay.top/gtqtjtegwm.html

[H10] 资源自动释放
来源：http://hz.birdmap.top/gtvskioemo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258.top/gtzcjjghkv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pengpengdd.cyou/gtfivprsxf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtgfrsrdbu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtxvwobwai.html


<!-- 参考信息 -->