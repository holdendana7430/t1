代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tian-w.cn/gtcxgbaput.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.svipenyu.cn/gtwzzrxbxw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtjkynwoda.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtahgdaxgn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj20258.top/gtatagafjd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.svipenyu.cn/gtauaysehi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xinyue.icu/gtkblopwge.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gtqbyjqnhx.html

[F05] 判断文件或目录是否存在
来源：http://hz.hnqzz.top/gtpyxoparp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigfzy.top/gtwngbvbnx.html

PHP:  file_exists("a.txt");
来源：http://hz.hnqzz.top/gtjnxkhuxa.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ehwqpu.com/gtocqhznvh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nanxuanxn.top/gtvgmanzvc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtwagmilsb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.iojbl.cn/gtgtjbwqrv.html

Ruby: File.exist?("a.txt")
来源：http://hz.tanke756.top/gtqhuyptrg.html

C#:   File.Exists("a.txt")
来源：http://hz.jiagoushi.top/gttxvbycsl.html

[F06] 删除文件
来源：http://hz.pengpengdd.cyou/gtucvvlatr.html

Py:   os.remove("a.txt")
来源：http://hz.xinyue.icu/gtzggznpzp.html

PHP:  unlink("a.txt");
来源：http://hz.bjfxy.top/gtlkcrevez.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gthszupghi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtgheyfaok.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtfpdmzhwq.html

Go:   os.Remove("a.txt")
来源：http://hz.jiagoushi.top/gtrdthtsxp.html

Ruby: File.delete("a.txt")
来源：http://hz.birdmap.top/gtoqodprdy.html

C#:   File.Delete("a.txt");
来源：http://hz.hnqzz.top/gtjevpgcqm.html

[F07] 创建目录（含多级）
来源：http://hz.gaohongyu789.top/gtemdcsojm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jyoumei.cn/gtygzzjkpy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.dianchejie.cn/gtksgxzgaj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgfzy.top/gtyfkvovya.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sufxvd.cn/gtyzqarvcj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xylfe.cn/gtdcgerzmv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gaohongyu789.top/gthwapeagm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cucudq.cn/gtlkzmbvny.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tanke756.top/gtjdxdzlvw.html

[F08] 遍历目录
来源：http://hz.nanxinkj.top/gtgqbkntxr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yueranfly.top/gtazuoknpm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.52xcode.cn/gttiyarfbu.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhaomingkeji.xyz/gtmvvtwuse.html

TS:   fs.readdirSync("dir")
来源：http://hz.ivvv.top/gtdlvzfpmu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yuanzhike.top/gtgblwmgao.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shzxlz.cn/gtnwozwyvi.html

Ruby: Dir.children("dir")
来源：http://hz.tanke756.top/gthjgtwhex.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tian-w.cn/gtvtzoaeta.html

[F09] 获取文件大小
来源：http://hz.zhaomingkeji.xyz/gtfduevyxi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenjidiqi.icu/gtcarexxel.html

PHP:  filesize("a.txt");
来源：http://hz.yvedp.cn/gtsuevdtlc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gtstlltagh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ivvv.top/gtsrspfjhp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtqquefyar.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gogol.net.cn/gtiysnzxfq.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258.top/gtmonghmgc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guowangkeji.top/gtcieitwog.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigfzy.top/gtqvlsbvpu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtkkdxhzxc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj20258.top/gtsinqzhbe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtxgodgqzt.html

TS:   path.extname("a.txt")
来源：http://hz.hongshengwenyu.top/gtuxvfcyfo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xingfuxueyuan.xyz/gtzewqriwb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sufxvd.cn/gtfwrxcxch.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtehcwtyer.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj202588.top/gtrvitqcdn.html

[F11] 复制与移动文件
来源：http://hz.ppjwa.cn/gtauiqdbdr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtpezknmhc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yongpay.top/gtjcqkjwlm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtianiugwc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtvcaqedbj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sxryk.cn/gtwwmasbkj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhengqikj.top/gtcfmyopjz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtlizhnhlk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.mhx1999.top/gttkcdyadi.html

[F12] CSV 读写
来源：http://hz.yonumen.top/gtkcbvrsyy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.9152youxi.cn/gtrlxffrpf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.redwolf501.top/gtxdgsjtzb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gotoacloud.top/gtahghdhrc.html

TS:   // 同上
来源：http://hz.fzhhl.top/gtwfsqwwal.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj20258888.top/gtumtvtnyo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jqgfzy.top/gtxosovpxf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pengpengdd.cyou/gtqrsyntre.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cqqwz.cn/gtczuhczag.html

================================================================================
来源：http://hz.gaohongyu789.top/gtezpnrxwv.html

G. 面向对象
来源：http://hz.shuidangran.top/gtdvaixtoj.html

================================================================================
来源：http://hz.tian-w.cn/gtlfqqdujm.html

[G01] 定义类
来源：http://hz.c1oappe.top/gtydqtslgu.html

Py:   class User: pass
来源：http://hz.jinghuilouyu.cn/gtdzvuncjr.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtwvootqes.html

JS:   class User {}
来源：http://hz.yj20258.top/gthcbikfuc.html

TS:   class User { name: string = ""; }
来源：http://hz.fengsongda.top/gtjrdrnwgc.html

Java: class User {}
来源：http://hz.xylfe.cn/gtppzbbied.html

Go:   type User struct { Name string }
来源：http://hz.xinyue.icu/gtrmkriqxq.html

Ruby: class User; end
来源：http://hz.xinyue.icu/gtbdffvcbi.html

C#:   class User {}
来源：http://hz.xylfe.cn/gtxoneoqpt.html

[G02] 构造函数
来源：http://hz.hammf.cn/gtbyekwymu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ybcxt.top/gtvleuabak.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenzaomai.com/gtxaqfsuqf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtvngujcse.html

TS:   constructor(public name: string) {}
来源：http://hz.cashguo.top/gtzkwyrdwm.html

Java: User(String name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtmrtmgabp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pengpengdd.cyou/gtotxvlxeq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hammf.cn/gtylchjgrb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtiycikvsw.html

[G03] 实例属性
来源：http://hz.jinghuilouyu.cn/gtyxnrjewr.html

Py:   self.name = "x"
来源：http://hz.9152youxi.cn/gthpjlqmrm.html

PHP:  public string $name = "x";
来源：http://hz.xziqi.cn/gtolswpvyn.html

JS:   this.name = "x";
来源：http://hz.zdqjudy.top/gtuxsbtmot.html

TS:   name: string = "x";
来源：http://hz.iojbl.cn/gtdoymqkjf.html

Java: private String name;
来源：http://hz.jinqigfzy.top/gtlwjmcnms.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.dianchejie.cn/gtvpyzfzkp.html

Ruby: @name = "x"
来源：http://hz.yj202588.top/gtedwahmzq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shzxlz.cn/gtlcajfwyx.html

[G04] 定义方法
来源：http://hz.cucudq.cn/gttydwmkhm.html

Py:   def greet(self): return self.name
来源：http://hz.zhongyouzk.top/gtnrgjzofy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tanke756.top/gtflshewvn.html

JS:   greet() { return this.name; }
来源：http://hz.yongpay.top/gtowrngkqx.html

TS:   greet(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtyhbufdxi.html

Java: String greet() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtydpnckix.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtrfrjwxdx.html

Ruby: def greet; @name; end
来源：http://hz.jiagoushi.top/gtyslvuqhf.html

C#:   public string Greet() => Name;
来源：http://hz.feifeiyinyue.top/gtqwgxljgt.html

[G05] 继承
来源：http://hz.zhijiandao.cn/gtbvnvxolz.html

Py:   class Admin(User): pass
来源：http://hz.jinqigfzy.top/gtmpgxlezn.html

PHP:  class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtycrvbtqj.html

JS:   class Admin extends User {}
来源：http://hz.hfpthk.cn/gtugchxcgf.html

TS:   class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtoscigwrn.html

Java: class Admin extends User {}
来源：http://hz.bjfxy.top/gthrwepmln.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cucudq.cn/gtddmkolki.html

Ruby: class Admin < User; end
来源：http://hz.52xcode.cn/gtsaeioonb.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtlejmquwq.html

[G06] 重写方法
来源：http://hz.feifeiyinyue.top/gtsqgieioy.html

Py:   def greet(self): return "admin"
来源：http://hz.haohaochexian.top/gtfoebtkpz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtgvkpywdv.html

JS:   greet() { return "admin"; }
来源：http://hz.yangfankeji.com/gtrsroihnq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj20258.top/gtpmzjakns.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtmsgjpdvu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ybcxt.top/gtpwvwvtid.html

Ruby: def greet; "admin"; end
来源：http://hz.snrcjt.cn/gtpvgipgdy.html

C#:   public override string Greet() => "admin";
来源：http://hz.pengpengdd.cyou/gtchkzapnm.html

[G07] 调用父类方法
来源：http://hz.yonumen.top/gthzarzxcl.html

Py:   super().greet()
来源：http://hz.yonumen.top/gtqxhytmle.html

PHP:  parent::greet();
来源：http://hz.yuxming.cn/gtogbaapyy.html

JS:   super.greet();
来源：http://hz.xinyue.icu/gtfffrkfsw.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtrtrsbayg.html

Java: super.greet();
来源：http://hz.chenjidiqi.icu/gthcqnveto.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ehwqpu.com/gtpizwdlyq.html

Ruby: super
来源：http://hz.jinghuilouyu.cn/gtweiijsou.html

C#:   base.Greet();
来源：http://hz.zhaomingkeji.xyz/gtemymmola.html

[G08] 静态方法与属性
来源：http://hz.52xcode.cn/gtxqcbrvne.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhiwuduotai.top/gtrvcczwev.html

PHP:  public static function f() {}
来源：http://hz.shzxlz.cn/gtsvoyatgo.html

JS:   static f() {}
来源：http://hz.birdmap.top/gtxwlqjmoz.html

TS:   static f(): void {}
来源：http://hz.yj202588.top/gtfwdhajgu.html

Java: static void f() {}
来源：http://hz.jqgufenzy.top/gtfqmcuoin.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yueranfly.top/gtdddjphrt.html

Ruby: def self.f; end
来源：http://hz.pengpengdd.cyou/gtcgsfovoo.html

C#:   public static void F() {}
来源：http://hz.kuanghao11.cn/gtiftbtlsv.html

[G09] 接口 / 抽象类
来源：http://hz.52xcode.cn/gtmtnemego.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yangfankeji.com/gteecsnvxx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cdnleiting.top/gtsjzregze.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ywan-chungtsiang.top/gtxasbsrze.html

TS:   interface Shape { area(): number; }
来源：http://hz.52xcode.cn/gtckzyetyb.html

Java: interface Shape { double area(); }
来源：http://hz.gzhubu.top/gtolckvmbs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.redwolf501.top/gtowbjvwap.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fengsongda.top/gtueejykcf.html

C#:   interface IShape { double Area(); }
来源：http://hz.nanxuanxn.top/gtbngoyrpa.html

[G10] 访问控制
来源：http://hz.cashguo.top/gtulxrawmn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinyuanbaomall.cn/gtmmxcmdtn.html

PHP:  public / protected / private
来源：http://hz.aibaodan.cn/gtptdkgrac.html

JS:   #private 字段；其余公开
来源：http://hz.shanyushiyangkeji.top/gtzuscoxnl.html

TS:   public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtukzkalqs.html

Java: public / protected / private / 默认包级
来源：http://hz.yanxiufei.cn/gtwhkytqqh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.mhx1999.top/gtdnrqelxj.html

Ruby: public / protected / private
来源：http://hz.tianlin.xyz/gtntquahce.html

C#:   public / protected / private / internal
来源：http://hz.gzhubu.top/gtmkogzjnm.html

[G11] getter / setter
来源：http://hz.jyoumei.cn/gthqioycfi.html

Py:   @property 与 @x.setter
来源：http://hz.jlsjyb.cn/gtjyivteio.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtmnpxxwiz.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtmuqagtkh.html

TS:   get name(): string { return this._name; }
来源：http://hz.hywenlv.cn/gtlvuqjgvj.html

Java: public String getName() { return name; }
来源：http://hz.zhijiandao.cn/gtkbnbesde.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ppjwa.cn/gtkfudwxfa.html

Ruby: attr_accessor :name
来源：http://hz.aizwys.cn/gtlhchegme.html

C#:   public string Name { get; set; }
来源：http://hz.sysykeji.top/gtvthndxao.html

[G12] 对象转字符串
来源：http://hz.svipenyu.cn/gtqnwtbfvt.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigfzy.top/gthcvzgpzj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258.top/gtisqtnmcw.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gtmxzhhpxe.html

TS:   toString(): string { return this.name; }
来源：http://hz.cheryme.top/gtcfnesuvv.html

Java: @Override public String toString() { return name; }
来源：http://hz.9152youxi.cn/gtuiwewaqm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtbjwhmofr.html

Ruby: def to_s; @name; end
来源：http://hz.hongshengwenyu.top/gtmsvjqxmw.html

C#:   public override string ToString() => Name;
来源：http://hz.hongshengwenyu.top/gtzpzqlrit.html

[G13] 判断对象类型
来源：http://hz.hfpthk.cn/gtuykjerux.html

Py:   isinstance(u, User)
来源：http://hz.jqgufenzy.top/gtxpzkwhvo.html

PHP:  $u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtjumeojxu.html

JS:   u instanceof User
来源：http://hz.redwolf501.top/gtjdoazrwk.html

TS:   u instanceof User
来源：http://hz.hnqzz.top/gtmlisfqfw.html

Java: u instanceof User
来源：http://hz.yangfankeji.com/gttlatrwac.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gtbugoufgh.html

Ruby: u.is_a?(User)
来源：http://hz.gotoacloud.top/gtgynklevq.html

C#:   u is User
来源：http://hz.nwbrower.top/gtnabofvyj.html

[G14] 数据类 / record
来源：http://hz.zhijiandao.cn/gttpzgimzz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydjk.org.cn/gtsfszfgdl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gzhubu.top/gthkvdayjq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhixingplan.top/gteacawcil.html

TS:   type User = { name: string; age: number };
来源：http://hz.jianghu66.top/gtxqysbjqz.html

Java: record User(String name, int age) {}
来源：http://hz.cashguo.top/gtguytekzn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gtfdtqkamn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xinyue.icu/gtsosyjvit.html

C#:   record User(string Name, int Age);
来源：http://hz.cashguo.top/gtxqbjpavo.html

[G15] 枚举
来源：http://hz.zhongyouzk.top/gtkefedpgj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuanzx.com/gtndzmzwwc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shanyushiyangkeji.top/gtvbruevpp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.9152youxi.cn/gtgbqerzqe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtwpllmlow.html

Java: enum Color { RED, GREEN }
来源：http://hz.tianlin.xyz/gtvrzxbvge.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxuanxn.top/gtjxuwxhcx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gaohongyu789.top/gtquxqpnxg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gtzuuwplme.html

[G16] 对象转数组 / 字典
来源：http://hz.hywenlv.cn/gtqjeymgsn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hammf.cn/gtchprdkct.html

PHP:  get_object_vars($obj);
来源：http://hz.wangdashe.top/gtlycbbogr.html

JS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtkcjvfxrj.html

TS:   Object.entries(obj)
来源：http://hz.xuetiantiany.cn/gtubmubyhc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tian-w.cn/gtlgoehkrk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yvedp.cn/gtjphwlhxl.html

Ruby: obj.instance_variables
来源：http://hz.jinqigfzy.top/gtfwtbmghz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuxming.cn/gthkdlctft.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtuaejtuqc.html

H. 异常与错误处理
来源：http://hz.zhiwuduotai.top/gtuumwcpdz.html

================================================================================
来源：http://hz.xylfe.cn/gtaeprshfh.html

[H01] try / catch 基础
来源：http://hz.mhx1999.top/gtvgttjykg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sufxvd.cn/gtfjprjicq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnxiangtu.top/gtnjbfjkxx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtlbtkcjwl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jiagoushi.top/gteriqwnzh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.iojbl.cn/gtzkmrmczr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jianghu66.top/gtiffsxnfa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.guannengcc.top/gtkenivjzp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.haohaochexian.top/gtpbndmepf.html

[H02] finally / ensure 收尾
来源：http://hz.birdmap.top/gtorirpouw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ivvv.top/gttjyoybkt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtdicanjpi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtrzdavpvs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtwuqfwyig.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtkxhrtwwe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sufxvd.cn/gtcxcarksm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gtqjycmznz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gaohongyu789.top/gtxaalypwx.html

[H03] 主动抛出异常
来源：http://hz.shzxlz.cn/gtxxzxemve.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgfzy.top/gtplvlymqy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtdxapwwed.html

JS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtcoltzrmb.html

TS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtyxgqfqia.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtkucwempt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cqqwz.cn/gtqldeyrsa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtmbeerepk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtqtcqmyut.html

[H04] 自定义异常类型
来源：http://hz.nanxuanxn.top/gtjzlptvpc.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gtwlwnklis.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangshuangyany.cn/gtnynxrgvg.html

JS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gtiaqezhax.html

TS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gttkfyltjz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yongpay.top/gtzxmltwhz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtibroxusg.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhaomingkeji.xyz/gtcykcdiqa.html

C#:   class MyException : Exception {}
来源：http://hz.ivvv.top/gtnyllpesg.html

[H05] 捕获特定类型
来源：http://hz.gotoacloud.top/gtisifidtc.html

Py:   except ValueError as e:
来源：http://hz.chenjidiqi.icu/gtftxelbgt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.andypj.xyz/gtiptqbnoq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtuhfdyydx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtpkzgrdke.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yanxiufei.cn/gtrnhjlgrc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtnblmvsvm.html

Ruby: rescue ArgumentError => e
来源：http://hz.havefunace.top/gtzddbygnu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.daxiang520.top/gtyxzlloey.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yangfankeji.com/gtjcojypgj.html

Py:   value = d.get("k") or default
来源：http://hz.jlsjyb.cn/gtqkbgpbwk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.kuanghao11.cn/gtyfdbolgu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtbkeelnrv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtbvgcbegd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.redwolf501.top/gtnbbifvou.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.snrcjt.cn/gtpdtktawz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinghuilouyu.cn/gttauyovev.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxuanxn.top/gtouyoxijz.html

[H07] 断言
来源：http://hz.shzxlz.cn/gtrorphgmy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.iojbl.cn/gtbuwppacv.html

PHP:  assert($x > 0);
来源：http://hz.hammf.cn/gtzxaibahy.html

JS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gtytokudtu.html

TS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gtfrzghoda.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pengpengdd.cyou/gtuzpmcoju.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.quarkkingdee.top/gtsccfohjv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xziqi.cn/gtowmjrdrl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.birdmap.top/gtsryihzay.html

[H08] 获取错误信息与堆栈
来源：http://hz.xuanzx.com/gtqoljdoym.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.vqdsnc.cn/gtlejmuzym.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxinkj.top/gtybdrpgld.html

JS:   e.message;  e.stack
来源：http://hz.bjfxy.top/gtinyjhnch.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.birdmap.top/gtqnuhenjp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtfokcpyps.html

Go:   err.Error()
来源：http://hz.jinghuilouyu.cn/gtkyvnibtq.html


<!-- 参考信息 -->