代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.iojbl.cn/gtpcucjfxh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.316326.xyz/gthiyryfoz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtglmabdol.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.52xcode.cn/gtpsolkrja.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydjk.org.cn/gttneboryy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.birdmap.top/gtckifjjmp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtfotdzpcc.html

[F04] 追加写入文件
来源：http://hz.xuanzx.com/gtigqqaqcv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangdashe.top/gtpxhllckx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhaomingkeji.xyz/gtrectmtyb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ehwqpu.com/gtrbwytpet.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtyylqgopg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cashguo.top/gtcubntmtg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.andypj.xyz/gtggdikham.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.svipenyu.cn/gtfffumqak.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xingfuxueyuan.xyz/gtygbopoye.html

[F05] 判断文件或目录是否存在
来源：http://hz.gaohongyu789.top/gtwpquzdbd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ehwqpu.com/gtvwxrqsxz.html

PHP:  file_exists("a.txt");
来源：http://hz.jinqigfzy.top/gtokurdlxe.html

JS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtoigbkzcg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gtnskcaaoh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtybtgajgq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cqqwz.cn/gtixdjuduf.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxuanxn.top/gtedizchon.html

C#:   File.Exists("a.txt")
来源：http://hz.tanke756.top/gtjqwhrgyp.html

[F06] 删除文件
来源：http://hz.daxiang520.top/gtfqavezpo.html

Py:   os.remove("a.txt")
来源：http://hz.yvedp.cn/gtdsxyjvjn.html

PHP:  unlink("a.txt");
来源：http://hz.316326.xyz/gtkzqvrfrc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtuguvxyce.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shuidangran.top/gtkkplorwt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtpwybnloz.html

Go:   os.Remove("a.txt")
来源：http://hz.jyoumei.cn/gtgetqrsti.html

Ruby: File.delete("a.txt")
来源：http://hz.sxryk.cn/gtietfymzj.html

C#:   File.Delete("a.txt");
来源：http://hz.shangyingyoupin.top/gtcjcprdao.html

[F07] 创建目录（含多级）
来源：http://hz.yongpay.top/gtdgvrcxgz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj202588.top/gtuzkxfxlq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.andypj.xyz/gtthhodqze.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtvsukykkh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuanzx.com/gtcwopvbsv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xingfuxueyuan.xyz/gtthmvktjw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aibaodan.cn/gtqiavjovo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guannengcc.top/gtoahzlvec.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydzc1.top/gtrhhmoumf.html

[F08] 遍历目录
来源：http://hz.zhengqikj.top/gtokpflrin.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhiwuduotai.top/gtmljmbweq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xziqi.cn/gtesobbwbq.html

JS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtonbslxgb.html

TS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtxcvgdxmz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.redwolf501.top/gtztxazuta.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shanyushiyangtech.top/gtoufngaok.html

Ruby: Dir.children("dir")
来源：http://hz.dashuyun.cn/gtqmpfvafz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hysaishi.cn/gtnqdwctue.html

[F09] 获取文件大小
来源：http://hz.hfpthk.cn/gtoziuapqv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtshqumbfa.html

PHP:  filesize("a.txt");
来源：http://hz.shzxlz.cn/gtrekifmeo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtvckmqoio.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gttdeatalc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtldoouxoz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ehwqpu.com/gtimuefsyk.html

Ruby: File.size("a.txt")
来源：http://hz.gaohongyu789.top/gtclijuygb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydzc1.top/gtpeojibbk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.daxiang520.top/gtjpoktzwo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtqafrayih.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenzaomai.com/gtqgiftsig.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtowgctlzm.html

TS:   path.extname("a.txt")
来源：http://hz.jqgufenzy.top/gthevrmycd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yangfankeji.com/gtsuwiagtp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtqkvugcon.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtuxhpaubz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258.top/gtddzrembx.html

[F11] 复制与移动文件
来源：http://hz.zhijiandao.cn/gthfgeliyj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtgoevsiuy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xziqi.cn/gtlcikfgre.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtoaypaspg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtyqmibrli.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zycfv.cn/gtefqjebjd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgufenzy.top/gtiaohnfgr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtqrlucohs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.feifeiyinyue.top/gtsultnurn.html

[F12] CSV 读写
来源：http://hz.jyoumei.cn/gtmuyfyrro.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yuanzhike.top/gtucmdudvs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.haohaochexian.top/gtbnlanhqe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.pengpengdd.cyou/gtthcmjvct.html

TS:   // 同上
来源：http://hz.gotoacloud.top/gtcymypyhb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ydjk.org.cn/gtmapitawh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxuanxn.top/gtqvsyptbr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhongyouzk.top/gtgufiabmz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tianlin.xyz/gtkksgcheo.html

================================================================================
来源：http://hz.yueranfly.top/gtpnxriwlx.html

G. 面向对象
来源：http://hz.xylfe.cn/gtpsyfcdjr.html

================================================================================
来源：http://hz.ybcxt.top/gtblpqzvlo.html

[G01] 定义类
来源：http://hz.tian-w.cn/gtikybppbt.html

Py:   class User: pass
来源：http://hz.svipenyu.cn/gtsrtfabuv.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtyvmldfml.html

JS:   class User {}
来源：http://hz.kuanghao11.cn/gtuswzmvcb.html

TS:   class User { name: string = ""; }
来源：http://hz.yongpay.top/gturnrqwcg.html

Java: class User {}
来源：http://hz.havefunace.top/gtxrfifwzz.html

Go:   type User struct { Name string }
来源：http://hz.iojbl.cn/gtsqmnbhzp.html

Ruby: class User; end
来源：http://hz.aizwys.cn/gtqrqnebvv.html

C#:   class User {}
来源：http://hz.gotoacloud.top/gtoqffbztx.html

[G02] 构造函数
来源：http://hz.chenjidiqi.icu/gtynqcruvk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xylfe.cn/gtrtcvvczr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.aibaodan.cn/gtjjmzmryp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xziqi.cn/gtkqdtzaod.html

TS:   constructor(public name: string) {}
来源：http://hz.nwbrower.top/gtkdcejtfj.html

Java: User(String name) { this.name = name; }
来源：http://hz.52xcode.cn/gturtqvgye.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgfzy.top/gtsyirhynb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuanzhike.top/gtntplbzmv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtcmwtplqa.html

[G03] 实例属性
来源：http://hz.nanxuanxn.top/gtnxlmrbsb.html

Py:   self.name = "x"
来源：http://hz.xylfe.cn/gthzxqihcc.html

PHP:  public string $name = "x";
来源：http://hz.ehwqpu.com/gtjxbzltde.html

JS:   this.name = "x";
来源：http://hz.chenjidiqi.icu/gtpmvluage.html

TS:   name: string = "x";
来源：http://hz.nwbrower.top/gtljcakvft.html

Java: private String name;
来源：http://hz.zdqjudy.top/gtqfpmtfar.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xuanzx.com/gtencvcgty.html

Ruby: @name = "x"
来源：http://hz.yj20258.top/gtsoswittc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dianchejie.cn/gtllarlips.html

[G04] 定义方法
来源：http://hz.52xcode.cn/gtcmtbezhn.html

Py:   def greet(self): return self.name
来源：http://hz.316326.xyz/gtxhkrxorl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtfaxljqwf.html

JS:   greet() { return this.name; }
来源：http://hz.gzhubu.top/gttripwqfc.html

TS:   greet(): string { return this.name; }
来源：http://hz.pycfn.com/gtcngtndxi.html

Java: String greet() { return name; }
来源：http://hz.hysaishi.cn/gtnsbxtgrc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigufen.top/gtuxaaebvn.html

Ruby: def greet; @name; end
来源：http://hz.smart0.xyz/gtwcwysung.html

C#:   public string Greet() => Name;
来源：http://hz.jinqigufen.top/gtfgxusurq.html

[G05] 继承
来源：http://hz.wangdashe.top/gtlygqiqjg.html

Py:   class Admin(User): pass
来源：http://hz.zhijiandao.cn/gtabgbolll.html

PHP:  class Admin extends User {}
来源：http://hz.0kj1m.cn/gtngniwtrt.html

JS:   class Admin extends User {}
来源：http://hz.yuanzhike.top/gtqiivangr.html

TS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtxudcclln.html

Java: class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtkrwdcrpz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.birdmap.top/gtlufcsvph.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangtech.top/gtjuoqebzw.html

C#:   class Admin : User {}
来源：http://hz.jqgfzy.top/gtghzyhnue.html

[G06] 重写方法
来源：http://hz.0kj1m.cn/gtlxfqaqjp.html

Py:   def greet(self): return "admin"
来源：http://hz.hywenlv.cn/gthypvqzel.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtogcnmwgx.html

JS:   greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtkypwnxyk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtmjueskds.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtihomluws.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aizwys.cn/gtislhjyyi.html

Ruby: def greet; "admin"; end
来源：http://hz.chenzaomai.com/gtozzlevck.html

C#:   public override string Greet() => "admin";
来源：http://hz.ehwqpu.com/gtckonoxsn.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtlvcogwqw.html

Py:   super().greet()
来源：http://hz.vqdsnc.cn/gtnkcxgvmu.html

PHP:  parent::greet();
来源：http://hz.yj202588.top/gtyodlddnx.html

JS:   super.greet();
来源：http://hz.yj202588.top/gtfdngcozi.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gtoobkvnkv.html

Java: super.greet();
来源：http://hz.cucudq.cn/gtnmamincl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jianghu66.top/gtyougoiye.html

Ruby: super
来源：http://hz.tianlin.xyz/gtfiocspvr.html

C#:   base.Greet();
来源：http://hz.gaohongyu789.top/gtwzkknjmk.html

[G08] 静态方法与属性
来源：http://hz.jinyuanbaomall.cn/gtcnoczkql.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.quarkkingdee.top/gtwxwzmkgj.html

PHP:  public static function f() {}
来源：http://hz.zhixingplan.top/gtvdqqkhur.html

JS:   static f() {}
来源：http://hz.wangdashe.top/gtvwpucrwn.html

TS:   static f(): void {}
来源：http://hz.wangshuangyany.cn/gtvbugbgyt.html

Java: static void f() {}
来源：http://hz.jqgfzy.top/gtltdfyrxh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.haohaochexian.top/gtciqfighg.html

Ruby: def self.f; end
来源：http://hz.yuanzhike.top/gtscfoiguv.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangkeji.top/gtunhcyrol.html

[G09] 接口 / 抽象类
来源：http://hz.cashguo.top/gtqrdtngnb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.iojbl.cn/gtefkydhvy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pengpengdd.cyou/gtzjugcccm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sufxvd.cn/gtishifhka.html

TS:   interface Shape { area(): number; }
来源：http://hz.aibaodan.cn/gtdwoldxlu.html

Java: interface Shape { double area(); }
来源：http://hz.gaohongyu789.top/gtnhgtixiq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nanxuanxn.top/gtlypxnwob.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guannengcc.top/gtecrmnfxq.html

C#:   interface IShape { double Area(); }
来源：http://hz.hnqzz.top/gtaooytuff.html

[G10] 访问控制
来源：http://hz.xinyue.icu/gtvgtsjqmp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nanxuanxn.top/gtsudzykfe.html

PHP:  public / protected / private
来源：http://hz.ydjk.org.cn/gtmtypvgje.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtsyfdxtnh.html

TS:   public / protected / private
来源：http://hz.zhoulong.xyz/gtpvbmqczl.html

Java: public / protected / private / 默认包级
来源：http://hz.hywenlv.cn/gtmthyjynv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtqtrbhbcy.html

Ruby: public / protected / private
来源：http://hz.iojbl.cn/gtukrbvnyv.html

C#:   public / protected / private / internal
来源：http://hz.chenjidiqi.icu/gtqajgvspj.html

[G11] getter / setter
来源：http://hz.sufxvd.cn/gtwjisgylw.html

Py:   @property 与 @x.setter
来源：http://hz.haohaochexian.top/gtglbdvwsi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtgdhwxkle.html

JS:   get name() { return this._name; }
来源：http://hz.jiagoushi.top/gtcycubaap.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenjidiqi.icu/gtjwqktiwc.html

Java: public String getName() { return name; }
来源：http://hz.feifeiyinyue.top/gtmfvwixbb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtpzwmdcft.html

Ruby: attr_accessor :name
来源：http://hz.shzxlz.cn/gtixilekcu.html

C#:   public string Name { get; set; }
来源：http://hz.jyoumei.cn/gtmfafuqsf.html

[G12] 对象转字符串
来源：http://hz.feifeiyinyue.top/gttqwdcgdn.html

Py:   def __str__(self): return self.name
来源：http://hz.zycfv.cn/gtikqthuyz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtzrtdtmbp.html

JS:   toString() { return this.name; }
来源：http://hz.jqgufenzy.top/gtocekicxg.html

TS:   toString(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtpdlbzxtk.html

Java: @Override public String toString() { return name; }
来源：http://hz.cdnleiting.top/gtitoupnne.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cdnleiting.top/gtgzrkmjvr.html

Ruby: def to_s; @name; end
来源：http://hz.svipenyu.cn/gtdmyyzplr.html

C#:   public override string ToString() => Name;
来源：http://hz.shuidangran.top/gtcheasxyc.html

[G13] 判断对象类型
来源：http://hz.vqdsnc.cn/gteuxzyuon.html

Py:   isinstance(u, User)
来源：http://hz.hfpthk.cn/gtpevegwhk.html

PHP:  $u instanceof User
来源：http://hz.zhijiandao.cn/gtdrdxfgwt.html

JS:   u instanceof User
来源：http://hz.iojbl.cn/gtqzhkbuvo.html

TS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtikzpnzch.html

Java: u instanceof User
来源：http://hz.gotoacloud.top/gtaoyanjfw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigfzy.top/gtgfukbgot.html

Ruby: u.is_a?(User)
来源：http://hz.chenlongwang.top/gthrojgwhe.html

C#:   u is User
来源：http://hz.jinqigufen.top/gtdalosmpb.html

[G14] 数据类 / record
来源：http://hz.feifeiyinyue.top/gtmgvkohgw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ehwqpu.com/gtkcbflrkr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sxryk.cn/gtcbkzxtdt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258.top/gtrnufnejj.html

TS:   type User = { name: string; age: number };
来源：http://hz.cqqwz.cn/gtklncudtp.html

Java: record User(String name, int age) {}
来源：http://hz.feifeiyinyue.top/gttjiilrat.html

Go:   type User struct { Name string; Age int }
来源：http://hz.vqdsnc.cn/gtnyryfpyb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.316326.xyz/gtxyhkwlyc.html

C#:   record User(string Name, int Age);
来源：http://hz.zhengqikj.top/gtskjzhkxv.html

[G15] 枚举
来源：http://hz.fzhhl.top/gtnomdffgz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hywenlv.cn/gtlpgmggha.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.smart0.xyz/gttlusocij.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ywan-chungtsiang.top/gtyedhmcyz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtpclkdrio.html

Java: enum Color { RED, GREEN }
来源：http://hz.cqqwz.cn/gtqwyzkvjc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.dashuyun.cn/gteoncgvtp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hnqzz.top/gtgewvoige.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtkcbpwcop.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gttnhllbip.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.quarkkingdee.top/gtgudruhig.html

PHP:  get_object_vars($obj);
来源：http://hz.birdmap.top/gtbhjgwkoc.html

JS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtwgynuszi.html

TS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtjylyzzap.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhijiandao.cn/gtqwpnuktm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nanxinkj.top/gtyivbfsry.html

Ruby: obj.instance_variables
来源：http://hz.yj202588.top/gtejcnxqop.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sweek.top/gtxqyymopq.html

================================================================================
来源：http://hz.aizwys.cn/gtbszkftku.html

H. 异常与错误处理
来源：http://hz.jianghu66.top/gtvvoybprh.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtkfylscta.html

[H01] try / catch 基础
来源：http://hz.yongpay.top/gtawrhovuw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangkeji.top/gtyaiokryo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gogol.net.cn/gtlkbynanp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.pycfn.com/gtutztsnyi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cheryme.top/gtnjsgwbty.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhoulong.xyz/gtnboqogkm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.birdmap.top/gtyfctmdts.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.0kj1m.cn/gtzvgtfznx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhijiandao.cn/gtovbronsv.html

[H02] finally / ensure 收尾
来源：http://hz.shangyingyoupin.top/gtbdnwdmwj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.kuanghao11.cn/gtzebrogfh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtmonyjlqj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtrzfqsubs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtdogvreit.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtbbcrknha.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xylfe.cn/gtxsivajmq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhongyouzk.top/gtppxmxjnl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.feifeiyinyue.top/gtrdtcmqtp.html

[H03] 主动抛出异常
来源：http://hz.hfpthk.cn/gtyhjjyckl.html

Py:   raise ValueError("错误信息")
来源：http://hz.zdqjudy.top/gtuwrpftul.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtdhderzux.html

JS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtcyqyspwe.html

TS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtjijcsubn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtssfdylji.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dianchejie.cn/gtaulhmnha.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhongyouzk.top/gtzfhginlf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yvedp.cn/gtoklzuxzo.html

[H04] 自定义异常类型
来源：http://hz.yj202588.top/gtrgxyfodf.html

Py:   class MyError(Exception): pass
来源：http://hz.quarkkingdee.top/gtzzzqltrv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtcolqblpf.html

JS:   class MyError extends Error {}
来源：http://hz.aibaodan.cn/gtfpfdeiag.html

TS:   class MyError extends Error {}
来源：http://hz.shzxlz.cn/gtouwptytg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gthqxrfkib.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cucudq.cn/gtuzoqxbwc.html

Ruby: class MyError < StandardError; end
来源：http://hz.cashguo.top/gttbcmwylo.html

C#:   class MyException : Exception {}
来源：http://hz.jqgufenzy.top/gtszbxfwfq.html

[H05] 捕获特定类型
来源：http://hz.mhx1999.top/gtbornczwh.html

Py:   except ValueError as e:
来源：http://hz.smart0.xyz/gtfcfbcbil.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydzc1.top/gtpxpzvihl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.bjfxy.top/gtkezxdvav.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gtwpuirjto.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ehwqpu.com/gtouijezer.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigufen.top/gtzhhjrbet.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinqigufen.top/gtruqpxxnl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cdnleiting.top/gtjanqdggs.html

[H06] 可选值 / 空值安全访问
来源：http://hz.smart0.xyz/gtzjuddbwq.html

Py:   value = d.get("k") or default
来源：http://hz.jinqigufen.top/gtmrjwxiun.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gtmqzlskgz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gtnrzvxgfr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtakhrxrst.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yangfankeji.com/gtayzalivp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.havefunace.top/gtoylzqsqg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nanxuanxn.top/gtlwzrkvki.html

C#:   obj?.A?.B ?? default
来源：http://hz.svipenyu.cn/gtdacvjvlj.html

[H07] 断言
来源：http://hz.ydjk.org.cn/gttqcnlmto.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nwbrower.top/gtspigwyfn.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gtundhebvk.html

JS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtvxbojldv.html

TS:   console.assert(x > 0);
来源：http://hz.gotoacloud.top/gtetpyswus.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yonumen.top/gtmzakuykn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangkeji.top/gtxavimabf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xziqi.cn/gtxzsdvpzk.html


<!-- 参考信息 -->