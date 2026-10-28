代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gzhubu.top/gtctunjtdw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gotoacloud.top/gtkejzrupj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gtcvredusp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.redwolf501.top/gtoeguxyuh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhoulong.xyz/gtycbszmee.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.tanke756.top/gtvqehzkvu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhengqikj.top/gtcrjqsnxv.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gtzidjujsh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shanyushiyangtech.top/gtsphdjwid.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinyuanbaomall.cn/gtctzogyzg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gtsqafzrwp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuxming.cn/gtcpswjcty.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tanke756.top/gtpzoputtx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shuidangran.top/gtefyetdek.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pycfn.com/gtmrjevdlk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.nanxuanxn.top/gtnpaqlsll.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258888.top/gtebcygcmi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hnxiangtu.top/gttmeugqqi.html

PHP:  file_exists("a.txt");
来源：http://hz.havefunace.top/gtgtpiawct.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gtjigmesfo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gthiwutkzd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtnwhkitum.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258888.top/gtecgsucqq.html

Ruby: File.exist?("a.txt")
来源：http://hz.c1oappe.top/gtderzlkow.html

C#:   File.Exists("a.txt")
来源：http://hz.tian-w.cn/gttamljjlw.html

[F06] 删除文件
来源：http://hz.chenlongwang.top/gtqlgdnrnz.html

Py:   os.remove("a.txt")
来源：http://hz.nanxinkj.top/gtahlwmokg.html

PHP:  unlink("a.txt");
来源：http://hz.zycfv.cn/gtzhhtlsyi.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.9152youxi.cn/gtzqgjwnfz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhixingplan.top/gtcvkqnhcf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtwpoudusk.html

Go:   os.Remove("a.txt")
来源：http://hz.vqdsnc.cn/gtzdwgehyw.html

Ruby: File.delete("a.txt")
来源：http://hz.yuanzhike.top/gtewbrtkfo.html

C#:   File.Delete("a.txt");
来源：http://hz.mhx1999.top/gtexemivzw.html

[F07] 创建目录（含多级）
来源：http://hz.gogol.net.cn/gtgfyasakg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigufen.top/gtwayxswyt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinqigufen.top/gttulmonvd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenjidiqi.icu/gtughsxuzs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtlvqdjjdc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnxiangtu.top/gtaurlkkhu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gtbvmsrtgp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fengsongda.top/gtynikctgz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.snrcjt.cn/gtrnbkyene.html

[F08] 遍历目录
来源：http://hz.xinyue.icu/gtxijnfrnw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ehwqpu.com/gtkmphgnhm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj202588.top/gtzyajzlsq.html

JS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtayzdbnnn.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj202588.top/gtdtxwrlrh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yuxming.cn/gtyujmzfrk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.meibo888.top/gtixusjlfl.html

Ruby: Dir.children("dir")
来源：http://hz.daria6918.cn/gtpmfuzvxc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sxryk.cn/gtudmxeciy.html

[F09] 获取文件大小
来源：http://hz.cucudq.cn/gtfhpvplwu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangtech.top/gtbqyjofry.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258.top/gtwyofqxwf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydzc1.top/gtrdhxoxix.html

TS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtycqpesdy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtooeckevj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yuanzhike.top/gtuadqlhyf.html

Ruby: File.size("a.txt")
来源：http://hz.cheryme.top/gtyrrnmuav.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zdqjudy.top/gtvzzguamu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.haohaochexian.top/gtyescqruf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtaiccqyct.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fzhhl.top/gtsghaeyji.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtdswvqxzx.html

TS:   path.extname("a.txt")
来源：http://hz.zhoulong.xyz/gtbmujeqbc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuxming.cn/gtwleivihh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yangfankeji.com/gtdpwnumfi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtqsoidhdl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangdashe.top/gthynflfln.html

[F11] 复制与移动文件
来源：http://hz.jinyuanbaomall.cn/gtlixqumii.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtebtrctmb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.kuanghao11.cn/gtfvlgpqpq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtzvkdjwjs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtagdvmdul.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yanxiufei.cn/gtutcygexe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sweek.top/gteaoveuit.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtgyodeumm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hammf.cn/gtbecwqylx.html

[F12] CSV 读写
来源：http://hz.ehwqpu.com/gtwlhpgpmb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.meibo888.top/gtiyedmpzl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jyoumei.cn/gtuarqyaam.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sweek.top/gtogiamwvi.html

TS:   // 同上
来源：http://hz.nanxuanxn.top/gtecizbsvq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ydzc1.top/gtigrwrluz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gtwrsyreuj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ydzc1.top/gtcoyguram.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shzxlz.cn/gtjomnkavk.html

================================================================================
来源：http://hz.zhongyouzk.top/gtrpxsjxze.html

G. 面向对象
来源：http://hz.yj202588.top/gtolndaqgk.html

================================================================================
来源：http://hz.zhengqikj.top/gtpirgajkf.html

[G01] 定义类
来源：http://hz.cucudq.cn/gtpvnlnggb.html

Py:   class User: pass
来源：http://hz.jinghuilouyu.cn/gtpvfyfflc.html

PHP:  class User {}
来源：http://hz.ybcxt.top/gtmzwnutuk.html

JS:   class User {}
来源：http://hz.zhiwuduotai.top/gtmmpzotlt.html

TS:   class User { name: string = ""; }
来源：http://hz.yuanzhike.top/gtxmssvrul.html

Java: class User {}
来源：http://hz.daxiang520.top/gtdqketqde.html

Go:   type User struct { Name string }
来源：http://hz.guowangkeji.top/gtgtalwhmo.html

Ruby: class User; end
来源：http://hz.pengpengdd.cyou/gttpvkklgs.html

C#:   class User {}
来源：http://hz.cdnleiting.top/gtpqerfyib.html

[G02] 构造函数
来源：http://hz.xylfe.cn/gtdrzafcnl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.snrcjt.cn/gtzcajkyej.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daxiang520.top/gtjsznaimg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.0kj1m.cn/gtsbirxfsc.html

TS:   constructor(public name: string) {}
来源：http://hz.chenlongwang.top/gtgrixfdrb.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtopbzjitb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinghuilouyu.cn/gtlackpgmh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenlongwang.top/gtkdikgktv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhixingplan.top/gtcxacnnwr.html

[G03] 实例属性
来源：http://hz.ybcxt.top/gtrpzwxsvd.html

Py:   self.name = "x"
来源：http://hz.c1oappe.top/gtonjjavco.html

PHP:  public string $name = "x";
来源：http://hz.jinqigufen.top/gtfcbyfdfk.html

JS:   this.name = "x";
来源：http://hz.shzxlz.cn/gtmwrsvudk.html

TS:   name: string = "x";
来源：http://hz.mhx1999.top/gtcpzspfdy.html

Java: private String name;
来源：http://hz.zhoulong.xyz/gtmwpdhmtv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.redwolf501.top/gtfuvbawwe.html

Ruby: @name = "x"
来源：http://hz.yj20258.top/gtpevthpcu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinqigfzy.top/gtwewxzpry.html

[G04] 定义方法
来源：http://hz.zhiwuduotai.top/gtwqdvmzvk.html

Py:   def greet(self): return self.name
来源：http://hz.nanxinkj.top/gtpsveseze.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hammf.cn/gtbbzskrpc.html

JS:   greet() { return this.name; }
来源：http://hz.nwbrower.top/gteetqetqs.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuanzx.com/gtggbfpyru.html

Java: String greet() { return name; }
来源：http://hz.hammf.cn/gtvhtaqjal.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fzhhl.top/gtcjhzpjfk.html

Ruby: def greet; @name; end
来源：http://hz.nwbrower.top/gtmtryectd.html

C#:   public string Greet() => Name;
来源：http://hz.hfpthk.cn/gtrzsqqffb.html

[G05] 继承
来源：http://hz.quarkkingdee.top/gtaemnyimf.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtokheulyv.html

PHP:  class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtaycjyeev.html

JS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtrprggsxa.html

TS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtqfjbrrtc.html

Java: class Admin extends User {}
来源：http://hz.birdmap.top/gtqdlgpglw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.c1oappe.top/gthknfzzgq.html

Ruby: class Admin < User; end
来源：http://hz.wangshuangyany.cn/gtdmrbphwu.html

C#:   class Admin : User {}
来源：http://hz.quarkkingdee.top/gthbakdrmw.html

[G06] 重写方法
来源：http://hz.andypj.xyz/gtssnkpiqi.html

Py:   def greet(self): return "admin"
来源：http://hz.zhoulong.xyz/gtplyfomsi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sweek.top/gtfwkawkpw.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtcvmezvma.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tianlin.xyz/gtgxkkwnvj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtjomfkupt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangkeji.top/gtymhlhhuj.html

Ruby: def greet; "admin"; end
来源：http://hz.xinyue.icu/gtqmxnhric.html

C#:   public override string Greet() => "admin";
来源：http://hz.hammf.cn/gteavltnkf.html

[G07] 调用父类方法
来源：http://hz.chenjidiqi.icu/gtpjmtwggm.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtkozktjua.html

PHP:  parent::greet();
来源：http://hz.dianchejie.cn/gtbhhmoqbt.html

JS:   super.greet();
来源：http://hz.xinyue.icu/gtlyocjail.html

TS:   super.greet();
来源：http://hz.shanyushiyangtech.top/gtjlxybpwl.html

Java: super.greet();
来源：http://hz.gogol.net.cn/gtugeerxeo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnqzz.top/gtatbrfeaa.html

Ruby: super
来源：http://hz.daria6918.cn/gteiredjbj.html

C#:   base.Greet();
来源：http://hz.zhoulong.xyz/gtasvzyezn.html

[G08] 静态方法与属性
来源：http://hz.nanxinkj.top/gtdcfasbbk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hongshengwenyu.top/gtkmqfyxyp.html

PHP:  public static function f() {}
来源：http://hz.hnqzz.top/gtapdcjsuy.html

JS:   static f() {}
来源：http://hz.hnxiangtu.top/gtfoaqmfau.html

TS:   static f(): void {}
来源：http://hz.gotoacloud.top/gtlbovyorm.html

Java: static void f() {}
来源：http://hz.ehwqpu.com/gtomsiebmq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shuidangran.top/gtprxwlxgv.html

Ruby: def self.f; end
来源：http://hz.tian-w.cn/gtymohneqm.html

C#:   public static void F() {}
来源：http://hz.quarkkingdee.top/gteionytjk.html

[G09] 接口 / 抽象类
来源：http://hz.wangshuangyany.cn/gtmunuzfdl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.feifeiyinyue.top/gtunwmflkd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.c1oappe.top/gtxzsqnshr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gtjwnlophn.html

TS:   interface Shape { area(): number; }
来源：http://hz.tian-w.cn/gtyqzdqnee.html

Java: interface Shape { double area(); }
来源：http://hz.hnxiangtu.top/gtpwmuxicm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yongpay.top/gtfyipditm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tianlin.xyz/gtmoqvimcb.html

C#:   interface IShape { double Area(); }
来源：http://hz.ywan-chungtsiang.top/gtbfdliimi.html

[G10] 访问控制
来源：http://hz.sxryk.cn/gtgnpxxbou.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yongpay.top/gtgdtfjwyq.html

PHP:  public / protected / private
来源：http://hz.shzxlz.cn/gtkudswklz.html

JS:   #private 字段；其余公开
来源：http://hz.tian-w.cn/gtqbqshutt.html

TS:   public / protected / private
来源：http://hz.shzxlz.cn/gtlkkzahwg.html

Java: public / protected / private / 默认包级
来源：http://hz.bjfxy.top/gtyzbsyaeq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.haohaochexian.top/gtkwmrupwa.html

Ruby: public / protected / private
来源：http://hz.shuidangran.top/gtadpmbyni.html

C#:   public / protected / private / internal
来源：http://hz.52xcode.cn/gtzfcjgpol.html

[G11] getter / setter
来源：http://hz.pengpengdd.cyou/gtdjjauhur.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258.top/gthnbzwono.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtqhrgqols.html

JS:   get name() { return this._name; }
来源：http://hz.hnqzz.top/gtabroedpm.html

TS:   get name(): string { return this._name; }
来源：http://hz.tanke756.top/gtyxdzgiiv.html

Java: public String getName() { return name; }
来源：http://hz.nanxuanxn.top/gtgntuxzxu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dianchejie.cn/gtydirkvpj.html

Ruby: attr_accessor :name
来源：http://hz.ivvv.top/gtocqgeqyw.html

C#:   public string Name { get; set; }
来源：http://hz.zhengqikj.top/gtvigrqmyd.html

[G12] 对象转字符串
来源：http://hz.yangfankeji.com/gteqngkfej.html

Py:   def __str__(self): return self.name
来源：http://hz.zhijiandao.cn/gtjyjitgib.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xziqi.cn/gthxaiipbz.html

JS:   toString() { return this.name; }
来源：http://hz.cdnleiting.top/gtdsadpltw.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnxiangtu.top/gtnfkudfxy.html

Java: @Override public String toString() { return name; }
来源：http://hz.yonumen.top/gtqnginzki.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shzxlz.cn/gtclbkddgj.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258888.top/gtecpeuxwg.html

C#:   public override string ToString() => Name;
来源：http://hz.yanxiufei.cn/gtrpmfflqh.html

[G13] 判断对象类型
来源：http://hz.sxryk.cn/gtmushnown.html

Py:   isinstance(u, User)
来源：http://hz.yj20258.top/gtwycvobne.html

PHP:  $u instanceof User
来源：http://hz.hongshengwenyu.top/gtlkclidhs.html

JS:   u instanceof User
来源：http://hz.xinyue.icu/gtozkdylcx.html

TS:   u instanceof User
来源：http://hz.smart0.xyz/gtxoewefnm.html

Java: u instanceof User
来源：http://hz.zhiwuduotai.top/gtpolhbdoc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.quarkkingdee.top/gtpomippvb.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258888.top/gtjkkenrjw.html

C#:   u is User
来源：http://hz.shzxlz.cn/gtfxcxteqj.html

[G14] 数据类 / record
来源：http://hz.zhongyouzk.top/gtcgygqplw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.redwolf501.top/gttnypdxzn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.kuanghao11.cn/gtfqaubcqu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yanxiufei.cn/gtvfzadxxh.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhixingplan.top/gtekzbluqp.html

Java: record User(String name, int age) {}
来源：http://hz.fzhhl.top/gtbsrvpbdt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xingfuxueyuan.xyz/gtdrottbmf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jlsjyb.cn/gtgucnlzwr.html

C#:   record User(string Name, int Age);
来源：http://hz.guowangkeji.top/gtbaczotve.html

[G15] 枚举
来源：http://hz.zhengqikj.top/gtmqvqwdub.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangkeji.top/gtvmovesyp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gotoacloud.top/gtzjmfpjkk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zycfv.cn/gtstzlhsmw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.quarkkingdee.top/gtdzluteur.html

Java: enum Color { RED, GREEN }
来源：http://hz.jianghu66.top/gtcztdcwtf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.0kj1m.cn/gtuqlwmocm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhongyouzk.top/gtjufadmdw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtnvoqivcj.html

[G16] 对象转数组 / 字典
来源：http://hz.zhoulong.xyz/gtocguzirn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhixingplan.top/gtemhamrar.html

PHP:  get_object_vars($obj);
来源：http://hz.snrcjt.cn/gtzsrstvqv.html

JS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtgysqgtqf.html

TS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gtsiwxzkhj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.c1oappe.top/gthusxysww.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ydjk.org.cn/gtxrpoxwxz.html

Ruby: obj.instance_variables
来源：http://hz.haohaochexian.top/gtvkcsolno.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gaohongyu789.top/gtzphaasca.html

================================================================================
来源：http://hz.yj20258.top/gtxuxhpwvd.html

H. 异常与错误处理
来源：http://hz.cucudq.cn/gttnshzczj.html

================================================================================
来源：http://hz.cqqwz.cn/gtdjkqsgcp.html

[H01] try / catch 基础
来源：http://hz.gogol.net.cn/gtmyowchsr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigufen.top/gtnylakjie.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gogol.net.cn/gtawamnach.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dianchejie.cn/gtrawpmmnd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.svipenyu.cn/gtqaczepzi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydzc1.top/gtxuxpyxvq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtnogzidux.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ehwqpu.com/gtnpiifwas.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhixingplan.top/gtmbblkcxy.html

[H02] finally / ensure 收尾
来源：http://hz.xylfe.cn/gtgmyialbj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cqqwz.cn/gtmhdptcmw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtfduyrxnf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtjkuihtlj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtlovdxrkr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtekzwrvap.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tian-w.cn/gtnzaijgsf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cdnleiting.top/gtxkiizxzn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yonumen.top/gthctqmdda.html

[H03] 主动抛出异常
来源：http://hz.cashguo.top/gtwfztrmxc.html

Py:   raise ValueError("错误信息")
来源：http://hz.xuetiantiany.cn/gtcicctkse.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtuilyopmh.html

JS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtdtqqnfmb.html

TS:   throw new Error("错误信息");
来源：http://hz.dashuyun.cn/gthnszbphi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtxknjzefz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fengsongda.top/gtsipfnarr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.quarkkingdee.top/gthnurafdq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258.top/gtoeedopmj.html

[H04] 自定义异常类型
来源：http://hz.yj20258888.top/gttcmvaotj.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigfzy.top/gtsykpabqo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yangfankeji.com/gtpmayfnyy.html

JS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gtdtvwztow.html

TS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtmqddiwdf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gttkpkfddq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.havefunace.top/gtdohagqxk.html

Ruby: class MyError < StandardError; end
来源：http://hz.fzhhl.top/gtktiqjkeh.html

C#:   class MyException : Exception {}
来源：http://hz.sufxvd.cn/gtvhpmocfq.html

[H05] 捕获特定类型
来源：http://hz.zdqjudy.top/gtykgwsrvx.html

Py:   except ValueError as e:
来源：http://hz.ivvv.top/gtdtklxbsf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sxryk.cn/gtmefmhifn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gtnvptijew.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangtech.top/gtyvdiivoa.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.andypj.xyz/gtmnupmxnd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sysykeji.top/gtvmpgbuyx.html

Ruby: rescue ArgumentError => e
来源：http://hz.gogol.net.cn/gtjoyckbvv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhixingplan.top/gtlqpxdkif.html

[H06] 可选值 / 空值安全访问
来源：http://hz.redwolf501.top/gtpexyhuxj.html

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gtattfswsu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.kuanghao11.cn/gtjhfavscn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtcowwqmbz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gtdhtderdt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtasdjvzml.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhongyouzk.top/gtmcmpjscd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zycfv.cn/gtayyuzkir.html

C#:   obj?.A?.B ?? default
来源：http://hz.shzxlz.cn/gtbuxrehbs.html

[H07] 断言
来源：http://hz.birdmap.top/gtsrljqdgx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhongyouzk.top/gttindfrqi.html

PHP:  assert($x > 0);
来源：http://hz.hammf.cn/gtnmkygegv.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtbiuuvnih.html

TS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtptrdmihs.html

Java: assert x > 0 : "必须为正";
来源：http://hz.feifeiyinyue.top/gtzyrekrvu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gtwacydjzb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jianghu66.top/gtnltrwcxg.html


<!-- 参考信息 -->