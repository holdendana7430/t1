代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://hz.cqqwz.cn/gtpujaeuqn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ybcxt.top/gtgzgkzxge.html

PHP:  file_exists("a.txt");
来源：http://hz.wangdashe.top/gtfeanqzbw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gtpyrwqlat.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ehwqpu.com/gttxkzskum.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtsyrzesgo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xylfe.cn/gtgzvkkkdj.html

Ruby: File.exist?("a.txt")
来源：http://hz.cucudq.cn/gtoxdoizqu.html

C#:   File.Exists("a.txt")
来源：http://hz.vqdsnc.cn/gthizlskwn.html

[F06] 删除文件
来源：http://hz.ywan-chungtsiang.top/gtlzznneox.html

Py:   os.remove("a.txt")
来源：http://hz.vqdsnc.cn/gtoazlyozl.html

PHP:  unlink("a.txt");
来源：http://hz.kuanghao11.cn/gtfvwxqnpl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ybcxt.top/gtiacyzeie.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtdfxkidsh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtgjhoxpjb.html

Go:   os.Remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtzdbhnyle.html

Ruby: File.delete("a.txt")
来源：http://hz.316326.xyz/gtvdlfseom.html

C#:   File.Delete("a.txt");
来源：http://hz.zycfv.cn/gthwldkbah.html

[F07] 创建目录（含多级）
来源：http://hz.yuxming.cn/gtscnohdcp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.52xcode.cn/gtanlxfnzh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.wangshuangyany.cn/gtgogpbjas.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.0kj1m.cn/gtyhqlixrg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.havefunace.top/gtxdxijulv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.kuanghao11.cn/gtwqzikanu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuanzhike.top/gtqzidcukd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhoulong.xyz/gtzqzmxgph.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhongyouzk.top/gtguroxnuq.html

[F08] 遍历目录
来源：http://hz.xingfuxueyuan.xyz/gtpxykztdm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nanxinkj.top/gtwvgmolef.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenzaomai.com/gtwwsdepcv.html

JS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtluhovxtv.html

TS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtpistjkoh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258.top/gthlhtmqdc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xinyue.icu/gtnckgwhok.html

Ruby: Dir.children("dir")
来源：http://hz.snrcjt.cn/gtzveawiia.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sysykeji.top/gtanspaspy.html

[F09] 获取文件大小
来源：http://hz.gogol.net.cn/gttqbbbhoa.html

Py:   os.path.getsize("a.txt")
来源：http://hz.andypj.xyz/gtpvhxvwms.html

PHP:  filesize("a.txt");
来源：http://hz.haohaochexian.top/gtvrzopmhh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jianghu66.top/gtjmbnqnrx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhijiandao.cn/gtmopspdbc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtbdmttigc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.kuanghao11.cn/gtuyczhfsi.html

Ruby: File.size("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtncybfmft.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hammf.cn/gtfcbldpip.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ivvv.top/gtvtcuyevl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtidzioejd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.quarkkingdee.top/gtyaolqlqd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtwlwknpqk.html

TS:   path.extname("a.txt")
来源：http://hz.aizwys.cn/gtkavmtuzh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinghuilouyu.cn/gtgbszbkst.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.316326.xyz/gtbtfhlinf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtlrmtjtje.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jlsjyb.cn/gteginxatt.html

[F11] 复制与移动文件
来源：http://hz.andypj.xyz/gtbizeasnr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtoflpupzh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ehwqpu.com/gtxizqznci.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtkvrssrma.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtpptcrobd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinyuanbaomall.cn/gtjkunvwuz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj202588.top/gtkezjpjge.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtdexexxdn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jlsjyb.cn/gtoomzgnvn.html

[F12] CSV 读写
来源：http://hz.kuanghao11.cn/gtzqsvxupr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xingfuxueyuan.xyz/gtqqbkbxhf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xinyue.icu/gtyzjjgiph.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gaohongyu789.top/gtlqqkhwqi.html

TS:   // 同上
来源：http://hz.chenzaomai.com/gtostuulsk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cheryme.top/gttgvimqwt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydjk.org.cn/gtmxihwndn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cashguo.top/gtdljsnlkb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.kuanghao11.cn/gtcsdphloa.html

================================================================================
来源：http://hz.birdmap.top/gtxwfqudqg.html

G. 面向对象
来源：http://hz.tian-w.cn/gtdbdazoui.html

================================================================================
来源：http://hz.tian-w.cn/gtklkxiehs.html

[G01] 定义类
来源：http://hz.gotoacloud.top/gtmdtxtggk.html

Py:   class User: pass
来源：http://hz.yj20258888.top/gtjbdqnqzo.html

PHP:  class User {}
来源：http://hz.jlsjyb.cn/gtlusxtfqn.html

JS:   class User {}
来源：http://hz.tanke756.top/gtxmnjzjig.html

TS:   class User { name: string = ""; }
来源：http://hz.wangdashe.top/gtksxmvvpp.html

Java: class User {}
来源：http://hz.cucudq.cn/gtrfgzjmmu.html

Go:   type User struct { Name string }
来源：http://hz.ybcxt.top/gtdapwkdhv.html

Ruby: class User; end
来源：http://hz.chenzaomai.com/gtrckoabeh.html

C#:   class User {}
来源：http://hz.yongpay.top/gtsccxfvsj.html

[G02] 构造函数
来源：http://hz.jqgfzy.top/gtxijbyvfw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.feifeiyinyue.top/gtgzndkarn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sxryk.cn/gtsdgbqdru.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ivvv.top/gttflckyfk.html

TS:   constructor(public name: string) {}
来源：http://hz.sweek.top/gterrovvgp.html

Java: User(String name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtcrxrwdid.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuetiantiany.cn/gttuqphuek.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhiwuduotai.top/gtvbydthod.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hysaishi.cn/gtvooapfnw.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gtirzjjumh.html

Py:   self.name = "x"
来源：http://hz.jinqigufen.top/gthbtmnfov.html

PHP:  public string $name = "x";
来源：http://hz.jiagoushi.top/gthijgrqep.html

JS:   this.name = "x";
来源：http://hz.daria6918.cn/gtibtxjspj.html

TS:   name: string = "x";
来源：http://hz.cashguo.top/gtvdqjulbu.html

Java: private String name;
来源：http://hz.guowangkeji.top/gtsrkgyvbv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sxryk.cn/gtlipgzejq.html

Ruby: @name = "x"
来源：http://hz.shuidangran.top/gteoodleow.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.mhx1999.top/gtaalnxbvu.html

[G04] 定义方法
来源：http://hz.cdnleiting.top/gtjxqyitrd.html

Py:   def greet(self): return self.name
来源：http://hz.yueranfly.top/gtbviddcrr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtwvtjxpyx.html

JS:   greet() { return this.name; }
来源：http://hz.jianghu66.top/gttvecgjyv.html

TS:   greet(): string { return this.name; }
来源：http://hz.feifeiyinyue.top/gtqvsfjyog.html

Java: String greet() { return name; }
来源：http://hz.xuetiantiany.cn/gtktjfnuwe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guowangkeji.top/gtlnljjubn.html

Ruby: def greet; @name; end
来源：http://hz.xinyue.icu/gtjiwezrhn.html

C#:   public string Greet() => Name;
来源：http://hz.gotoacloud.top/gtforuxupf.html

[G05] 继承
来源：http://hz.xylfe.cn/gtiobdcuxq.html

Py:   class Admin(User): pass
来源：http://hz.hysaishi.cn/gtmjwthrgn.html

PHP:  class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtxskdtnfd.html

JS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gtybatydgn.html

TS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtiwvnwzfw.html

Java: class Admin extends User {}
来源：http://hz.daria6918.cn/gtbpidhosb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.vqdsnc.cn/gteuwkulao.html

Ruby: class Admin < User; end
来源：http://hz.hnxiangtu.top/gtaecvzmab.html

C#:   class Admin : User {}
来源：http://hz.jqgufenzy.top/gtbbucztjd.html

[G06] 重写方法
来源：http://hz.cashguo.top/gtotserjsy.html

Py:   def greet(self): return "admin"
来源：http://hz.hnxiangtu.top/gtsjxeredw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtchkkwqme.html

JS:   greet() { return "admin"; }
来源：http://hz.cqqwz.cn/gthtictbsj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ehwqpu.com/gtytaqnbkg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cdnleiting.top/gtkpjtjlaq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgufenzy.top/gtvitswcmk.html

Ruby: def greet; "admin"; end
来源：http://hz.chenlongwang.top/gtrwyhgpal.html

C#:   public override string Greet() => "admin";
来源：http://hz.xingfuxueyuan.xyz/gtvrnfdohf.html

[G07] 调用父类方法
来源：http://hz.ydzc1.top/gtpgrpxgnl.html

Py:   super().greet()
来源：http://hz.zhaomingkeji.xyz/gtsffbapgo.html

PHP:  parent::greet();
来源：http://hz.hysaishi.cn/gtgvjzdprw.html

JS:   super.greet();
来源：http://hz.cheryme.top/gtqmeytdks.html

TS:   super.greet();
来源：http://hz.jinqigufen.top/gtwpuakdaz.html

Java: super.greet();
来源：http://hz.chenjidiqi.icu/gtwfkjngct.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgfzy.top/gtszhlwfms.html

Ruby: super
来源：http://hz.tanke756.top/gtxvcuisjq.html

C#:   base.Greet();
来源：http://hz.zhengqikj.top/gtsgyjmifa.html

[G08] 静态方法与属性
来源：http://hz.hnxiangtu.top/gtvukwwylk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhixingplan.top/gtzpylklcf.html

PHP:  public static function f() {}
来源：http://hz.gotoacloud.top/gttcsxaoqt.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gtnnaamtqk.html

TS:   static f(): void {}
来源：http://hz.aizwys.cn/gtgmjadbvz.html

Java: static void f() {}
来源：http://hz.kuanghao11.cn/gtocfzsbfl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.haohaochexian.top/gttevxlesn.html

Ruby: def self.f; end
来源：http://hz.ywan-chungtsiang.top/gtyszfpcsw.html

C#:   public static void F() {}
来源：http://hz.shuidangran.top/gtdzndjofg.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangtech.top/gtkdtolfwp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.quarkkingdee.top/gtljkuwnvn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yonumen.top/gthfnruqmn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yongpay.top/gttqxkgnqp.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenjidiqi.icu/gtzoiauhxm.html

Java: interface Shape { double area(); }
来源：http://hz.jinghuilouyu.cn/gtmjqwrfae.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258.top/gtfbnqflun.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigfzy.top/gtthjcvmyv.html

C#:   interface IShape { double Area(); }
来源：http://hz.0kj1m.cn/gtztfeylyj.html

[G10] 访问控制
来源：http://hz.shzxlz.cn/gtxseyescd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.0kj1m.cn/gtvuonnzwc.html

PHP:  public / protected / private
来源：http://hz.gogol.net.cn/gtkflbgqyw.html

JS:   #private 字段；其余公开
来源：http://hz.jiagoushi.top/gtwdavzawp.html

TS:   public / protected / private
来源：http://hz.aizwys.cn/gtivnhuqhq.html

Java: public / protected / private / 默认包级
来源：http://hz.yj202588.top/gtwejskgsk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hysaishi.cn/gtkhhkxbhv.html

Ruby: public / protected / private
来源：http://hz.hysaishi.cn/gtkejwrpqf.html

C#:   public / protected / private / internal
来源：http://hz.jinqigufen.top/gtzcztstby.html

[G11] getter / setter
来源：http://hz.xylfe.cn/gtbjlrapdb.html

Py:   @property 与 @x.setter
来源：http://hz.gzhubu.top/gtkshlolvm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtoeoczhjy.html

JS:   get name() { return this._name; }
来源：http://hz.zhoulong.xyz/gtlhcfovsj.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangkeji.top/gtgempjpjo.html

Java: public String getName() { return name; }
来源：http://hz.tanke756.top/gtgurrwcdh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtwwczqqpy.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtbiivqcim.html

C#:   public string Name { get; set; }
来源：http://hz.jianghu66.top/gtnqidviwp.html

[G12] 对象转字符串
来源：http://hz.sweek.top/gtwedjgydm.html

Py:   def __str__(self): return self.name
来源：http://hz.shangyingyoupin.top/gtovzufcpk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtmjdgfozi.html

JS:   toString() { return this.name; }
来源：http://hz.tian-w.cn/gtzvdgdwnx.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhijiandao.cn/gtjsnvhzvv.html

Java: @Override public String toString() { return name; }
来源：http://hz.sysykeji.top/gtmkzmutaj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sxryk.cn/gtjpgidpko.html

Ruby: def to_s; @name; end
来源：http://hz.quarkkingdee.top/gtajfcsqus.html

C#:   public override string ToString() => Name;
来源：http://hz.feifeiyinyue.top/gtmpkqqfmq.html

[G13] 判断对象类型
来源：http://hz.zhiwuduotai.top/gtgtmtffsd.html

Py:   isinstance(u, User)
来源：http://hz.cashguo.top/gtvyogchxf.html

PHP:  $u instanceof User
来源：http://hz.zycfv.cn/gtergvsyjc.html

JS:   u instanceof User
来源：http://hz.zhijiandao.cn/gtwqiinvhx.html

TS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtblwngnkr.html

Java: u instanceof User
来源：http://hz.316326.xyz/gtfndwwske.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenzaomai.com/gtheidsuay.html

Ruby: u.is_a?(User)
来源：http://hz.smart0.xyz/gtbvlqrkkf.html

C#:   u is User
来源：http://hz.zhoulong.xyz/gtyrnyxiqi.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gtfkosdkjy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.guowangkeji.top/gtqnxcnzba.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.iojbl.cn/gtlvlhcyfy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ybcxt.top/gtntrjocda.html

TS:   type User = { name: string; age: number };
来源：http://hz.ppjwa.cn/gtxmejatvm.html

Java: record User(String name, int age) {}
来源：http://hz.jqgfzy.top/gtkegbuwmb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhaomingkeji.xyz/gtmstqmhkn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jiagoushi.top/gtpoeyyucw.html

C#:   record User(string Name, int Age);
来源：http://hz.dianchejie.cn/gtzqxxauxs.html

[G15] 枚举
来源：http://hz.cqqwz.cn/gtsmqmwkpm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tanke756.top/gtainexxft.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sweek.top/gtncgwwaqu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhixingplan.top/gtgyjimpmf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hywenlv.cn/gttnudtqqm.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenjidiqi.icu/gtzhdurnes.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhongyouzk.top/gtcnnqlkql.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sxryk.cn/gtpguxhubn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aibaodan.cn/gtpylfwnxr.html

[G16] 对象转数组 / 字典
来源：http://hz.xziqi.cn/gtdkqaxqdr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ivvv.top/gtxtponujx.html

PHP:  get_object_vars($obj);
来源：http://hz.guannengcc.top/gtqhswyugc.html

JS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtbxbnjdar.html

TS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gthxpzerse.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenzaomai.com/gtnbhxoasw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yueranfly.top/gtffyymojm.html

Ruby: obj.instance_variables
来源：http://hz.smart0.xyz/gtlhpexatm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zycfv.cn/gtdzrqzjbt.html

================================================================================
来源：http://hz.zhixingplan.top/gtthkforui.html

H. 异常与错误处理
来源：http://hz.9152youxi.cn/gtbljqinyv.html

================================================================================
来源：http://hz.gaohongyu789.top/gtwmllvdec.html

[H01] try / catch 基础
来源：http://hz.yj20258.top/gthjcsfkfu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hammf.cn/gtwytsmdcl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtxczgpfat.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daria6918.cn/gtopfdsibu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtzkijexep.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxinkj.top/gtxjnzzixf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhengqikj.top/gtuqzrkqvy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtsoyrdbmb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.mhx1999.top/gttltshvjz.html

[H02] finally / ensure 收尾
来源：http://hz.hongshengwenyu.top/gtiqyjikzd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jlsjyb.cn/gtqxvcffhq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtbqotksqy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtwllxllew.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtjieqonoo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtkpxrqydq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.kuanghao11.cn/gtnzxqxsnt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shzxlz.cn/gtfhzuhjrn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigfzy.top/gtrlftqxbi.html

[H03] 主动抛出异常
来源：http://hz.zdqjudy.top/gthyknsvgf.html

Py:   raise ValueError("错误信息")
来源：http://hz.ybcxt.top/gtxavpqgpd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtvsdkpoke.html

JS:   throw new Error("错误信息");
来源：http://hz.bjfxy.top/gtzxnftnlh.html

TS:   throw new Error("错误信息");
来源：http://hz.smart0.xyz/gtpqanaffx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtdkrpxsxv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hfpthk.cn/gtozfxhiuc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daxiang520.top/gtrpvfdtyd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtquhxkefe.html

[H04] 自定义异常类型
来源：http://hz.meibo888.top/gtwaceumij.html

Py:   class MyError(Exception): pass
来源：http://hz.jinyuanbaomall.cn/gtxewzwosu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gtibdxvkqg.html

JS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtrccjnltw.html

TS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gtldvvoyea.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gtxmtlvoox.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.haohaochexian.top/gtgsyarcuv.html

Ruby: class MyError < StandardError; end
来源：http://hz.quarkkingdee.top/gtkqpphovc.html

C#:   class MyException : Exception {}
来源：http://hz.yuxming.cn/gtnmhinnqz.html

[H05] 捕获特定类型
来源：http://hz.chenjidiqi.icu/gtatcppohm.html

Py:   except ValueError as e:
来源：http://hz.dashuyun.cn/gtcwlklgfi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yongpay.top/gtcmobvqzy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtvtipmnxl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtvnvgnzve.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenjidiqi.icu/gtuicrumfn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.52xcode.cn/gtmzyvbxdf.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydzc1.top/gtrnbywilh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hammf.cn/gtrnytyyqp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cqqwz.cn/gttnetrokh.html

Py:   value = d.get("k") or default
来源：http://hz.fzhhl.top/gtvxdfuzlq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.birdmap.top/gtvpwkcavu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtncopkbkh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtumshdrff.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yueranfly.top/gtvclycics.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guowangkeji.top/gtflisdbkd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zycfv.cn/gthwrmahtt.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gtahwpyslp.html

[H07] 断言
来源：http://hz.cqqwz.cn/gtfuywjkpf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hammf.cn/gtkqukarhs.html

PHP:  assert($x > 0);
来源：http://hz.guannengcc.top/gtwdftfqcs.html

JS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtgiitqtsg.html

TS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtwkthknsu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yonumen.top/gttrparaca.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yangfankeji.com/gtuiismuux.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.andypj.xyz/gteqemxdxt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nwbrower.top/gtkwxawqul.html

[H08] 获取错误信息与堆栈
来源：http://hz.hywenlv.cn/gtiliqscxo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtopzejzyv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gogol.net.cn/gttxbeaylh.html

JS:   e.message;  e.stack
来源：http://hz.zhongyouzk.top/gtzamnjlsp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigfzy.top/gtwubqdqmi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hongshengwenyu.top/gtggoadtik.html

Go:   err.Error()
来源：http://hz.jlsjyb.cn/gtbfocovqw.html

Ruby: e.message;  e.backtrace
来源：http://hz.guowangkeji.top/gtkuibuona.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daxiang520.top/gtjohosasu.html

[H09] 带错误码的异常
来源：http://hz.xinyue.icu/gtzgpsuoky.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtmhivtpel.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gtqjiqzeqi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fengsongda.top/gthdmifjnr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yangfankeji.com/gtqydmdngl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sufxvd.cn/gtqtpqjetg.html


<!-- 参考信息 -->