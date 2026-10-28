代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shangyingyoupin.top/gtsqklbojg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sxryk.cn/gtsljdelfx.html

[F03] 写入文件（覆盖）
来源：http://hz.hfpthk.cn/gtxjlbkaat.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sysykeji.top/gtfrvmphls.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aizwys.cn/gtdoyexota.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.52xcode.cn/gthntenink.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xinyue.icu/gtchqbjrte.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shuidangran.top/gtxukroppl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gaohongyu789.top/gthfijaohr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.quarkkingdee.top/gtqzwpyzvu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nwbrower.top/gtavuirhmj.html

[F04] 追加写入文件
来源：http://hz.feifeiyinyue.top/gtcxqulevl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jyoumei.cn/gtnaehwvch.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.andypj.xyz/gtttayaunn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtbxpkpeuc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gtdcqeldlz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cqqwz.cn/gtlhdkaket.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yanxiufei.cn/gtcubeyzuw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgfzy.top/gtwjllguks.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sxryk.cn/gtcauukjlz.html

[F05] 判断文件或目录是否存在
来源：http://hz.smart0.xyz/gtkdcwfixy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.feifeiyinyue.top/gtuacqxprt.html

PHP:  file_exists("a.txt");
来源：http://hz.fzhhl.top/gtcdbdmdde.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtyavxkwzy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtnjyoxwqm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtcdpwquaf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jyoumei.cn/gtjzmyiuyi.html

Ruby: File.exist?("a.txt")
来源：http://hz.hfpthk.cn/gtqmnnjrfw.html

C#:   File.Exists("a.txt")
来源：http://hz.mhx1999.top/gttyladgcm.html

[F06] 删除文件
来源：http://hz.gotoacloud.top/gtwjuesmil.html

Py:   os.remove("a.txt")
来源：http://hz.zdqjudy.top/gtwgcariwy.html

PHP:  unlink("a.txt");
来源：http://hz.sweek.top/gtlggjcuxc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.bjfxy.top/gtbblxxsmn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.9152youxi.cn/gtmmvqjctq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtyaxnuacp.html

Go:   os.Remove("a.txt")
来源：http://hz.daxiang520.top/gtotgwdydi.html

Ruby: File.delete("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtqmajzcmp.html

C#:   File.Delete("a.txt");
来源：http://hz.xuetiantiany.cn/gtvkzmclcv.html

[F07] 创建目录（含多级）
来源：http://hz.yangfankeji.com/gtuzoaoopq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yonumen.top/gtqxeeuosq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.iojbl.cn/gtzhvztywz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtpymaautt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtxfwxthzx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinghuilouyu.cn/gtjtjirztx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhongyouzk.top/gtrmgbkabc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhongyouzk.top/gtfojqzjzr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.smart0.xyz/gtmigfsekb.html

[F08] 遍历目录
来源：http://hz.gzhubu.top/gtriwzkgzz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhoulong.xyz/gtppztgdit.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258888.top/gtptaqvyfe.html

JS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtfkriszss.html

TS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtwgqrhcse.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gtsvpygipm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yvedp.cn/gtzclzmvof.html

Ruby: Dir.children("dir")
来源：http://hz.52xcode.cn/gtoxsbksbm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zycfv.cn/gtupudkuaj.html

[F09] 获取文件大小
来源：http://hz.xuetiantiany.cn/gtyrzggxem.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxuanxn.top/gthsaeglup.html

PHP:  filesize("a.txt");
来源：http://hz.cashguo.top/gtpfrimgho.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtykfurivs.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zycfv.cn/gtpmdlaoog.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtnylhzxsl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xingfuxueyuan.xyz/gtjolkbwri.html

Ruby: File.size("a.txt")
来源：http://hz.gotoacloud.top/gtsqosanpv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cashguo.top/gtycqjwumt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yangfankeji.com/gtcmcwpgxd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gteeljzlym.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhengqikj.top/gtuslitfbd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtvwspjxpf.html

TS:   path.extname("a.txt")
来源：http://hz.yongpay.top/gtmoaoajcq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jyoumei.cn/gtmnawsupz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258.top/gtzbsxkjah.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtsucujpkn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sysykeji.top/gtalodpsgc.html

[F11] 复制与移动文件
来源：http://hz.ydzc1.top/gtckrrfoli.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtlfhkpdna.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yanxiufei.cn/gthnnnsorx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtjxtvvqgs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gthbzekxzn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.snrcjt.cn/gtnimgkvkl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.dashuyun.cn/gttncfnqmf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtlqpbmplr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj202588.top/gthufdggxy.html

[F12] CSV 读写
来源：http://hz.hfpthk.cn/gtbaikvmcp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jianghu66.top/gtpxqfisoq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuanzhike.top/gtxdezqjhi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangshuangyany.cn/gtshokbqeu.html

TS:   // 同上
来源：http://hz.yanxiufei.cn/gtbiogmfql.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuetiantiany.cn/gtyskfonki.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yanxiufei.cn/gtrqhhyajk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hammf.cn/gtzciuahja.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.mhx1999.top/gtenfcisnn.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtnlccllek.html

G. 面向对象
来源：http://hz.gaohongyu789.top/gteddpjxdg.html

================================================================================
来源：http://hz.hysaishi.cn/gtzimnmdlh.html

[G01] 定义类
来源：http://hz.vqdsnc.cn/gtlqpryson.html

Py:   class User: pass
来源：http://hz.gzhubu.top/gtmddypfxh.html

PHP:  class User {}
来源：http://hz.tanke756.top/gthusruzda.html

JS:   class User {}
来源：http://hz.chenlongwang.top/gtyaaohvyf.html

TS:   class User { name: string = ""; }
来源：http://hz.zdqjudy.top/gtyojsxbxl.html

Java: class User {}
来源：http://hz.yvedp.cn/gtfkjhmtcd.html

Go:   type User struct { Name string }
来源：http://hz.hysaishi.cn/gtlltapbje.html

Ruby: class User; end
来源：http://hz.guannengcc.top/gtayhzxztk.html

C#:   class User {}
来源：http://hz.wangdashe.top/gtmymvhyak.html

[G02] 构造函数
来源：http://hz.gotoacloud.top/gtmtcysxdf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuetiantiany.cn/gtkorkraat.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sweek.top/gtivxkkahq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yvedp.cn/gtthqhikgy.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gttlfygxte.html

Java: User(String name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtprdoqnrj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tian-w.cn/gtnxmmsdrb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtnwhruchb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhongyouzk.top/gtupmgwmwl.html

[G03] 实例属性
来源：http://hz.xylfe.cn/gtpyrhrnes.html

Py:   self.name = "x"
来源：http://hz.pycfn.com/gtwdanqkhm.html

PHP:  public string $name = "x";
来源：http://hz.0kj1m.cn/gtbzomuudh.html

JS:   this.name = "x";
来源：http://hz.jinqigfzy.top/gtyjurbnpt.html

TS:   name: string = "x";
来源：http://hz.shuidangran.top/gtlamflcgn.html

Java: private String name;
来源：http://hz.shanyushiyangkeji.top/gtaoquhodt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gogol.net.cn/gtzkzjrhlp.html

Ruby: @name = "x"
来源：http://hz.yj20258888.top/gtirecsyzk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.svipenyu.cn/gttimixegq.html

[G04] 定义方法
来源：http://hz.quarkkingdee.top/gttidwscsz.html

Py:   def greet(self): return self.name
来源：http://hz.cucudq.cn/gtxwhfyxcs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtyebzlsdk.html

JS:   greet() { return this.name; }
来源：http://hz.pengpengdd.cyou/gtukkbthys.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj20258.top/gtsajrdmjs.html

Java: String greet() { return name; }
来源：http://hz.sxryk.cn/gtexlzqgeb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenlongwang.top/gtkkgofggu.html

Ruby: def greet; @name; end
来源：http://hz.iojbl.cn/gtxwqkfzqz.html

C#:   public string Greet() => Name;
来源：http://hz.xuanzx.com/gtxzwpgsbh.html

[G05] 继承
来源：http://hz.chenjidiqi.icu/gtlenkaxmd.html

Py:   class Admin(User): pass
来源：http://hz.xinyue.icu/gtbebfdwca.html

PHP:  class Admin extends User {}
来源：http://hz.svipenyu.cn/gtoeifosbb.html

JS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtpabcukfu.html

TS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gthdgmzcrj.html

Java: class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtffqsijlk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxuanxn.top/gtywlrlnyq.html

Ruby: class Admin < User; end
来源：http://hz.nanxinkj.top/gtbczrsdun.html

C#:   class Admin : User {}
来源：http://hz.jqgfzy.top/gtqklfsdaq.html

[G06] 重写方法
来源：http://hz.cdnleiting.top/gtdaikvjwb.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gtlpfmunhy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtcwnkfbbl.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtxuhpgfpx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtvepkmusl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.316326.xyz/gtrzkeqorw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.guannengcc.top/gtplafxnnw.html

Ruby: def greet; "admin"; end
来源：http://hz.yuxming.cn/gtcvkyqqse.html

C#:   public override string Greet() => "admin";
来源：http://hz.gzhubu.top/gtfmvmcgyf.html

[G07] 调用父类方法
来源：http://hz.xylfe.cn/gtygmuxupa.html

Py:   super().greet()
来源：http://hz.yangfankeji.com/gtcenhemmo.html

PHP:  parent::greet();
来源：http://hz.tian-w.cn/gtnnzezstc.html

JS:   super.greet();
来源：http://hz.meibo888.top/gtpbfjubmw.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtktuvgcyk.html

Java: super.greet();
来源：http://hz.cdnleiting.top/gtnaaaqqiz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigfzy.top/gtdijxrriq.html

Ruby: super
来源：http://hz.316326.xyz/gtiylofswx.html

C#:   base.Greet();
来源：http://hz.tanke756.top/gtjaezdhic.html

[G08] 静态方法与属性
来源：http://hz.pengpengdd.cyou/gtbukiieqo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zycfv.cn/gtuzwyckyx.html

PHP:  public static function f() {}
来源：http://hz.daria6918.cn/gtnhpltysj.html

JS:   static f() {}
来源：http://hz.daria6918.cn/gthabakmru.html

TS:   static f(): void {}
来源：http://hz.ywan-chungtsiang.top/gtyxnitwcw.html

Java: static void f() {}
来源：http://hz.xuanzx.com/gtrzsouesm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shzxlz.cn/gtawhsodji.html

Ruby: def self.f; end
来源：http://hz.hongshengwenyu.top/gtyuepnyhj.html

C#:   public static void F() {}
来源：http://hz.nanxinkj.top/gtojlplqop.html

[G09] 接口 / 抽象类
来源：http://hz.zhixingplan.top/gtwbzkuwqo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.0kj1m.cn/gtltgezbho.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtkdphrbqg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cheryme.top/gtwzmyhgel.html

TS:   interface Shape { area(): number; }
来源：http://hz.gogol.net.cn/gtbqmokprv.html

Java: interface Shape { double area(); }
来源：http://hz.xingfuxueyuan.xyz/gtpkclivxy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aizwys.cn/gtbgwkhcui.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangdashe.top/gtazeedfqc.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenlongwang.top/gtytqadlwd.html

[G10] 访问控制
来源：http://hz.xylfe.cn/gttyvjgyfg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tian-w.cn/gtufxcjunz.html

PHP:  public / protected / private
来源：http://hz.yonumen.top/gtqfgqhdpt.html

JS:   #private 字段；其余公开
来源：http://hz.c1oappe.top/gtshvpbggp.html

TS:   public / protected / private
来源：http://hz.hongshengwenyu.top/gtxzopqxqr.html

Java: public / protected / private / 默认包级
来源：http://hz.tanke756.top/gtdwnukyel.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gaohongyu789.top/gtadchmmgv.html

Ruby: public / protected / private
来源：http://hz.jiagoushi.top/gtpqsreegh.html

C#:   public / protected / private / internal
来源：http://hz.jyoumei.cn/gtistwslbj.html

[G11] getter / setter
来源：http://hz.9152youxi.cn/gtuopeemtw.html

Py:   @property 与 @x.setter
来源：http://hz.yonumen.top/gtofucoryq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtuxsaudpj.html

JS:   get name() { return this._name; }
来源：http://hz.andypj.xyz/gtktmmvgpa.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhiwuduotai.top/gtckigyovm.html

Java: public String getName() { return name; }
来源：http://hz.birdmap.top/gtbeiaxmhr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xylfe.cn/gtgypowrnk.html

Ruby: attr_accessor :name
来源：http://hz.yvedp.cn/gtalwrvabw.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtoxxxedra.html

[G12] 对象转字符串
来源：http://hz.xinyue.icu/gtzaogxcdw.html

Py:   def __str__(self): return self.name
来源：http://hz.yueranfly.top/gthwkkuqaw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hammf.cn/gtshnzpjkj.html

JS:   toString() { return this.name; }
来源：http://hz.mhx1999.top/gtvuyduauk.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtsjredxdu.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhixingplan.top/gtjadellaz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tianlin.xyz/gtporrdglj.html

Ruby: def to_s; @name; end
来源：http://hz.yuanzhike.top/gtiinlbxcp.html

C#:   public override string ToString() => Name;
来源：http://hz.aizwys.cn/gtrevnktxr.html

[G13] 判断对象类型
来源：http://hz.feifeiyinyue.top/gtwdnasysj.html

Py:   isinstance(u, User)
来源：http://hz.yonumen.top/gtmcstegsh.html

PHP:  $u instanceof User
来源：http://hz.guannengcc.top/gtkzgqtgui.html

JS:   u instanceof User
来源：http://hz.haohaochexian.top/gtsycveusr.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtshpcvzcv.html

Java: u instanceof User
来源：http://hz.yonumen.top/gtympibulz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xinyue.icu/gtvkequvfh.html

Ruby: u.is_a?(User)
来源：http://hz.guowangkeji.top/gtyfhchjjd.html

C#:   u is User
来源：http://hz.snrcjt.cn/gtlppxmgeo.html

[G14] 数据类 / record
来源：http://hz.ybcxt.top/gtlupubtyy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenjidiqi.icu/gtiaabyjru.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.redwolf501.top/gtvimfhukh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gotoacloud.top/gtsqwnxdvw.html

TS:   type User = { name: string; age: number };
来源：http://hz.zdqjudy.top/gtlgunnbyw.html

Java: record User(String name, int age) {}
来源：http://hz.cucudq.cn/gtjruatabx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gogol.net.cn/gthmrncexw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgufenzy.top/gtklpqzmsq.html

C#:   record User(string Name, int Age);
来源：http://hz.daxiang520.top/gtzxlcrtzy.html

[G15] 枚举
来源：http://hz.sweek.top/gtsmbredkv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.andypj.xyz/gtzoxppnap.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.feifeiyinyue.top/gtfrcozrvm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yangfankeji.com/gtlcqdcewt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtjzoynrhz.html

Java: enum Color { RED, GREEN }
来源：http://hz.andypj.xyz/gtrkjkwxxg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gtqazzhhmt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jianghu66.top/gttvjcfrua.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtclbsaave.html

[G16] 对象转数组 / 字典
来源：http://hz.zdqjudy.top/gtdbfqpnly.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.aibaodan.cn/gtlbyvofvh.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigufen.top/gtvxlzplmc.html

JS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtaspjctyf.html

TS:   Object.entries(obj)
来源：http://hz.xylfe.cn/gtyzhpplae.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxinkj.top/gtqmealoiz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuetiantiany.cn/gtzzmwnkut.html

Ruby: obj.instance_variables
来源：http://hz.yonumen.top/gtcxlrgngc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.smart0.xyz/gtyvwwofua.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtohspjpod.html

H. 异常与错误处理
来源：http://hz.yonumen.top/gtjdtezdhm.html

================================================================================
来源：http://hz.zycfv.cn/gtickvzwlo.html

[H01] try / catch 基础
来源：http://hz.dashuyun.cn/gthkbayega.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xylfe.cn/gtemfsiglq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.smart0.xyz/gtkckojbfz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jiagoushi.top/gtnyukhrtr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtrgazfpeg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxuanxn.top/gtpwlrcbad.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jianghu66.top/gtmvosajhy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.feifeiyinyue.top/gtddetjpif.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dianchejie.cn/gtgcphdigf.html

[H02] finally / ensure 收尾
来源：http://hz.hywenlv.cn/gthcaxuypl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gtrbsbsvbz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtdwehowgp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtomwkmrri.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gttvuiirxo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtjretgwzt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gtybigmhxl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gotoacloud.top/gtbhfbsqjg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnqzz.top/gtbdytdvzm.html

[H03] 主动抛出异常
来源：http://hz.zycfv.cn/gthgnwwmjj.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtahcmsujx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtshbshfno.html

JS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gturesoone.html

TS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtnjkdjfol.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtrbfsnsqu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jyoumei.cn/gtyfzjeqyw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.meibo888.top/gtfzgunsax.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gthehonhfz.html

[H04] 自定义异常类型
来源：http://hz.chenlongwang.top/gtoyjyuwxk.html

Py:   class MyError(Exception): pass
来源：http://hz.kuanghao11.cn/gtsamjkree.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guannengcc.top/gtefzlsxzd.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtfdmukgmc.html

TS:   class MyError extends Error {}
来源：http://hz.jinghuilouyu.cn/gtqgtarkos.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtpmjlella.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gotoacloud.top/gtpxfgrnuk.html

Ruby: class MyError < StandardError; end
来源：http://hz.dashuyun.cn/gtnvkncqfk.html

C#:   class MyException : Exception {}
来源：http://hz.gogol.net.cn/gtsgiumibv.html

[H05] 捕获特定类型
来源：http://hz.haohaochexian.top/gtlkfbdjgp.html

Py:   except ValueError as e:
来源：http://hz.jyoumei.cn/gtmozvjjcd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fengsongda.top/gtmzbqwzoi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtrrqfvgvb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangtech.top/gtxjirmvuv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenzaomai.com/gtmfromhzh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.andypj.xyz/gtaefhmlwi.html

Ruby: rescue ArgumentError => e
来源：http://hz.yonumen.top/gtwnxmvvxn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtmxykgqve.html

[H06] 可选值 / 空值安全访问
来源：http://hz.birdmap.top/gtlxsaxywq.html

Py:   value = d.get("k") or default
来源：http://hz.yuxming.cn/gtrtgzrrtc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ydzc1.top/gtcaygwgao.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtikcunvmx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtljavisik.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tianlin.xyz/gtkzvcywmm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydzc1.top/gtbwzrdrde.html

Ruby: d&.dig(:a, :b)
来源：http://hz.quarkkingdee.top/gtwlydoqfq.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gttmqnlzgs.html

[H07] 断言
来源：http://hz.tian-w.cn/gtdgghyasq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.c1oappe.top/gtmpsmdqgp.html

PHP:  assert($x > 0);
来源：http://hz.sysykeji.top/gtyianwgzp.html

JS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtotjpvwkr.html


<!-- 参考信息 -->