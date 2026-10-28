代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenjidiqi.icu/gtdqmlqxay.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nwbrower.top/gtkqwthjgv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxinkj.top/gtwyjjvmqs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.wangdashe.top/gtlkokogmw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.smart0.xyz/gtlaumpuqm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhijiandao.cn/gtdygsilhp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtqcftzkdz.html

[F04] 追加写入文件
来源：http://hz.yuanzhike.top/gtsdpgtpsu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yongpay.top/gtcgapurzh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hywenlv.cn/gtjhzgihvl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nwbrower.top/gtlxoqwyws.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yvedp.cn/gtopqpukbj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ppjwa.cn/gtcwujioqr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhengqikj.top/gtwrsntwtx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ehwqpu.com/gtapupfazr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhixingplan.top/gtefikggnx.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangdashe.top/gtcnhvwbxi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.52xcode.cn/gtjhnnogmp.html

PHP:  file_exists("a.txt");
来源：http://hz.daxiang520.top/gtnsjbpnnb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtlubybjvy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtwkpwypnh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtrswprugh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xziqi.cn/gtyyssdeol.html

Ruby: File.exist?("a.txt")
来源：http://hz.feifeiyinyue.top/gtodsvcbfj.html

C#:   File.Exists("a.txt")
来源：http://hz.zhiwuduotai.top/gtfzafyfsm.html

[F06] 删除文件
来源：http://hz.jinyuanbaomall.cn/gtjldtovqw.html

Py:   os.remove("a.txt")
来源：http://hz.guannengcc.top/gtdumsyqot.html

PHP:  unlink("a.txt");
来源：http://hz.iojbl.cn/gtxzxwhvbq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtvjphoxus.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cashguo.top/gtvboqnefe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gteebpxzrd.html

Go:   os.Remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtxazaofqy.html

Ruby: File.delete("a.txt")
来源：http://hz.cdnleiting.top/gtnlurkfqb.html

C#:   File.Delete("a.txt");
来源：http://hz.iojbl.cn/gtbepaduhc.html

[F07] 创建目录（含多级）
来源：http://hz.316326.xyz/gtvlwcfzbl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cucudq.cn/gtiqwthpeu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ehwqpu.com/gtxpfiekfy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinyuanbaomall.cn/gtkqdrbbhf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.kuanghao11.cn/gtqzwagtcy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tian-w.cn/gtwzplsihu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnxiangtu.top/gtvlbjxdbl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cdnleiting.top/gtmuzxbxom.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tianlin.xyz/gtalxjzofl.html

[F08] 遍历目录
来源：http://hz.hywenlv.cn/gtodobhplq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zdqjudy.top/gtayplkobe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.feifeiyinyue.top/gtfwvvbfuv.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxuanxn.top/gtibcznoei.html

TS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gtpwaoafsi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtrluabang.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gogol.net.cn/gtgzomkkwj.html

Ruby: Dir.children("dir")
来源：http://hz.jqgufenzy.top/gthabzygne.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sxryk.cn/gtnifxmefl.html

[F09] 获取文件大小
来源：http://hz.yj20258888.top/gttnkldgzo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigfzy.top/gtnddgkebv.html

PHP:  filesize("a.txt");
来源：http://hz.feifeiyinyue.top/gtsqdvbsce.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtjhbyhmxc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gtcufwerzu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtnvnsipno.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ydzc1.top/gtoofzxxku.html

Ruby: File.size("a.txt")
来源：http://hz.yanxiufei.cn/gtbfqvjvdi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.kuanghao11.cn/gtlkgfqzuu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cqqwz.cn/gtvpwzrmfm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtlwttbhjk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cdnleiting.top/gtxlauokyu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtifjujgmf.html

TS:   path.extname("a.txt")
来源：http://hz.svipenyu.cn/gtqjvppeul.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.birdmap.top/gtinagtikt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.dashuyun.cn/gtcibgouwr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtxbxsfxso.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hnqzz.top/gtbgmglmqg.html

[F11] 复制与移动文件
来源：http://hz.birdmap.top/gtipfsvcwi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gthqiooubu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258888.top/gtbmuiiwoo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gthntjhtsa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtnfymjbio.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.dashuyun.cn/gtzgaoatcp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.quarkkingdee.top/gtpwjamuhb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtjgzbuuyl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jqgfzy.top/gtoidlxzzf.html

[F12] CSV 读写
来源：http://hz.ppjwa.cn/gtkdttqyce.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnqzz.top/gtpnrswwsu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ydjk.org.cn/gtdbvzybnj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgfzy.top/gtfhhthtat.html

TS:   // 同上
来源：http://hz.ywan-chungtsiang.top/gtooufqsox.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zycfv.cn/gtccyejxvj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.redwolf501.top/gtilkzrtdm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hammf.cn/gtloblwgvv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.52xcode.cn/gtbzxweqdd.html

================================================================================
来源：http://hz.xylfe.cn/gtxjrbrqle.html

G. 面向对象
来源：http://hz.nwbrower.top/gtnfkgntjz.html

================================================================================
来源：http://hz.jiagoushi.top/gtoaoqspge.html

[G01] 定义类
来源：http://hz.pengpengdd.cyou/gtmfnqclow.html

Py:   class User: pass
来源：http://hz.iojbl.cn/gttnseywya.html

PHP:  class User {}
来源：http://hz.daria6918.cn/gtuzghqhah.html

JS:   class User {}
来源：http://hz.sxryk.cn/gthdrsjgrl.html

TS:   class User { name: string = ""; }
来源：http://hz.wangdashe.top/gtqnwnsiip.html

Java: class User {}
来源：http://hz.zhaomingkeji.xyz/gtmnagzams.html

Go:   type User struct { Name string }
来源：http://hz.xuetiantiany.cn/gtfqhjtxtg.html

Ruby: class User; end
来源：http://hz.fengsongda.top/gtvuuueqkb.html

C#:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtcvoyegwb.html

[G02] 构造函数
来源：http://hz.zhijiandao.cn/gtutdiwvqi.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nwbrower.top/gtpashxrhh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jiagoushi.top/gtyftksnqx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daria6918.cn/gtyvombkst.html

TS:   constructor(public name: string) {}
来源：http://hz.andypj.xyz/gtrfdqitlf.html

Java: User(String name) { this.name = name; }
来源：http://hz.fzhhl.top/gtcnxuvvem.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuetiantiany.cn/gtflfokwkc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtawxdlpht.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxuanxn.top/gtgctnhrez.html

[G03] 实例属性
来源：http://hz.0kj1m.cn/gtbabzqevw.html

Py:   self.name = "x"
来源：http://hz.cdnleiting.top/gtcexyctjv.html

PHP:  public string $name = "x";
来源：http://hz.yj202588.top/gtbkrqpbsp.html

JS:   this.name = "x";
来源：http://hz.ywan-chungtsiang.top/gtxhdvcmfd.html

TS:   name: string = "x";
来源：http://hz.havefunace.top/gtncsbrehn.html

Java: private String name;
来源：http://hz.sxryk.cn/gtetopxvou.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangkeji.top/gtzbbusskm.html

Ruby: @name = "x"
来源：http://hz.xinyue.icu/gtuudrflop.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhoulong.xyz/gtaetoofby.html

[G04] 定义方法
来源：http://hz.jqgfzy.top/gtjapxvyrx.html

Py:   def greet(self): return self.name
来源：http://hz.ivvv.top/gtevetjvcv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gzhubu.top/gteccfhueb.html

JS:   greet() { return this.name; }
来源：http://hz.gaohongyu789.top/gteaerwexr.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhiwuduotai.top/gtnksajqqg.html

Java: String greet() { return name; }
来源：http://hz.fengsongda.top/gtynyfubxy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sweek.top/gtankzplue.html

Ruby: def greet; @name; end
来源：http://hz.xuanzx.com/gtvspczujx.html

C#:   public string Greet() => Name;
来源：http://hz.bjfxy.top/gtkfruhsqu.html

[G05] 继承
来源：http://hz.zhoulong.xyz/gtgtyrnqmo.html

Py:   class Admin(User): pass
来源：http://hz.yuanzhike.top/gtejhypacx.html

PHP:  class Admin extends User {}
来源：http://hz.cashguo.top/gtgxxqvamk.html

JS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gttpnrruvb.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtmiuikbdv.html

Java: class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtgrdjeksq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sysykeji.top/gtiajusypw.html

Ruby: class Admin < User; end
来源：http://hz.iojbl.cn/gthncikntb.html

C#:   class Admin : User {}
来源：http://hz.cdnleiting.top/gtunbatvqn.html

[G06] 重写方法
来源：http://hz.hnxiangtu.top/gtqaygptkt.html

Py:   def greet(self): return "admin"
来源：http://hz.xingfuxueyuan.xyz/gtnajyyvcv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtheqzxmbm.html

JS:   greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gtkscwkjkd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtryhmhmzu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtnnrslujd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.feifeiyinyue.top/gtrlmsbfly.html

Ruby: def greet; "admin"; end
来源：http://hz.pengpengdd.cyou/gtihdofovr.html

C#:   public override string Greet() => "admin";
来源：http://hz.xinyue.icu/gtvnohbckp.html

[G07] 调用父类方法
来源：http://hz.316326.xyz/gtrpmmcgzy.html

Py:   super().greet()
来源：http://hz.tian-w.cn/gtmrmewbcn.html

PHP:  parent::greet();
来源：http://hz.zhijiandao.cn/gtkvgwifqv.html

JS:   super.greet();
来源：http://hz.c1oappe.top/gtpfhqtihg.html

TS:   super.greet();
来源：http://hz.shuidangran.top/gtyksnejrn.html

Java: super.greet();
来源：http://hz.hammf.cn/gtwaihrqth.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtynfpespx.html

Ruby: super
来源：http://hz.andypj.xyz/gtioxunvve.html

C#:   base.Greet();
来源：http://hz.vqdsnc.cn/gtfzndkgxl.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gtnzdbyzqh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xingfuxueyuan.xyz/gtblpprsvw.html

PHP:  public static function f() {}
来源：http://hz.zycfv.cn/gtwlrcwtuw.html

JS:   static f() {}
来源：http://hz.zycfv.cn/gtymdpyrux.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtaiayovxn.html

Java: static void f() {}
来源：http://hz.jianghu66.top/gtbuehupux.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigufen.top/gtjonbshoi.html

Ruby: def self.f; end
来源：http://hz.iojbl.cn/gtyuaedcqi.html

C#:   public static void F() {}
来源：http://hz.cqqwz.cn/gtodxbxylt.html

[G09] 接口 / 抽象类
来源：http://hz.cdnleiting.top/gtbeqmhfam.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cucudq.cn/gtecomluot.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jlsjyb.cn/gtunbmynqs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xingfuxueyuan.xyz/gtrjifpncs.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenzaomai.com/gtvutksrkf.html

Java: interface Shape { double area(); }
来源：http://hz.hywenlv.cn/gtqhzvokxf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhoulong.xyz/gtpbvmcruy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hnqzz.top/gtpfaoigci.html

C#:   interface IShape { double Area(); }
来源：http://hz.yonumen.top/gtgdvhythv.html

[G10] 访问控制
来源：http://hz.zhixingplan.top/gtatyzstzc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gtoxcnoeqo.html

PHP:  public / protected / private
来源：http://hz.zhongyouzk.top/gtpnojqeqm.html

JS:   #private 字段；其余公开
来源：http://hz.xuetiantiany.cn/gtmdqggzhv.html

TS:   public / protected / private
来源：http://hz.zycfv.cn/gtegpcutwn.html

Java: public / protected / private / 默认包级
来源：http://hz.feifeiyinyue.top/gtyqfkrgsf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tanke756.top/gtjdrpvhjn.html

Ruby: public / protected / private
来源：http://hz.jinghuilouyu.cn/gtkkuxmkvn.html

C#:   public / protected / private / internal
来源：http://hz.316326.xyz/gtofsmcflg.html

[G11] getter / setter
来源：http://hz.aizwys.cn/gtvlyhdoqv.html

Py:   @property 与 @x.setter
来源：http://hz.shuidangran.top/gtqozvgyea.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtrjvacviv.html

JS:   get name() { return this._name; }
来源：http://hz.gzhubu.top/gtrjsrymzz.html

TS:   get name(): string { return this._name; }
来源：http://hz.cqqwz.cn/gtrvfawmui.html

Java: public String getName() { return name; }
来源：http://hz.birdmap.top/gtdcfuafsy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtiqyvmszn.html

Ruby: attr_accessor :name
来源：http://hz.hnxiangtu.top/gtqvlwgsnq.html

C#:   public string Name { get; set; }
来源：http://hz.cheryme.top/gttrljkvsi.html

[G12] 对象转字符串
来源：http://hz.yonumen.top/gtkmypbzja.html

Py:   def __str__(self): return self.name
来源：http://hz.jyoumei.cn/gtvuebnkwn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.havefunace.top/gtmhqeadxn.html

JS:   toString() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtktxvfwsg.html

TS:   toString(): string { return this.name; }
来源：http://hz.feifeiyinyue.top/gtcetnktdr.html

Java: @Override public String toString() { return name; }
来源：http://hz.ybcxt.top/gtsowhovgx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hywenlv.cn/gtufclbyvj.html

Ruby: def to_s; @name; end
来源：http://hz.guannengcc.top/gtoqyxwcgi.html

C#:   public override string ToString() => Name;
来源：http://hz.ydzc1.top/gtuxgefynp.html

[G13] 判断对象类型
来源：http://hz.jiagoushi.top/gtgxnvafnf.html

Py:   isinstance(u, User)
来源：http://hz.tian-w.cn/gtdppkgwfw.html

PHP:  $u instanceof User
来源：http://hz.feifeiyinyue.top/gtccqjepce.html

JS:   u instanceof User
来源：http://hz.bjfxy.top/gtpbumuhvs.html

TS:   u instanceof User
来源：http://hz.pengpengdd.cyou/gtgwvzhmsn.html

Java: u instanceof User
来源：http://hz.yongpay.top/gtwfyddccz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pengpengdd.cyou/gtibdhvsfj.html

Ruby: u.is_a?(User)
来源：http://hz.shuidangran.top/gtutnsfkog.html

C#:   u is User
来源：http://hz.quarkkingdee.top/gtvvjpcafx.html

[G14] 数据类 / record
来源：http://hz.jinqigfzy.top/gtosqobjgm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.snrcjt.cn/gtpreqasvs.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgfzy.top/gtozlqffyg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhijiandao.cn/gtdnuchmgi.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhiwuduotai.top/gtvrvaacie.html

Java: record User(String name, int age) {}
来源：http://hz.ywan-chungtsiang.top/gtjsfmfnda.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuxming.cn/gtnuaixzni.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pengpengdd.cyou/gtsktaxsfk.html

C#:   record User(string Name, int Age);
来源：http://hz.cheryme.top/gtbbyrcyzq.html

[G15] 枚举
来源：http://hz.zhixingplan.top/gtaiubvoyt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenlongwang.top/gtybxabvmz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tanke756.top/gtdqapcedl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guowangkeji.top/gttuptmrln.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258.top/gtcqbfljpu.html

Java: enum Color { RED, GREEN }
来源：http://hz.nwbrower.top/gtvrzakrch.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gaohongyu789.top/gtlozwhlrr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sufxvd.cn/gtrmtzhmok.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtftgaaofb.html

[G16] 对象转数组 / 字典
来源：http://hz.zhongyouzk.top/gtufetqxxg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangdashe.top/gtmzijlyoh.html

PHP:  get_object_vars($obj);
来源：http://hz.hywenlv.cn/gteqihfngk.html

JS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtaebzpmyr.html

TS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtfpmkwlxe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxinkj.top/gtzwbvttqo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.9152youxi.cn/gtlvisbcsd.html

Ruby: obj.instance_variables
来源：http://hz.jyoumei.cn/gtalhjdjys.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.havefunace.top/gtmlxwjmed.html

================================================================================
来源：http://hz.jianghu66.top/gtuhesogbt.html

H. 异常与错误处理
来源：http://hz.sweek.top/gtckirkdmt.html

================================================================================
来源：http://hz.nanxinkj.top/gtrsjsjwtu.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gtvihajbzu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xinyue.icu/gtyegbvnvb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.vqdsnc.cn/gtsekpvagw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtydzulskd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.daria6918.cn/gtfbmuljwf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shzxlz.cn/gtldtkfhpa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhijiandao.cn/gthpifooys.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dianchejie.cn/gtdsrsbuai.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenjidiqi.icu/gtrvyomfme.html

[H02] finally / ensure 收尾
来源：http://hz.yvedp.cn/gtfrekuwiu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.smart0.xyz/gtjmqtrjpo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtjzjmmplq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtxotbxhzz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtsvubruww.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtmcbgqjub.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.guannengcc.top/gtsvywuntu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gtqiptfywc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xylfe.cn/gtxegqhgkc.html

[H03] 主动抛出异常
来源：http://hz.zdqjudy.top/gtkurmnwyg.html

Py:   raise ValueError("错误信息")
来源：http://hz.ehwqpu.com/gtfugjtrej.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtvvnicycp.html

JS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtnvyeogib.html

TS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtnapqxgmm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtkfzhalig.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ehwqpu.com/gtjlzddqtq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shangyingyoupin.top/gtwtbkbtww.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtmkywhwub.html

[H04] 自定义异常类型
来源：http://hz.nwbrower.top/gtbkrlatck.html

Py:   class MyError(Exception): pass
来源：http://hz.zhixingplan.top/gttdgavkid.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangdashe.top/gtuwizvbre.html

JS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtuexdbswm.html

TS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gtedoomhgw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuanzx.com/gtmzvpjthl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhengqikj.top/gtsmmcchuw.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangdashe.top/gtdowjhaqd.html

C#:   class MyException : Exception {}
来源：http://hz.svipenyu.cn/gtyqzdexfl.html

[H05] 捕获特定类型
来源：http://hz.kuanghao11.cn/gturemzrcg.html

Py:   except ValueError as e:
来源：http://hz.wangdashe.top/gtvbcpkfml.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangdashe.top/gtbrqizqxi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtlnllnkjv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258.top/gtreoucgwl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.redwolf501.top/gtbsdjatup.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydjk.org.cn/gtprufnrva.html

Ruby: rescue ArgumentError => e
来源：http://hz.0kj1m.cn/gtlwdinhzv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nanxinkj.top/gtetqvdipi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sufxvd.cn/gtafgqxhmm.html

Py:   value = d.get("k") or default
来源：http://hz.xuanzx.com/gtsofkyqmp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.fzhhl.top/gtrwsxfjbr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gtthafxvty.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtgfyxntsx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daxiang520.top/gtiyrxymep.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daria6918.cn/gtoklkuezk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daria6918.cn/gtlqvqixfg.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhijiandao.cn/gthubknxfx.html

[H07] 断言
来源：http://hz.zhengqikj.top/gtlagakmex.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cdnleiting.top/gtpqbzgbto.html

PHP:  assert($x > 0);
来源：http://hz.cashguo.top/gtnidgllbb.html

JS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtuykyiapc.html

TS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtpaolxtet.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xinyue.icu/gtkujptfvy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhiwuduotai.top/gtsjynyaye.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxinkj.top/gtzjxqhebh.html


<!-- 参考信息 -->