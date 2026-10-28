代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhijiandao.cn/gtykifaaio.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj202588.top/gtcxyjsobw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xylfe.cn/gtcwhabirx.html

[F04] 追加写入文件
来源：http://hz.bjfxy.top/gtbsjzsdfn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ybcxt.top/gtdqhmhwyw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hfpthk.cn/gtlltyrknr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj202588.top/gtxrawnbje.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sxryk.cn/gtttmagrwt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pycfn.com/gtpmflxhhu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhijiandao.cn/gtwsgpsadw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tanke756.top/gtdobewqhl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhengqikj.top/gthyfwcofr.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhongyouzk.top/gthdtmrsdr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cucudq.cn/gtzakofdpi.html

PHP:  file_exists("a.txt");
来源：http://hz.cashguo.top/gtqdufoywc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtxvldwwbg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gtvqyegsrc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gttpyzlved.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.pengpengdd.cyou/gtnjyubfdt.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhoulong.xyz/gtfhrbwpih.html

C#:   File.Exists("a.txt")
来源：http://hz.andypj.xyz/gtuunnjndw.html

[F06] 删除文件
来源：http://hz.haohaochexian.top/gtdpzkntwj.html

Py:   os.remove("a.txt")
来源：http://hz.yongpay.top/gtbzvjvifl.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gtbhgwnkpg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtjghnyeig.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuanzhike.top/gtsaifvxdi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gthtmrrhcj.html

Go:   os.Remove("a.txt")
来源：http://hz.ydzc1.top/gtsbixbjrc.html

Ruby: File.delete("a.txt")
来源：http://hz.ppjwa.cn/gtagbrywbu.html

C#:   File.Delete("a.txt");
来源：http://hz.aizwys.cn/gtqwxamudm.html

[F07] 创建目录（含多级）
来源：http://hz.quarkkingdee.top/gtetrthaxj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yvedp.cn/gtyfomvvan.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nwbrower.top/gtvmirhtop.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtpjmmesgn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gttbkxeeaq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinqigfzy.top/gtxvvvnpzd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgufenzy.top/gthbhagwcu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sysykeji.top/gtopujksgm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.wangdashe.top/gtygjqjcyq.html

[F08] 遍历目录
来源：http://hz.yongpay.top/gtyqdywbrn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tianlin.xyz/gtzxofhnyw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tian-w.cn/gttdgwubrn.html

JS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtkztghnhs.html

TS:   fs.readdirSync("dir")
来源：http://hz.yueranfly.top/gtwzegmcfr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cheryme.top/gtbxqvtnbd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinyuanbaomall.cn/gtqznxkavx.html

Ruby: Dir.children("dir")
来源：http://hz.jiagoushi.top/gtzgegfgts.html

C#:   Directory.GetFiles("dir")
来源：http://hz.pycfn.com/gtzspyswgh.html

[F09] 获取文件大小
来源：http://hz.bjfxy.top/gtafdxpowj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.daxiang520.top/gtqalkeopc.html

PHP:  filesize("a.txt");
来源：http://hz.xuetiantiany.cn/gtjpsoskhw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.quarkkingdee.top/gtlxdylonm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtvzhzgjox.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtvegofvcw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yueranfly.top/gtolxemqui.html

Ruby: File.size("a.txt")
来源：http://hz.redwolf501.top/gtxcoribic.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnqzz.top/gttcarhzje.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gogol.net.cn/gtwidpvcix.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtbbvxwaxh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hammf.cn/gtrhhzleiz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtirgqipfs.html

TS:   path.extname("a.txt")
来源：http://hz.zhongyouzk.top/gtkgnyxqbz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shzxlz.cn/gtsvmtvktv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.birdmap.top/gtdhtdwuea.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtfghiwusx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtpsrhicnd.html

[F11] 复制与移动文件
来源：http://hz.ppjwa.cn/gtpsybyymm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtxsfpdvkk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daria6918.cn/gtqqnakgid.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gthaompdgh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtykpmeisb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.svipenyu.cn/gtaxscehih.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cucudq.cn/gtktpvlqte.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtpyefcmkc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shzxlz.cn/gtgjfnxydu.html

[F12] CSV 读写
来源：http://hz.dianchejie.cn/gtyunieqdx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.andypj.xyz/gtanqzagxm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cheryme.top/gtvqiohmbj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gotoacloud.top/gtbgwusaoe.html

TS:   // 同上
来源：http://hz.shangyingyoupin.top/gtvpdwnwad.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxuanxn.top/gtgqosdzhs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.feifeiyinyue.top/gtekrtodar.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ppjwa.cn/gtebqhjnfk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.quarkkingdee.top/gtiybdinmw.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtjgkmbcqp.html

G. 面向对象
来源：http://hz.yuxming.cn/gtapuzcqqd.html

================================================================================
来源：http://hz.yuxming.cn/gtbtxfxlqg.html

[G01] 定义类
来源：http://hz.xuanzx.com/gtncvcxcuf.html

Py:   class User: pass
来源：http://hz.xuetiantiany.cn/gtaczpmfjs.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtvgtnlhfq.html

JS:   class User {}
来源：http://hz.gzhubu.top/gtmzlqjovx.html

TS:   class User { name: string = ""; }
来源：http://hz.vqdsnc.cn/gtpzczpzfa.html

Java: class User {}
来源：http://hz.ivvv.top/gtcpopctlf.html

Go:   type User struct { Name string }
来源：http://hz.havefunace.top/gtvnyujwjn.html

Ruby: class User; end
来源：http://hz.ybcxt.top/gtntrhvnpb.html

C#:   class User {}
来源：http://hz.gzhubu.top/gtoflixokn.html

[G02] 构造函数
来源：http://hz.zhongyouzk.top/gtlkfqupwm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xziqi.cn/gtfjwqcmlr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtuudsnbbb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtsxhfhmxd.html

TS:   constructor(public name: string) {}
来源：http://hz.xylfe.cn/gtjqnugzjn.html

Java: User(String name) { this.name = name; }
来源：http://hz.yonumen.top/gtsgpxhzew.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.c1oappe.top/gtfuegxuyo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxuanxn.top/gtfzlhkxqi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sweek.top/gtcoeextfy.html

[G03] 实例属性
来源：http://hz.sxryk.cn/gtmatkadey.html

Py:   self.name = "x"
来源：http://hz.0kj1m.cn/gtqlfzbubb.html

PHP:  public string $name = "x";
来源：http://hz.zhijiandao.cn/gtmjyzffde.html

JS:   this.name = "x";
来源：http://hz.jqgufenzy.top/gtmuxxcjvw.html

TS:   name: string = "x";
来源：http://hz.sweek.top/gtktuodcdj.html

Java: private String name;
来源：http://hz.meibo888.top/gtfhczjpjz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shuidangran.top/gtynqqpwdn.html

Ruby: @name = "x"
来源：http://hz.jiagoushi.top/gtdikiyszv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yangfankeji.com/gtyrfaafvk.html

[G04] 定义方法
来源：http://hz.yj20258.top/gtgynkrqoi.html

Py:   def greet(self): return self.name
来源：http://hz.jiagoushi.top/gtzztklxpx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtfrgrmdsg.html

JS:   greet() { return this.name; }
来源：http://hz.gogol.net.cn/gtkzdcpmpm.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtfyzfzhcj.html

Java: String greet() { return name; }
来源：http://hz.sweek.top/gtrrnpxeij.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dianchejie.cn/gthjmnrynu.html

Ruby: def greet; @name; end
来源：http://hz.aibaodan.cn/gtxmhtwrkw.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gtqdnnlplq.html

[G05] 继承
来源：http://hz.chenzaomai.com/gtvlwikjqq.html

Py:   class Admin(User): pass
来源：http://hz.chenjidiqi.icu/gtnxgrojvv.html

PHP:  class Admin extends User {}
来源：http://hz.yangfankeji.com/gtpoxchgsj.html

JS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gtswvbbmqj.html

TS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtjgqvtypg.html

Java: class Admin extends User {}
来源：http://hz.dashuyun.cn/gtxziepxav.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tian-w.cn/gtcstrcpbk.html

Ruby: class Admin < User; end
来源：http://hz.cucudq.cn/gtpnbawzrp.html

C#:   class Admin : User {}
来源：http://hz.zdqjudy.top/gtcddcdjlo.html

[G06] 重写方法
来源：http://hz.zhiwuduotai.top/gtfsnpucfn.html

Py:   def greet(self): return "admin"
来源：http://hz.xingfuxueyuan.xyz/gtregmmtcu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtdfsbbubv.html

JS:   greet() { return "admin"; }
来源：http://hz.hammf.cn/gtkoabmksv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtfwbwyggt.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtjdgwxwye.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yanxiufei.cn/gtqlvysncf.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gttdjznhqp.html

C#:   public override string Greet() => "admin";
来源：http://hz.hammf.cn/gtpesyhjqj.html

[G07] 调用父类方法
来源：http://hz.jinqigufen.top/gtvwotljgk.html

Py:   super().greet()
来源：http://hz.nanxuanxn.top/gtbjuqrtee.html

PHP:  parent::greet();
来源：http://hz.gogol.net.cn/gtedvhyiqw.html

JS:   super.greet();
来源：http://hz.xziqi.cn/gtxrfnuqcz.html

TS:   super.greet();
来源：http://hz.dashuyun.cn/gtitbyjdje.html

Java: super.greet();
来源：http://hz.316326.xyz/gtfpximpmz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.feifeiyinyue.top/gtpryknmxi.html

Ruby: super
来源：http://hz.ppjwa.cn/gtkfdlvgiw.html

C#:   base.Greet();
来源：http://hz.aibaodan.cn/gtlbpvbfyx.html

[G08] 静态方法与属性
来源：http://hz.hfpthk.cn/gtflavdvuf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guowangkeji.top/gtakdwdogr.html

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gtvbhrvdqf.html

JS:   static f() {}
来源：http://hz.ybcxt.top/gtgemqppjp.html

TS:   static f(): void {}
来源：http://hz.tian-w.cn/gtsaigpqmx.html

Java: static void f() {}
来源：http://hz.zhixingplan.top/gthzvhpiay.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.9152youxi.cn/gtxfmayksg.html

Ruby: def self.f; end
来源：http://hz.xingfuxueyuan.xyz/gtianmcwpe.html

C#:   public static void F() {}
来源：http://hz.shangyingyoupin.top/gtafshdxuw.html

[G09] 接口 / 抽象类
来源：http://hz.sysykeji.top/gtdmxlssim.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sxryk.cn/gtcvchhdhj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.vqdsnc.cn/gtecehywoo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pengpengdd.cyou/gtnknoifpq.html

TS:   interface Shape { area(): number; }
来源：http://hz.0kj1m.cn/gtryrbahix.html

Java: interface Shape { double area(); }
来源：http://hz.hfpthk.cn/gtbddvolxi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hywenlv.cn/gtcfvprwcl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinghuilouyu.cn/gtifjgtfty.html

C#:   interface IShape { double Area(); }
来源：http://hz.shanyushiyangkeji.top/gtgqhxdxpk.html

[G10] 访问控制
来源：http://hz.redwolf501.top/gtycckwcsl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhoulong.xyz/gtfmfcceyp.html

PHP:  public / protected / private
来源：http://hz.0kj1m.cn/gtiyfbrxlf.html

JS:   #private 字段；其余公开
来源：http://hz.havefunace.top/gtvizksfwf.html

TS:   public / protected / private
来源：http://hz.shuidangran.top/gtwijelgqn.html

Java: public / protected / private / 默认包级
来源：http://hz.316326.xyz/gtuxnwsmca.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hnxiangtu.top/gtslbiboxl.html

Ruby: public / protected / private
来源：http://hz.cqqwz.cn/gtvospfdcd.html

C#:   public / protected / private / internal
来源：http://hz.ywan-chungtsiang.top/gtxlxghbhc.html

[G11] getter / setter
来源：http://hz.svipenyu.cn/gthoksqdqr.html

Py:   @property 与 @x.setter
来源：http://hz.fengsongda.top/gtnyqfujvh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtnvfrddum.html

JS:   get name() { return this._name; }
来源：http://hz.ydzc1.top/gtlvcfigkl.html

TS:   get name(): string { return this._name; }
来源：http://hz.sweek.top/gtjhmdplss.html

Java: public String getName() { return name; }
来源：http://hz.ydzc1.top/gtwjrgftcv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cheryme.top/gthldlnfwh.html

Ruby: attr_accessor :name
来源：http://hz.xuanzx.com/gtsvdkxlyq.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtalxpgcyz.html

[G12] 对象转字符串
来源：http://hz.pycfn.com/gtkubuggah.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgufenzy.top/gtvfsetkfe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtelqilgwj.html

JS:   toString() { return this.name; }
来源：http://hz.cqqwz.cn/gtoeyafblv.html

TS:   toString(): string { return this.name; }
来源：http://hz.zdqjudy.top/gtnhgcvxzc.html

Java: @Override public String toString() { return name; }
来源：http://hz.sufxvd.cn/gtdaajlzdf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhengqikj.top/gtpzjkiwwr.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtkjjdauec.html

C#:   public override string ToString() => Name;
来源：http://hz.yj202588.top/gtvsjnjzdg.html

[G13] 判断对象类型
来源：http://hz.sweek.top/gtddiwkpil.html

Py:   isinstance(u, User)
来源：http://hz.mhx1999.top/gtrvfszccl.html

PHP:  $u instanceof User
来源：http://hz.0kj1m.cn/gtluphvdeg.html

JS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtypcecqqq.html

TS:   u instanceof User
来源：http://hz.chenlongwang.top/gthjcqwhcx.html

Java: u instanceof User
来源：http://hz.bjfxy.top/gtjquhymwm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gaohongyu789.top/gtgqyvjpaz.html

Ruby: u.is_a?(User)
来源：http://hz.52xcode.cn/gtigrciwwo.html

C#:   u is User
来源：http://hz.iojbl.cn/gtmokdyjun.html

[G14] 数据类 / record
来源：http://hz.chenlongwang.top/gtzjzryczd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sysykeji.top/gtkojbrdvf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shangyingyoupin.top/gtjvpabszl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gaohongyu789.top/gtehmwczyj.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhixingplan.top/gtjkjwmltk.html

Java: record User(String name, int age) {}
来源：http://hz.hfpthk.cn/gtlfmsfhpo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.andypj.xyz/gtnqkoothf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgfzy.top/gthrfbfxir.html

C#:   record User(string Name, int Age);
来源：http://hz.zhoulong.xyz/gtyemdazzu.html

[G15] 枚举
来源：http://hz.yj20258.top/gtpfulvvmx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dianchejie.cn/gtpcfxgydq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shanyushiyangkeji.top/gtkdcpotce.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.feifeiyinyue.top/gtonkzrubn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtvwgwwtiq.html

Java: enum Color { RED, GREEN }
来源：http://hz.xylfe.cn/gtepexfdig.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sxryk.cn/gtqsibyuhu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuxming.cn/gtnphekhot.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtkqxunicc.html

[G16] 对象转数组 / 字典
来源：http://hz.xuetiantiany.cn/gtvxvrrynw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtctephenw.html

PHP:  get_object_vars($obj);
来源：http://hz.havefunace.top/gtanojvqyf.html

JS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtnoirukmz.html

TS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtsghfihmr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yangfankeji.com/gtzvhowklw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.52xcode.cn/gtwhtpgckr.html

Ruby: obj.instance_variables
来源：http://hz.nanxuanxn.top/gteqvojdhw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daria6918.cn/gtvkiolciz.html

================================================================================
来源：http://hz.c1oappe.top/gtzyapuoxv.html

H. 异常与错误处理
来源：http://hz.daria6918.cn/gtbndihmzp.html

================================================================================
来源：http://hz.ybcxt.top/gtogwvjwkx.html

[H01] try / catch 基础
来源：http://hz.wangshuangyany.cn/gtzaqohzqv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gtckqammia.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhixingplan.top/gtgiijsmbx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtqtpnnddf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tanke756.top/gtaaftxzep.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jianghu66.top/gtbnrhqdwe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hywenlv.cn/gtgzgzztqf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenlongwang.top/gtzlhxvgdx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cheryme.top/gtyvfeqtbq.html

[H02] finally / ensure 收尾
来源：http://hz.aizwys.cn/gteytifsrc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hongshengwenyu.top/gtzallqzly.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtdpovmusk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtefdgggha.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtuheqsmkg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtzmjfwyge.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.316326.xyz/gtdkfbbzbo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ehwqpu.com/gtsmaasnhp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.andypj.xyz/gtktqjzucp.html

[H03] 主动抛出异常
来源：http://hz.pengpengdd.cyou/gtnrwwfpkr.html

Py:   raise ValueError("错误信息")
来源：http://hz.guannengcc.top/gtlyuqsvqa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtlopawwzi.html

JS:   throw new Error("错误信息");
来源：http://hz.xylfe.cn/gtjepteukw.html

TS:   throw new Error("错误信息");
来源：http://hz.sysykeji.top/gtopkvqeuq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtbbrisact.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.mhx1999.top/gtcuyhyxgz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shangyingyoupin.top/gtperqowmu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtvpemobjk.html

[H04] 自定义异常类型
来源：http://hz.gogol.net.cn/gtouxvhcgi.html

Py:   class MyError(Exception): pass
来源：http://hz.fzhhl.top/gtcfzvdctz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangkeji.top/gtbcxgqtxx.html

JS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtrlaclyfo.html

TS:   class MyError extends Error {}
来源：http://hz.yuxming.cn/gthyhizxzc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.smart0.xyz/gtrlgqrrdc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gogol.net.cn/gtrtldhiyp.html

Ruby: class MyError < StandardError; end
来源：http://hz.hfpthk.cn/gtljiwkqrl.html

C#:   class MyException : Exception {}
来源：http://hz.jyoumei.cn/gtmurjoers.html

[H05] 捕获特定类型
来源：http://hz.mhx1999.top/gtqhmlnxfs.html

Py:   except ValueError as e:
来源：http://hz.gaohongyu789.top/gtpewcxkxq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenzaomai.com/gtbgoieojb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtbjjaegaz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtjmmehfez.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aibaodan.cn/gteheotzzs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuetiantiany.cn/gtofwobtzp.html

Ruby: rescue ArgumentError => e
来源：http://hz.9152youxi.cn/gtqoxqsvbz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgfzy.top/gtokuqfjoc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jianghu66.top/gtrlkcyzlv.html

Py:   value = d.get("k") or default
来源：http://hz.jinqigufen.top/gtqywuxzes.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.dashuyun.cn/gtwrwmwmic.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtjamegcte.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gtpiluollz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hywenlv.cn/gtpcoywwnp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxuanxn.top/gtlsbqnxme.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj20258.top/gtweyqiiin.html

C#:   obj?.A?.B ?? default
来源：http://hz.andypj.xyz/gtjsonzxxx.html

[H07] 断言
来源：http://hz.feifeiyinyue.top/gtaryiekvt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.feifeiyinyue.top/gtinpihcoo.html

PHP:  assert($x > 0);
来源：http://hz.svipenyu.cn/gtxlazpvpq.html

JS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gteefsvlxp.html

TS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtmyravyct.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yueranfly.top/gtrkwifrtx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xziqi.cn/gtycgfccqh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gtbjodzarg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jiagoushi.top/gtgpzgywle.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhijiandao.cn/gtxyqdmwng.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dianchejie.cn/gtdzziqwzj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.0kj1m.cn/gtywccjaxr.html


<!-- 参考信息 -->