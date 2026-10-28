代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gtbodljrqm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtdajpyeie.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.andypj.xyz/gtqotebbya.html

Ruby: File.exist?("a.txt")
来源：http://hz.ppjwa.cn/gtskjqwlsz.html

C#:   File.Exists("a.txt")
来源：http://hz.ivvv.top/gtnqfzjxkt.html

[F06] 删除文件
来源：http://hz.pengpengdd.cyou/gtocjculxq.html

Py:   os.remove("a.txt")
来源：http://hz.jinqigfzy.top/gtjgufhoqy.html

PHP:  unlink("a.txt");
来源：http://hz.ybcxt.top/gtknhpdnrt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnxiangtu.top/gtvwtejiee.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gtyqqhqmws.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtrboeswzp.html

Go:   os.Remove("a.txt")
来源：http://hz.shuidangran.top/gtvbsnohzf.html

Ruby: File.delete("a.txt")
来源：http://hz.jiagoushi.top/gttozdmyaa.html

C#:   File.Delete("a.txt");
来源：http://hz.svipenyu.cn/gtcrbtongt.html

[F07] 创建目录（含多级）
来源：http://hz.mhx1999.top/gtftwyltjt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuanzx.com/gtbyadnanz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinyuanbaomall.cn/gthkjzqzni.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtmnazwjps.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hongshengwenyu.top/gttjyuyqot.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cheryme.top/gttlvyzpnq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aizwys.cn/gtwmzvaqbx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shangyingyoupin.top/gtmmcyqasq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.fzhhl.top/gteiyccazn.html

[F08] 遍历目录
来源：http://hz.gotoacloud.top/gtghpxnojf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangtech.top/gtolqxaqcj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cqqwz.cn/gtpjvmyavz.html

JS:   fs.readdirSync("dir")
来源：http://hz.aizwys.cn/gtrpvmekvl.html

TS:   fs.readdirSync("dir")
来源：http://hz.xuetiantiany.cn/gtjswwxuwg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.pycfn.com/gtezihscva.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.52xcode.cn/gtllciaueb.html

Ruby: Dir.children("dir")
来源：http://hz.jinqigfzy.top/gtrqvbwxrt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aizwys.cn/gtvsuvkedn.html

[F09] 获取文件大小
来源：http://hz.zhengqikj.top/gtaulunpqv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.feifeiyinyue.top/gterkhpuhh.html

PHP:  filesize("a.txt");
来源：http://hz.iojbl.cn/gtfdounbsg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenjidiqi.icu/gtkmgscpmg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gtnujvyeio.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtrvvzsupl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.daxiang520.top/gtwmyvdzti.html

Ruby: File.size("a.txt")
来源：http://hz.yangfankeji.com/gtuffqclee.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daxiang520.top/gtdnmkarab.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.bjfxy.top/gtkvnsgubk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gtenjtduum.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yongpay.top/gtpfqxrdcm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtqabpjncv.html

TS:   path.extname("a.txt")
来源：http://hz.yangfankeji.com/gtxlluimcp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shangyingyoupin.top/gtcnqvsphd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.andypj.xyz/gtpijcyxzp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtsqbybqmj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtjyiwbwlm.html

[F11] 复制与移动文件
来源：http://hz.nwbrower.top/gtpcjtrsyd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtziunfisr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhixingplan.top/gtqnqbhwlh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtepjyzcby.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtmemudklx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aizwys.cn/gtfxpqtihs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tianlin.xyz/gtvsjvoutn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtyaiwymdp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigfzy.top/gthsghxzfq.html

[F12] CSV 读写
来源：http://hz.xuanzx.com/gtetluoedt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhengqikj.top/gtloyufabr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cheryme.top/gthiiauyxo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xziqi.cn/gtyenrwpeo.html

TS:   // 同上
来源：http://hz.iojbl.cn/gttzyxqcie.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtwyipmrmn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sysykeji.top/gtcwnllwdx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jlsjyb.cn/gtaepwqfbk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nwbrower.top/gtpfumzgun.html

================================================================================
来源：http://hz.yj202588.top/gthomvegdl.html

G. 面向对象
来源：http://hz.zhoulong.xyz/gtrkfyzbbr.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtftikzyjj.html

[G01] 定义类
来源：http://hz.zhaomingkeji.xyz/gtlhcsfuaa.html

Py:   class User: pass
来源：http://hz.nanxinkj.top/gtjkpwzydd.html

PHP:  class User {}
来源：http://hz.gzhubu.top/gtqeiqjgdf.html

JS:   class User {}
来源：http://hz.yuxming.cn/gteqwbdypw.html

TS:   class User { name: string = ""; }
来源：http://hz.ydjk.org.cn/gthxdwgadl.html

Java: class User {}
来源：http://hz.ybcxt.top/gtitvigltx.html

Go:   type User struct { Name string }
来源：http://hz.pycfn.com/gttbjclnhs.html

Ruby: class User; end
来源：http://hz.kuanghao11.cn/gtbdhtamlr.html

C#:   class User {}
来源：http://hz.cqqwz.cn/gtciuwysgu.html

[G02] 构造函数
来源：http://hz.hywenlv.cn/gtiefehzkz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cqqwz.cn/gteglddyfm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj202588.top/gtkjlvuyqf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sweek.top/gtlmntcppq.html

TS:   constructor(public name: string) {}
来源：http://hz.yvedp.cn/gtuictysxh.html

Java: User(String name) { this.name = name; }
来源：http://hz.sweek.top/gtbmsgaqff.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.smart0.xyz/gtlmkaymow.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.iojbl.cn/gtjlakituv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhengqikj.top/gtedvfvhew.html

[G03] 实例属性
来源：http://hz.dashuyun.cn/gtqiavtzff.html

Py:   self.name = "x"
来源：http://hz.yonumen.top/gtedmcvuio.html

PHP:  public string $name = "x";
来源：http://hz.gotoacloud.top/gtvddgrefy.html

JS:   this.name = "x";
来源：http://hz.0kj1m.cn/gtrjufpakk.html

TS:   name: string = "x";
来源：http://hz.jinqigufen.top/gttlwwykdb.html

Java: private String name;
来源：http://hz.xuetiantiany.cn/gtjhfdsbxd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.birdmap.top/gtskqbjnan.html

Ruby: @name = "x"
来源：http://hz.yueranfly.top/gtddmgfpkt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhijiandao.cn/gtetexdoxq.html

[G04] 定义方法
来源：http://hz.sweek.top/gtwckarsnu.html

Py:   def greet(self): return self.name
来源：http://hz.xuanzx.com/gtcegnvpfv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tian-w.cn/gthcoglgra.html

JS:   greet() { return this.name; }
来源：http://hz.yuanzhike.top/gtcbduwlio.html

TS:   greet(): string { return this.name; }
来源：http://hz.ydzc1.top/gtnqhvezis.html

Java: String greet() { return name; }
来源：http://hz.yanxiufei.cn/gtqrlunuoa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hysaishi.cn/gtszwgmlff.html

Ruby: def greet; @name; end
来源：http://hz.xziqi.cn/gtudfioqeh.html

C#:   public string Greet() => Name;
来源：http://hz.wangshuangyany.cn/gtyeandwcf.html

[G05] 继承
来源：http://hz.cucudq.cn/gtuktlothw.html

Py:   class Admin(User): pass
来源：http://hz.gaohongyu789.top/gtbbgcgxqk.html

PHP:  class Admin extends User {}
来源：http://hz.xylfe.cn/gtpuufzjso.html

JS:   class Admin extends User {}
来源：http://hz.mhx1999.top/gtbqibkejq.html

TS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtvaqaanmk.html

Java: class Admin extends User {}
来源：http://hz.redwolf501.top/gtspqdlxor.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yangfankeji.com/gtvkbmzwhp.html

Ruby: class Admin < User; end
来源：http://hz.hongshengwenyu.top/gtkbdvyprl.html

C#:   class Admin : User {}
来源：http://hz.gogol.net.cn/gtidtkyxsf.html

[G06] 重写方法
来源：http://hz.dashuyun.cn/gttenmnqoj.html

Py:   def greet(self): return "admin"
来源：http://hz.ywan-chungtsiang.top/gtwkjyzcuc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenzaomai.com/gtmoqqvfyk.html

JS:   greet() { return "admin"; }
来源：http://hz.haohaochexian.top/gtesflmmsr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gthwoltlja.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtrlpgpqtk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yongpay.top/gtuzbducat.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgufenzy.top/gtavnqpjyl.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhixingplan.top/gtybkcrmwj.html

[G07] 调用父类方法
来源：http://hz.tianlin.xyz/gtpvrwagup.html

Py:   super().greet()
来源：http://hz.tanke756.top/gtgtjnspfm.html

PHP:  parent::greet();
来源：http://hz.9152youxi.cn/gtncgtmbwb.html

JS:   super.greet();
来源：http://hz.yangfankeji.com/gtkvcoqeex.html

TS:   super.greet();
来源：http://hz.zhixingplan.top/gtgzdynrab.html

Java: super.greet();
来源：http://hz.yuxming.cn/gtklhtpxxz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dianchejie.cn/gtuirbxerg.html

Ruby: super
来源：http://hz.c1oappe.top/gtbtvmlwta.html

C#:   base.Greet();
来源：http://hz.cqqwz.cn/gtszgncmjt.html

[G08] 静态方法与属性
来源：http://hz.yj20258.top/gtbbafwmsq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.mhx1999.top/gtllpudxxb.html

PHP:  public static function f() {}
来源：http://hz.316326.xyz/gthklnwbzs.html

JS:   static f() {}
来源：http://hz.sxryk.cn/gtrrfyuxuk.html

TS:   static f(): void {}
来源：http://hz.ydzc1.top/gtnecwyxif.html

Java: static void f() {}
来源：http://hz.yanxiufei.cn/gtbjtwkrab.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.kuanghao11.cn/gtzuulesoy.html

Ruby: def self.f; end
来源：http://hz.kuanghao11.cn/gtjtopdypj.html

C#:   public static void F() {}
来源：http://hz.ehwqpu.com/gtpnbfcqwz.html

[G09] 接口 / 抽象类
来源：http://hz.xuetiantiany.cn/gtsimexcet.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guannengcc.top/gtcbuatefp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jqgfzy.top/gtsswbsrsr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.smart0.xyz/gtaadtpbyx.html

TS:   interface Shape { area(): number; }
来源：http://hz.svipenyu.cn/gtfqpwlguy.html

Java: interface Shape { double area(); }
来源：http://hz.xuanzx.com/gthyecfxsy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gotoacloud.top/gtvocycjbe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.snrcjt.cn/gtoqcjnqan.html

C#:   interface IShape { double Area(); }
来源：http://hz.shangyingyoupin.top/gtlrmgzkhx.html

[G10] 访问控制
来源：http://hz.gzhubu.top/gtvzrqgdbw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.316326.xyz/gtyhejnkte.html

PHP:  public / protected / private
来源：http://hz.guannengcc.top/gtmqqzubcn.html

JS:   #private 字段；其余公开
来源：http://hz.cdnleiting.top/gtfkdzvlkn.html

TS:   public / protected / private
来源：http://hz.hfpthk.cn/gtdutufpui.html

Java: public / protected / private / 默认包级
来源：http://hz.ppjwa.cn/gtipauhaiu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hfpthk.cn/gtguwmithi.html

Ruby: public / protected / private
来源：http://hz.iojbl.cn/gtrlwcjqrz.html

C#:   public / protected / private / internal
来源：http://hz.zhijiandao.cn/gtmzutwcey.html

[G11] getter / setter
来源：http://hz.kuanghao11.cn/gtxcnufvto.html

Py:   @property 与 @x.setter
来源：http://hz.fengsongda.top/gtesxeqjzw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtfjucexpk.html

JS:   get name() { return this._name; }
来源：http://hz.jqgufenzy.top/gtocsvosgi.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gtziifpyit.html

Java: public String getName() { return name; }
来源：http://hz.guowangkeji.top/gtyjxllcoo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhengqikj.top/gtorsqctal.html

Ruby: attr_accessor :name
来源：http://hz.jqgfzy.top/gtivguoxjx.html

C#:   public string Name { get; set; }
来源：http://hz.meibo888.top/gtaovkzwdt.html

[G12] 对象转字符串
来源：http://hz.aibaodan.cn/gtrlmbdkjv.html

Py:   def __str__(self): return self.name
来源：http://hz.yongpay.top/gtcvnilnae.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtbonnxhjt.html

JS:   toString() { return this.name; }
来源：http://hz.cashguo.top/gtzwvicxqg.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnqzz.top/gtzcqpisht.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258888.top/gtpzkjhrfr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.c1oappe.top/gtejigjucf.html

Ruby: def to_s; @name; end
来源：http://hz.wangshuangyany.cn/gtkbzjqljv.html

C#:   public override string ToString() => Name;
来源：http://hz.xuanzx.com/gtoqmdvhbw.html

[G13] 判断对象类型
来源：http://hz.sysykeji.top/gtnekuoxtr.html

Py:   isinstance(u, User)
来源：http://hz.cheryme.top/gtjvomwwbq.html

PHP:  $u instanceof User
来源：http://hz.sxryk.cn/gttjupsyap.html

JS:   u instanceof User
来源：http://hz.dashuyun.cn/gtgzsgtevb.html

TS:   u instanceof User
来源：http://hz.smart0.xyz/gtswnyuvhg.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gthmrfelbn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ybcxt.top/gtqeeslfsd.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtpqhlrmhy.html

C#:   u is User
来源：http://hz.zhoulong.xyz/gtsyszjeyu.html

[G14] 数据类 / record
来源：http://hz.ydjk.org.cn/gtiplxvyaz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.316326.xyz/gtgfmtjcjg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gteagleiuv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.kuanghao11.cn/gtjimgavia.html

TS:   type User = { name: string; age: number };
来源：http://hz.mhx1999.top/gtcyjwhbks.html

Java: record User(String name, int age) {}
来源：http://hz.hfpthk.cn/gtbrafktdj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.havefunace.top/gtodwygvkt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtucbexenk.html

C#:   record User(string Name, int Age);
来源：http://hz.pengpengdd.cyou/gtexchqpcu.html

[G15] 枚举
来源：http://hz.zhengqikj.top/gtybqmhblj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jiagoushi.top/gtpnktrgxc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.birdmap.top/gtmdynudzp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.feifeiyinyue.top/gtgbgecymk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gtcytkzhxm.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhixingplan.top/gtrfawxzxt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tanke756.top/gtjbmtwxce.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shangyingyoupin.top/gteukxycvb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenzaomai.com/gtakebumzu.html

[G16] 对象转数组 / 字典
来源：http://hz.meibo888.top/gttsicjprc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenjidiqi.icu/gtzdqplicz.html

PHP:  get_object_vars($obj);
来源：http://hz.jinyuanbaomall.cn/gtgobzhcxg.html

JS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtoscjwrps.html

TS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gtxaaogaeq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.c1oappe.top/gtyffipxli.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtisvmlxvr.html

Ruby: obj.instance_variables
来源：http://hz.gogol.net.cn/gtpbpexwdu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gtluncsjgo.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgiqfiwum.html

H. 异常与错误处理
来源：http://hz.zhixingplan.top/gtjavjniod.html

================================================================================
来源：http://hz.ivvv.top/gtiuswlnjn.html

[H01] try / catch 基础
来源：http://hz.ehwqpu.com/gtmzfhxobi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinyuanbaomall.cn/gtjprsmevx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuxming.cn/gtakjalafb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj202588.top/gtiffukgdw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtalvanrmp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangshuangyany.cn/gtsgdwxfjz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hammf.cn/gtekctbcmk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydjk.org.cn/gtihtcrolz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shuidangran.top/gtrcjjsjmw.html

[H02] finally / ensure 收尾
来源：http://hz.wangdashe.top/gtuydjibkr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinyuanbaomall.cn/gtdcwnkrcn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtpbepwfch.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gthvurzkmt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtworapzlz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtxetpdosw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tian-w.cn/gtbwutoptz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ybcxt.top/gtdrpggyae.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tianlin.xyz/gtpokpknqr.html

[H03] 主动抛出异常
来源：http://hz.zdqjudy.top/gtwivugxky.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhixingplan.top/gtpccgqopc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gthunmuepx.html

JS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtfopfavzy.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxuanxn.top/gtwcyqgsil.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gthcbjyzvo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hfpthk.cn/gtvrthklqb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aizwys.cn/gtntpmdefq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtpfepeoro.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtcpdwukjg.html

Py:   class MyError(Exception): pass
来源：http://hz.0kj1m.cn/gtkphhuubp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yonumen.top/gtfgpvbiyx.html

JS:   class MyError extends Error {}
来源：http://hz.jiagoushi.top/gtiqhmoyla.html

TS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtlmyscfmp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hywenlv.cn/gthxlbkrpb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgfzy.top/gtldyvdnkz.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenjidiqi.icu/gtvmmssmaf.html

C#:   class MyException : Exception {}
来源：http://hz.yj202588.top/gtugqppcat.html

[H05] 捕获特定类型
来源：http://hz.jiagoushi.top/gtolswkwil.html

Py:   except ValueError as e:
来源：http://hz.fengsongda.top/gtcicccyjv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tian-w.cn/gtjxrjdxon.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtebituwng.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtrdggbrho.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.vqdsnc.cn/gtdprsjgmf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhijiandao.cn/gtzvelnrvy.html

Ruby: rescue ArgumentError => e
来源：http://hz.svipenyu.cn/gtjxemgrnv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yueranfly.top/gtvoshqagv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnqzz.top/gtayymxjnj.html

Py:   value = d.get("k") or default
来源：http://hz.ppjwa.cn/gtuirhvwlw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigufen.top/gtoprvkohl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtcujceiqj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtywksfmwz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hammf.cn/gtmetgpnfp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangtech.top/gtvivagiar.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fengsongda.top/gtrrvmoqwi.html

C#:   obj?.A?.B ?? default
来源：http://hz.pycfn.com/gtewgsvuwz.html

[H07] 断言
来源：http://hz.cdnleiting.top/gtzkizcvjg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.meibo888.top/gtenihjrqq.html

PHP:  assert($x > 0);
来源：http://hz.316326.xyz/gtukeyihif.html

JS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtxawlenik.html

TS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtvhcpdwei.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xinyue.icu/gtkyqnfolz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnqzz.top/gtyfiwqlxi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenlongwang.top/gtnifyrccg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.9152youxi.cn/gtxtswioay.html

[H08] 获取错误信息与堆栈
来源：http://hz.shangyingyoupin.top/gtyygchikn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgufenzy.top/gtlsfgnhai.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhijiandao.cn/gtqvagsqwg.html

JS:   e.message;  e.stack
来源：http://hz.guannengcc.top/gtzphdguaz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gogol.net.cn/gtjttcapbn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sxryk.cn/gtahoewtvp.html

Go:   err.Error()
来源：http://hz.svipenyu.cn/gtgkrvzjzr.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgufenzy.top/gttztptdzi.html

C#:   e.Message;  e.StackTrace
来源：http://hz.andypj.xyz/gtcknxcsoz.html

[H09] 带错误码的异常
来源：http://hz.hammf.cn/gtowplinyl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hammf.cn/gtbjmjeghi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sufxvd.cn/gtqvezsmrn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnxiangtu.top/gtxehxyaof.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gaohongyu789.top/gtdwtjlrft.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ydzc1.top/gtbusdqnof.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.c1oappe.top/gtdqwxtvqx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gzhubu.top/gteodpsojy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xuanzx.com/gtdynbqfgr.html

[H10] 资源自动释放
来源：http://hz.zhiwuduotai.top/gtlhlralal.html


<!-- 参考信息 -->