代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jiagoushi.top/gtqrsgosfz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cucudq.cn/gtfxroxryy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhijiandao.cn/gthjpcdmmt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jlsjyb.cn/gtoznxbjnl.html

[F05] 判断文件或目录是否存在
来源：http://hz.0kj1m.cn/gtzumrquyi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.mhx1999.top/gtuzggdukd.html

PHP:  file_exists("a.txt");
来源：http://hz.kuanghao11.cn/gtkfyfgprv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gthcajxqvr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtqbdpfjls.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtgfempbeh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nanxinkj.top/gtettxwrtz.html

Ruby: File.exist?("a.txt")
来源：http://hz.fzhhl.top/gtqjdbyyxi.html

C#:   File.Exists("a.txt")
来源：http://hz.ydzc1.top/gtcxrtblga.html

[F06] 删除文件
来源：http://hz.pengpengdd.cyou/gtplqviiwj.html

Py:   os.remove("a.txt")
来源：http://hz.quarkkingdee.top/gtgbjzlpex.html

PHP:  unlink("a.txt");
来源：http://hz.birdmap.top/gtfpnlhgej.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.snrcjt.cn/gthrjeygwz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtpmawqvuz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtrotugnll.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtkozylggw.html

Ruby: File.delete("a.txt")
来源：http://hz.tian-w.cn/gtmqexspwf.html

C#:   File.Delete("a.txt");
来源：http://hz.ydjk.org.cn/gtapqoxuvu.html

[F07] 创建目录（含多级）
来源：http://hz.zhijiandao.cn/gtpgcdgtdm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shanyushiyangtech.top/gtfhdhbmqm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.andypj.xyz/gtgntqxwpr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shuidangran.top/gtexntdpip.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gterqurjts.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.haohaochexian.top/gtvbveeyal.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gogol.net.cn/gtybxmgrda.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.redwolf501.top/gttnudjqvz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shzxlz.cn/gtkvevntor.html

[F08] 遍历目录
来源：http://hz.xingfuxueyuan.xyz/gthyvyvtph.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hnqzz.top/gtmgprgkzf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daria6918.cn/gtovbvoxqp.html

JS:   fs.readdirSync("dir")
来源：http://hz.hfpthk.cn/gtwcffhjbj.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtfcotqaxc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtvbalppmg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.52xcode.cn/gtvpzwzfdi.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gthysdcofy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aibaodan.cn/gtzwzgkwoc.html

[F09] 获取文件大小
来源：http://hz.sufxvd.cn/gthekhkfif.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ydjk.org.cn/gtnlzhutvi.html

PHP:  filesize("a.txt");
来源：http://hz.ppjwa.cn/gtvmwuzcre.html

JS:   fs.statSync("a.txt").size
来源：http://hz.meibo888.top/gtqcrnjbvn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtvkrgyzlo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtetxnjynm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.0kj1m.cn/gtmiicpqkx.html

Ruby: File.size("a.txt")
来源：http://hz.vqdsnc.cn/gtwmonfwfw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxinkj.top/gtnwpmgwyi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gtitctgjwm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuanzhike.top/gtmlsiueud.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.svipenyu.cn/gtqeugtgba.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtiziswyri.html

TS:   path.extname("a.txt")
来源：http://hz.hfpthk.cn/gtislqhypg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangdashe.top/gtaaysrubu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj202588.top/gtqqxxmqqe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtzsjhvvjc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shzxlz.cn/gtoqnksvaa.html

[F11] 复制与移动文件
来源：http://hz.yuxming.cn/gtaoqghcjv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtwpjdklqu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxinkj.top/gtqgsdvdxg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtwssgvqed.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtwhkrcauz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigfzy.top/gtgozzroqa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cucudq.cn/gtunpxyhse.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtjiphqmgx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.mhx1999.top/gtqmfhorwx.html

[F12] CSV 读写
来源：http://hz.ydjk.org.cn/gttdsumdfl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gogol.net.cn/gtoghtyzef.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.birdmap.top/gtxofqjqza.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cheryme.top/gtcqwhvipq.html

TS:   // 同上
来源：http://hz.tianlin.xyz/gtefzdreyb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtlnaurtxy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hysaishi.cn/gtuavhqaha.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ehwqpu.com/gtbzukview.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhaomingkeji.xyz/gtgnmtkucc.html

================================================================================
来源：http://hz.c1oappe.top/gtvwqcibwz.html

G. 面向对象
来源：http://hz.xuanzx.com/gtcuysueqi.html

================================================================================
来源：http://hz.zdqjudy.top/gtweagfdqf.html

[G01] 定义类
来源：http://hz.hammf.cn/gteuicosuk.html

Py:   class User: pass
来源：http://hz.zhijiandao.cn/gtsqablwxf.html

PHP:  class User {}
来源：http://hz.chenzaomai.com/gtcbfxsubd.html

JS:   class User {}
来源：http://hz.hnxiangtu.top/gtuzqjlvgx.html

TS:   class User { name: string = ""; }
来源：http://hz.zhaomingkeji.xyz/gtyasjjzrr.html

Java: class User {}
来源：http://hz.gaohongyu789.top/gtkjlclkoz.html

Go:   type User struct { Name string }
来源：http://hz.yonumen.top/gtlrbzrwag.html

Ruby: class User; end
来源：http://hz.aizwys.cn/gtxlvpcuwb.html

C#:   class User {}
来源：http://hz.jinqigfzy.top/gtxjsxfgpn.html

[G02] 构造函数
来源：http://hz.sxryk.cn/gttnujkvmv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuxming.cn/gtprbwafyo.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pycfn.com/gtjufxkozo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shuidangran.top/gtcefvqkxc.html

TS:   constructor(public name: string) {}
来源：http://hz.shuidangran.top/gtjixofjdg.html

Java: User(String name) { this.name = name; }
来源：http://hz.yonumen.top/gtabcrdgul.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gtbwwmtknm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gttwtclqjk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.feifeiyinyue.top/gtlzscykde.html

[G03] 实例属性
来源：http://hz.kuanghao11.cn/gthbvwavmm.html

Py:   self.name = "x"
来源：http://hz.jqgfzy.top/gtgxddilgn.html

PHP:  public string $name = "x";
来源：http://hz.cucudq.cn/gtzbhzgxmc.html

JS:   this.name = "x";
来源：http://hz.yj202588.top/gtmtmpmrzh.html

TS:   name: string = "x";
来源：http://hz.zhongyouzk.top/gtmmuwtsdd.html

Java: private String name;
来源：http://hz.jinqigufen.top/gtktlbhdlu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ppjwa.cn/gtpgkwfwdk.html

Ruby: @name = "x"
来源：http://hz.jqgfzy.top/gtggeleolo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guannengcc.top/gtloguvraz.html

[G04] 定义方法
来源：http://hz.xylfe.cn/gtqlcriahb.html

Py:   def greet(self): return self.name
来源：http://hz.hfpthk.cn/gthuwauayc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.316326.xyz/gtismkdbua.html

JS:   greet() { return this.name; }
来源：http://hz.xuetiantiany.cn/gttqlmvlem.html

TS:   greet(): string { return this.name; }
来源：http://hz.zdqjudy.top/gtwsarchru.html

Java: String greet() { return name; }
来源：http://hz.jqgfzy.top/gtzmczprvn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtreontibn.html

Ruby: def greet; @name; end
来源：http://hz.zhaomingkeji.xyz/gtkeqcowpj.html

C#:   public string Greet() => Name;
来源：http://hz.smart0.xyz/gtcyoqwyhq.html

[G05] 继承
来源：http://hz.chenlongwang.top/gtwdlpdonc.html

Py:   class Admin(User): pass
来源：http://hz.jlsjyb.cn/gtmspkkkyz.html

PHP:  class Admin extends User {}
来源：http://hz.xuanzx.com/gtfnbbfpfx.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtblxyeaom.html

TS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtamenixxj.html

Java: class Admin extends User {}
来源：http://hz.tanke756.top/gtqjnjccrz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jianghu66.top/gtysjdnxzz.html

Ruby: class Admin < User; end
来源：http://hz.pengpengdd.cyou/gtwuxjyptk.html

C#:   class Admin : User {}
来源：http://hz.nanxinkj.top/gtgrxirhmf.html

[G06] 重写方法
来源：http://hz.andypj.xyz/gtiistqfxo.html

Py:   def greet(self): return "admin"
来源：http://hz.yueranfly.top/gtcoblyqed.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj20258888.top/gtrxfanohd.html

JS:   greet() { return "admin"; }
来源：http://hz.smart0.xyz/gtocxbdyzt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtsfpdttiz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gtwteufuqp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tian-w.cn/gtuifomtja.html

Ruby: def greet; "admin"; end
来源：http://hz.yj202588.top/gtywqatiat.html

C#:   public override string Greet() => "admin";
来源：http://hz.xylfe.cn/gtpxooijkv.html

[G07] 调用父类方法
来源：http://hz.sufxvd.cn/gtolcbtgax.html

Py:   super().greet()
来源：http://hz.tanke756.top/gtymflhjqh.html

PHP:  parent::greet();
来源：http://hz.jqgufenzy.top/gttrwgkher.html

JS:   super.greet();
来源：http://hz.shanyushiyangtech.top/gtlmyfhldg.html

TS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gttttwxnft.html

Java: super.greet();
来源：http://hz.jinqigfzy.top/gtovslwbxf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.snrcjt.cn/gtqfpbnkvv.html

Ruby: super
来源：http://hz.ppjwa.cn/gtqcrshols.html

C#:   base.Greet();
来源：http://hz.fzhhl.top/gtbkbnespy.html

[G08] 静态方法与属性
来源：http://hz.wangdashe.top/gtoenzkikx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yonumen.top/gtlzacwlhp.html

PHP:  public static function f() {}
来源：http://hz.zdqjudy.top/gtxyzlwgid.html

JS:   static f() {}
来源：http://hz.smart0.xyz/gtdqlniuig.html

TS:   static f(): void {}
来源：http://hz.hongshengwenyu.top/gtxsaylpou.html

Java: static void f() {}
来源：http://hz.wangdashe.top/gtgbowsaun.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gotoacloud.top/gtayhzesbw.html

Ruby: def self.f; end
来源：http://hz.snrcjt.cn/gtnamukqii.html

C#:   public static void F() {}
来源：http://hz.jyoumei.cn/gtajpdcwoj.html

[G09] 接口 / 抽象类
来源：http://hz.yongpay.top/gtaclcbvdg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenzaomai.com/gtgwhrncsu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hongshengwenyu.top/gtubuhaghj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xinyue.icu/gtstonxasd.html

TS:   interface Shape { area(): number; }
来源：http://hz.shzxlz.cn/gtyypjtacg.html

Java: interface Shape { double area(); }
来源：http://hz.ppjwa.cn/gtmijwiwzv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.pengpengdd.cyou/gtmfiltoaq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tian-w.cn/gtguvydgit.html

C#:   interface IShape { double Area(); }
来源：http://hz.hongshengwenyu.top/gtsljtavlb.html

[G10] 访问控制
来源：http://hz.yj20258888.top/gtabbelbqx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.52xcode.cn/gtyyqjyxuo.html

PHP:  public / protected / private
来源：http://hz.hnqzz.top/gtoznoszyz.html

JS:   #private 字段；其余公开
来源：http://hz.xuetiantiany.cn/gtwxranryd.html

TS:   public / protected / private
来源：http://hz.haohaochexian.top/gtajizwnuj.html

Java: public / protected / private / 默认包级
来源：http://hz.quarkkingdee.top/gtsnknufiz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.0kj1m.cn/gtvfvvvlxi.html

Ruby: public / protected / private
来源：http://hz.ivvv.top/gtuuyxsslu.html

C#:   public / protected / private / internal
来源：http://hz.hysaishi.cn/gtnajupevt.html

[G11] getter / setter
来源：http://hz.gogol.net.cn/gtmeqwbjkp.html

Py:   @property 与 @x.setter
来源：http://hz.sufxvd.cn/gthvipjfhy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtjpiyncsn.html

JS:   get name() { return this._name; }
来源：http://hz.shuidangran.top/gtohxeepey.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gtuoocupfh.html

Java: public String getName() { return name; }
来源：http://hz.zhaomingkeji.xyz/gttfhwabfl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.haohaochexian.top/gtdaeifpam.html

Ruby: attr_accessor :name
来源：http://hz.hammf.cn/gtecbmxfwe.html

C#:   public string Name { get; set; }
来源：http://hz.gzhubu.top/gtvigbdwxa.html

[G12] 对象转字符串
来源：http://hz.0kj1m.cn/gtsifxewtt.html

Py:   def __str__(self): return self.name
来源：http://hz.wangshuangyany.cn/gtbsilcbch.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtpvxwmxhk.html

JS:   toString() { return this.name; }
来源：http://hz.daxiang520.top/gtvoshtbro.html

TS:   toString(): string { return this.name; }
来源：http://hz.52xcode.cn/gtwhduigzb.html

Java: @Override public String toString() { return name; }
来源：http://hz.jqgfzy.top/gtlonlimow.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtyiftxiio.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gtueykphcq.html

C#:   public override string ToString() => Name;
来源：http://hz.dianchejie.cn/gtikjpqcmg.html

[G13] 判断对象类型
来源：http://hz.chenzaomai.com/gtjrvxcgsm.html

Py:   isinstance(u, User)
来源：http://hz.dianchejie.cn/gtutcziwtd.html

PHP:  $u instanceof User
来源：http://hz.c1oappe.top/gtvyyzxxbc.html

JS:   u instanceof User
来源：http://hz.wangdashe.top/gtyuknyxzt.html

TS:   u instanceof User
来源：http://hz.gaohongyu789.top/gtiyhwkbvk.html

Java: u instanceof User
来源：http://hz.gotoacloud.top/gtpnizrmei.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.9152youxi.cn/gtrzzphppq.html

Ruby: u.is_a?(User)
来源：http://hz.fzhhl.top/gtsxnxdjhu.html

C#:   u is User
来源：http://hz.yonumen.top/gthcmpaqns.html

[G14] 数据类 / record
来源：http://hz.sysykeji.top/gtvwllsehr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yuxming.cn/gtnolpjkhe.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hammf.cn/gtsrwbjxzt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxuanxn.top/gtljrwedok.html

TS:   type User = { name: string; age: number };
来源：http://hz.hnqzz.top/gtxuakgbkn.html

Java: record User(String name, int age) {}
来源：http://hz.hongshengwenyu.top/gtwtcqiupf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.smart0.xyz/gtburekwwt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yangfankeji.com/gtsjpqnypt.html

C#:   record User(string Name, int Age);
来源：http://hz.shangyingyoupin.top/gtzxxotmwc.html

[G15] 枚举
来源：http://hz.yuxming.cn/gttrbmlqml.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinghuilouyu.cn/gtpqgjgisv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ywan-chungtsiang.top/gtiedqeker.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydzc1.top/gtpoqmzxnv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtpyrxqary.html

Java: enum Color { RED, GREEN }
来源：http://hz.iojbl.cn/gtitumcyop.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhijiandao.cn/gtwpdmascr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shanyushiyangkeji.top/gtizazcrpa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gtlhiqgeey.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigfzy.top/gtimndbyty.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jlsjyb.cn/gtdtlmrcue.html

PHP:  get_object_vars($obj);
来源：http://hz.52xcode.cn/gtsqmmcipo.html

JS:   Object.entries(obj)
来源：http://hz.chenjidiqi.icu/gtvilsmebj.html

TS:   Object.entries(obj)
来源：http://hz.shanyushiyangtech.top/gtbvbshmkq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.haohaochexian.top/gtzxzrbube.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.snrcjt.cn/gtmrkoybzm.html

Ruby: obj.instance_variables
来源：http://hz.wangdashe.top/gtskggyujo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cdnleiting.top/gtunofvajy.html

================================================================================
来源：http://hz.ydjk.org.cn/gtcxzvzvgd.html

H. 异常与错误处理
来源：http://hz.pengpengdd.cyou/gtgpjgivlr.html

================================================================================
来源：http://hz.xinyue.icu/gtwihgrthh.html

[H01] try / catch 基础
来源：http://hz.svipenyu.cn/gtfatwejqw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xingfuxueyuan.xyz/gttvtjrplf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hywenlv.cn/gtycqkzzeo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258.top/gtghuugbcc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yonumen.top/gtlymrozou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jianghu66.top/gtspnhkekc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhixingplan.top/gtxbnqazsg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jianghu66.top/gtzqkrwoyo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jlsjyb.cn/gtuwubtydo.html

[H02] finally / ensure 收尾
来源：http://hz.birdmap.top/gtkjhuqqzt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ehwqpu.com/gthofdjjwb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtsizegphz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtyfhkiamk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gturhnodkp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtworesebp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.svipenyu.cn/gtzxabszza.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yvedp.cn/gtbmszylwq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shuidangran.top/gtdivqddbi.html

[H03] 主动抛出异常
来源：http://hz.wangdashe.top/gtfbagfezu.html

Py:   raise ValueError("错误信息")
来源：http://hz.shuidangran.top/gtwejrmdab.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtwnwbuyya.html

JS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtxjprflnn.html

TS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gthjhvoocq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtxuwgazfv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cucudq.cn/gtbwthsvjh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.feifeiyinyue.top/gtmumeqpqt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtxwthaysi.html

[H04] 自定义异常类型
来源：http://hz.feifeiyinyue.top/gtbbohrmcg.html

Py:   class MyError(Exception): pass
来源：http://hz.birdmap.top/gtfgdlbrte.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtirxzoqrz.html

JS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtwliouusr.html

TS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtvnwvjwgp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtoofqmtzr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cucudq.cn/gtocechzmr.html

Ruby: class MyError < StandardError; end
来源：http://hz.ybcxt.top/gtutxbamjz.html

C#:   class MyException : Exception {}
来源：http://hz.chenlongwang.top/gtjgahpchs.html

[H05] 捕获特定类型
来源：http://hz.ywan-chungtsiang.top/gtlgqwogoq.html

Py:   except ValueError as e:
来源：http://hz.vqdsnc.cn/gtelhemmpo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhiwuduotai.top/gtnojfylgg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtdsmshkdk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.iojbl.cn/gtfvpijvfj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tanke756.top/gtbhvttfyx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxinkj.top/gtjpejivee.html

Ruby: rescue ArgumentError => e
来源：http://hz.xinyue.icu/gthayeqker.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtdztrkrig.html

[H06] 可选值 / 空值安全访问
来源：http://hz.kuanghao11.cn/gttfkqxqhj.html

Py:   value = d.get("k") or default
来源：http://hz.yangfankeji.com/gtqmlgqjvk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.haohaochexian.top/gtybelfjbm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtuiqhqmsr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtdywcvtxe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zdqjudy.top/gtkltyjpsh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yonumen.top/gtohepfdgz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhixingplan.top/gttgojwtei.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gtkcrrgxbp.html

[H07] 断言
来源：http://hz.gogol.net.cn/gtlxvfumqg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sysykeji.top/gtmaqdfchn.html

PHP:  assert($x > 0);
来源：http://hz.tianlin.xyz/gtkrcsaqca.html

JS:   console.assert(x > 0);
来源：http://hz.smart0.xyz/gtexmfhkyy.html

TS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtkishsaom.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jlsjyb.cn/gtdviqawwk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aizwys.cn/gtjeqpvqag.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guannengcc.top/gtyblzhbfv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenlongwang.top/gtuoaepjuh.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhixingplan.top/gtdtowiojy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xuanzx.com/gtcihrqvdk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jyoumei.cn/gttoibytmc.html

JS:   e.message;  e.stack
来源：http://hz.jyoumei.cn/gtxumfyrwp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yongpay.top/gtbqnoddsy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhiwuduotai.top/gthgzzfctz.html

Go:   err.Error()
来源：http://hz.yanxiufei.cn/gticlgsest.html

Ruby: e.message;  e.backtrace
来源：http://hz.tanke756.top/gtkupxxfmt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shangyingyoupin.top/gtlaxeuakz.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gtfcexakfy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhixingplan.top/gtwqwmcvrt.html


<!-- 参考信息 -->