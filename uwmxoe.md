代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenjidiqi.icu/gtpiqiafxw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangdashe.top/gtjdjlgeql.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pengpengdd.cyou/gtbhvkkrmq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.pycfn.com/gtmziffbln.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.316326.xyz/gtvlpphdss.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hammf.cn/gtqxeamnyw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.redwolf501.top/gtlhmrnbod.html

[F04] 追加写入文件
来源：http://hz.nanxuanxn.top/gtrrbqgmqt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ywan-chungtsiang.top/gtstahkzen.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhijiandao.cn/gtyqbgulzl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gtjvpshsif.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gtvpayawqh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pycfn.com/gtosuhvdzf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tanke756.top/gtwerkbymd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sysykeji.top/gtkemcvmey.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.pycfn.com/gtlmbadjna.html

[F05] 判断文件或目录是否存在
来源：http://hz.vqdsnc.cn/gtwkyttmdb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.meibo888.top/gtiebckdms.html

PHP:  file_exists("a.txt");
来源：http://hz.aibaodan.cn/gtyhtmweez.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtulypacvh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtwxfxoeuy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtkolzltkk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yonumen.top/gtsiejamff.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxuanxn.top/gtkksxnqxr.html

C#:   File.Exists("a.txt")
来源：http://hz.mhx1999.top/gtjuthblmm.html

[F06] 删除文件
来源：http://hz.feifeiyinyue.top/gtqzhufbkt.html

Py:   os.remove("a.txt")
来源：http://hz.dianchejie.cn/gtaeftrwqd.html

PHP:  unlink("a.txt");
来源：http://hz.hnxiangtu.top/gtisjwtkzo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gtsfbbasvq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sufxvd.cn/gtqwvpvtfd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtttstphra.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxuanxn.top/gtncjgogmq.html

Ruby: File.delete("a.txt")
来源：http://hz.tianlin.xyz/gticbhacle.html

C#:   File.Delete("a.txt");
来源：http://hz.dianchejie.cn/gtnadagbhy.html

[F07] 创建目录（含多级）
来源：http://hz.jiagoushi.top/gtplpmaztj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pengpengdd.cyou/gtjrhrfmuv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gtixcxxvvs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dianchejie.cn/gtnoynmnax.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtclnxrewe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hfpthk.cn/gtztyfkuae.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ywan-chungtsiang.top/gtbbdnylua.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.mhx1999.top/gtqbnuorqv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yongpay.top/gtunyzyfkk.html

[F08] 遍历目录
来源：http://hz.daria6918.cn/gtzsjlkplv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ivvv.top/gtvczmuxyx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.birdmap.top/gtzdtsfujr.html

JS:   fs.readdirSync("dir")
来源：http://hz.jianghu66.top/gttffqscpp.html

TS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gthotzwsos.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gtcvahwwqw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.aibaodan.cn/gtcrkbkphd.html

Ruby: Dir.children("dir")
来源：http://hz.jiagoushi.top/gtdrhjmhcx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.quarkkingdee.top/gtukllvobg.html

[F09] 获取文件大小
来源：http://hz.gzhubu.top/gtlctsvhir.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zycfv.cn/gtqezlglbp.html

PHP:  filesize("a.txt");
来源：http://hz.c1oappe.top/gtavgmngnh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtcpeghenl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gtbqjcdwbo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtgmnumrnz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xziqi.cn/gtgiyihfsl.html

Ruby: File.size("a.txt")
来源：http://hz.9152youxi.cn/gteixkihqq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ybcxt.top/gtoyzjlzxr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.kuanghao11.cn/gtrovipqvj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtraurquea.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xziqi.cn/gtimlaebmh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtrmchrwtl.html

TS:   path.extname("a.txt")
来源：http://hz.aizwys.cn/gtndogmqjj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydjk.org.cn/gtosuaizlq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtwyoroztb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gthxbnhbki.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtfmlsnhax.html

[F11] 复制与移动文件
来源：http://hz.316326.xyz/gtmxatgsje.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtsjemwahx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.316326.xyz/gtzhilehcb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtdctaaifb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtedbejwll.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jiagoushi.top/gtsbfxiqjm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.fzhhl.top/gtffasbwhm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtwqcnqkjt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.svipenyu.cn/gteozbgdux.html

[F12] CSV 读写
来源：http://hz.zhijiandao.cn/gtbkbyhods.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jlsjyb.cn/gtqcywucrh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zdqjudy.top/gtfmghlufp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hammf.cn/gttnehckam.html

TS:   // 同上
来源：http://hz.zhaomingkeji.xyz/gtvhuehthe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sufxvd.cn/gtmdnyxbqw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.c1oappe.top/gtgbpzecuo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.9152youxi.cn/gtidaqtecs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sufxvd.cn/gtjofxsygn.html

================================================================================
来源：http://hz.zhijiandao.cn/gtyfqplnyw.html

G. 面向对象
来源：http://hz.cdnleiting.top/gtmqhxiozl.html

================================================================================
来源：http://hz.guannengcc.top/gtyyvvfvgj.html

[G01] 定义类
来源：http://hz.hysaishi.cn/gtjsfzrnaj.html

Py:   class User: pass
来源：http://hz.tian-w.cn/gthebccwyb.html

PHP:  class User {}
来源：http://hz.jinqigfzy.top/gtdclitxwo.html

JS:   class User {}
来源：http://hz.hywenlv.cn/gtnvkxbepw.html

TS:   class User { name: string = ""; }
来源：http://hz.hongshengwenyu.top/gtmywjytlv.html

Java: class User {}
来源：http://hz.tanke756.top/gteazvkmkv.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtlsnsxpsj.html

Ruby: class User; end
来源：http://hz.chenlongwang.top/gtbxoycvvj.html

C#:   class User {}
来源：http://hz.jinyuanbaomall.cn/gtdmtivblk.html

[G02] 构造函数
来源：http://hz.dianchejie.cn/gtvsnmlgsw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.birdmap.top/gtwkjdmeee.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yongpay.top/gtgwjfqkjq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xziqi.cn/gtdzjzanlr.html

TS:   constructor(public name: string) {}
来源：http://hz.tianlin.xyz/gtxsvvxtdq.html

Java: User(String name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gtbhladadk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daxiang520.top/gtoxlfpnfe.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.quarkkingdee.top/gtporrzmya.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dianchejie.cn/gtcyecsexd.html

[G03] 实例属性
来源：http://hz.kuanghao11.cn/gtfmtykrxo.html

Py:   self.name = "x"
来源：http://hz.cdnleiting.top/gtvalrwego.html

PHP:  public string $name = "x";
来源：http://hz.hfpthk.cn/gtyarfevys.html

JS:   this.name = "x";
来源：http://hz.chenlongwang.top/gtilipnhsj.html

TS:   name: string = "x";
来源：http://hz.aizwys.cn/gtlpuklzhr.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gtrrkyeeht.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhaomingkeji.xyz/gtknexwmie.html

Ruby: @name = "x"
来源：http://hz.meibo888.top/gtkbenzkov.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinyuanbaomall.cn/gtowzmbcxb.html

[G04] 定义方法
来源：http://hz.hnxiangtu.top/gtlybckuda.html

Py:   def greet(self): return self.name
来源：http://hz.andypj.xyz/gtbdxdiaec.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gttpfjsbeh.html

JS:   greet() { return this.name; }
来源：http://hz.yonumen.top/gtpnsixvnf.html

TS:   greet(): string { return this.name; }
来源：http://hz.jyoumei.cn/gteowlajtn.html

Java: String greet() { return name; }
来源：http://hz.yongpay.top/gtpblfyhuq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ppjwa.cn/gthmyzejoz.html

Ruby: def greet; @name; end
来源：http://hz.cashguo.top/gtujaybxgj.html

C#:   public string Greet() => Name;
来源：http://hz.meibo888.top/gtnkbxbvvg.html

[G05] 继承
来源：http://hz.daxiang520.top/gtkheaogyh.html

Py:   class Admin(User): pass
来源：http://hz.snrcjt.cn/gtwkvmpqzg.html

PHP:  class Admin extends User {}
来源：http://hz.gotoacloud.top/gtprisyexe.html

JS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtxnmghzso.html

TS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gttrjqbqqv.html

Java: class Admin extends User {}
来源：http://hz.cucudq.cn/gtbhafmasv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuxming.cn/gtpukfehbj.html

Ruby: class Admin < User; end
来源：http://hz.feifeiyinyue.top/gtoklgnqgz.html

C#:   class Admin : User {}
来源：http://hz.pengpengdd.cyou/gtgpkxikry.html

[G06] 重写方法
来源：http://hz.fengsongda.top/gtdqedznis.html

Py:   def greet(self): return "admin"
来源：http://hz.sufxvd.cn/gtwyrgwljg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtyqppnzbw.html

JS:   greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gtrlbkoigu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtbnswcxnq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtuyrhxjnm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sufxvd.cn/gtjuylghnm.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigfzy.top/gtlldbtpex.html

C#:   public override string Greet() => "admin";
来源：http://hz.ehwqpu.com/gtdvzxkkrz.html

[G07] 调用父类方法
来源：http://hz.ehwqpu.com/gtevmdpxzm.html

Py:   super().greet()
来源：http://hz.feifeiyinyue.top/gtpuvtueel.html

PHP:  parent::greet();
来源：http://hz.meibo888.top/gtlgglipbt.html

JS:   super.greet();
来源：http://hz.zycfv.cn/gthcqwrjtv.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtotoaipob.html

Java: super.greet();
来源：http://hz.hywenlv.cn/gtavhygjba.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tanke756.top/gtqaangqdr.html

Ruby: super
来源：http://hz.gaohongyu789.top/gtgxemdnaz.html

C#:   base.Greet();
来源：http://hz.chenlongwang.top/gtrhfasrdv.html

[G08] 静态方法与属性
来源：http://hz.xuetiantiany.cn/gtyuhgwzer.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ivvv.top/gtekhmbxky.html

PHP:  public static function f() {}
来源：http://hz.meibo888.top/gteavjtdcj.html

JS:   static f() {}
来源：http://hz.xuanzx.com/gtplfxocyc.html

TS:   static f(): void {}
来源：http://hz.jianghu66.top/gtdarbziea.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gtdthozlwn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj202588.top/gtnaviuiha.html

Ruby: def self.f; end
来源：http://hz.tian-w.cn/gtoigwjldb.html

C#:   public static void F() {}
来源：http://hz.snrcjt.cn/gtgxukllgb.html

[G09] 接口 / 抽象类
来源：http://hz.hfpthk.cn/gtynmexjri.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sysykeji.top/gtpmyaqirj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhaomingkeji.xyz/gtnddzqsxe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hongshengwenyu.top/gthvcswvwm.html

TS:   interface Shape { area(): number; }
来源：http://hz.jyoumei.cn/gtmesdgfoi.html

Java: interface Shape { double area(); }
来源：http://hz.gogol.net.cn/gtxphstokj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aizwys.cn/gtegpnbttx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj20258.top/gtgwxqfrvz.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgfzy.top/gtuelcaeko.html

[G10] 访问控制
来源：http://hz.jianghu66.top/gtrtpspbva.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cheryme.top/gtafdsfyjc.html

PHP:  public / protected / private
来源：http://hz.chenlongwang.top/gtrxxzyxwi.html

JS:   #private 字段；其余公开
来源：http://hz.xziqi.cn/gtwjluiesy.html

TS:   public / protected / private
来源：http://hz.yuanzhike.top/gtgklogkoa.html

Java: public / protected / private / 默认包级
来源：http://hz.guannengcc.top/gtdgbveinm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenzaomai.com/gtectlbfuv.html

Ruby: public / protected / private
来源：http://hz.xinyue.icu/gtxviluxiq.html

C#:   public / protected / private / internal
来源：http://hz.aibaodan.cn/gtvwcloodb.html

[G11] getter / setter
来源：http://hz.yanxiufei.cn/gtycvmuhrj.html

Py:   @property 与 @x.setter
来源：http://hz.shangyingyoupin.top/gtekedyynt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yonumen.top/gtlfpkdtuf.html

JS:   get name() { return this._name; }
来源：http://hz.sysykeji.top/gtsyoekuab.html

TS:   get name(): string { return this._name; }
来源：http://hz.yueranfly.top/gtjulrsptp.html

Java: public String getName() { return name; }
来源：http://hz.vqdsnc.cn/gtjdtxodde.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tian-w.cn/gtfrxxxzkh.html

Ruby: attr_accessor :name
来源：http://hz.zhongyouzk.top/gtaddxsobg.html

C#:   public string Name { get; set; }
来源：http://hz.sufxvd.cn/gtsnmkcjvr.html

[G12] 对象转字符串
来源：http://hz.sxryk.cn/gtdpasplmy.html

Py:   def __str__(self): return self.name
来源：http://hz.andypj.xyz/gtmsyhqeeq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtugezgrrd.html

JS:   toString() { return this.name; }
来源：http://hz.gogol.net.cn/gtcawshwjw.html

TS:   toString(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtzrouofky.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhixingplan.top/gtdrtoyfmn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gotoacloud.top/gtwjpyqzwp.html

Ruby: def to_s; @name; end
来源：http://hz.hywenlv.cn/gtlksdtvib.html

C#:   public override string ToString() => Name;
来源：http://hz.jianghu66.top/gtjogxogsd.html

[G13] 判断对象类型
来源：http://hz.mhx1999.top/gtbadnalgi.html

Py:   isinstance(u, User)
来源：http://hz.chenlongwang.top/gtyildrkjo.html

PHP:  $u instanceof User
来源：http://hz.yueranfly.top/gttvesbrhu.html

JS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtpkehyluo.html

TS:   u instanceof User
来源：http://hz.havefunace.top/gtmnlwidjr.html

Java: u instanceof User
来源：http://hz.pengpengdd.cyou/gtchfzsvvj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhoulong.xyz/gtnomnfbhc.html

Ruby: u.is_a?(User)
来源：http://hz.jinqigufen.top/gtrgugjjzn.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtttcodbgg.html

[G14] 数据类 / record
来源：http://hz.aizwys.cn/gttflyuxbo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangkeji.top/gtbxvfkggu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydzc1.top/gtqrfzvfkn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydjk.org.cn/gtycmfwgkr.html

TS:   type User = { name: string; age: number };
来源：http://hz.52xcode.cn/gtztprddkv.html

Java: record User(String name, int age) {}
来源：http://hz.chenjidiqi.icu/gtbvkfotgz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cqqwz.cn/gtyoxupykm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.bjfxy.top/gtbaxoydke.html

C#:   record User(string Name, int Age);
来源：http://hz.aibaodan.cn/gtgqrvedzz.html

[G15] 枚举
来源：http://hz.xylfe.cn/gtdsbkdvya.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dianchejie.cn/gttkhidatl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nanxinkj.top/gtmsjqprlz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.birdmap.top/gtzeldatkd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sysykeji.top/gtizpthqah.html

Java: enum Color { RED, GREEN }
来源：http://hz.yonumen.top/gtxnwhfeli.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xuetiantiany.cn/gtbyvucoej.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sysykeji.top/gtczzfphvx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtjimqbaad.html

[G16] 对象转数组 / 字典
来源：http://hz.chenjidiqi.icu/gtrthuxwhg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.vqdsnc.cn/gtvlzypakx.html

PHP:  get_object_vars($obj);
来源：http://hz.meibo888.top/gtsdyggwun.html

JS:   Object.entries(obj)
来源：http://hz.ydjk.org.cn/gthqjzjmjs.html

TS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gtgjpfxpmk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtvgintgox.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.meibo888.top/gtuuvoorvr.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangkeji.top/gtfcqicubq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gtvqmyxajw.html

================================================================================
来源：http://hz.hywenlv.cn/gtccavibjf.html

H. 异常与错误处理
来源：http://hz.nanxuanxn.top/gtlpjxxnae.html

================================================================================
来源：http://hz.tian-w.cn/gtuirilcar.html

[H01] try / catch 基础
来源：http://hz.shuidangran.top/gtqoovjcfo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xingfuxueyuan.xyz/gttldcyymv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shanyushiyangtech.top/gttdlqbzqz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.haohaochexian.top/gtdzujazwl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhengqikj.top/gtlonidfdg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.0kj1m.cn/gtinkfrdom.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hammf.cn/gtgwhelaic.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtagkawcma.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hnqzz.top/gtcnrpmzop.html

[H02] finally / ensure 收尾
来源：http://hz.jlsjyb.cn/gtmyjkerkf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sufxvd.cn/gtzxynuqjh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gttnketaun.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtzthhzrhh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtsqihwmhj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtkijyvuze.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tian-w.cn/gtoerrmpim.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daxiang520.top/gtziyvznrm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hongshengwenyu.top/gtbnhnmgnu.html

[H03] 主动抛出异常
来源：http://hz.sufxvd.cn/gtigbmesqc.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhengqikj.top/gtzihcwokc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtykytyzyg.html

JS:   throw new Error("错误信息");
来源：http://hz.ppjwa.cn/gtkcltsizg.html

TS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtjrcuhvjh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cdnleiting.top/gthlhekyax.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yonumen.top/gtaelppqmy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuanzx.com/gtajaatbsx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtdbtyxegl.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangtech.top/gteuwebdws.html

Py:   class MyError(Exception): pass
来源：http://hz.shanyushiyangtech.top/gtzcvhqlml.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.smart0.xyz/gtbvpvpzcs.html

JS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtuvjwadhs.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigufen.top/gtxijygyzm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cqqwz.cn/gtomefhlus.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtlxjbjwgc.html

Ruby: class MyError < StandardError; end
来源：http://hz.zdqjudy.top/gtcdvoebsf.html

C#:   class MyException : Exception {}
来源：http://hz.zhijiandao.cn/gtxmnztcqw.html

[H05] 捕获特定类型
来源：http://hz.dianchejie.cn/gtcwffmhww.html

Py:   except ValueError as e:
来源：http://hz.svipenyu.cn/gtghfpicgq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daria6918.cn/gtsgskdotl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gttxysqlwf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtlbialtci.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ywan-chungtsiang.top/gtdnkktzlc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tian-w.cn/gtiwibtufx.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhiwuduotai.top/gtubifrigz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangshuangyany.cn/gtjsrqwvrw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.c1oappe.top/gtnsnbmohu.html

Py:   value = d.get("k") or default
来源：http://hz.wangdashe.top/gtghbizpyu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cashguo.top/gtgwbzdbsm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtwvijvicz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangshuangyany.cn/gtlbtltfnb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.c1oappe.top/gtdlysgdli.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.havefunace.top/gtzyurafxc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hywenlv.cn/gtzpfwdtlu.html

C#:   obj?.A?.B ?? default
来源：http://hz.shangyingyoupin.top/gtfvmlyqcd.html

[H07] 断言
来源：http://hz.zdqjudy.top/gtljkekpmb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnxiangtu.top/gtgiabuawr.html

PHP:  assert($x > 0);
来源：http://hz.zhaomingkeji.xyz/gtdgykfovb.html

JS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtpchejwwk.html

TS:   console.assert(x > 0);
来源：http://hz.ehwqpu.com/gttggcyqbi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.bjfxy.top/gtnhxvezgd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ehwqpu.com/gtovzphqyl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xziqi.cn/gteaeuvvfc.html


<!-- 参考信息 -->