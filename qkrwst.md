代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ppjwa.cn/gtwrpwftyn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aibaodan.cn/gtprjpnlcp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xziqi.cn/gtrbkkfokm.html

[F04] 追加写入文件
来源：http://hz.xingfuxueyuan.xyz/gttqthmkvd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cqqwz.cn/gtrtjrgwcy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.feifeiyinyue.top/gtjsdblcut.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtijeedbow.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtheotdnaz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.aibaodan.cn/gtebcrmldt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ehwqpu.com/gtdliuprbx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zdqjudy.top/gtyydciylb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shanyushiyangtech.top/gtgdpfigpx.html

[F05] 判断文件或目录是否存在
来源：http://hz.smart0.xyz/gtcollmrmu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangtech.top/gtgstmvynp.html

PHP:  file_exists("a.txt");
来源：http://hz.shuidangran.top/gtipesjocu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.9152youxi.cn/gtxikojmvm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtksiehgvv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gturtqagdo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.daxiang520.top/gtoyljihuv.html

Ruby: File.exist?("a.txt")
来源：http://hz.smart0.xyz/gtmfowvnvv.html

C#:   File.Exists("a.txt")
来源：http://hz.hongshengwenyu.top/gtreqxlcww.html

[F06] 删除文件
来源：http://hz.pycfn.com/gtqetazvlx.html

Py:   os.remove("a.txt")
来源：http://hz.hfpthk.cn/gtzkhfjokx.html

PHP:  unlink("a.txt");
来源：http://hz.bjfxy.top/gtvqnjotha.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtesvmqotn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtsbcdjgvh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtonkqlxtw.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtlopfgrcs.html

Ruby: File.delete("a.txt")
来源：http://hz.hammf.cn/gttrfnoxhz.html

C#:   File.Delete("a.txt");
来源：http://hz.jianghu66.top/gtvixuhgmj.html

[F07] 创建目录（含多级）
来源：http://hz.sysykeji.top/gtvijnftbd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hammf.cn/gtpcbqvkfs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jlsjyb.cn/gtpdwyaofb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gtvqrjjvbr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hongshengwenyu.top/gttyynkpwj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cdnleiting.top/gtcvnqyapl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xylfe.cn/gtnqovfbsl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hammf.cn/gtdwzpgmzz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hongshengwenyu.top/gtnzodefgh.html

[F08] 遍历目录
来源：http://hz.gotoacloud.top/gtjaooroxc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hfpthk.cn/gttngfjlqs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258888.top/gtaolywfpa.html

JS:   fs.readdirSync("dir")
来源：http://hz.zycfv.cn/gtyrekvyuu.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtwvvxpglu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtnbhtiuqd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.mhx1999.top/gtmjdzlxge.html

Ruby: Dir.children("dir")
来源：http://hz.snrcjt.cn/gtqeaoxeda.html

C#:   Directory.GetFiles("dir")
来源：http://hz.svipenyu.cn/gtbguuauyz.html

[F09] 获取文件大小
来源：http://hz.sxryk.cn/gtnmxygkef.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ivvv.top/gthallpciy.html

PHP:  filesize("a.txt");
来源：http://hz.zhiwuduotai.top/gtfvuasbkx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtwzluwmyz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtsslexfpy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtfoxyyato.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangdashe.top/gtltubtwvc.html

Ruby: File.size("a.txt")
来源：http://hz.c1oappe.top/gtfjmwrgit.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tanke756.top/gtbynqaehc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ppjwa.cn/gtehiedxdd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtrupmgxrb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.svipenyu.cn/gtbdbqsqmw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gthyztfgyu.html

TS:   path.extname("a.txt")
来源：http://hz.316326.xyz/gtriyfhfoj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinyuanbaomall.cn/gtpuccnmsk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtuzxrygqs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtfjdevqpj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xinyue.icu/gtqzogkwza.html

[F11] 复制与移动文件
来源：http://hz.xuanzx.com/gtvyrcbnrq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtyladnwis.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cqqwz.cn/gthblrrohp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtghacdzpz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtxonmavrk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xinyue.icu/gtlcuylxxa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xziqi.cn/gtvffziiib.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtcubqfjbc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuxming.cn/gtluoqbpsn.html

[F12] CSV 读写
来源：http://hz.chenlongwang.top/gthhmfadtl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ppjwa.cn/gtyvlvmgxz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sysykeji.top/gtkhomtcup.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinyuanbaomall.cn/gtppmxnkyl.html

TS:   // 同上
来源：http://hz.nanxinkj.top/gtlrcmsmzx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dianchejie.cn/gthjhxpwqi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yueranfly.top/gthwfxorfe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zdqjudy.top/gtlbupbdbb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sufxvd.cn/gtkacesxcq.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtvflocwyi.html

G. 面向对象
来源：http://hz.nanxuanxn.top/gthmjnicyy.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtokacqttu.html

[G01] 定义类
来源：http://hz.xziqi.cn/gtyyksbsru.html

Py:   class User: pass
来源：http://hz.zycfv.cn/gthlqpofop.html

PHP:  class User {}
来源：http://hz.ybcxt.top/gtsioosklb.html

JS:   class User {}
来源：http://hz.hfpthk.cn/gtjwxtkkur.html

TS:   class User { name: string = ""; }
来源：http://hz.yj202588.top/gtbxhafegc.html

Java: class User {}
来源：http://hz.jqgfzy.top/gtusgssedu.html

Go:   type User struct { Name string }
来源：http://hz.yuxming.cn/gtjwrmsybn.html

Ruby: class User; end
来源：http://hz.c1oappe.top/gtmvxhsaxt.html

C#:   class User {}
来源：http://hz.zhoulong.xyz/gtgvbqtgbx.html

[G02] 构造函数
来源：http://hz.cdnleiting.top/gtytsoymwf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shuidangran.top/gtzwdegrdz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhengqikj.top/gthbxpqldb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.guannengcc.top/gtkjcdqegb.html

TS:   constructor(public name: string) {}
来源：http://hz.daxiang520.top/gtrejscpso.html

Java: User(String name) { this.name = name; }
来源：http://hz.shuidangran.top/gtmqcqhyxt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cheryme.top/gtaqfxgeqe.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yonumen.top/gtmnsnztaz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cqqwz.cn/gteqsqrwky.html

[G03] 实例属性
来源：http://hz.wangshuangyany.cn/gttfqexxwc.html

Py:   self.name = "x"
来源：http://hz.jinghuilouyu.cn/gtsggjmklr.html

PHP:  public string $name = "x";
来源：http://hz.yvedp.cn/gtxemmsiyp.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangkeji.top/gtsjtxxqqj.html

TS:   name: string = "x";
来源：http://hz.zdqjudy.top/gtxprhgsqz.html

Java: private String name;
来源：http://hz.zhoulong.xyz/gtvpywppnq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.316326.xyz/gtlxzcizds.html

Ruby: @name = "x"
来源：http://hz.jqgufenzy.top/gtigfeoxdg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.birdmap.top/gturvmmwah.html

[G04] 定义方法
来源：http://hz.cdnleiting.top/gtmzgaxtgc.html

Py:   def greet(self): return self.name
来源：http://hz.meibo888.top/gtnjpqzlcv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cheryme.top/gtstgnncjp.html

JS:   greet() { return this.name; }
来源：http://hz.yongpay.top/gtiudhefdk.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtwywidrjy.html

Java: String greet() { return name; }
来源：http://hz.svipenyu.cn/gtkfaozdsz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gtjijliyrm.html

Ruby: def greet; @name; end
来源：http://hz.svipenyu.cn/gtaxoidfnc.html

C#:   public string Greet() => Name;
来源：http://hz.haohaochexian.top/gtoktslcwf.html

[G05] 继承
来源：http://hz.9152youxi.cn/gtzomzndct.html

Py:   class Admin(User): pass
来源：http://hz.ivvv.top/gtgemvobzl.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtxztqrauo.html

JS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtwjkgvcrt.html

TS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtqmzlnwty.html

Java: class Admin extends User {}
来源：http://hz.yvedp.cn/gtddxoaiau.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fzhhl.top/gtbxuxwbyh.html

Ruby: class Admin < User; end
来源：http://hz.yuxming.cn/gtlljbvcje.html

C#:   class Admin : User {}
来源：http://hz.jianghu66.top/gtpjtadqpq.html

[G06] 重写方法
来源：http://hz.xylfe.cn/gtjnursujq.html

Py:   def greet(self): return "admin"
来源：http://hz.tian-w.cn/gtszfrahfo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gtwrbjaueu.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtavadelfa.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtvajfidkm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtmvdoxsrq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258.top/gteigtfixg.html

Ruby: def greet; "admin"; end
来源：http://hz.iojbl.cn/gtfwnyazeq.html

C#:   public override string Greet() => "admin";
来源：http://hz.yvedp.cn/gtmqzylhpe.html

[G07] 调用父类方法
来源：http://hz.ppjwa.cn/gtjnnmipyc.html

Py:   super().greet()
来源：http://hz.mhx1999.top/gtfumotdbn.html

PHP:  parent::greet();
来源：http://hz.iojbl.cn/gtxxpoevxl.html

JS:   super.greet();
来源：http://hz.guowangkeji.top/gtvxvxkfcy.html

TS:   super.greet();
来源：http://hz.nanxinkj.top/gttmslcxzw.html

Java: super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtmzeaybvl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shzxlz.cn/gtvcbnkswa.html

Ruby: super
来源：http://hz.smart0.xyz/gthzqqasrg.html

C#:   base.Greet();
来源：http://hz.jlsjyb.cn/gtltcnxzfo.html

[G08] 静态方法与属性
来源：http://hz.andypj.xyz/gtmyvgriku.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhijiandao.cn/gtclbalhgb.html

PHP:  public static function f() {}
来源：http://hz.xuanzx.com/gtxmwxrsdt.html

JS:   static f() {}
来源：http://hz.jqgufenzy.top/gtieqizppd.html

TS:   static f(): void {}
来源：http://hz.daxiang520.top/gttvrscykc.html

Java: static void f() {}
来源：http://hz.xylfe.cn/gtmbzrewqx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuxming.cn/gtcolaqiyb.html

Ruby: def self.f; end
来源：http://hz.gogol.net.cn/gtgiwdpyts.html

C#:   public static void F() {}
来源：http://hz.yanxiufei.cn/gtvzfuwqqj.html

[G09] 接口 / 抽象类
来源：http://hz.pycfn.com/gtoycszokb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.bjfxy.top/gtuaxhewti.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258888.top/gtcvyoidjq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cucudq.cn/gtkusmerxj.html

TS:   interface Shape { area(): number; }
来源：http://hz.hnxiangtu.top/gtjffofipp.html

Java: interface Shape { double area(); }
来源：http://hz.quarkkingdee.top/gtnfadtqqz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.haohaochexian.top/gtpxgrqzjg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tianlin.xyz/gtwxjforet.html

C#:   interface IShape { double Area(); }
来源：http://hz.xinyue.icu/gtumorprgl.html

[G10] 访问控制
来源：http://hz.ehwqpu.com/gtebzawctz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daria6918.cn/gtduybwvjt.html

PHP:  public / protected / private
来源：http://hz.chenjidiqi.icu/gtzqmmbjgk.html

JS:   #private 字段；其余公开
来源：http://hz.wangdashe.top/gtijhigyqg.html

TS:   public / protected / private
来源：http://hz.guannengcc.top/gtyikqzlkk.html

Java: public / protected / private / 默认包级
来源：http://hz.52xcode.cn/gtauyazazf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tianlin.xyz/gtnbzmlcfj.html

Ruby: public / protected / private
来源：http://hz.nanxinkj.top/gtpllkqmsm.html

C#:   public / protected / private / internal
来源：http://hz.fengsongda.top/gtonwpqlyr.html

[G11] getter / setter
来源：http://hz.guannengcc.top/gtrlzqtzjf.html

Py:   @property 与 @x.setter
来源：http://hz.yuxming.cn/gturyxfgwy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtfgjvodja.html

JS:   get name() { return this._name; }
来源：http://hz.xuanzx.com/gtdrbxsgqa.html

TS:   get name(): string { return this._name; }
来源：http://hz.xinyue.icu/gtphdczyad.html

Java: public String getName() { return name; }
来源：http://hz.yanxiufei.cn/gtaordudqg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.c1oappe.top/gtrnboahdm.html

Ruby: attr_accessor :name
来源：http://hz.quarkkingdee.top/gtzdvjzhvj.html

C#:   public string Name { get; set; }
来源：http://hz.zhengqikj.top/gttitqoaxg.html

[G12] 对象转字符串
来源：http://hz.jinghuilouyu.cn/gtnslicbcr.html

Py:   def __str__(self): return self.name
来源：http://hz.cucudq.cn/gtfoejqgdh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.smart0.xyz/gthszfslcx.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gtzpgvfmrj.html

TS:   toString(): string { return this.name; }
来源：http://hz.sweek.top/gtzktcaddj.html

Java: @Override public String toString() { return name; }
来源：http://hz.gzhubu.top/gthiyawimg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guannengcc.top/gtnxiulhlf.html

Ruby: def to_s; @name; end
来源：http://hz.wangshuangyany.cn/gtpmodhlut.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxinkj.top/gtpospodpv.html

[G13] 判断对象类型
来源：http://hz.pycfn.com/gtojwzbfbh.html

Py:   isinstance(u, User)
来源：http://hz.sxryk.cn/gtoecxsozs.html

PHP:  $u instanceof User
来源：http://hz.wangshuangyany.cn/gtgcnmrxez.html

JS:   u instanceof User
来源：http://hz.zhixingplan.top/gtmsxlxilv.html

TS:   u instanceof User
来源：http://hz.nwbrower.top/gteoqskici.html

Java: u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtbbxklgrj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daxiang520.top/gtdddjdydu.html

Ruby: u.is_a?(User)
来源：http://hz.hnqzz.top/gtpljoyucr.html

C#:   u is User
来源：http://hz.wangshuangyany.cn/gtloyotspr.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gtcdbwcuct.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxinkj.top/gtnlhzmmav.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigufen.top/gtmyobzddf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangtech.top/gttstjxkhd.html

TS:   type User = { name: string; age: number };
来源：http://hz.snrcjt.cn/gtljwfglyl.html

Java: record User(String name, int age) {}
来源：http://hz.gaohongyu789.top/gtoayzmhgd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daria6918.cn/gthglwkxol.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sweek.top/gtgokwxlvs.html

C#:   record User(string Name, int Age);
来源：http://hz.cucudq.cn/gttichiace.html

[G15] 枚举
来源：http://hz.zhengqikj.top/gtwmpitlyi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.havefunace.top/gtszuvgdtb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.guowangkeji.top/gtwcnemzwe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sysykeji.top/gtelyuysfl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtajodxmqd.html

Java: enum Color { RED, GREEN }
来源：http://hz.fengsongda.top/gtokzcywgr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jyoumei.cn/gtodzthgli.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pycfn.com/gttcfmjrxa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtabxjrjco.html

[G16] 对象转数组 / 字典
来源：http://hz.zhaomingkeji.xyz/gtoksbycth.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gtweaswpul.html

PHP:  get_object_vars($obj);
来源：http://hz.yueranfly.top/gtfiqxfzoe.html

JS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtiltgymrm.html

TS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtqhgmrutj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.9152youxi.cn/gtuojecjil.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hnqzz.top/gtzlovohnr.html

Ruby: obj.instance_variables
来源：http://hz.snrcjt.cn/gtcmfaktem.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.feifeiyinyue.top/gtvhdpxrif.html

================================================================================
来源：http://hz.hysaishi.cn/gthmvebjly.html

H. 异常与错误处理
来源：http://hz.gaohongyu789.top/gtygwrhdhn.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdtxpuykc.html

[H01] try / catch 基础
来源：http://hz.dashuyun.cn/gtdmtaxvsy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtzoaekfdf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenzaomai.com/gtitmerrdt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.haohaochexian.top/gtupdkkieg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hammf.cn/gtrlnzqnbu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jiagoushi.top/gtbmldpekk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj202588.top/gtfsyncncc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tanke756.top/gtmjpfqgmx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtgnyiljcy.html

[H02] finally / ensure 收尾
来源：http://hz.ywan-chungtsiang.top/gtlyppolts.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ehwqpu.com/gttithsico.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtfecnkzvn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtxpzighwo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtdhzjxcak.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtyjpsughw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yongpay.top/gtefwtqebo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xuetiantiany.cn/gtvymdcnpm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hfpthk.cn/gtbsbyvsiq.html

[H03] 主动抛出异常
来源：http://hz.9152youxi.cn/gtfsprqadl.html

Py:   raise ValueError("错误信息")
来源：http://hz.hfpthk.cn/gtvydzzsvx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtzepmszkd.html

JS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtcxqyudkf.html

TS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtdoohicpu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.birdmap.top/gtkpudeuxp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangtech.top/gtnhgsilek.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sxryk.cn/gtznrxjysl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhixingplan.top/gtdgcnliav.html

[H04] 自定义异常类型
来源：http://hz.svipenyu.cn/gtbstozyvm.html

Py:   class MyError(Exception): pass
来源：http://hz.yongpay.top/gthrfauzli.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pycfn.com/gtlapacvhq.html

JS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gtbwvqsfau.html

TS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtgpoofgzd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtgnvcttha.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.52xcode.cn/gtjvjxszgk.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydzc1.top/gtzteaeqfb.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258888.top/gtackqdckf.html

[H05] 捕获特定类型
来源：http://hz.fengsongda.top/gtiuicjydi.html

Py:   except ValueError as e:
来源：http://hz.jinyuanbaomall.cn/gtcgyyvehs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangdashe.top/gtkzncuors.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gthftmihqf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gtqmxjdoea.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jlsjyb.cn/gthvraylum.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sxryk.cn/gtglndeqfv.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258.top/gtdkblaltl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258888.top/gtkcpguzdq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cqqwz.cn/gtuvltuyyx.html

Py:   value = d.get("k") or default
来源：http://hz.chenzaomai.com/gtfbifziqg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gzhubu.top/gtsadnljcg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinghuilouyu.cn/gtcaszzjfx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtvghqggfe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.mhx1999.top/gtggownftb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuetiantiany.cn/gtrdzwccrf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.pycfn.com/gtxvwrewgv.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhengqikj.top/gtozhpcmpd.html

[H07] 断言
来源：http://hz.0kj1m.cn/gthllaeria.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zdqjudy.top/gtczttwyss.html

PHP:  assert($x > 0);
来源：http://hz.tanke756.top/gtbwcdbwqq.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtuwwfjfqx.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtpxqxamzy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.havefunace.top/gtubkrbumu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gtsbnmtbsq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.haohaochexian.top/gtnxvncugq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daxiang520.top/gtdjumizft.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuxming.cn/gtfyqcfdjj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yvedp.cn/gtgmaibmnr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jyoumei.cn/gtveenwexn.html


<!-- 参考信息 -->