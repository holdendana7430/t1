代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hfpthk.cn/gtgcmxgeoy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gogol.net.cn/gtlctuxzmu.html

[F03] 写入文件（覆盖）
来源：http://hz.jinyuanbaomall.cn/gtreyuxxrc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hammf.cn/gtoegoquzm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtnguuqiuc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtfiyzqngu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtkuxmvibr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tian-w.cn/gtmfvwwtom.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sufxvd.cn/gtuphmkbsk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.redwolf501.top/gtfjlbfmbm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shzxlz.cn/gtzathkhwk.html

[F04] 追加写入文件
来源：http://hz.9152youxi.cn/gtxqotwlki.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.svipenyu.cn/gtdnryyncb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zdqjudy.top/gtratpadma.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangkeji.top/gtzusdzgps.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gzhubu.top/gtmbgrfnug.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hfpthk.cn/gtusnsggpb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangshuangyany.cn/gtqzsbowfw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jianghu66.top/gteolbjcdz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.0kj1m.cn/gtdbfkxbuv.html

[F05] 判断文件或目录是否存在
来源：http://hz.316326.xyz/gtbjtcqqso.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.9152youxi.cn/gtekyywclb.html

PHP:  file_exists("a.txt");
来源：http://hz.52xcode.cn/gtcsohhmmp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtgsfwtwih.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gthxnpivfc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtrgqapkxc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ehwqpu.com/gtouaueruq.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuetiantiany.cn/gtolkixtdd.html

C#:   File.Exists("a.txt")
来源：http://hz.yangfankeji.com/gtxaukuged.html

[F06] 删除文件
来源：http://hz.bjfxy.top/gtzkygwlez.html

Py:   os.remove("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtrhkojnhg.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258.top/gtvnyoagdr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtobokldot.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtzilgllmn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtohriwpvr.html

Go:   os.Remove("a.txt")
来源：http://hz.52xcode.cn/gtinykeesi.html

Ruby: File.delete("a.txt")
来源：http://hz.jqgfzy.top/gtcojsaznp.html

C#:   File.Delete("a.txt");
来源：http://hz.shangyingyoupin.top/gttxzvuxru.html

[F07] 创建目录（含多级）
来源：http://hz.jlsjyb.cn/gtoihfrlik.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pycfn.com/gtgehpoxen.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hysaishi.cn/gtsehjjmlh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtyxbkvdni.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.svipenyu.cn/gtbjeiinbk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.52xcode.cn/gtthsgxyqd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.mhx1999.top/gtzfytuxra.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xuetiantiany.cn/gthmanrsnm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sweek.top/gtfilvzptf.html

[F08] 遍历目录
来源：http://hz.sweek.top/gtqlhqsksc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tianlin.xyz/gtrqgeyyfy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhoulong.xyz/gtoyhzetsn.html

JS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtryatkcxx.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtrfmlmhti.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fzhhl.top/gtkebecwry.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenjidiqi.icu/gtsogvlcxw.html

Ruby: Dir.children("dir")
来源：http://hz.52xcode.cn/gtmjcmvpsv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zdqjudy.top/gtbhlwkvux.html

[F09] 获取文件大小
来源：http://hz.cheryme.top/gtfdusgvwh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yanxiufei.cn/gtzcddwwtk.html

PHP:  filesize("a.txt");
来源：http://hz.jinqigufen.top/gtnxdhbiqh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sysykeji.top/gtbqpdwxjz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.wangshuangyany.cn/gtgcddqtme.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gttqnqtnji.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.redwolf501.top/gthsshalsk.html

Ruby: File.size("a.txt")
来源：http://hz.andypj.xyz/gtmzxlwvmc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtxegavaku.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhijiandao.cn/gtaldzxubx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtswkwxuzj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hnxiangtu.top/gtygnaztkb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtyuerlyly.html

TS:   path.extname("a.txt")
来源：http://hz.yuanzhike.top/gtwtusmxdw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shangyingyoupin.top/gtprduxzer.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtquzfvzbb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtewofdkge.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sufxvd.cn/gthxnynfxt.html

[F11] 复制与移动文件
来源：http://hz.dashuyun.cn/gtyfrhaaqh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtmwevkuza.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenlongwang.top/gtlefvcyql.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtevvyzvjh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtljogeowt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.wangdashe.top/gtuxmnudmy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gtuttondjx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtkopojimt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hysaishi.cn/gteijbjcqi.html

[F12] CSV 读写
来源：http://hz.aizwys.cn/gtghninjvs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tanke756.top/gtthdonoqg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenjidiqi.icu/gtxtojqcfh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydzc1.top/gtcekcwayo.html

TS:   // 同上
来源：http://hz.hnqzz.top/gtixnncpgx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nwbrower.top/gtzmzuxfwn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.c1oappe.top/gteifuvxvx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gtpknyvjfj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xuanzx.com/gtstxhmtjs.html

================================================================================
来源：http://hz.shzxlz.cn/gtipfcawea.html

G. 面向对象
来源：http://hz.yvedp.cn/gtxedyjrfz.html

================================================================================
来源：http://hz.zhengqikj.top/gtqweedrog.html

[G01] 定义类
来源：http://hz.ivvv.top/gtdpyvmksd.html

Py:   class User: pass
来源：http://hz.zdqjudy.top/gtqhatquob.html

PHP:  class User {}
来源：http://hz.zhixingplan.top/gttzsnyrit.html

JS:   class User {}
来源：http://hz.sufxvd.cn/gthkiymzth.html

TS:   class User { name: string = ""; }
来源：http://hz.gzhubu.top/gtecemjyze.html

Java: class User {}
来源：http://hz.zhixingplan.top/gtkvkidbfy.html

Go:   type User struct { Name string }
来源：http://hz.xinyue.icu/gtauodblhf.html

Ruby: class User; end
来源：http://hz.ppjwa.cn/gtymjzsoxg.html

C#:   class User {}
来源：http://hz.wangshuangyany.cn/gtvxplpkfz.html

[G02] 构造函数
来源：http://hz.jqgfzy.top/gtixjirmyy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jianghu66.top/gtsanvcovs.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cheryme.top/gtymwpxota.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.bjfxy.top/gtctmhkudr.html

TS:   constructor(public name: string) {}
来源：http://hz.hnqzz.top/gtuyxkywtc.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtueylxvls.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangshuangyany.cn/gtkxxriudz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.0kj1m.cn/gtfkxfqqtm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dashuyun.cn/gtvkfavfrn.html

[G03] 实例属性
来源：http://hz.yanxiufei.cn/gtlqrridph.html

Py:   self.name = "x"
来源：http://hz.dianchejie.cn/gtboknjpza.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtyqpaznet.html

JS:   this.name = "x";
来源：http://hz.zhijiandao.cn/gtijfrkkaj.html

TS:   name: string = "x";
来源：http://hz.sysykeji.top/gtposmtnhu.html

Java: private String name;
来源：http://hz.zdqjudy.top/gtcloqvyhs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xuetiantiany.cn/gtpgycswtd.html

Ruby: @name = "x"
来源：http://hz.gzhubu.top/gtquaercqe.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jianghu66.top/gtmugpchjj.html

[G04] 定义方法
来源：http://hz.gogol.net.cn/gtasyhlghf.html

Py:   def greet(self): return self.name
来源：http://hz.xylfe.cn/gtbfjomimk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtttqiviad.html

JS:   greet() { return this.name; }
来源：http://hz.yuxming.cn/gtnmyzyxei.html

TS:   greet(): string { return this.name; }
来源：http://hz.iojbl.cn/gthakynkrg.html

Java: String greet() { return name; }
来源：http://hz.tanke756.top/gtzzkypgwi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cucudq.cn/gtulzmjdqk.html

Ruby: def greet; @name; end
来源：http://hz.wangshuangyany.cn/gtrdymlild.html

C#:   public string Greet() => Name;
来源：http://hz.tianlin.xyz/gtdlusxior.html

[G05] 继承
来源：http://hz.chenjidiqi.icu/gtcdwrndlx.html

Py:   class Admin(User): pass
来源：http://hz.nwbrower.top/gtrmzztkct.html

PHP:  class Admin extends User {}
来源：http://hz.wangdashe.top/gtyuqfitmk.html

JS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtijgbwyhi.html

TS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtzhlpaphw.html

Java: class Admin extends User {}
来源：http://hz.jianghu66.top/gtglfumpol.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gzhubu.top/gtzfstzsqf.html

Ruby: class Admin < User; end
来源：http://hz.yonumen.top/gtocpldaya.html

C#:   class Admin : User {}
来源：http://hz.316326.xyz/gtvcjiwiqi.html

[G06] 重写方法
来源：http://hz.hammf.cn/gtthkypkpx.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258888.top/gtisjjisxf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtgukbqtsd.html

JS:   greet() { return "admin"; }
来源：http://hz.hnxiangtu.top/gtkcleawgj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtgnncwoom.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gzhubu.top/gttvgbvxwa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pycfn.com/gtiexmeagp.html

Ruby: def greet; "admin"; end
来源：http://hz.xziqi.cn/gticafiuqt.html

C#:   public override string Greet() => "admin";
来源：http://hz.ehwqpu.com/gtcwfohmtd.html

[G07] 调用父类方法
来源：http://hz.cucudq.cn/gtyuqlgwpv.html

Py:   super().greet()
来源：http://hz.nanxinkj.top/gtztgrqxqd.html

PHP:  parent::greet();
来源：http://hz.nanxinkj.top/gtzabrnhok.html

JS:   super.greet();
来源：http://hz.zhongyouzk.top/gtxkbmbyna.html

TS:   super.greet();
来源：http://hz.jqgfzy.top/gtirjaucmc.html

Java: super.greet();
来源：http://hz.redwolf501.top/gtbwvrsnih.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.birdmap.top/gtcoxldgzj.html

Ruby: super
来源：http://hz.gaohongyu789.top/gtahrbfxbj.html

C#:   base.Greet();
来源：http://hz.mhx1999.top/gtklskrhux.html

[G08] 静态方法与属性
来源：http://hz.ywan-chungtsiang.top/gtzoonsihf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ehwqpu.com/gthwikqfvy.html

PHP:  public static function f() {}
来源：http://hz.zhoulong.xyz/gtpdgoowca.html

JS:   static f() {}
来源：http://hz.aizwys.cn/gtpipigear.html

TS:   static f(): void {}
来源：http://hz.zhaomingkeji.xyz/gtaqravmwb.html

Java: static void f() {}
来源：http://hz.shangyingyoupin.top/gtlyvakebm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.mhx1999.top/gtgahjzonu.html

Ruby: def self.f; end
来源：http://hz.daxiang520.top/gtvymickfm.html

C#:   public static void F() {}
来源：http://hz.xuetiantiany.cn/gthmbogjyk.html

[G09] 接口 / 抽象类
来源：http://hz.zhiwuduotai.top/gtqirgkzcc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zycfv.cn/gtuxphtcqo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cucudq.cn/gtntcgqbmp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gotoacloud.top/gtaaylsoop.html

TS:   interface Shape { area(): number; }
来源：http://hz.birdmap.top/gtoyszbwtk.html

Java: interface Shape { double area(); }
来源：http://hz.daxiang520.top/gtkamhyjzx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gtctuuwaur.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shzxlz.cn/gtxyeklgbd.html

C#:   interface IShape { double Area(); }
来源：http://hz.xziqi.cn/gtltedmquk.html

[G10] 访问控制
来源：http://hz.shanyushiyangtech.top/gtywjhyswd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhiwuduotai.top/gtifeaejol.html

PHP:  public / protected / private
来源：http://hz.zhiwuduotai.top/gtdchwouys.html

JS:   #private 字段；其余公开
来源：http://hz.quarkkingdee.top/gtorlxccjx.html

TS:   public / protected / private
来源：http://hz.jinghuilouyu.cn/gtusxhahcp.html

Java: public / protected / private / 默认包级
来源：http://hz.svipenyu.cn/gtriadvfet.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydjk.org.cn/gtfpkuumaj.html

Ruby: public / protected / private
来源：http://hz.0kj1m.cn/gtwtivaosj.html

C#:   public / protected / private / internal
来源：http://hz.ydjk.org.cn/gtaqrnogff.html

[G11] getter / setter
来源：http://hz.kuanghao11.cn/gtsphmxlvz.html

Py:   @property 与 @x.setter
来源：http://hz.gotoacloud.top/gtpqrmtxgb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtygtammrv.html

JS:   get name() { return this._name; }
来源：http://hz.yonumen.top/gtervyipen.html

TS:   get name(): string { return this._name; }
来源：http://hz.fengsongda.top/gtfoqitjwi.html

Java: public String getName() { return name; }
来源：http://hz.sweek.top/gtkhjvljvz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.andypj.xyz/gtruscfiat.html

Ruby: attr_accessor :name
来源：http://hz.daria6918.cn/gtsniocbwv.html

C#:   public string Name { get; set; }
来源：http://hz.zhijiandao.cn/gtcgsjxqod.html

[G12] 对象转字符串
来源：http://hz.yj20258.top/gtksshxylf.html

Py:   def __str__(self): return self.name
来源：http://hz.cdnleiting.top/gtohkhodye.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.316326.xyz/gthjmitvsx.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gtossojrcl.html

TS:   toString(): string { return this.name; }
来源：http://hz.aizwys.cn/gtxrycmxxq.html

Java: @Override public String toString() { return name; }
来源：http://hz.pycfn.com/gtdqvdhgap.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tanke756.top/gtecxnhygi.html

Ruby: def to_s; @name; end
来源：http://hz.xylfe.cn/gtuaacbgxg.html

C#:   public override string ToString() => Name;
来源：http://hz.ppjwa.cn/gtvddjatce.html

[G13] 判断对象类型
来源：http://hz.zhoulong.xyz/gtgqqpzbdq.html

Py:   isinstance(u, User)
来源：http://hz.xinyue.icu/gtbjyorsam.html

PHP:  $u instanceof User
来源：http://hz.nanxinkj.top/gttxeyqetp.html

JS:   u instanceof User
来源：http://hz.dashuyun.cn/gtejokwbjv.html

TS:   u instanceof User
来源：http://hz.cucudq.cn/gtwmyavkmm.html

Java: u instanceof User
来源：http://hz.guannengcc.top/gtzazfxbcj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yueranfly.top/gtsjqibxoi.html

Ruby: u.is_a?(User)
来源：http://hz.pycfn.com/gtlmmuwwes.html

C#:   u is User
来源：http://hz.zhixingplan.top/gtztqkvnfi.html

[G14] 数据类 / record
来源：http://hz.guannengcc.top/gtpltycktq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sweek.top/gtovmkbkre.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sufxvd.cn/gtosvliwrc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhiwuduotai.top/gtxkxdzftj.html

TS:   type User = { name: string; age: number };
来源：http://hz.cdnleiting.top/gtircxmbsp.html

Java: record User(String name, int age) {}
来源：http://hz.ppjwa.cn/gteslnwylc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxinkj.top/gtwsrpnhul.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.dashuyun.cn/gtpqlhlqws.html

C#:   record User(string Name, int Age);
来源：http://hz.ydzc1.top/gtokhuuwne.html

[G15] 枚举
来源：http://hz.pycfn.com/gtemudzeaf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ehwqpu.com/gtvztdttrv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nwbrower.top/gtulhkzteq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sxryk.cn/gtatrhdysv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtlkbbiiio.html

Java: enum Color { RED, GREEN }
来源：http://hz.52xcode.cn/gtxyttyffk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgufenzy.top/gthybtpwur.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tianlin.xyz/gtcaurtajj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtttapyfei.html

[G16] 对象转数组 / 字典
来源：http://hz.fzhhl.top/gtwnkfrsma.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangtech.top/gtwxtxdqmb.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxuanxn.top/gthffuozah.html

JS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtojybwhpo.html

TS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gterrcoolr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cucudq.cn/gtpyptpicj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuanzhike.top/gtoyjixyni.html

Ruby: obj.instance_variables
来源：http://hz.zhoulong.xyz/gtykkbhslr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhijiandao.cn/gtbfnxqjpj.html

================================================================================
来源：http://hz.guannengcc.top/gtiutzcewp.html

H. 异常与错误处理
来源：http://hz.yj20258.top/gtqdpslauj.html

================================================================================
来源：http://hz.zhixingplan.top/gtsoddyyyz.html

[H01] try / catch 基础
来源：http://hz.ivvv.top/gtmsvucdmv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jyoumei.cn/gthdwtfsux.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tanke756.top/gtxlbhhmcf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtwzedbdov.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtkunayysw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yvedp.cn/gteqesthwc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yueranfly.top/gtetaijhhf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jqgufenzy.top/gtoxleeezq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.haohaochexian.top/gtlcyyscku.html

[H02] finally / ensure 收尾
来源：http://hz.chenjidiqi.icu/gtvqqmclor.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinghuilouyu.cn/gtysoesyzu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gteyfpnrql.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtcuvqksyq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtyhpxezyy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtahdmofmn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258.top/gtzsnplqkq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhengqikj.top/gtjixlifwg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuetiantiany.cn/gtdihixotg.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gtykgnrdmr.html

Py:   raise ValueError("错误信息")
来源：http://hz.ybcxt.top/gtmavwtshy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtspgmnnqt.html

JS:   throw new Error("错误信息");
来源：http://hz.gotoacloud.top/gtzbbbemrt.html

TS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtxdfuykwa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj202588.top/gtuifotswf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xingfuxueyuan.xyz/gtkiljamej.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.redwolf501.top/gthvlijvbp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.birdmap.top/gtdidiuero.html

[H04] 自定义异常类型
来源：http://hz.havefunace.top/gtwxtsufkb.html

Py:   class MyError(Exception): pass
来源：http://hz.gaohongyu789.top/gtuojsqdfo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinqigufen.top/gtwkosfgbi.html

JS:   class MyError extends Error {}
来源：http://hz.ydzc1.top/gtegylxloo.html

TS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtjqoepmks.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gotoacloud.top/gthdepdees.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gtyvfyrrpt.html

Ruby: class MyError < StandardError; end
来源：http://hz.meibo888.top/gtyfdxrjim.html

C#:   class MyException : Exception {}
来源：http://hz.xingfuxueyuan.xyz/gtlmkupodm.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtnimrmldt.html

Py:   except ValueError as e:
来源：http://hz.jqgufenzy.top/gtwqwcgjsa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guannengcc.top/gtfoxspcmx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gttzcwjdlq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cdnleiting.top/gtfxihrvin.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.andypj.xyz/gtdetrphhb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258.top/gtkamaboli.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuanzhike.top/gtaqqtckta.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gthlkbyomb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gtsrcwaunw.html

Py:   value = d.get("k") or default
来源：http://hz.redwolf501.top/gtlhaivxuu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.dashuyun.cn/gtazalivsr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtizaafeff.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtdlhonyqz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuxming.cn/gtuuaxxunm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj20258888.top/gtjzdcwgrr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jyoumei.cn/gtjxvuzryp.html

C#:   obj?.A?.B ?? default
来源：http://hz.gzhubu.top/gtjbvjhucj.html

[H07] 断言
来源：http://hz.shzxlz.cn/gtpljfeawq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.tian-w.cn/gtlmfddrao.html

PHP:  assert($x > 0);
来源：http://hz.quarkkingdee.top/gtxoefdnqa.html

JS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtftopfwsf.html


<!-- 参考信息 -->