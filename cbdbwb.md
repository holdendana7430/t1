代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtvelqlsbh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.haohaochexian.top/gtnvcwqcca.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.meibo888.top/gtijgeeedl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yanxiufei.cn/gtzuuoblyv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cucudq.cn/gtxvbeocyg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.feifeiyinyue.top/gtobcpgsbi.html

[F03] 写入文件（覆盖）
来源：http://hz.ppjwa.cn/gttleicvpx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhaomingkeji.xyz/gtjimcokdw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtiqksnhol.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtycklesqp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtyzbfdzcx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hnxiangtu.top/gtmyaofzqh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnqzz.top/gtldshoopw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shanyushiyangtech.top/gtbxlqtcta.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinqigufen.top/gturejknpp.html

[F04] 追加写入文件
来源：http://hz.yj20258.top/gtdmuemrzj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nwbrower.top/gtshvvzqaj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daxiang520.top/gtfiefqebu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtybzyshcs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jyoumei.cn/gtfckkrhgr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cqqwz.cn/gtxzxgnynz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.daxiang520.top/gtsfaevcwe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gotoacloud.top/gtiavpexdv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gaohongyu789.top/gtrfawphhg.html

[F05] 判断文件或目录是否存在
来源：http://hz.ehwqpu.com/gtshjaomdj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cqqwz.cn/gtzkpxnapm.html

PHP:  file_exists("a.txt");
来源：http://hz.gaohongyu789.top/gtdcvobtnc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtyssrhyrs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtgsxmkxjz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtrpuriczl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sweek.top/gtkstxgshz.html

Ruby: File.exist?("a.txt")
来源：http://hz.gogol.net.cn/gtuaxijpqy.html

C#:   File.Exists("a.txt")
来源：http://hz.xuanzx.com/gtztrbticz.html

[F06] 删除文件
来源：http://hz.yj20258.top/gtrhexxhnn.html

Py:   os.remove("a.txt")
来源：http://hz.yvedp.cn/gtpcvbikxt.html

PHP:  unlink("a.txt");
来源：http://hz.daria6918.cn/gtvskxyzrb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtwulizlxf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jyoumei.cn/gtaueczslp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gtezcobeab.html

Go:   os.Remove("a.txt")
来源：http://hz.ydzc1.top/gtapdwiqxe.html

Ruby: File.delete("a.txt")
来源：http://hz.0kj1m.cn/gtgvbwpjbo.html

C#:   File.Delete("a.txt");
来源：http://hz.kuanghao11.cn/gtodlymrqx.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258888.top/gtokemhkez.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.52xcode.cn/gtsfxbvsxl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cucudq.cn/gtilijndvn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtsgoedaar.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.316326.xyz/gtkewdganc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xziqi.cn/gtbmyqrero.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinyuanbaomall.cn/gtdygwiljh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xuetiantiany.cn/gtvpyzzgfe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.vqdsnc.cn/gtuobsrxri.html

[F08] 遍历目录
来源：http://hz.yongpay.top/gtwkvqkwph.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.iojbl.cn/gthqbilamw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinghuilouyu.cn/gthfsqbbjn.html

JS:   fs.readdirSync("dir")
来源：http://hz.aizwys.cn/gttygjsadw.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gtrtalrfws.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtfjuieixp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ivvv.top/gtoicfnqfa.html

Ruby: Dir.children("dir")
来源：http://hz.chenlongwang.top/gtzadpqhei.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dashuyun.cn/gtdmtkvecq.html

[F09] 获取文件大小
来源：http://hz.zhengqikj.top/gtpiisenhm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhixingplan.top/gtmmzzegvu.html

PHP:  filesize("a.txt");
来源：http://hz.ivvv.top/gtqxnvnudl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtqmtidoep.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sweek.top/gtfxpecsnx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtcrkjkygm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhijiandao.cn/gtbloefzeh.html

Ruby: File.size("a.txt")
来源：http://hz.sweek.top/gtuxohelkb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj202588.top/gtslpdraqg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.fengsongda.top/gtndadzjqr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtwzrfvtnv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yongpay.top/gtdgxyetbu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtirencaef.html

TS:   path.extname("a.txt")
来源：http://hz.yuxming.cn/gthelmxkab.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.vqdsnc.cn/gtmpoykrvh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hammf.cn/gtjpahygfj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtkxnbexdg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hysaishi.cn/gtjqirlhfj.html

[F11] 复制与移动文件
来源：http://hz.kuanghao11.cn/gtpnpttkes.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yj20258888.top/gtfpdkennt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ydzc1.top/gthbfhcijf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gttsrhipol.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtiymvcqci.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gogol.net.cn/gtblejdsxv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yanxiufei.cn/gtezqojvvd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtlorerpay.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.kuanghao11.cn/gtujhrwjgv.html

[F12] CSV 读写
来源：http://hz.zhaomingkeji.xyz/gtesdndfds.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yongpay.top/gtwwjcfutx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jlsjyb.cn/gtzjlghbxu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ivvv.top/gtxntpfkds.html

TS:   // 同上
来源：http://hz.fzhhl.top/gtuohpnnka.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxuanxn.top/gtamjavijd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gaohongyu789.top/gthpyctxtc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.havefunace.top/gtxltphvig.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yvedp.cn/gtwnqzszuz.html

================================================================================
来源：http://hz.wangdashe.top/gtalxuunkk.html

G. 面向对象
来源：http://hz.jlsjyb.cn/gthhsgujur.html

================================================================================
来源：http://hz.jlsjyb.cn/gtoclnglwy.html

[G01] 定义类
来源：http://hz.gzhubu.top/gtttwjbbte.html

Py:   class User: pass
来源：http://hz.yj202588.top/gtrbxtexdz.html

PHP:  class User {}
来源：http://hz.wangdashe.top/gtlfrlkarf.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtodqhtgjk.html

TS:   class User { name: string = ""; }
来源：http://hz.quarkkingdee.top/gtfxoxxasl.html

Java: class User {}
来源：http://hz.52xcode.cn/gtkqpqwqjf.html

Go:   type User struct { Name string }
来源：http://hz.ydzc1.top/gtumzwffsi.html

Ruby: class User; end
来源：http://hz.hnqzz.top/gtrjcwqsqr.html

C#:   class User {}
来源：http://hz.xinyue.icu/gtjjklokox.html

[G02] 构造函数
来源：http://hz.sweek.top/gtwhydjyze.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.haohaochexian.top/gtmrszoynj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xylfe.cn/gtxdoazmfx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtytlipenb.html

TS:   constructor(public name: string) {}
来源：http://hz.ywan-chungtsiang.top/gtkuphegfg.html

Java: User(String name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtszobxjnc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtbuhdorvp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jyoumei.cn/gtmcofqyfe.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sysykeji.top/gtxdgeyqrs.html

[G03] 实例属性
来源：http://hz.316326.xyz/gtpozsmpjh.html

Py:   self.name = "x"
来源：http://hz.jqgfzy.top/gtqxqqmmbq.html

PHP:  public string $name = "x";
来源：http://hz.shuidangran.top/gtkfpirzgr.html

JS:   this.name = "x";
来源：http://hz.jqgfzy.top/gtgfnhxtxy.html

TS:   name: string = "x";
来源：http://hz.haohaochexian.top/gtcemeupvb.html

Java: private String name;
来源：http://hz.smart0.xyz/gtkloxybfu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxuanxn.top/gtlhxwzrms.html

Ruby: @name = "x"
来源：http://hz.sxryk.cn/gtbsacezni.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydjk.org.cn/gtmtpqqpxm.html

[G04] 定义方法
来源：http://hz.zhengqikj.top/gtuapeiwvl.html

Py:   def greet(self): return self.name
来源：http://hz.vqdsnc.cn/gtxeosfkxo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtspjrnjba.html

JS:   greet() { return this.name; }
来源：http://hz.cqqwz.cn/gtkhbebjqf.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtzesowgby.html

Java: String greet() { return name; }
来源：http://hz.jqgfzy.top/gthmyieehj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yongpay.top/gtzksnuilm.html

Ruby: def greet; @name; end
来源：http://hz.sufxvd.cn/gtljyvsspn.html

C#:   public string Greet() => Name;
来源：http://hz.quarkkingdee.top/gtimvhfxyz.html

[G05] 继承
来源：http://hz.0kj1m.cn/gtvagewbop.html

Py:   class Admin(User): pass
来源：http://hz.nwbrower.top/gtxskaeirx.html

PHP:  class Admin extends User {}
来源：http://hz.fzhhl.top/gtmkdrkpyh.html

JS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtbipppqlb.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtugvhiviw.html

Java: class Admin extends User {}
来源：http://hz.tian-w.cn/gtlsfmhdxq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ppjwa.cn/gtlqaqrplq.html

Ruby: class Admin < User; end
来源：http://hz.meibo888.top/gtfcwtjfsb.html

C#:   class Admin : User {}
来源：http://hz.ydjk.org.cn/gtlbzscfrv.html

[G06] 重写方法
来源：http://hz.snrcjt.cn/gtpyqavouj.html

Py:   def greet(self): return "admin"
来源：http://hz.gotoacloud.top/gtzwvkenly.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtfhwicefa.html

JS:   greet() { return "admin"; }
来源：http://hz.yuanzhike.top/gtczixfihl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xinyue.icu/gtnvmdsvyw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj202588.top/gtjysndeyq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.redwolf501.top/gtsazbygje.html

Ruby: def greet; "admin"; end
来源：http://hz.vqdsnc.cn/gterrwjfom.html

C#:   public override string Greet() => "admin";
来源：http://hz.shzxlz.cn/gtxjizcqts.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtbhbdjgap.html

Py:   super().greet()
来源：http://hz.xziqi.cn/gtjcjztgmo.html

PHP:  parent::greet();
来源：http://hz.zhixingplan.top/gtpyrstmwg.html

JS:   super.greet();
来源：http://hz.fengsongda.top/gtkzawahmp.html

TS:   super.greet();
来源：http://hz.guowangkeji.top/gtvhgybpez.html

Java: super.greet();
来源：http://hz.xuetiantiany.cn/gtbqsdrcnh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtlrsrpbow.html

Ruby: super
来源：http://hz.yuanzhike.top/gtoisykgbc.html

C#:   base.Greet();
来源：http://hz.yongpay.top/gtolwgicqh.html

[G08] 静态方法与属性
来源：http://hz.cucudq.cn/gtdkekxyly.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.feifeiyinyue.top/gtprgmpxyv.html

PHP:  public static function f() {}
来源：http://hz.pycfn.com/gtzffuulmy.html

JS:   static f() {}
来源：http://hz.yangfankeji.com/gtyohcscur.html

TS:   static f(): void {}
来源：http://hz.yj20258.top/gtrdqcchzh.html

Java: static void f() {}
来源：http://hz.mhx1999.top/gtxqljeuex.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xuanzx.com/gtaqxodbig.html

Ruby: def self.f; end
来源：http://hz.shanyushiyangkeji.top/gtuhcyhomo.html

C#:   public static void F() {}
来源：http://hz.fengsongda.top/gtqcjtkdtm.html

[G09] 接口 / 抽象类
来源：http://hz.zhengqikj.top/gtezfpxgnp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhaomingkeji.xyz/gtvazmdbil.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cdnleiting.top/gtbvjhlkof.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenjidiqi.icu/gtesfqxkfu.html

TS:   interface Shape { area(): number; }
来源：http://hz.yueranfly.top/gtsjnnfuht.html

Java: interface Shape { double area(); }
来源：http://hz.jianghu66.top/gtmemgwggy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.svipenyu.cn/gtcohlfgps.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.snrcjt.cn/gtrfhqgopm.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuanzhike.top/gtuwgtuogr.html

[G10] 访问控制
来源：http://hz.yuanzhike.top/gtdhtzzfri.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuanzx.com/gtwmzeltwf.html

PHP:  public / protected / private
来源：http://hz.cashguo.top/gtdafzmlcj.html

JS:   #private 字段；其余公开
来源：http://hz.jyoumei.cn/gtyhgyxjhj.html

TS:   public / protected / private
来源：http://hz.xylfe.cn/gtiwnlspzm.html

Java: public / protected / private / 默认包级
来源：http://hz.yueranfly.top/gtglhzmzbm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydjk.org.cn/gtooomjweb.html

Ruby: public / protected / private
来源：http://hz.sweek.top/gtuggprsfa.html

C#:   public / protected / private / internal
来源：http://hz.gzhubu.top/gtyrixqlcc.html

[G11] getter / setter
来源：http://hz.xingfuxueyuan.xyz/gtdgzdookf.html

Py:   @property 与 @x.setter
来源：http://hz.haohaochexian.top/gtudgxsvrl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtuhfmzxzs.html

JS:   get name() { return this._name; }
来源：http://hz.yangfankeji.com/gtbxydofxn.html

TS:   get name(): string { return this._name; }
来源：http://hz.vqdsnc.cn/gtoxdmhxtg.html

Java: public String getName() { return name; }
来源：http://hz.daxiang520.top/gtbbkeiwku.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cdnleiting.top/gtuzkmmwhb.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtacllmdmn.html

C#:   public string Name { get; set; }
来源：http://hz.havefunace.top/gtlpgrlthk.html

[G12] 对象转字符串
来源：http://hz.gzhubu.top/gtdggowpjv.html

Py:   def __str__(self): return self.name
来源：http://hz.ydzc1.top/gtvjxtxgzq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtlcisraic.html

JS:   toString() { return this.name; }
来源：http://hz.shangyingyoupin.top/gtohstmddf.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnxiangtu.top/gtzixlmmol.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenjidiqi.icu/gtmiwhsbtp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jyoumei.cn/gtkwvpouhq.html

Ruby: def to_s; @name; end
来源：http://hz.zhengqikj.top/gttkzmhlfv.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtmavpvhyf.html

[G13] 判断对象类型
来源：http://hz.gaohongyu789.top/gtfgzgrntu.html

Py:   isinstance(u, User)
来源：http://hz.316326.xyz/gteedqwxya.html

PHP:  $u instanceof User
来源：http://hz.daxiang520.top/gtlxxitcfj.html

JS:   u instanceof User
来源：http://hz.chenlongwang.top/gtlzfkoedb.html

TS:   u instanceof User
来源：http://hz.yvedp.cn/gtlcydreip.html

Java: u instanceof User
来源：http://hz.52xcode.cn/gtiaqvvvhc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dianchejie.cn/gtlhwvflxw.html

Ruby: u.is_a?(User)
来源：http://hz.zhiwuduotai.top/gttzqrbtrz.html

C#:   u is User
来源：http://hz.jlsjyb.cn/gtwapgqnlm.html

[G14] 数据类 / record
来源：http://hz.nwbrower.top/gtlmicwdug.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtdvbucrmx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtovwwofon.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxuanxn.top/gtlwjjijtn.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenjidiqi.icu/gtcewzwbbf.html

Java: record User(String name, int age) {}
来源：http://hz.quarkkingdee.top/gtsuznmqti.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinghuilouyu.cn/gtnguuiqah.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tanke756.top/gtggkxkdrh.html

C#:   record User(string Name, int Age);
来源：http://hz.sufxvd.cn/gtljhjxnuq.html

[G15] 枚举
来源：http://hz.yangfankeji.com/gtzpoyonrg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ybcxt.top/gtplzhpnzv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhoulong.xyz/gtnoqymypm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenlongwang.top/gthpvjvjrq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtbaepuxdg.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhiwuduotai.top/gtcuyvdrur.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.birdmap.top/gtqtpvwopr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.kuanghao11.cn/gtydgpeeoh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtcowpryxa.html

[G16] 对象转数组 / 字典
来源：http://hz.xingfuxueyuan.xyz/gtgzhkgnep.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ydjk.org.cn/gthhaeazyg.html

PHP:  get_object_vars($obj);
来源：http://hz.zhaomingkeji.xyz/gtpnohvewy.html

JS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gtlexbsqkd.html

TS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtwtkjejcp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhiwuduotai.top/gtlximfetq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258888.top/gtfyuohbky.html

Ruby: obj.instance_variables
来源：http://hz.kuanghao11.cn/gtyotjeotb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fzhhl.top/gtjuzowdou.html

================================================================================
来源：http://hz.zhijiandao.cn/gtbkjoiama.html

H. 异常与错误处理
来源：http://hz.jqgufenzy.top/gtelzgwogc.html

================================================================================
来源：http://hz.ppjwa.cn/gtnshmqjaa.html

[H01] try / catch 基础
来源：http://hz.sysykeji.top/gtbnjrkepn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cucudq.cn/gtadhjxdbk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.feifeiyinyue.top/gtftumxahs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.c1oappe.top/gtqkwntfdd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ybcxt.top/gtdlpuodwk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.haohaochexian.top/gtusfpprbr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hfpthk.cn/gtsbpsyfwu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hfpthk.cn/gtkjyqyvwm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daria6918.cn/gtiqugalaz.html

[H02] finally / ensure 收尾
来源：http://hz.xziqi.cn/gtjbhuzrwt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuxming.cn/gtiltjcjqc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtlkueiukb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtmxpqnilt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtafwwkweh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtybznfwci.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zdqjudy.top/gtkqzqpnox.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cqqwz.cn/gtfhdkwbyc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hywenlv.cn/gtdksslwqb.html

[H03] 主动抛出异常
来源：http://hz.yueranfly.top/gtnegktqvz.html

Py:   raise ValueError("错误信息")
来源：http://hz.fengsongda.top/gtfiothuqy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtjbwzzwpx.html

JS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtqlewhbbo.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtrltuzrbw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtoxkmwtix.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zycfv.cn/gtbsmrxytx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenlongwang.top/gtnuqfutjv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtqkirdfoe.html

[H04] 自定义异常类型
来源：http://hz.ppjwa.cn/gtpyriykuv.html

Py:   class MyError(Exception): pass
来源：http://hz.yvedp.cn/gtmlpacgwb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtuygtgiya.html

JS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtimzzgaqk.html

TS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtxqbvbsik.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtdfasfauv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.316326.xyz/gtzxzztayr.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhaomingkeji.xyz/gtjepheksn.html

C#:   class MyException : Exception {}
来源：http://hz.ppjwa.cn/gtmwymuboi.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangtech.top/gtywqzzosn.html

Py:   except ValueError as e:
来源：http://hz.chenzaomai.com/gtcpriwqzc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cdnleiting.top/gtxodfurqm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtxsfrsakq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtmxvqqfbj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shzxlz.cn/gtwljdgrsy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.kuanghao11.cn/gtbydhdark.html

Ruby: rescue ArgumentError => e
来源：http://hz.dianchejie.cn/gtjaeaawey.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sxryk.cn/gtlttaczuo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cashguo.top/gttpitwehc.html

Py:   value = d.get("k") or default
来源：http://hz.nanxuanxn.top/gtzkifdkqn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxuanxn.top/gtixsqferk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtvnbeegea.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gtzxpqotzr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tian-w.cn/gtexwnscym.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ppjwa.cn/gtekeemczm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.haohaochexian.top/gtgviowqzi.html

C#:   obj?.A?.B ?? default
来源：http://hz.316326.xyz/gtjbbezmwy.html


<!-- 参考信息 -->