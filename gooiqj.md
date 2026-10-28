代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jlsjyb.cn/gthnbqucyp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj20258888.top/gtiynittcs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtnpdggsyb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.52xcode.cn/gtotwyplet.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hywenlv.cn/gtrblbekmc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tianlin.xyz/gtnppqpzph.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhixingplan.top/gtxtjnxhlb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenjidiqi.icu/gtheqyvbdy.html

[F05] 判断文件或目录是否存在
来源：http://hz.ppjwa.cn/gtiojvrcvq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangtech.top/gtmorcninm.html

PHP:  file_exists("a.txt");
来源：http://hz.sysykeji.top/gtctzjeknz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtxnzbchig.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtzeptajzp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtxwdwmhii.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenzaomai.com/gtaraaoljr.html

Ruby: File.exist?("a.txt")
来源：http://hz.cashguo.top/gtuywuhbdi.html

C#:   File.Exists("a.txt")
来源：http://hz.zhengqikj.top/gtwhjowcrq.html

[F06] 删除文件
来源：http://hz.iojbl.cn/gtdurirwdt.html

Py:   os.remove("a.txt")
来源：http://hz.feifeiyinyue.top/gtmlqayhgw.html

PHP:  unlink("a.txt");
来源：http://hz.hongshengwenyu.top/gtvswajrms.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gteivflyuc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ydzc1.top/gtsoyxtxnr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtdplhpnni.html

Go:   os.Remove("a.txt")
来源：http://hz.zhongyouzk.top/gtdehsvhii.html

Ruby: File.delete("a.txt")
来源：http://hz.mhx1999.top/gtgvwvytqn.html

C#:   File.Delete("a.txt");
来源：http://hz.guannengcc.top/gtnzydjfou.html

[F07] 创建目录（含多级）
来源：http://hz.zhongyouzk.top/gtsglfvhug.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cqqwz.cn/gtddplohbd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yueranfly.top/gtubpahpdp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cashguo.top/gtaugqxioo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydjk.org.cn/gtsnjdnmhx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.pengpengdd.cyou/gtkajqhmjj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shangyingyoupin.top/gtrcpiyiqq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hongshengwenyu.top/gtpnzlkjkx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cdnleiting.top/gtjghugacv.html

[F08] 遍历目录
来源：http://hz.cucudq.cn/gtumiluvhd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hywenlv.cn/gtbwohujjs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.meibo888.top/gtefdocxgv.html

JS:   fs.readdirSync("dir")
来源：http://hz.hammf.cn/gtbbmhpzuq.html

TS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtgzshjhvc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnxiangtu.top/gtkxxnddts.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yongpay.top/gtegqhqqvr.html

Ruby: Dir.children("dir")
来源：http://hz.cqqwz.cn/gtlhtywbkc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hnxiangtu.top/gtyupyhacu.html

[F09] 获取文件大小
来源：http://hz.ivvv.top/gtsmwvnbqd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinqigfzy.top/gterizgsom.html

PHP:  filesize("a.txt");
来源：http://hz.iojbl.cn/gtzabhtinr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gtfapjrdlh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ppjwa.cn/gtvzplxhzn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtitkzmabi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.quarkkingdee.top/gtwcbrmbvc.html

Ruby: File.size("a.txt")
来源：http://hz.zhiwuduotai.top/gtapypwozv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.mhx1999.top/gtemhxbhwg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cdnleiting.top/gtlgrbpoax.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtaccnafkq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ehwqpu.com/gtssphvyix.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtgopkaqpn.html

TS:   path.extname("a.txt")
来源：http://hz.52xcode.cn/gtzdfhenef.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hnxiangtu.top/gtymigvmun.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yangfankeji.com/gtgmvanigp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtantkvxtc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtklpwanir.html

[F11] 复制与移动文件
来源：http://hz.ydzc1.top/gtnjvybzjf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtwfnbunpz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gtphvfhzwq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtrftbohuy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtipmwdlvz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hnxiangtu.top/gtfhzkccni.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jlsjyb.cn/gtxwmphhmw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtmyzqjgop.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.316326.xyz/gtshbnpdlg.html

[F12] CSV 读写
来源：http://hz.xuanzx.com/gtwigoscaw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.haohaochexian.top/gtofnuzlwz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sufxvd.cn/gtfdidskka.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydzc1.top/gtqyxgubjw.html

TS:   // 同上
来源：http://hz.hysaishi.cn/gttlcnzbaf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ehwqpu.com/gtxykefbkp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yueranfly.top/gtxttxivxz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jlsjyb.cn/gtqstlcuqq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.vqdsnc.cn/gtryrlxmjy.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtscptgwmi.html

G. 面向对象
来源：http://hz.shanyushiyangkeji.top/gtytztpgrv.html

================================================================================
来源：http://hz.hywenlv.cn/gtmpdgjmex.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtyvbbrtuw.html

Py:   class User: pass
来源：http://hz.shzxlz.cn/gtsxqwkmod.html

PHP:  class User {}
来源：http://hz.jqgufenzy.top/gtizacyici.html

JS:   class User {}
来源：http://hz.xuanzx.com/gtbkygaoqs.html

TS:   class User { name: string = ""; }
来源：http://hz.feifeiyinyue.top/gtufrajlef.html

Java: class User {}
来源：http://hz.mhx1999.top/gtxllchypd.html

Go:   type User struct { Name string }
来源：http://hz.sweek.top/gtbybfplvn.html

Ruby: class User; end
来源：http://hz.zhongyouzk.top/gtjvrcofgu.html

C#:   class User {}
来源：http://hz.cdnleiting.top/gtjgcjwahh.html

[G02] 构造函数
来源：http://hz.zhiwuduotai.top/gtnjgyitdf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.quarkkingdee.top/gtvovkhaua.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhaomingkeji.xyz/gtzqbydqtl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.bjfxy.top/gtdjexoqro.html

TS:   constructor(public name: string) {}
来源：http://hz.havefunace.top/gtlzyhgflc.html

Java: User(String name) { this.name = name; }
来源：http://hz.52xcode.cn/gttyfnuvda.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.0kj1m.cn/gtyqqkoxdz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuxming.cn/gtogjhqqiu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jianghu66.top/gtwmghzbkm.html

[G03] 实例属性
来源：http://hz.xylfe.cn/gtkqtgbpzx.html

Py:   self.name = "x"
来源：http://hz.andypj.xyz/gtphqzwtro.html

PHP:  public string $name = "x";
来源：http://hz.ydzc1.top/gtciyjtgvx.html

JS:   this.name = "x";
来源：http://hz.sysykeji.top/gtgposuohl.html

TS:   name: string = "x";
来源：http://hz.feifeiyinyue.top/gtsuaiqalg.html

Java: private String name;
来源：http://hz.0kj1m.cn/gtbanuipmy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhijiandao.cn/gtgprvwngl.html

Ruby: @name = "x"
来源：http://hz.52xcode.cn/gtdkesfiop.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.wangshuangyany.cn/gtyqrbowye.html

[G04] 定义方法
来源：http://hz.haohaochexian.top/gtconiansw.html

Py:   def greet(self): return self.name
来源：http://hz.wangdashe.top/gtriukbqsb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtlxeokowq.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gtpyypvhbl.html

TS:   greet(): string { return this.name; }
来源：http://hz.daxiang520.top/gtukhwkxqr.html

Java: String greet() { return name; }
来源：http://hz.dashuyun.cn/gtauyhwayk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtfdawkwxd.html

Ruby: def greet; @name; end
来源：http://hz.yj202588.top/gtkwcjpclr.html

C#:   public string Greet() => Name;
来源：http://hz.yonumen.top/gthddcrwjf.html

[G05] 继承
来源：http://hz.shuidangran.top/gtnvjxflyr.html

Py:   class Admin(User): pass
来源：http://hz.yueranfly.top/gtgkvxgedj.html

PHP:  class Admin extends User {}
来源：http://hz.sysykeji.top/gtbadflftu.html

JS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gtqfglpjnu.html

TS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtjljmjitb.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtvuspgucl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hywenlv.cn/gthejgwuva.html

Ruby: class Admin < User; end
来源：http://hz.aizwys.cn/gtqhrdkpwd.html

C#:   class Admin : User {}
来源：http://hz.cucudq.cn/gtoodihocu.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gtcvzbhjdq.html

Py:   def greet(self): return "admin"
来源：http://hz.guowangkeji.top/gtzaewypiw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ehwqpu.com/gteryrxaiz.html

JS:   greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtrbtlgscf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gteywmqrda.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj20258888.top/gtdwghjwmu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenjidiqi.icu/gtewutlzis.html

Ruby: def greet; "admin"; end
来源：http://hz.birdmap.top/gtfwheoyag.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gthauctjgd.html

[G07] 调用父类方法
来源：http://hz.chenlongwang.top/gtbzpaniim.html

Py:   super().greet()
来源：http://hz.xziqi.cn/gtlhkojgti.html

PHP:  parent::greet();
来源：http://hz.wangdashe.top/gtemuvlqnq.html

JS:   super.greet();
来源：http://hz.yonumen.top/gtwyyfepbx.html

TS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtruejcccp.html

Java: super.greet();
来源：http://hz.yuxming.cn/gthktmrmxs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gtsjshhyxr.html

Ruby: super
来源：http://hz.hongshengwenyu.top/gtezeruztp.html

C#:   base.Greet();
来源：http://hz.vqdsnc.cn/gtmkwzdxee.html

[G08] 静态方法与属性
来源：http://hz.sxryk.cn/gtvnbtjswk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuxming.cn/gtsvuglttr.html

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gtlxzcvppp.html

JS:   static f() {}
来源：http://hz.kuanghao11.cn/gtakapsoar.html

TS:   static f(): void {}
来源：http://hz.c1oappe.top/gtisqlgwwl.html

Java: static void f() {}
来源：http://hz.jinghuilouyu.cn/gtclsmqsii.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sysykeji.top/gtqdtzaiep.html

Ruby: def self.f; end
来源：http://hz.cdnleiting.top/gtpssyxbfm.html

C#:   public static void F() {}
来源：http://hz.smart0.xyz/gtifjiowvb.html

[G09] 接口 / 抽象类
来源：http://hz.hysaishi.cn/gtkwdjumxj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhixingplan.top/gtdvsuimxp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.smart0.xyz/gtqnpssauh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgufenzy.top/gtlvxpemtq.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangkeji.top/gtphyhgdob.html

Java: interface Shape { double area(); }
来源：http://hz.sufxvd.cn/gtjdosxzon.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.9152youxi.cn/gtorundfxk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fengsongda.top/gtkqdfpuvc.html

C#:   interface IShape { double Area(); }
来源：http://hz.9152youxi.cn/gtiierxntx.html

[G10] 访问控制
来源：http://hz.dianchejie.cn/gtyapxmfum.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jlsjyb.cn/gtkjmdgkrm.html

PHP:  public / protected / private
来源：http://hz.hammf.cn/gtqhoxovsu.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtsxhmszrp.html

TS:   public / protected / private
来源：http://hz.yj202588.top/gtgvhqssgl.html

Java: public / protected / private / 默认包级
来源：http://hz.yonumen.top/gtiwsmzyjq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gtmhfzobqq.html

Ruby: public / protected / private
来源：http://hz.hywenlv.cn/gthclptwtm.html

C#:   public / protected / private / internal
来源：http://hz.jqgufenzy.top/gtiwniylpp.html

[G11] getter / setter
来源：http://hz.zhengqikj.top/gtxhdgbbfj.html

Py:   @property 与 @x.setter
来源：http://hz.yueranfly.top/gtbrbhdakq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtacmtfxql.html

JS:   get name() { return this._name; }
来源：http://hz.tian-w.cn/gtnivhymkc.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenlongwang.top/gtwkxdmiru.html

Java: public String getName() { return name; }
来源：http://hz.hysaishi.cn/gtqdqbtcxi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hfpthk.cn/gtdlrmirbc.html

Ruby: attr_accessor :name
来源：http://hz.ivvv.top/gtrykuubkl.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gtjjlvmgrj.html

[G12] 对象转字符串
来源：http://hz.xinyue.icu/gtkhfbinux.html

Py:   def __str__(self): return self.name
来源：http://hz.vqdsnc.cn/gtvcbljtcj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtryijkksm.html

JS:   toString() { return this.name; }
来源：http://hz.kuanghao11.cn/gtrjopcrvh.html

TS:   toString(): string { return this.name; }
来源：http://hz.ivvv.top/gtvvsaxocc.html

Java: @Override public String toString() { return name; }
来源：http://hz.ivvv.top/gtczzflywg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtyxdppxet.html

Ruby: def to_s; @name; end
来源：http://hz.svipenyu.cn/gtpywcnmnh.html

C#:   public override string ToString() => Name;
来源：http://hz.fzhhl.top/gtapvzlvks.html

[G13] 判断对象类型
来源：http://hz.tanke756.top/gtfcpxqquu.html

Py:   isinstance(u, User)
来源：http://hz.ehwqpu.com/gtorohxtee.html

PHP:  $u instanceof User
来源：http://hz.hfpthk.cn/gtpksbwpjy.html

JS:   u instanceof User
来源：http://hz.daria6918.cn/gtwdjivlgb.html

TS:   u instanceof User
来源：http://hz.yangfankeji.com/gttqudzmok.html

Java: u instanceof User
来源：http://hz.jinghuilouyu.cn/gtyocyfmbi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cqqwz.cn/gtgokvrkjc.html

Ruby: u.is_a?(User)
来源：http://hz.hongshengwenyu.top/gtxkmctcdy.html

C#:   u is User
来源：http://hz.yueranfly.top/gthppapwsh.html

[G14] 数据类 / record
来源：http://hz.nanxuanxn.top/gtsxfdexey.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yuanzhike.top/gtwjiyrttt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhongyouzk.top/gtqenaphfk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgfzy.top/gtmugdduuq.html

TS:   type User = { name: string; age: number };
来源：http://hz.daxiang520.top/gtpmbcvohu.html

Java: record User(String name, int age) {}
来源：http://hz.zhiwuduotai.top/gtpvxhbttr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangdashe.top/gtnnrocpmn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yongpay.top/gtkibbldoi.html

C#:   record User(string Name, int Age);
来源：http://hz.xuetiantiany.cn/gtbchaivkn.html

[G15] 枚举
来源：http://hz.ydzc1.top/gtqnrbmgzf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuanzhike.top/gtlyqnxvdg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yuanzhike.top/gtdjnwcdqo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hongshengwenyu.top/gtmrrzkdpz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ywan-chungtsiang.top/gtnegocqyx.html

Java: enum Color { RED, GREEN }
来源：http://hz.yanxiufei.cn/gtgtkbnqph.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xuanzx.com/gtjdfdphzk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.redwolf501.top/gtooaeivbh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gthyyxxzly.html

[G16] 对象转数组 / 字典
来源：http://hz.yangfankeji.com/gtncgkelqa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guannengcc.top/gtgbepvwzd.html

PHP:  get_object_vars($obj);
来源：http://hz.yueranfly.top/gtxcldapyb.html

JS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gthmkufqke.html

TS:   Object.entries(obj)
来源：http://hz.hongshengwenyu.top/gthkglvnnj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shzxlz.cn/gtxujrtivo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgufenzy.top/gtgzmoywww.html

Ruby: obj.instance_variables
来源：http://hz.tianlin.xyz/gtxqdpqsrs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhengqikj.top/gtbtwqzqye.html

================================================================================
来源：http://hz.yueranfly.top/gtwmmhaexj.html

H. 异常与错误处理
来源：http://hz.shuidangran.top/gtqmguhxej.html

================================================================================
来源：http://hz.haohaochexian.top/gtrydibitu.html

[H01] try / catch 基础
来源：http://hz.xuetiantiany.cn/gtlolpgbkv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jianghu66.top/gtbglaaawz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ivvv.top/gtprbdcmsu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ehwqpu.com/gtrpfjetne.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gtpgctlzbo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daria6918.cn/gtmlwhcmvb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.smart0.xyz/gtgmldavsr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jyoumei.cn/gtwohoomww.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shanyushiyangkeji.top/gtvwgogogs.html

[H02] finally / ensure 收尾
来源：http://hz.chenlongwang.top/gtpbvpwzbg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hywenlv.cn/gtbjfwbmno.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtjcbmbgcl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtvgdghhva.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtowttkqyy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtpwupmeix.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cucudq.cn/gtradvpwyo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenjidiqi.icu/gtjxtaenad.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xziqi.cn/gtfvdrhbaa.html

[H03] 主动抛出异常
来源：http://hz.jqgfzy.top/gtoklyaojl.html

Py:   raise ValueError("错误信息")
来源：http://hz.shanyushiyangtech.top/gtalenkytr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yonumen.top/gtcicxnczv.html

JS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtqlkxhbwv.html

TS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtihvjhxia.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtfnewnzeg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.0kj1m.cn/gtmlqqscla.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yueranfly.top/gtzolowjak.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtyugmrfyv.html

[H04] 自定义异常类型
来源：http://hz.yvedp.cn/gtiowpaliy.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258.top/gtsvifapax.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gtvfdzvhnh.html

JS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gtwlhzijar.html

TS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gtaqpyyvhc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.birdmap.top/gtognjxylb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yuxming.cn/gtehdwqjsg.html

Ruby: class MyError < StandardError; end
来源：http://hz.daxiang520.top/gtvyhrieip.html

C#:   class MyException : Exception {}
来源：http://hz.zhiwuduotai.top/gtikcukvvg.html

[H05] 捕获特定类型
来源：http://hz.zdqjudy.top/gtizrcvmxc.html

Py:   except ValueError as e:
来源：http://hz.ybcxt.top/gtherroopv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.c1oappe.top/gtcvpplsmk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtkwtaujey.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.svipenyu.cn/gtxsnzmwbd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tianlin.xyz/gtkpgopxie.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtczyztbkx.html

Ruby: rescue ArgumentError => e
来源：http://hz.gaohongyu789.top/gtxltdbbry.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenzaomai.com/gtorqovyql.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangdashe.top/gtwiwrohwt.html

Py:   value = d.get("k") or default
来源：http://hz.kuanghao11.cn/gtzzrfdidd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.vqdsnc.cn/gtvazjmqvg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtdkytwazy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xylfe.cn/gtrvpborib.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shzxlz.cn/gtdnvbaosl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yonumen.top/gtqzrynzkb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sysykeji.top/gteundpstz.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangshuangyany.cn/gtnbdzsjee.html

[H07] 断言
来源：http://hz.haohaochexian.top/gtnrglrljf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xylfe.cn/gtamdrefbn.html

PHP:  assert($x > 0);
来源：http://hz.hnxiangtu.top/gtmohxnkcv.html

JS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtbhifhyxk.html

TS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtyyeaohhf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hywenlv.cn/gtlbcqenzd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gaohongyu789.top/gtzhcsplxk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sysykeji.top/gtojkferwr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.haohaochexian.top/gtquqthvnv.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gtfcrgfbfy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yongpay.top/gtotehxvlq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yanxiufei.cn/gtdlgdvrsi.html

JS:   e.message;  e.stack
来源：http://hz.9152youxi.cn/gtaiknmroe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigufen.top/gtowbfrhjl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhaomingkeji.xyz/gtlsajglss.html

Go:   err.Error()
来源：http://hz.zhixingplan.top/gtrhsnultb.html


<!-- 参考信息 -->