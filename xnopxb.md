代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.mhx1999.top/gtznexyipd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhijiandao.cn/gtauqtztqu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gotoacloud.top/gtyykvxtcq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.kuanghao11.cn/gtqmwjsvfa.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangdashe.top/gtsaohmxuc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guowangkeji.top/gtdxktyjlm.html

PHP:  file_exists("a.txt");
来源：http://hz.xylfe.cn/gtbwrlgnqc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gtvtthyaej.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gthgfdejux.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtvmobokxt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tianlin.xyz/gtnnpmjjzo.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258888.top/gtgqxssmni.html

C#:   File.Exists("a.txt")
来源：http://hz.9152youxi.cn/gtztfjcyur.html

[F06] 删除文件
来源：http://hz.ydjk.org.cn/gtjsxbtszo.html

Py:   os.remove("a.txt")
来源：http://hz.yuxming.cn/gtccizxhys.html

PHP:  unlink("a.txt");
来源：http://hz.sxryk.cn/gtysrkjxqs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yongpay.top/gthzzkjmeo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ivvv.top/gtipwtplrv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gttsqureha.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgufenzy.top/gtikmrbwxh.html

Ruby: File.delete("a.txt")
来源：http://hz.mhx1999.top/gttkhwsfjd.html

C#:   File.Delete("a.txt");
来源：http://hz.hysaishi.cn/gtqazovbcu.html

[F07] 创建目录（含多级）
来源：http://hz.ivvv.top/gtjmbldtvb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.bjfxy.top/gtieawkkeb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigfzy.top/gtuuuqbxkl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtgxffnisx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnqzz.top/gtmmadrfzb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtwstbcxpj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhaomingkeji.xyz/gtmkrttxgr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.feifeiyinyue.top/gtxphrqzfn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.feifeiyinyue.top/gtgmqzozvo.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtqkhjggvn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nwbrower.top/gtdypccfxg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.bjfxy.top/gtfsxpbclm.html

JS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtjwpjgzje.html

TS:   fs.readdirSync("dir")
来源：http://hz.xingfuxueyuan.xyz/gtouioiiee.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtntolqnms.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tanke756.top/gtmmzxbyqe.html

Ruby: Dir.children("dir")
来源：http://hz.jyoumei.cn/gtihefmeef.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhoulong.xyz/gtdgkxsske.html

[F09] 获取文件大小
来源：http://hz.shzxlz.cn/gtmmrjrkky.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenlongwang.top/gthaqsvomh.html

PHP:  filesize("a.txt");
来源：http://hz.xylfe.cn/gtjujdpknr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gtlcvmjnso.html

TS:   fs.statSync("a.txt").size
来源：http://hz.feifeiyinyue.top/gtibwallxu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtjttpmzpi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yongpay.top/gteqokoysn.html

Ruby: File.size("a.txt")
来源：http://hz.mhx1999.top/gtnlkqtquk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.snrcjt.cn/gtxdjlpvhd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jqgfzy.top/gtpnlywmcg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtvnskbzxg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhijiandao.cn/gtfvagsrvm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtcqqegsca.html

TS:   path.extname("a.txt")
来源：http://hz.yanxiufei.cn/gtnhjmgsix.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.andypj.xyz/gtgayzchxp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xziqi.cn/gteceswvqe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gteoqyszbu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinqigufen.top/gtinogqvzm.html

[F11] 复制与移动文件
来源：http://hz.yonumen.top/gtmhffxppt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtuuvoxmob.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhengqikj.top/gtyotdnwol.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtqwjyxxbe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gttrubuelp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jyoumei.cn/gtjfzqqlhz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xuanzx.com/gtuztjxnmi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtscdgcuon.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xuanzx.com/gtqjalgbun.html

[F12] CSV 读写
来源：http://hz.guannengcc.top/gtebtrncwb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.guannengcc.top/gtvajjmfjy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhongyouzk.top/gtrqghfbfm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gotoacloud.top/gttoczxqnc.html

TS:   // 同上
来源：http://hz.quarkkingdee.top/gtlmypbphm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sxryk.cn/gtihdstjnp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenjidiqi.icu/gtnyqqkxfs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yueranfly.top/gtxrulbljf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sysykeji.top/gtxrmmjgqe.html

================================================================================
来源：http://hz.mhx1999.top/gtgkbvimkn.html

G. 面向对象
来源：http://hz.birdmap.top/gtithcwmbj.html

================================================================================
来源：http://hz.ivvv.top/gtfwontgie.html

[G01] 定义类
来源：http://hz.jyoumei.cn/gtpatuwjug.html

Py:   class User: pass
来源：http://hz.xingfuxueyuan.xyz/gtakjkpbka.html

PHP:  class User {}
来源：http://hz.aizwys.cn/gttewgmees.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtzioryoyt.html

TS:   class User { name: string = ""; }
来源：http://hz.mhx1999.top/gtbqxjbptf.html

Java: class User {}
来源：http://hz.bjfxy.top/gtlurfrmnu.html

Go:   type User struct { Name string }
来源：http://hz.9152youxi.cn/gtrsulagke.html

Ruby: class User; end
来源：http://hz.vqdsnc.cn/gtqlqslgak.html

C#:   class User {}
来源：http://hz.feifeiyinyue.top/gtefnqynjf.html

[G02] 构造函数
来源：http://hz.pengpengdd.cyou/gtlbrqxfod.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gotoacloud.top/gtiaziaeya.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.mhx1999.top/gtrxlrjonm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.meibo888.top/gtemrqkyrz.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258888.top/gtfbykjohi.html

Java: User(String name) { this.name = name; }
来源：http://hz.nwbrower.top/gtmcxsemxl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ybcxt.top/gtovcjzysf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ydjk.org.cn/gtzckmbvzp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.birdmap.top/gtucnxszzn.html

[G03] 实例属性
来源：http://hz.zhongyouzk.top/gtyqitjgxf.html

Py:   self.name = "x"
来源：http://hz.bjfxy.top/gtggzgenlm.html

PHP:  public string $name = "x";
来源：http://hz.mhx1999.top/gttnsfhucd.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtxoodkjwj.html

TS:   name: string = "x";
来源：http://hz.pengpengdd.cyou/gtleagqreh.html

Java: private String name;
来源：http://hz.wangdashe.top/gtnxdbnwgv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.svipenyu.cn/gtqwlpbuzf.html

Ruby: @name = "x"
来源：http://hz.vqdsnc.cn/gtchymwkpl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.fzhhl.top/gtyjigceiy.html

[G04] 定义方法
来源：http://hz.shangyingyoupin.top/gtagqqunhp.html

Py:   def greet(self): return self.name
来源：http://hz.cashguo.top/gtivqmtufr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.316326.xyz/gthrnndhev.html

JS:   greet() { return this.name; }
来源：http://hz.xuanzx.com/gtdtxgreig.html

TS:   greet(): string { return this.name; }
来源：http://hz.jyoumei.cn/gtiklwltpv.html

Java: String greet() { return name; }
来源：http://hz.daxiang520.top/gtcaullrkz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jianghu66.top/gtkcskphqn.html

Ruby: def greet; @name; end
来源：http://hz.yj202588.top/gtcrorgiuu.html

C#:   public string Greet() => Name;
来源：http://hz.ivvv.top/gtybczvppz.html

[G05] 继承
来源：http://hz.pycfn.com/gtdrjztcmn.html

Py:   class Admin(User): pass
来源：http://hz.xinyue.icu/gturkfqazc.html

PHP:  class Admin extends User {}
来源：http://hz.cqqwz.cn/gtwnhfrbre.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gteyvjvpey.html

TS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gtrhnggjts.html

Java: class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtgkqyircp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yanxiufei.cn/gthslmjsri.html

Ruby: class Admin < User; end
来源：http://hz.svipenyu.cn/gthjsgemvx.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtywxiwomb.html

[G06] 重写方法
来源：http://hz.jqgfzy.top/gtaflxyshg.html

Py:   def greet(self): return "admin"
来源：http://hz.yuxming.cn/gtrlbmdabx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtkfqcbpek.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtjxcovydc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtvwvezgsr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtuklnpbae.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tanke756.top/gtqxutwiok.html

Ruby: def greet; "admin"; end
来源：http://hz.52xcode.cn/gtufxienfl.html

C#:   public override string Greet() => "admin";
来源：http://hz.wangshuangyany.cn/gtqsgepzxt.html

[G07] 调用父类方法
来源：http://hz.jinqigufen.top/gtmfpqhvdk.html

Py:   super().greet()
来源：http://hz.chenjidiqi.icu/gtrmwdlztd.html

PHP:  parent::greet();
来源：http://hz.andypj.xyz/gtxswgavkg.html

JS:   super.greet();
来源：http://hz.xziqi.cn/gtndsojtmj.html

TS:   super.greet();
来源：http://hz.tanke756.top/gtpoqamzql.html

Java: super.greet();
来源：http://hz.ydzc1.top/gtrwjutscl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hysaishi.cn/gtrmiezoja.html

Ruby: super
来源：http://hz.shuidangran.top/gtwuzvweff.html

C#:   base.Greet();
来源：http://hz.hongshengwenyu.top/gtoteypujd.html

[G08] 静态方法与属性
来源：http://hz.gotoacloud.top/gtimacmofp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hywenlv.cn/gtzikwfhdn.html

PHP:  public static function f() {}
来源：http://hz.gzhubu.top/gtnavvdjpt.html

JS:   static f() {}
来源：http://hz.jqgfzy.top/gtroorxski.html

TS:   static f(): void {}
来源：http://hz.yvedp.cn/gticgqegwv.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gtmwtyayfb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jlsjyb.cn/gtfyucysif.html

Ruby: def self.f; end
来源：http://hz.nanxuanxn.top/gtpywofmda.html

C#:   public static void F() {}
来源：http://hz.yj20258888.top/gtrzcjkcan.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangtech.top/gtybxrseqe.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xinyue.icu/gtlqibiilc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yueranfly.top/gtezhsapmh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yueranfly.top/gtdhapcihb.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinghuilouyu.cn/gtnmcgbptc.html

Java: interface Shape { double area(); }
来源：http://hz.yangfankeji.com/gtfhqcfilt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhixingplan.top/gtqgrovqsq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenzaomai.com/gtsuiaqyyf.html

C#:   interface IShape { double Area(); }
来源：http://hz.redwolf501.top/gtwfgqntyd.html

[G10] 访问控制
来源：http://hz.hysaishi.cn/gtboaygzhb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shzxlz.cn/gtfaciisiv.html

PHP:  public / protected / private
来源：http://hz.xziqi.cn/gtcybbvtxg.html

JS:   #private 字段；其余公开
来源：http://hz.zycfv.cn/gtkioulwgg.html

TS:   public / protected / private
来源：http://hz.tianlin.xyz/gtpktoyaqj.html

Java: public / protected / private / 默认包级
来源：http://hz.pycfn.com/gtpxadnslo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.vqdsnc.cn/gtrcvukbfb.html

Ruby: public / protected / private
来源：http://hz.zhiwuduotai.top/gtbklzbpqe.html

C#:   public / protected / private / internal
来源：http://hz.zhijiandao.cn/gttvtbofnm.html

[G11] getter / setter
来源：http://hz.vqdsnc.cn/gtjyszyxtr.html

Py:   @property 与 @x.setter
来源：http://hz.ybcxt.top/gthixajqbx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtdvrgrdqy.html

JS:   get name() { return this._name; }
来源：http://hz.zhengqikj.top/gtpdzaedpd.html

TS:   get name(): string { return this._name; }
来源：http://hz.yangfankeji.com/gtxbiezsiq.html

Java: public String getName() { return name; }
来源：http://hz.zhijiandao.cn/gtzckfklfl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gttvijyjtd.html

Ruby: attr_accessor :name
来源：http://hz.hammf.cn/gtlacvlnmi.html

C#:   public string Name { get; set; }
来源：http://hz.dashuyun.cn/gtehzdeoug.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtldqrfsgx.html

Py:   def __str__(self): return self.name
来源：http://hz.zhoulong.xyz/gtddoyshgi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtiebpjqqo.html

JS:   toString() { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtsfpahxyn.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj20258888.top/gtddhjcxrq.html

Java: @Override public String toString() { return name; }
来源：http://hz.kuanghao11.cn/gttffeandu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xinyue.icu/gtuvwqkyod.html

Ruby: def to_s; @name; end
来源：http://hz.tian-w.cn/gtixhtbdnt.html

C#:   public override string ToString() => Name;
来源：http://hz.jqgfzy.top/gtlkwyftbj.html

[G13] 判断对象类型
来源：http://hz.yj202588.top/gtmxcdoigk.html

Py:   isinstance(u, User)
来源：http://hz.nanxuanxn.top/gtvpyehlty.html

PHP:  $u instanceof User
来源：http://hz.xziqi.cn/gtngbpakkh.html

JS:   u instanceof User
来源：http://hz.hfpthk.cn/gtjooowvtf.html

TS:   u instanceof User
来源：http://hz.gaohongyu789.top/gtypsidfqx.html

Java: u instanceof User
来源：http://hz.kuanghao11.cn/gtfnssosot.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hammf.cn/gtqryiflfo.html

Ruby: u.is_a?(User)
来源：http://hz.52xcode.cn/gtthlvtffj.html

C#:   u is User
来源：http://hz.ivvv.top/gtfzysvvul.html

[G14] 数据类 / record
来源：http://hz.hywenlv.cn/gtczylajve.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgufenzy.top/gtxjpgghkk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xinyue.icu/gtalnxvlob.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gzhubu.top/gtktbseydi.html

TS:   type User = { name: string; age: number };
来源：http://hz.jqgfzy.top/gtenghylyl.html

Java: record User(String name, int age) {}
来源：http://hz.aibaodan.cn/gtvliayjbp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tanke756.top/gtqpsttkmw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.feifeiyinyue.top/gtvyvldcrn.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtvzrpbnlk.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtpilqkhfd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cdnleiting.top/gthjjttkqj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.wangshuangyany.cn/gtgcacemct.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zycfv.cn/gtutdwlwwa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtdrkunrgo.html

Java: enum Color { RED, GREEN }
来源：http://hz.bjfxy.top/gtixdqvkxi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nwbrower.top/gtxjqqncyz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jqgfzy.top/gtzwyoidgi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtxiwioech.html

[G16] 对象转数组 / 字典
来源：http://hz.gaohongyu789.top/gtlggdeczu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yanxiufei.cn/gtipijglmb.html

PHP:  get_object_vars($obj);
来源：http://hz.xuanzx.com/gtmvwatbog.html

JS:   Object.entries(obj)
来源：http://hz.hongshengwenyu.top/gtkhdlkega.html

TS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtlodoqpig.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jiagoushi.top/gtlpignfzo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shuidangran.top/gtmwpsquhm.html

Ruby: obj.instance_variables
来源：http://hz.chenlongwang.top/gtrgvrfjaz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ybcxt.top/gtiszzobpf.html

================================================================================
来源：http://hz.yj20258.top/gtjkfegwfq.html

H. 异常与错误处理
来源：http://hz.dashuyun.cn/gtclhgslja.html

================================================================================
来源：http://hz.jqgufenzy.top/gtenmonaye.html

[H01] try / catch 基础
来源：http://hz.iojbl.cn/gtdcxbhjxf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenjidiqi.icu/gtzlxclchd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhaomingkeji.xyz/gtourmxbqp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtezgmgiob.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hfpthk.cn/gtcutmnbfe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigufen.top/gtunydxnie.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhaomingkeji.xyz/gtvlfdncjg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cucudq.cn/gthrbmrsow.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.fzhhl.top/gteexvpqqn.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gtmjyytgpa.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.feifeiyinyue.top/gtqgviyqcr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtpepevcst.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtmnsfhgtw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtgsymnvpz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtkdgbpxct.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydzc1.top/gteuqmdldz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258888.top/gtnqgizfpw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnxiangtu.top/gtloglfbjo.html

[H03] 主动抛出异常
来源：http://hz.guannengcc.top/gtoegkzuui.html

Py:   raise ValueError("错误信息")
来源：http://hz.c1oappe.top/gtjnulfeua.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtlxxhiitp.html

JS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gttkivougw.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtqhqakitg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gttsbdnvbx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jqgufenzy.top/gtezwstfge.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shanyushiyangtech.top/gtywzjyvzo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtaixsoewb.html

[H04] 自定义异常类型
来源：http://hz.kuanghao11.cn/gtciaxrbfe.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgfzy.top/gtbjmsfdcc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gtcqebfojn.html

JS:   class MyError extends Error {}
来源：http://hz.zhongyouzk.top/gtzwrjxcjn.html

TS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtdigwyqwc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtnffrhaxn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtyymeccfa.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxinkj.top/gtvjzbuzay.html

C#:   class MyException : Exception {}
来源：http://hz.hongshengwenyu.top/gtvfwhelba.html

[H05] 捕获特定类型
来源：http://hz.yj20258888.top/gtfsajfbpv.html

Py:   except ValueError as e:
来源：http://hz.hnxiangtu.top/gtyifomadx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ivvv.top/gtadfudgkn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.316326.xyz/gtcmbovjkm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigufen.top/gtthdjzxke.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nwbrower.top/gteviibnjl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.haohaochexian.top/gtrivznwkh.html

Ruby: rescue ArgumentError => e
来源：http://hz.nwbrower.top/gtcucshoji.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.smart0.xyz/gtshkhkrqe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.daxiang520.top/gtwudgnupq.html

Py:   value = d.get("k") or default
来源：http://hz.mhx1999.top/gtmiwpvvlf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.c1oappe.top/gtlwkdrjnc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.9152youxi.cn/gtyjxpibmq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gtccftmltx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinghuilouyu.cn/gtnvzyxgxj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhongyouzk.top/gtqxsbxvjs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.0kj1m.cn/gtsqudffir.html

C#:   obj?.A?.B ?? default
来源：http://hz.hammf.cn/gtmqabbxxs.html

[H07] 断言
来源：http://hz.redwolf501.top/gtxrtthswd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fzhhl.top/gtfxbsrknv.html

PHP:  assert($x > 0);
来源：http://hz.zhijiandao.cn/gtllekakwq.html

JS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gtkrphlvjf.html

TS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtletixxev.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj20258888.top/gtmlthofre.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xuetiantiany.cn/gtnqiixawu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinghuilouyu.cn/gtphtghfqi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtqifxtpaf.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenjidiqi.icu/gtccisrgqx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aizwys.cn/gtieoacrqn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.feifeiyinyue.top/gtbgcdsvrv.html

JS:   e.message;  e.stack
来源：http://hz.yvedp.cn/gtrnxifacw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fengsongda.top/gtoebuztbs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnqzz.top/gtecgyhdyk.html

Go:   err.Error()
来源：http://hz.jinqigufen.top/gtwtjjgqly.html

Ruby: e.message;  e.backtrace
来源：http://hz.iojbl.cn/gtgrvwtgou.html

C#:   e.Message;  e.StackTrace
来源：http://hz.wangdashe.top/gtktjvnrgf.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gthkajguhs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhongyouzk.top/gtululovjv.html


<!-- 参考信息 -->