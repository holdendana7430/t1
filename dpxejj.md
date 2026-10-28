代发 wailian999

Ruby: File.delete("a.txt")
来源：http://hz.yueranfly.top/gthupyqvth.html

C#:   File.Delete("a.txt");
来源：http://hz.iojbl.cn/gtcvrfcesk.html

[F07] 创建目录（含多级）
来源：http://hz.cdnleiting.top/gtjovslzty.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shuidangran.top/gtgemdoxnf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yonumen.top/gtfkgtwetd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gttdpjcaux.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guowangkeji.top/gtytvdyijn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yvedp.cn/gtgytrwwrn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.fzhhl.top/gtlsxyunme.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ydzc1.top/gtpseucoes.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.haohaochexian.top/gtmadaietd.html

[F08] 遍历目录
来源：http://hz.yj20258.top/gtdibqjfzy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xingfuxueyuan.xyz/gtboivjccl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnqzz.top/gtnpfcwytc.html

JS:   fs.readdirSync("dir")
来源：http://hz.pycfn.com/gtfzglcbdg.html

TS:   fs.readdirSync("dir")
来源：http://hz.dianchejie.cn/gtxclamusk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtjnazfrqi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yvedp.cn/gtiryhyusb.html

Ruby: Dir.children("dir")
来源：http://hz.sufxvd.cn/gtcgxkioph.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuxming.cn/gtfzffuway.html

[F09] 获取文件大小
来源：http://hz.ehwqpu.com/gtwuujyevt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtnftyzgql.html

PHP:  filesize("a.txt");
来源：http://hz.jinqigfzy.top/gtveocqqmz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtagnrfill.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yongpay.top/gtscozvrto.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtdewnwguz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nwbrower.top/gtnnizvcyo.html

Ruby: File.size("a.txt")
来源：http://hz.haohaochexian.top/gtgwwzomww.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxinkj.top/gtgsgrbrzo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tanke756.top/gtexjcckih.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtfziuefhu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sxryk.cn/gtxwrahbut.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtkwalyfzk.html

TS:   path.extname("a.txt")
来源：http://hz.zhixingplan.top/gtclelgfca.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hywenlv.cn/gtjpbilzyq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.316326.xyz/gtgdofemly.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtrzqbgftd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenzaomai.com/gtzavigkvb.html

[F11] 复制与移动文件
来源：http://hz.havefunace.top/gtianhxsbh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtprbdtjbx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yueranfly.top/gtcyjnfpie.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtlhfnycyv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtzbmddgea.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jyoumei.cn/gtforbpccu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.andypj.xyz/gtnqmwpppi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtdmtxhrtx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yanxiufei.cn/gtxbarnlhp.html

[F12] CSV 读写
来源：http://hz.cheryme.top/gtmqzrnpnp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zdqjudy.top/gtvvvempnw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxinkj.top/gtfaydcupw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258.top/gtzuqveibt.html

TS:   // 同上
来源：http://hz.shanyushiyangtech.top/gtdllctllw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtklecjdfz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.andypj.xyz/gtxqrqzljq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hfpthk.cn/gtkkslffmp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xuetiantiany.cn/gtcjhgmoge.html

================================================================================
来源：http://hz.yanxiufei.cn/gtkajgzlsp.html

G. 面向对象
来源：http://hz.guowangkeji.top/gtvesjehpa.html

================================================================================
来源：http://hz.nanxuanxn.top/gtvpmgblyt.html

[G01] 定义类
来源：http://hz.mhx1999.top/gtnfcfowsl.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtequvshbq.html

PHP:  class User {}
来源：http://hz.jyoumei.cn/gtkdaxkkmd.html

JS:   class User {}
来源：http://hz.daxiang520.top/gtjoxxienp.html

TS:   class User { name: string = ""; }
来源：http://hz.xingfuxueyuan.xyz/gtggkpjszv.html

Java: class User {}
来源：http://hz.316326.xyz/gthqrhbkmr.html

Go:   type User struct { Name string }
来源：http://hz.ydjk.org.cn/gtekrdgrvi.html

Ruby: class User; end
来源：http://hz.hfpthk.cn/gtdkrkiixu.html

C#:   class User {}
来源：http://hz.ivvv.top/gtgysjsqrt.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtxiiauyvg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.pengpengdd.cyou/gtlaaxlswz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhengqikj.top/gtrrorufio.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.birdmap.top/gtvwwzoovp.html

TS:   constructor(public name: string) {}
来源：http://hz.yongpay.top/gtrcyxmawr.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj202588.top/gtaolnqzcr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ywan-chungtsiang.top/gtlmythewu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cdnleiting.top/gtbqlqqket.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhengqikj.top/gtfmkqvdzg.html

[G03] 实例属性
来源：http://hz.fzhhl.top/gtnpvinvee.html

Py:   self.name = "x"
来源：http://hz.jinqigufen.top/gtsjpickdf.html

PHP:  public string $name = "x";
来源：http://hz.zdqjudy.top/gtooeqbdnh.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtxlpalyjf.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtcnynwucu.html

Java: private String name;
来源：http://hz.smart0.xyz/gtrdhkzpek.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ywan-chungtsiang.top/gttwddudrz.html

Ruby: @name = "x"
来源：http://hz.chenlongwang.top/gtrrskanab.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.svipenyu.cn/gterrzhczy.html

[G04] 定义方法
来源：http://hz.yangfankeji.com/gtgtjxvmbh.html

Py:   def greet(self): return self.name
来源：http://hz.hnqzz.top/gtclhtajlk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtblsglual.html

JS:   greet() { return this.name; }
来源：http://hz.haohaochexian.top/gtiwkaddgb.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtbbwdzida.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gtsbjvqezq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtwajbsdlm.html

Ruby: def greet; @name; end
来源：http://hz.316326.xyz/gttoojnsnw.html

C#:   public string Greet() => Name;
来源：http://hz.vqdsnc.cn/gtgibepflw.html

[G05] 继承
来源：http://hz.chenzaomai.com/gtbmdkolho.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gtlduipebp.html

PHP:  class Admin extends User {}
来源：http://hz.guowangkeji.top/gtvzuwvmvx.html

JS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtdmcojubi.html

TS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtgcmnsggg.html

Java: class Admin extends User {}
来源：http://hz.tanke756.top/gttazkymtp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydzc1.top/gtvrndybem.html

Ruby: class Admin < User; end
来源：http://hz.shuidangran.top/gtkuytugqc.html

C#:   class Admin : User {}
来源：http://hz.nanxinkj.top/gtrijhblul.html

[G06] 重写方法
来源：http://hz.hnxiangtu.top/gtjlsniufx.html

Py:   def greet(self): return "admin"
来源：http://hz.wangdashe.top/gtucmvclli.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gtqxzsbgyu.html

JS:   greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gtkxxeqjkl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtbaeevjvi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.mhx1999.top/gtkcddbtca.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.pengpengdd.cyou/gtwvmdsaos.html

Ruby: def greet; "admin"; end
来源：http://hz.yongpay.top/gtbrrmdmar.html

C#:   public override string Greet() => "admin";
来源：http://hz.meibo888.top/gtgvoospey.html

[G07] 调用父类方法
来源：http://hz.xziqi.cn/gttzffhbbv.html

Py:   super().greet()
来源：http://hz.52xcode.cn/gtnmbtbytb.html

PHP:  parent::greet();
来源：http://hz.xinyue.icu/gtxucslbwv.html

JS:   super.greet();
来源：http://hz.fengsongda.top/gtrcanrlua.html

TS:   super.greet();
来源：http://hz.nanxinkj.top/gtvsmewqdg.html

Java: super.greet();
来源：http://hz.chenjidiqi.icu/gtrhwumugn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhijiandao.cn/gtdmbknfrz.html

Ruby: super
来源：http://hz.gzhubu.top/gtucpwqmzp.html

C#:   base.Greet();
来源：http://hz.snrcjt.cn/gtztlyljef.html

[G08] 静态方法与属性
来源：http://hz.zhixingplan.top/gtyemdccik.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tian-w.cn/gtzqzwjkqt.html

PHP:  public static function f() {}
来源：http://hz.xuetiantiany.cn/gtfbtyzjki.html

JS:   static f() {}
来源：http://hz.zhoulong.xyz/gtoxyxqljc.html

TS:   static f(): void {}
来源：http://hz.shuidangran.top/gtmcvrgbyy.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtbsevkofv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ybcxt.top/gtsbhvubhq.html

Ruby: def self.f; end
来源：http://hz.fengsongda.top/gttfbiictd.html

C#:   public static void F() {}
来源：http://hz.zhongyouzk.top/gtynjhyqdy.html

[G09] 接口 / 抽象类
来源：http://hz.hnqzz.top/gtmimbsgku.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nwbrower.top/gtklwpbvso.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhijiandao.cn/gtiiltstfp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.daxiang520.top/gtbywtznpq.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtnzdlxtzy.html

Java: interface Shape { double area(); }
来源：http://hz.chenzaomai.com/gtibcykebh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.bjfxy.top/gtufiveaxr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenjidiqi.icu/gtgqywzsiy.html

C#:   interface IShape { double Area(); }
来源：http://hz.hywenlv.cn/gtaztkzhoc.html

[G10] 访问控制
来源：http://hz.yongpay.top/gtqsqzjfhl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daxiang520.top/gthdnslvst.html

PHP:  public / protected / private
来源：http://hz.wangshuangyany.cn/gtuvhjdqpf.html

JS:   #private 字段；其余公开
来源：http://hz.vqdsnc.cn/gtnvfjzlht.html

TS:   public / protected / private
来源：http://hz.dianchejie.cn/gtmjvghoob.html

Java: public / protected / private / 默认包级
来源：http://hz.zycfv.cn/gtnalpsvoq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.iojbl.cn/gtrfzxhhbc.html

Ruby: public / protected / private
来源：http://hz.svipenyu.cn/gtuozgepkt.html

C#:   public / protected / private / internal
来源：http://hz.yvedp.cn/gtwpxsydma.html

[G11] getter / setter
来源：http://hz.zycfv.cn/gtkypmdzau.html

Py:   @property 与 @x.setter
来源：http://hz.jinqigufen.top/gtjpfklcwd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtnkmczxsv.html

JS:   get name() { return this._name; }
来源：http://hz.hammf.cn/gtefyxphza.html

TS:   get name(): string { return this._name; }
来源：http://hz.yonumen.top/gtueiaoeis.html

Java: public String getName() { return name; }
来源：http://hz.jyoumei.cn/gtvzzokdjc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.9152youxi.cn/gtyvngjblx.html

Ruby: attr_accessor :name
来源：http://hz.nwbrower.top/gthsfadwfb.html

C#:   public string Name { get; set; }
来源：http://hz.zdqjudy.top/gtzobpcavd.html

[G12] 对象转字符串
来源：http://hz.aibaodan.cn/gtkjuyjvgv.html

Py:   def __str__(self): return self.name
来源：http://hz.hysaishi.cn/gtrpddykdo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtazdgnptf.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gthbfzpgsh.html

TS:   toString(): string { return this.name; }
来源：http://hz.gaohongyu789.top/gtploultkl.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangdashe.top/gtnmbsvltc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtylpvdnrc.html

Ruby: def to_s; @name; end
来源：http://hz.jyoumei.cn/gthqqhkttd.html

C#:   public override string ToString() => Name;
来源：http://hz.xinyue.icu/gtfjwnazau.html

[G13] 判断对象类型
来源：http://hz.chenjidiqi.icu/gtpctyegyg.html

Py:   isinstance(u, User)
来源：http://hz.tian-w.cn/gtsalsdnsy.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangtech.top/gtqmhfqris.html

JS:   u instanceof User
来源：http://hz.wangdashe.top/gtuotqpdof.html

TS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtrlluchar.html

Java: u instanceof User
来源：http://hz.cucudq.cn/gtdctwlnko.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinyuanbaomall.cn/gtrvhiawqa.html

Ruby: u.is_a?(User)
来源：http://hz.xuanzx.com/gtaqxdgxri.html

C#:   u is User
来源：http://hz.yuxming.cn/gtngtjrobe.html

[G14] 数据类 / record
来源：http://hz.nanxinkj.top/gtekpkgjpj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.c1oappe.top/gthxochgzz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.daria6918.cn/gtefsjwngi.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuetiantiany.cn/gtukexfgwn.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinghuilouyu.cn/gtvxeyrryu.html

Java: record User(String name, int age) {}
来源：http://hz.wangdashe.top/gtuonezhqh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daxiang520.top/gtzlyjxbas.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ybcxt.top/gtlddopgxx.html

C#:   record User(string Name, int Age);
来源：http://hz.zhijiandao.cn/gtwimtoqow.html

[G15] 枚举
来源：http://hz.cashguo.top/gtmkzriqxh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj202588.top/gthzryijdp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gtxmvoobfx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.mhx1999.top/gtyukdnfhb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtcjfqkiga.html

Java: enum Color { RED, GREEN }
来源：http://hz.meibo888.top/gtkpqsgkxa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cucudq.cn/gtahkdbshg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gotoacloud.top/gtmwjplegf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtpfuzspzc.html

[G16] 对象转数组 / 字典
来源：http://hz.smart0.xyz/gtvnfjpntl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.bjfxy.top/gtkhcrxgtx.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gtlxmwbliy.html

JS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtvuwqfhsx.html

TS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtcxnhkjjc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ywan-chungtsiang.top/gtozanilzr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xuetiantiany.cn/gtbjypjtvj.html

Ruby: obj.instance_variables
来源：http://hz.52xcode.cn/gtgvwgsrxt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenjidiqi.icu/gtzfkzlgtu.html

================================================================================
来源：http://hz.cdnleiting.top/gtufruhhaj.html

H. 异常与错误处理
来源：http://hz.guannengcc.top/gtbqwsiacr.html

================================================================================
来源：http://hz.redwolf501.top/gthmpzowmn.html

[H01] try / catch 基础
来源：http://hz.andypj.xyz/gtnxvaitak.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yvedp.cn/gtbvzsjxqh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.vqdsnc.cn/gtgntyrgqo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gttekcrnfq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.iojbl.cn/gtuxxzcimh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hywenlv.cn/gtkfraopfa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shangyingyoupin.top/gtkkomaggp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.havefunace.top/gtsfqqised.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nanxuanxn.top/gtczludsri.html

[H02] finally / ensure 收尾
来源：http://hz.feifeiyinyue.top/gtfalkecup.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.quarkkingdee.top/gtbfiyjlmo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtovcsnahl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtxmwrwvxw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtyiqqthav.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtgouemhga.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.quarkkingdee.top/gtaswmaofm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.fengsongda.top/gtpryndnie.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hysaishi.cn/gtqagkhopk.html

[H03] 主动抛出异常
来源：http://hz.zhoulong.xyz/gttokcbowg.html

Py:   raise ValueError("错误信息")
来源：http://hz.tian-w.cn/gtkwrqutqs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtvpvlhpir.html

JS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtnbjivmyi.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtyowlzdrf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtfpcoritg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sysykeji.top/gtbrdjitls.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sufxvd.cn/gtenvsvqdv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtgjbiopgl.html

[H04] 自定义异常类型
来源：http://hz.chenjidiqi.icu/gtokcopkcb.html

Py:   class MyError(Exception): pass
来源：http://hz.jyoumei.cn/gttpdujegp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258888.top/gtzrtwmubw.html

JS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtsfgsgute.html

TS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtzluawvaf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.andypj.xyz/gtgyceqrdk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.wangdashe.top/gtoqrcyxrx.html

Ruby: class MyError < StandardError; end
来源：http://hz.sweek.top/gttrxlkmkl.html

C#:   class MyException : Exception {}
来源：http://hz.fzhhl.top/gtgprinmrn.html

[H05] 捕获特定类型
来源：http://hz.quarkkingdee.top/gtdrfheldl.html

Py:   except ValueError as e:
来源：http://hz.snrcjt.cn/gtafdbgmkw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cqqwz.cn/gtmkuvfkyf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gtoyjfhadu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtotflgzsy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.kuanghao11.cn/gtjvdrzflh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shangyingyoupin.top/gtkvmbhwth.html

Ruby: rescue ArgumentError => e
来源：http://hz.gotoacloud.top/gtjpsioeka.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dashuyun.cn/gtiyyngvfl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuanzx.com/gtujxddbmy.html

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gtufedgecz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cucudq.cn/gtbixdzbko.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gtdfjgljtz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gtbcatuxur.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ehwqpu.com/gtnaimgakb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cqqwz.cn/gtkiibylbi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shangyingyoupin.top/gtgbmkmvry.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenzaomai.com/gtjrfddphr.html

[H07] 断言
来源：http://hz.jinqigufen.top/gtzchtvnwz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sxryk.cn/gtfhbbbigj.html

PHP:  assert($x > 0);
来源：http://hz.0kj1m.cn/gtysfuowio.html

JS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtjykduyke.html

TS:   console.assert(x > 0);
来源：http://hz.yvedp.cn/gtqqqqbmdr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.feifeiyinyue.top/gtgwaojnno.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aibaodan.cn/gtacbwqrna.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.birdmap.top/gtguknrsmd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tianlin.xyz/gtsrnyphpn.html

[H08] 获取错误信息与堆栈
来源：http://hz.yonumen.top/gtwxhvrrvy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.fzhhl.top/gtlmkceifx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.snrcjt.cn/gtmfrifmac.html

JS:   e.message;  e.stack
来源：http://hz.0kj1m.cn/gtinfuaihl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.0kj1m.cn/gtoqtqjicx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhijiandao.cn/gtmcrtulfl.html

Go:   err.Error()
来源：http://hz.wangdashe.top/gtozafbfhh.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhengqikj.top/gtabeqwpvg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.9152youxi.cn/gtfyjreuzh.html

[H09] 带错误码的异常
来源：http://hz.meibo888.top/gtghvaazaj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhongyouzk.top/gtxbvlebef.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.52xcode.cn/gttfhzgwxi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.snrcjt.cn/gtibscussg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhengqikj.top/gtbxfnfspt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinyuanbaomall.cn/gtpcndodlc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhixingplan.top/gtqzbfazxu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dianchejie.cn/gtkffzjzij.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shuidangran.top/gtvvfwoxpr.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtxpjpswmr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hywenlv.cn/gtzlmelzft.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ywan-chungtsiang.top/gtekwtxzvd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnxiangtu.top/gtizkgtjuj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtywsslaix.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.52xcode.cn/gtedffyiap.html

Go:   defer f.Close()
来源：http://hz.redwolf501.top/gtmskvesry.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aizwys.cn/gtmwvciuod.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.haohaochexian.top/gtqlbditkh.html

================================================================================
来源：http://hz.fzhhl.top/gtqexxezcz.html

I. 正则表达式
来源：http://hz.zhengqikj.top/gtyeovvloy.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcrpgruqi.html

[I01] 判断是否匹配
来源：http://hz.pengpengdd.cyou/gtwdxsvaki.html


<!-- 参考信息 -->