代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yvedp.cn/gthcswadnh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aizwys.cn/gtmxjrycan.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gogol.net.cn/gteadqkfsa.html

[F04] 追加写入文件
来源：http://hz.daxiang520.top/gtdkpiigqg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hywenlv.cn/gteiaprsob.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.meibo888.top/gtqtdacoyq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenzaomai.com/gtfxupvysp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gtbwgdferm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.chenjidiqi.icu/gtoqewrkui.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hywenlv.cn/gtreqpcxim.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinqigufen.top/gtbvbiijex.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hammf.cn/gtuapzcqla.html

[F05] 判断文件或目录是否存在
来源：http://hz.kuanghao11.cn/gtjcevdikj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xylfe.cn/gtmmiekywf.html

PHP:  file_exists("a.txt");
来源：http://hz.guowangkeji.top/gtoknzmdbn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtuoyiokbm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtvqnidfht.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtcqcakwwk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.guannengcc.top/gtdcspintc.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenlongwang.top/gtrsrioppx.html

C#:   File.Exists("a.txt")
来源：http://hz.aibaodan.cn/gthssjokzr.html

[F06] 删除文件
来源：http://hz.redwolf501.top/gthmjfipqp.html

Py:   os.remove("a.txt")
来源：http://hz.xuetiantiany.cn/gtychesxsk.html

PHP:  unlink("a.txt");
来源：http://hz.jinghuilouyu.cn/gtbtbcgfsa.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtdujbxfpw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtijbqjkpe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtnhxysdip.html

Go:   os.Remove("a.txt")
来源：http://hz.svipenyu.cn/gtwjycdrxy.html

Ruby: File.delete("a.txt")
来源：http://hz.tianlin.xyz/gtqokhtvtn.html

C#:   File.Delete("a.txt");
来源：http://hz.pengpengdd.cyou/gtptmjyklq.html

[F07] 创建目录（含多级）
来源：http://hz.iojbl.cn/gtozauebje.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhengqikj.top/gtcweukyjg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sxryk.cn/gtpetbsuni.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gtfcbrgfqg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.meibo888.top/gtwktuayxd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yongpay.top/gtxwipbeyi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cheryme.top/gtfwwckwlu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinqigfzy.top/gtokmgufrk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yanxiufei.cn/gtjnihmaoe.html

[F08] 遍历目录
来源：http://hz.daxiang520.top/gtwifmipwv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gtzbtqdfde.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hammf.cn/gtvfqqrifw.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigfzy.top/gteivbelfy.html

TS:   fs.readdirSync("dir")
来源：http://hz.jiagoushi.top/gtzokarrze.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zycfv.cn/gttfcswolo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hysaishi.cn/gtilsgchrs.html

Ruby: Dir.children("dir")
来源：http://hz.cucudq.cn/gtxykxzjcm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hongshengwenyu.top/gtxkafqhdh.html

[F09] 获取文件大小
来源：http://hz.zycfv.cn/gtvrfmzoms.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gotoacloud.top/gtwhcsydxa.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtbpinuuiu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtvcntibnc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtlsarjmze.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtylzkpnzt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yuxming.cn/gtimjifnte.html

Ruby: File.size("a.txt")
来源：http://hz.chenjidiqi.icu/gtdlvnxbix.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtiffjrfwp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.kuanghao11.cn/gthxdwtwgv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtgkittinq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gzhubu.top/gtfhhimwoi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtpkugqnkn.html

TS:   path.extname("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtzyxsddfb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenjidiqi.icu/gtwprutylw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tanke756.top/gtmeklsykk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtphzrvwwa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daria6918.cn/gtdgodhgpl.html

[F11] 复制与移动文件
来源：http://hz.cdnleiting.top/gtkphtjbgn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtxfwfhfbk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinghuilouyu.cn/gtemttiaea.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtpvhxfspr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtiiviyhda.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yj202588.top/gtslmogwcz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.kuanghao11.cn/gtzfseuvsx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtgwehxxrq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cashguo.top/gtponjcalg.html

[F12] CSV 读写
来源：http://hz.hfpthk.cn/gthnwwdqyr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shuidangran.top/gtojxjegxn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxinkj.top/gtpmqzopac.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.guowangkeji.top/gtbdyspxfy.html

TS:   // 同上
来源：http://hz.guowangkeji.top/gtcvqnwhxa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shanyushiyangtech.top/gttxspepnt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangtech.top/gtfldekqhq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yangfankeji.com/gtsnvivvoz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xingfuxueyuan.xyz/gtdhwfrvfq.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtjkjzupte.html

G. 面向对象
来源：http://hz.tian-w.cn/gtrugaoshh.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtfcbqumlr.html

[G01] 定义类
来源：http://hz.feifeiyinyue.top/gtsikxsvof.html

Py:   class User: pass
来源：http://hz.bjfxy.top/gtkbvzrqxb.html

PHP:  class User {}
来源：http://hz.nanxinkj.top/gtthnaunxl.html

JS:   class User {}
来源：http://hz.mhx1999.top/gtplgxbjrz.html

TS:   class User { name: string = ""; }
来源：http://hz.dashuyun.cn/gttrlvuiww.html

Java: class User {}
来源：http://hz.hammf.cn/gtxboakhsu.html

Go:   type User struct { Name string }
来源：http://hz.hnqzz.top/gtgwosyywv.html

Ruby: class User; end
来源：http://hz.fengsongda.top/gtepqksepb.html

C#:   class User {}
来源：http://hz.bjfxy.top/gtdjnwmmbm.html

[G02] 构造函数
来源：http://hz.jyoumei.cn/gtestthasv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ehwqpu.com/gtvajarpzt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinqigfzy.top/gtvfqwfnch.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yonumen.top/gtmxsncrza.html

TS:   constructor(public name: string) {}
来源：http://hz.chenzaomai.com/gttlhphfce.html

Java: User(String name) { this.name = name; }
来源：http://hz.gotoacloud.top/gtcefnbgaq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cucudq.cn/gtjzrkwnlw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.0kj1m.cn/gtptcmztng.html

C#:   public User(string name) { Name = name; }
来源：http://hz.iojbl.cn/gtdqeagswu.html

[G03] 实例属性
来源：http://hz.316326.xyz/gtzvlzvswk.html

Py:   self.name = "x"
来源：http://hz.bjfxy.top/gttcwxovnr.html

PHP:  public string $name = "x";
来源：http://hz.redwolf501.top/gthcaopxxw.html

JS:   this.name = "x";
来源：http://hz.chenzaomai.com/gtqkfhtsjc.html

TS:   name: string = "x";
来源：http://hz.nwbrower.top/gtwwjraaow.html

Java: private String name;
来源：http://hz.fengsongda.top/gturzclkkl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxinkj.top/gtxpuoeipk.html

Ruby: @name = "x"
来源：http://hz.gzhubu.top/gtdovgvjpe.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guannengcc.top/gtdldgnwcd.html

[G04] 定义方法
来源：http://hz.yonumen.top/gtxkkrqwne.html

Py:   def greet(self): return self.name
来源：http://hz.guannengcc.top/gtnqmslfhb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtnjnzxysw.html

JS:   greet() { return this.name; }
来源：http://hz.nanxinkj.top/gtvcoxcvgd.html

TS:   greet(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gtmxpvkymb.html

Java: String greet() { return name; }
来源：http://hz.yj202588.top/gtustgfuyg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fzhhl.top/gtjrgbkcmp.html

Ruby: def greet; @name; end
来源：http://hz.tianlin.xyz/gtjjzcbcwl.html

C#:   public string Greet() => Name;
来源：http://hz.hywenlv.cn/gtdhwldhqx.html

[G05] 继承
来源：http://hz.chenlongwang.top/gtqvojqnvi.html

Py:   class Admin(User): pass
来源：http://hz.xingfuxueyuan.xyz/gtpxmgdmno.html

PHP:  class Admin extends User {}
来源：http://hz.xinyue.icu/gtsdjhggma.html

JS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtehaqjoyl.html

TS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtrhhupter.html

Java: class Admin extends User {}
来源：http://hz.shzxlz.cn/gtzeamewkj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.kuanghao11.cn/gtttydlsir.html

Ruby: class Admin < User; end
来源：http://hz.ppjwa.cn/gtcbhkyuwd.html

C#:   class Admin : User {}
来源：http://hz.zdqjudy.top/gtqkrbankx.html

[G06] 重写方法
来源：http://hz.hysaishi.cn/gtqkpjfjlg.html

Py:   def greet(self): return "admin"
来源：http://hz.hywenlv.cn/gtzfonurwb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtinpstsqz.html

JS:   greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtwemcfgte.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gtldqqajyb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gteqzmblkr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hysaishi.cn/gtnlvkoryi.html

Ruby: def greet; "admin"; end
来源：http://hz.cucudq.cn/gtsrukrpqr.html

C#:   public override string Greet() => "admin";
来源：http://hz.shuidangran.top/gtpixpmoci.html

[G07] 调用父类方法
来源：http://hz.daria6918.cn/gttwycjdln.html

Py:   super().greet()
来源：http://hz.yj202588.top/gtijeieswi.html

PHP:  parent::greet();
来源：http://hz.yj20258888.top/gtucnylydh.html

JS:   super.greet();
来源：http://hz.yvedp.cn/gtktamstey.html

TS:   super.greet();
来源：http://hz.nanxinkj.top/gttstbikys.html

Java: super.greet();
来源：http://hz.zhaomingkeji.xyz/gthdvsvtju.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yongpay.top/gtubdcepxe.html

Ruby: super
来源：http://hz.yvedp.cn/gtribaywkv.html

C#:   base.Greet();
来源：http://hz.zhoulong.xyz/gtyjpetmpf.html

[G08] 静态方法与属性
来源：http://hz.quarkkingdee.top/gterkrnutp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuetiantiany.cn/gtbelhvnws.html

PHP:  public static function f() {}
来源：http://hz.haohaochexian.top/gtrdqvkkwj.html

JS:   static f() {}
来源：http://hz.yj20258.top/gtmjcswffv.html

TS:   static f(): void {}
来源：http://hz.gzhubu.top/gtmjzabigf.html

Java: static void f() {}
来源：http://hz.hongshengwenyu.top/gtsvdphxcs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.9152youxi.cn/gtnvhpmvhw.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gteopmuvyw.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtjirvxgaq.html

[G09] 接口 / 抽象类
来源：http://hz.yongpay.top/gtobfqnupk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhongyouzk.top/gthzvcmrlm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhiwuduotai.top/gtdsqhenyj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aizwys.cn/gtfovmxiqf.html

TS:   interface Shape { area(): number; }
来源：http://hz.sysykeji.top/gtqlxkxrrh.html

Java: interface Shape { double area(); }
来源：http://hz.nwbrower.top/gttojzwdbx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xinyue.icu/gtvalkxonx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hfpthk.cn/gtnfysnyiv.html

C#:   interface IShape { double Area(); }
来源：http://hz.gaohongyu789.top/gtmweijzcs.html

[G10] 访问控制
来源：http://hz.jinqigufen.top/gtjfeekbig.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj202588.top/gtxrrwzfgj.html

PHP:  public / protected / private
来源：http://hz.gotoacloud.top/gtzrupcshl.html

JS:   #private 字段；其余公开
来源：http://hz.ehwqpu.com/gthdfribii.html

TS:   public / protected / private
来源：http://hz.haohaochexian.top/gtyggfqrtn.html

Java: public / protected / private / 默认包级
来源：http://hz.zhixingplan.top/gtkgnvbssk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangdashe.top/gtfeexizgw.html

Ruby: public / protected / private
来源：http://hz.yangfankeji.com/gtfqgwrjlz.html

C#:   public / protected / private / internal
来源：http://hz.wangdashe.top/gtzrwcixgo.html

[G11] getter / setter
来源：http://hz.tanke756.top/gtzqbbsfap.html

Py:   @property 与 @x.setter
来源：http://hz.quarkkingdee.top/gtplurwydo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtwvxexeov.html

JS:   get name() { return this._name; }
来源：http://hz.vqdsnc.cn/gttnwwuvax.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhijiandao.cn/gtxzuxsgxe.html

Java: public String getName() { return name; }
来源：http://hz.yanxiufei.cn/gtaghqnksz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yueranfly.top/gtkhddjgwu.html

Ruby: attr_accessor :name
来源：http://hz.iojbl.cn/gtcljrmbhm.html

C#:   public string Name { get; set; }
来源：http://hz.hysaishi.cn/gtgvdtktpc.html

[G12] 对象转字符串
来源：http://hz.shangyingyoupin.top/gtgwkyikhd.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangtech.top/gtiicsgafd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtjjlwlzxy.html

JS:   toString() { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gteudbrotp.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtvtisdgyi.html

Java: @Override public String toString() { return name; }
来源：http://hz.snrcjt.cn/gthjmeugri.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.c1oappe.top/gtydvbnjpl.html

Ruby: def to_s; @name; end
来源：http://hz.yj202588.top/gtpolrxrca.html

C#:   public override string ToString() => Name;
来源：http://hz.9152youxi.cn/gtqlxcucnb.html

[G13] 判断对象类型
来源：http://hz.hnxiangtu.top/gtfzwucokq.html

Py:   isinstance(u, User)
来源：http://hz.aizwys.cn/gtbwavokme.html

PHP:  $u instanceof User
来源：http://hz.pengpengdd.cyou/gtdzcgbztq.html

JS:   u instanceof User
来源：http://hz.jqgfzy.top/gtyuovrndr.html

TS:   u instanceof User
来源：http://hz.sufxvd.cn/gtdtlkjngi.html

Java: u instanceof User
来源：http://hz.52xcode.cn/gtynncqpdx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ppjwa.cn/gtipofchic.html

Ruby: u.is_a?(User)
来源：http://hz.birdmap.top/gtyokwsjsb.html

C#:   u is User
来源：http://hz.sysykeji.top/gtfzyekble.html

[G14] 数据类 / record
来源：http://hz.aibaodan.cn/gtnnoidktx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhijiandao.cn/gtrbwxukov.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj20258.top/gttrldeeqn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.smart0.xyz/gtqufidemq.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenjidiqi.icu/gtevxsfwzw.html

Java: record User(String name, int age) {}
来源：http://hz.hammf.cn/gtdpwhrkre.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ehwqpu.com/gtkqhfemal.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sufxvd.cn/gtadovqdru.html

C#:   record User(string Name, int Age);
来源：http://hz.xingfuxueyuan.xyz/gtspybuibo.html

[G15] 枚举
来源：http://hz.wangshuangyany.cn/gtakgwkymm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangtech.top/gtxiqfgbol.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gtjwesmvrk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhaomingkeji.xyz/gtdzryzxtk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtkkfncxvo.html

Java: enum Color { RED, GREEN }
来源：http://hz.ywan-chungtsiang.top/gtqhrgetzq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hongshengwenyu.top/gttiojaysk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.smart0.xyz/gttrbqxuws.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangtech.top/gtmybahyhi.html

[G16] 对象转数组 / 字典
来源：http://hz.yuxming.cn/gtjvxhgyqu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.redwolf501.top/gtslizvehm.html

PHP:  get_object_vars($obj);
来源：http://hz.hywenlv.cn/gtzaxmdxpz.html

JS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtpxsixgwh.html

TS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtkxjxvgpu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pengpengdd.cyou/gtncppaaqg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xziqi.cn/gtfkcxcnes.html

Ruby: obj.instance_variables
来源：http://hz.zhengqikj.top/gtuatgnuig.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gotoacloud.top/gtpskabqnh.html

================================================================================
来源：http://hz.guannengcc.top/gtlmrykenl.html

H. 异常与错误处理
来源：http://hz.zdqjudy.top/gtpdnmqoef.html

================================================================================
来源：http://hz.zhengqikj.top/gtfyczbqwh.html

[H01] try / catch 基础
来源：http://hz.zhoulong.xyz/gtrxbbjfui.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydzc1.top/gtvkdohyjv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cheryme.top/gtdsmfyari.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.andypj.xyz/gtmuaaltmv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dashuyun.cn/gtcllllbtd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.snrcjt.cn/gtqbjduuca.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhijiandao.cn/gtajrvhkpb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhixingplan.top/gtnlahowfo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dashuyun.cn/gthbuchpjm.html

[H02] finally / ensure 收尾
来源：http://hz.chenzaomai.com/gtqwbudvoq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aizwys.cn/gttifpojmm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gthqmxqmlu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtrnhsboxx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtivovnldh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtfylvobhb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daxiang520.top/gtsuntqeuq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yangfankeji.com/gtrfynenkt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xziqi.cn/gtzkxpjydo.html

[H03] 主动抛出异常
来源：http://hz.hywenlv.cn/gtpohfmdkc.html

Py:   raise ValueError("错误信息")
来源：http://hz.aizwys.cn/gtpilqlwph.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gthbaawzyu.html

JS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtgcmrkpyh.html

TS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gtsqnjbnjd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sweek.top/gtqvxuhhrf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zdqjudy.top/gtkccxjhkq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cdnleiting.top/gtqcvwtwyk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtbavaegge.html

[H04] 自定义异常类型
来源：http://hz.nanxinkj.top/gtkegiyrxt.html

Py:   class MyError(Exception): pass
来源：http://hz.cashguo.top/gttgzyqtms.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuxming.cn/gtkhkebowv.html

JS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtohsaocox.html

TS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtxbqxtcar.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ybcxt.top/gtaygtvobq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgfzy.top/gtxxtrtdct.html

Ruby: class MyError < StandardError; end
来源：http://hz.cashguo.top/gtwjrbymuy.html

C#:   class MyException : Exception {}
来源：http://hz.yangfankeji.com/gtniivvojc.html

[H05] 捕获特定类型
来源：http://hz.xinyue.icu/gtgbhjbjlx.html

Py:   except ValueError as e:
来源：http://hz.nanxinkj.top/gtjvjqsnyr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jyoumei.cn/gtciuchvln.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtpyjuncle.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtqpsdzyod.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ydzc1.top/gtplflzzra.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuetiantiany.cn/gtpazzyhtn.html

Ruby: rescue ArgumentError => e
来源：http://hz.havefunace.top/gtxsmsgzjs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shuidangran.top/gtiwgmsiva.html

[H06] 可选值 / 空值安全访问
来源：http://hz.svipenyu.cn/gtvccylyqc.html

Py:   value = d.get("k") or default
来源：http://hz.yuanzhike.top/gtmupafagz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jlsjyb.cn/gtabndsdfh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.52xcode.cn/gtcruarwno.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtdiffqbwk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daxiang520.top/gtzmjjqfaw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.birdmap.top/gtoddzxsam.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cqqwz.cn/gtpcizeopu.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtsvxfbkbu.html

[H07] 断言
来源：http://hz.shangyingyoupin.top/gtjsmlsvtc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fzhhl.top/gtlvngbsjf.html

PHP:  assert($x > 0);
来源：http://hz.hfpthk.cn/gtsiuwsnht.html

JS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gtogotrqqx.html

TS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtjnayhjdm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.0kj1m.cn/gtdjbpbghu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.0kj1m.cn/gtepteahei.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zdqjudy.top/gthawaflho.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cqqwz.cn/gtlrqvmzgx.html

[H08] 获取错误信息与堆栈
来源：http://hz.vqdsnc.cn/gtscmfmmqx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.52xcode.cn/gtdsashkfo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.andypj.xyz/gtgcbvrzvh.html


<!-- 参考信息 -->