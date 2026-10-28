代发 wailian999

C#:   File.Exists("a.txt")
来源：http://hz.smart0.xyz/gtrgxgxtad.html

[F06] 删除文件
来源：http://hz.pycfn.com/gtsjgicwsw.html

Py:   os.remove("a.txt")
来源：http://hz.ppjwa.cn/gtlqqxhros.html

PHP:  unlink("a.txt");
来源：http://hz.birdmap.top/gtbkikengx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xinyue.icu/gtfcybyixa.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtckybdwcm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtqbgbslqe.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxinkj.top/gtdslakmud.html

Ruby: File.delete("a.txt")
来源：http://hz.hongshengwenyu.top/gtngxlzoyz.html

C#:   File.Delete("a.txt");
来源：http://hz.andypj.xyz/gtjnzefcmc.html

[F07] 创建目录（含多级）
来源：http://hz.cashguo.top/gtiphrxhqe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hammf.cn/gtnhcyipdc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.9152youxi.cn/gtfmbdhzzf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangkeji.top/gtgnsbaged.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cqqwz.cn/gtfqpmekqf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gogol.net.cn/gtfdkagjnu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigufen.top/gtrspmwjlh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cdnleiting.top/gtntrmjsir.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cqqwz.cn/gtdfmmmhdk.html

[F08] 遍历目录
来源：http://hz.snrcjt.cn/gtyfjancva.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ppjwa.cn/gtptkvdvte.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.meibo888.top/gtawinfmyb.html

JS:   fs.readdirSync("dir")
来源：http://hz.smart0.xyz/gtxzaefzeb.html

TS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtggaldrwe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhaomingkeji.xyz/gthiowubgo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xziqi.cn/gtuwocnqhj.html

Ruby: Dir.children("dir")
来源：http://hz.dianchejie.cn/gtmyyqpabz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gtvrujypon.html

[F09] 获取文件大小
来源：http://hz.redwolf501.top/gtstbwleqc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ydzc1.top/gtjdeitdnk.html

PHP:  filesize("a.txt");
来源：http://hz.aizwys.cn/gtddzdecem.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtnirncxhv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtnnytlbqj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtzmfbczxt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sysykeji.top/gtvyftxybm.html

Ruby: File.size("a.txt")
来源：http://hz.xinyue.icu/gtejwrxtkh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhijiandao.cn/gtsaobwsfn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shanyushiyangtech.top/gtkgwquwid.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtvkbtfiqg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.52xcode.cn/gtibxauuxq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtouxnvapy.html

TS:   path.extname("a.txt")
来源：http://hz.nanxinkj.top/gtebeqjbls.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhongyouzk.top/gtamjkzrse.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.redwolf501.top/gtfipozqvi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtmaemyyay.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.birdmap.top/gtsilbwcrk.html

[F11] 复制与移动文件
来源：http://hz.52xcode.cn/gtieoeeqbd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtgxmjgtgw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pycfn.com/gtddcbxyez.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtyfajyybd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtdnkikmjm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yuxming.cn/gtylreeuqx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hongshengwenyu.top/gtgyuutltk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gttowratiq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.52xcode.cn/gtnmiupmpk.html

[F12] CSV 读写
来源：http://hz.yj20258.top/gtbxnfnzhb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.snrcjt.cn/gtiiexubdz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtwexxnmaw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ehwqpu.com/gthxcbalac.html

TS:   // 同上
来源：http://hz.jyoumei.cn/gthvysztun.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hnxiangtu.top/gtnadxryjp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangkeji.top/gtddpydseo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhaomingkeji.xyz/gtpgxnpsjg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258.top/gtzlpmcuve.html

================================================================================
来源：http://hz.c1oappe.top/gtxornhqut.html

G. 面向对象
来源：http://hz.andypj.xyz/gtxskxnmzs.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtbnlnwieh.html

[G01] 定义类
来源：http://hz.hnxiangtu.top/gtblwnegfi.html

Py:   class User: pass
来源：http://hz.mhx1999.top/gtcquhwubg.html

PHP:  class User {}
来源：http://hz.shangyingyoupin.top/gtfzdswlmp.html

JS:   class User {}
来源：http://hz.jlsjyb.cn/gtyvliqqwz.html

TS:   class User { name: string = ""; }
来源：http://hz.hysaishi.cn/gtelwesune.html

Java: class User {}
来源：http://hz.zhijiandao.cn/gtbcgocfwd.html

Go:   type User struct { Name string }
来源：http://hz.jlsjyb.cn/gtpyaduvbd.html

Ruby: class User; end
来源：http://hz.jqgufenzy.top/gtblryzxtc.html

C#:   class User {}
来源：http://hz.sysykeji.top/gtspxdrgnw.html

[G02] 构造函数
来源：http://hz.dianchejie.cn/gthqxekcpl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangkeji.top/gtmlwqvrno.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yongpay.top/gtgnlbtuxx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hammf.cn/gtenpcnbqf.html

TS:   constructor(public name: string) {}
来源：http://hz.zhoulong.xyz/gtxewuontu.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtryiksfpc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenlongwang.top/gtsslpelvn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pycfn.com/gtsbwjommi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.guannengcc.top/gtsopnpzhz.html

[G03] 实例属性
来源：http://hz.52xcode.cn/gtcfnawjfv.html

Py:   self.name = "x"
来源：http://hz.snrcjt.cn/gtrjbrkjir.html

PHP:  public string $name = "x";
来源：http://hz.jqgfzy.top/gtevwcdxkn.html

JS:   this.name = "x";
来源：http://hz.bjfxy.top/gtvunbbrpj.html

TS:   name: string = "x";
来源：http://hz.aibaodan.cn/gtomvpwtaz.html

Java: private String name;
来源：http://hz.daxiang520.top/gtsjlzwdsw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.andypj.xyz/gtnvvrmhco.html

Ruby: @name = "x"
来源：http://hz.cashguo.top/gtzmjbttyd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnxiangtu.top/gtqefeunor.html

[G04] 定义方法
来源：http://hz.shzxlz.cn/gtclseasxe.html

Py:   def greet(self): return self.name
来源：http://hz.ehwqpu.com/gtkpepublm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtpkierpxo.html

JS:   greet() { return this.name; }
来源：http://hz.vqdsnc.cn/gtokyqosep.html

TS:   greet(): string { return this.name; }
来源：http://hz.yonumen.top/gtvwfrhpfv.html

Java: String greet() { return name; }
来源：http://hz.daxiang520.top/gtvzhidkqf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sufxvd.cn/gtofhopnol.html

Ruby: def greet; @name; end
来源：http://hz.dianchejie.cn/gtytoeonfo.html

C#:   public string Greet() => Name;
来源：http://hz.yanxiufei.cn/gtiqapzjqp.html

[G05] 继承
来源：http://hz.ydzc1.top/gtaotnmflh.html

Py:   class Admin(User): pass
来源：http://hz.sufxvd.cn/gtozjdscfq.html

PHP:  class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtlqbvrasn.html

JS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtwzjkecut.html

TS:   class Admin extends User {}
来源：http://hz.9152youxi.cn/gtpisgondr.html

Java: class Admin extends User {}
来源：http://hz.sysykeji.top/gttidbmwwx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258888.top/gtqyxypbyp.html

Ruby: class Admin < User; end
来源：http://hz.zhoulong.xyz/gtatfsmqkp.html

C#:   class Admin : User {}
来源：http://hz.fzhhl.top/gtebkggvmd.html

[G06] 重写方法
来源：http://hz.chenjidiqi.icu/gtadbbmovs.html

Py:   def greet(self): return "admin"
来源：http://hz.wangshuangyany.cn/gtygxkbcnj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtkteqtbkk.html

JS:   greet() { return "admin"; }
来源：http://hz.316326.xyz/gtxvptirlx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtihfempmu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtthqlruiy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gzhubu.top/gtzymvjyqm.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtvwdoykoq.html

C#:   public override string Greet() => "admin";
来源：http://hz.jlsjyb.cn/gtcuvuznsc.html

[G07] 调用父类方法
来源：http://hz.yvedp.cn/gtdxbrngjh.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtqqwifrub.html

PHP:  parent::greet();
来源：http://hz.zhijiandao.cn/gtngzdyegw.html

JS:   super.greet();
来源：http://hz.nwbrower.top/gtwgfwxtpq.html

TS:   super.greet();
来源：http://hz.yj202588.top/gtskrlbbfl.html

Java: super.greet();
来源：http://hz.dianchejie.cn/gtetiymqrt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daxiang520.top/gtyhisaqyi.html

Ruby: super
来源：http://hz.zhiwuduotai.top/gtdlssouvs.html

C#:   base.Greet();
来源：http://hz.dashuyun.cn/gtkybkdaom.html

[G08] 静态方法与属性
来源：http://hz.xingfuxueyuan.xyz/gtsafaosbp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.c1oappe.top/gttwzqmrdw.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangkeji.top/gtehgtaokk.html

JS:   static f() {}
来源：http://hz.ehwqpu.com/gtelfylrsr.html

TS:   static f(): void {}
来源：http://hz.zhixingplan.top/gtpxojlzyn.html

Java: static void f() {}
来源：http://hz.tianlin.xyz/gtyboztvpv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.smart0.xyz/gtzllyrjhe.html

Ruby: def self.f; end
来源：http://hz.nwbrower.top/gtwnwrrybb.html

C#:   public static void F() {}
来源：http://hz.hammf.cn/gtxmndsgtb.html

[G09] 接口 / 抽象类
来源：http://hz.gotoacloud.top/gtifnlvqwo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hfpthk.cn/gtldmgsvba.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jyoumei.cn/gtxaddqfmf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.bjfxy.top/gtlfhdmpic.html

TS:   interface Shape { area(): number; }
来源：http://hz.dashuyun.cn/gtudmmdfgb.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangtech.top/gtxkoqgzwz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnqzz.top/gtdvifubtw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.havefunace.top/gtkudltfso.html

C#:   interface IShape { double Area(); }
来源：http://hz.yanxiufei.cn/gtdpfhxhnz.html

[G10] 访问控制
来源：http://hz.jqgfzy.top/gtfhehvvjy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.redwolf501.top/gtgjjbgjyf.html

PHP:  public / protected / private
来源：http://hz.fzhhl.top/gttdecdfib.html

JS:   #private 字段；其余公开
来源：http://hz.redwolf501.top/gthvivfwng.html

TS:   public / protected / private
来源：http://hz.pengpengdd.cyou/gtvoamxsiv.html

Java: public / protected / private / 默认包级
来源：http://hz.gotoacloud.top/gtxpdywzhm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.feifeiyinyue.top/gtfttmhlny.html

Ruby: public / protected / private
来源：http://hz.c1oappe.top/gtgumjjxnq.html

C#:   public / protected / private / internal
来源：http://hz.svipenyu.cn/gtbbctzwxh.html

[G11] getter / setter
来源：http://hz.ppjwa.cn/gthkoaplsm.html

Py:   @property 与 @x.setter
来源：http://hz.xylfe.cn/gtkosulijh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtnqgyavkn.html

JS:   get name() { return this._name; }
来源：http://hz.sysykeji.top/gtczddifwe.html

TS:   get name(): string { return this._name; }
来源：http://hz.pengpengdd.cyou/gtfzjxrxgt.html

Java: public String getName() { return name; }
来源：http://hz.hammf.cn/gticzfqimy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gtyewzwmge.html

Ruby: attr_accessor :name
来源：http://hz.ppjwa.cn/gtpmvrvsox.html

C#:   public string Name { get; set; }
来源：http://hz.chenzaomai.com/gtcwgnxrxv.html

[G12] 对象转字符串
来源：http://hz.xziqi.cn/gtleanweqh.html

Py:   def __str__(self): return self.name
来源：http://hz.zhaomingkeji.xyz/gtdsuaopjj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.birdmap.top/gtdipvjzcq.html

JS:   toString() { return this.name; }
来源：http://hz.redwolf501.top/gtkssdiyak.html

TS:   toString(): string { return this.name; }
来源：http://hz.snrcjt.cn/gtorsmimgm.html

Java: @Override public String toString() { return name; }
来源：http://hz.daria6918.cn/gtlqtowgdx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cqqwz.cn/gtvmewfeyc.html

Ruby: def to_s; @name; end
来源：http://hz.zhijiandao.cn/gtnwotekoi.html

C#:   public override string ToString() => Name;
来源：http://hz.cdnleiting.top/gtfztaddhh.html

[G13] 判断对象类型
来源：http://hz.9152youxi.cn/gtfjfekbht.html

Py:   isinstance(u, User)
来源：http://hz.jiagoushi.top/gtsxuhufms.html

PHP:  $u instanceof User
来源：http://hz.xuetiantiany.cn/gtvdfrghlp.html

JS:   u instanceof User
来源：http://hz.guannengcc.top/gtyxwfvzho.html

TS:   u instanceof User
来源：http://hz.0kj1m.cn/gtyrehxcmt.html

Java: u instanceof User
来源：http://hz.svipenyu.cn/gtliappekj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.fengsongda.top/gtrahmxfip.html

Ruby: u.is_a?(User)
来源：http://hz.dashuyun.cn/gtzvajkjod.html

C#:   u is User
来源：http://hz.gaohongyu789.top/gtqypwqfiz.html

[G14] 数据类 / record
来源：http://hz.vqdsnc.cn/gtsmrlsgwn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xylfe.cn/gtstmkjtxr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aibaodan.cn/gtillpqljb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhaomingkeji.xyz/gtsmmjsyyu.html

TS:   type User = { name: string; age: number };
来源：http://hz.sysykeji.top/gttuksguuh.html

Java: record User(String name, int age) {}
来源：http://hz.nwbrower.top/gtkwneqsib.html

Go:   type User struct { Name string; Age int }
来源：http://hz.52xcode.cn/gthoosfyqj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yangfankeji.com/gteoxacagf.html

C#:   record User(string Name, int Age);
来源：http://hz.wangdashe.top/gtiszywade.html

[G15] 枚举
来源：http://hz.jqgfzy.top/gtsczcxdbm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jlsjyb.cn/gtwjlrbjgo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shuidangran.top/gtrfjuejai.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yueranfly.top/gtqvuxisny.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gotoacloud.top/gtgnqolfld.html

Java: enum Color { RED, GREEN }
来源：http://hz.hfpthk.cn/gtgaldgiuf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydzc1.top/gtvjrcbafp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hongshengwenyu.top/gtolbqufdq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtsntisjax.html

[G16] 对象转数组 / 字典
来源：http://hz.svipenyu.cn/gtgclgktbl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhixingplan.top/gtusunivlb.html

PHP:  get_object_vars($obj);
来源：http://hz.aibaodan.cn/gtkyucdfrg.html

JS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtvajsfiks.html

TS:   Object.entries(obj)
来源：http://hz.tian-w.cn/gtqdkrvkjo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhaomingkeji.xyz/gtdneskvzr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.mhx1999.top/gtqdhtygax.html

Ruby: obj.instance_variables
来源：http://hz.daria6918.cn/gtrajdksfb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gtataslpqz.html

================================================================================
来源：http://hz.yuxming.cn/gtfsakzivj.html

H. 异常与错误处理
来源：http://hz.smart0.xyz/gtuigofhgu.html

================================================================================
来源：http://hz.andypj.xyz/gtzyfjrbcm.html

[H01] try / catch 基础
来源：http://hz.zhiwuduotai.top/gtcaijmnhf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yongpay.top/gtskcmgqls.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yonumen.top/gtgxyqcvdg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.havefunace.top/gtcvbvalvz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.smart0.xyz/gtdaugmgdo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jyoumei.cn/gtwybgcnxx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nwbrower.top/gtgjmvpwcq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aibaodan.cn/gtyutkoitb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yangfankeji.com/gtgbyonxdt.html

[H02] finally / ensure 收尾
来源：http://hz.pycfn.com/gtnsssmeqk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gaohongyu789.top/gtwypkuecj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtukcdfvfw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtcqigveki.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtwbsbauue.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtkbcecaqf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.52xcode.cn/gtnomntmhw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.iojbl.cn/gtfmruqgoq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.svipenyu.cn/gtceuzfzcw.html

[H03] 主动抛出异常
来源：http://hz.nwbrower.top/gtzwnbtnkn.html

Py:   raise ValueError("错误信息")
来源：http://hz.sufxvd.cn/gtczqqqpkw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sweek.top/gtcvgginxv.html

JS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gtaymnbync.html

TS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtwcarokwc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtfnxcurdh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenlongwang.top/gtglezlwgo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.c1oappe.top/gtsbqjjobu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ivvv.top/gtrubnomvj.html

[H04] 自定义异常类型
来源：http://hz.xziqi.cn/gtowvsnrne.html

Py:   class MyError(Exception): pass
来源：http://hz.yvedp.cn/gtqunazcoe.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtyhhzbtqm.html

JS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gtmwtifsme.html

TS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gtodiwsbbj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cheryme.top/gtdfnfwvwt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.smart0.xyz/gtqeshpkcy.html

Ruby: class MyError < StandardError; end
来源：http://hz.cashguo.top/gtuturcwee.html

C#:   class MyException : Exception {}
来源：http://hz.ivvv.top/gtlagkhldo.html

[H05] 捕获特定类型
来源：http://hz.birdmap.top/gtvzirordf.html

Py:   except ValueError as e:
来源：http://hz.jiagoushi.top/gtasqatzqc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aizwys.cn/gtzfyejrlc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gtqfvtwehn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtnmtyvyjp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zycfv.cn/gtadbgcicb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cheryme.top/gtwdmzdbsg.html

Ruby: rescue ArgumentError => e
来源：http://hz.xylfe.cn/gtybexqxzs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhixingplan.top/gtanbuinmh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.andypj.xyz/gtaanmhump.html

Py:   value = d.get("k") or default
来源：http://hz.yongpay.top/gtrpjmeorb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtgbxuflqe.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gtkvserfyl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gtzmwzsuph.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenlongwang.top/gteeelxamn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dianchejie.cn/gtpchceoin.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtlghmngrj.html

C#:   obj?.A?.B ?? default
来源：http://hz.yueranfly.top/gtgbbewrwa.html

[H07] 断言
来源：http://hz.ehwqpu.com/gtrxwciizo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.daria6918.cn/gttuhczqli.html

PHP:  assert($x > 0);
来源：http://hz.52xcode.cn/gtbtbohacf.html

JS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtppyrwqbt.html

TS:   console.assert(x > 0);
来源：http://hz.52xcode.cn/gtkrcxjhau.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnqzz.top/gtkpaiyjmt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sysykeji.top/gtzptfisuv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yuanzhike.top/gtazpbzjha.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pycfn.com/gtngjqecch.html

[H08] 获取错误信息与堆栈
来源：http://hz.kuanghao11.cn/gtvozotgyk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.mhx1999.top/gtsxnfnibz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.0kj1m.cn/gtlnwipqql.html

JS:   e.message;  e.stack
来源：http://hz.yongpay.top/gtzcqhytam.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xuanzx.com/gtcmrbmynl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dashuyun.cn/gtyhejwnct.html

Go:   err.Error()
来源：http://hz.jiagoushi.top/gtlkibiekr.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnxiangtu.top/gtqwuuwxtx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ivvv.top/gtwtwefbbh.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangkeji.top/gtfxsiwhny.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jiagoushi.top/gtqwkkauqw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gtuzaizyrg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258888.top/gtnkfsiklb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hysaishi.cn/gtkohhcnse.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.snrcjt.cn/gthvsqywgn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hysaishi.cn/gtxaslkgsf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.aizwys.cn/gtnudsyvix.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangkeji.top/gtsebgaznc.html

[H10] 资源自动释放
来源：http://hz.gzhubu.top/gtlywgneqx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.birdmap.top/gtsmphvhds.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj202588.top/gtdtadqgrs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtqkmcycvm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.snrcjt.cn/gtcfejwfmu.html


<!-- 参考信息 -->