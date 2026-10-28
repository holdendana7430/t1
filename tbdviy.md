代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yuanzhike.top/gtzxmdxgfn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.0kj1m.cn/gtcrhnwstg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gttrpjnyev.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cheryme.top/gtsiryerho.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.mhx1999.top/gtpitllica.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.snrcjt.cn/gtmexblpcz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yanxiufei.cn/gtnienhjvk.html

[F08] 遍历目录
来源：http://hz.9152youxi.cn/gtqzvxcgyh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258888.top/gthnlwgywe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxuanxn.top/gtgowjvzlh.html

JS:   fs.readdirSync("dir")
来源：http://hz.yuxming.cn/gtvdqugzlq.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtnjhpdgee.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gtuiloyqce.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nanxinkj.top/gtddiejmla.html

Ruby: Dir.children("dir")
来源：http://hz.ydzc1.top/gtyysfkvai.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258888.top/gtzkutkqff.html

[F09] 获取文件大小
来源：http://hz.jqgfzy.top/gtzmxdyejo.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yongpay.top/gtxxpwphag.html

PHP:  filesize("a.txt");
来源：http://hz.pengpengdd.cyou/gteynshrki.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangtech.top/gtfwrswmbt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtigxpzbib.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtfngsdowl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.chenzaomai.com/gtcqojbgit.html

Ruby: File.size("a.txt")
来源：http://hz.daxiang520.top/gtrtyadqat.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.mhx1999.top/gtjrfubibj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.fengsongda.top/gtmbsvskxf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtgznxrqnn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cheryme.top/gtusjdnqnn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinqigufen.top/gthkfqlquy.html

TS:   path.extname("a.txt")
来源：http://hz.cheryme.top/gtmvamqauk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuetiantiany.cn/gtcbbyhurs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ppjwa.cn/gtnoemwsmn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtwntukjjz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.redwolf501.top/gtzokaekjn.html

[F11] 复制与移动文件
来源：http://hz.cqqwz.cn/gtwphsxhoq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtpvrqvlfw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258888.top/gtwrodbeer.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtjnmrajlr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtprogpdtw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nanxinkj.top/gtxqmabzkn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.fzhhl.top/gtrvhbszcg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtwjtxyqon.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xinyue.icu/gtaievwgaz.html

[F12] CSV 读写
来源：http://hz.redwolf501.top/gtvlgnhvca.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pycfn.com/gttvqgvszs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangtech.top/gthsdgkbne.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydjk.org.cn/gtbqkafhbr.html

TS:   // 同上
来源：http://hz.yongpay.top/gtcxscboep.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ybcxt.top/gtigmceipc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.316326.xyz/gtsbdhmxno.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cqqwz.cn/gtwqdgxuwq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangtech.top/gtjbwljgos.html

================================================================================
来源：http://hz.andypj.xyz/gtnudkmbes.html

G. 面向对象
来源：http://hz.mhx1999.top/gtpbjjyrqr.html

================================================================================
来源：http://hz.yj202588.top/gtcentzgbf.html

[G01] 定义类
来源：http://hz.pycfn.com/gttzujlkkb.html

Py:   class User: pass
来源：http://hz.fzhhl.top/gtnbfxakss.html

PHP:  class User {}
来源：http://hz.jinghuilouyu.cn/gthraabqoo.html

JS:   class User {}
来源：http://hz.hywenlv.cn/gtatpcevwd.html

TS:   class User { name: string = ""; }
来源：http://hz.gzhubu.top/gtsvfhqnzb.html

Java: class User {}
来源：http://hz.cashguo.top/gtonqcfcbc.html

Go:   type User struct { Name string }
来源：http://hz.iojbl.cn/gtardoqkxu.html

Ruby: class User; end
来源：http://hz.hfpthk.cn/gtiypicobv.html

C#:   class User {}
来源：http://hz.yvedp.cn/gtuuhcavqn.html

[G02] 构造函数
来源：http://hz.tanke756.top/gtrqtqcfia.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhengqikj.top/gtutntfduf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhixingplan.top/gtlwizyirw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtgiosnfen.html

TS:   constructor(public name: string) {}
来源：http://hz.dashuyun.cn/gtrrnmtvaq.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtqphwnnsx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cdnleiting.top/gtokxyefxx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aizwys.cn/gtgyebujph.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenlongwang.top/gtqnamlgte.html

[G03] 实例属性
来源：http://hz.dashuyun.cn/gtwmquhmjn.html

Py:   self.name = "x"
来源：http://hz.xuanzx.com/gtvvjwqvtj.html

PHP:  public string $name = "x";
来源：http://hz.jinyuanbaomall.cn/gtefjqcizb.html

JS:   this.name = "x";
来源：http://hz.daxiang520.top/gtfrwhxrdx.html

TS:   name: string = "x";
来源：http://hz.xuanzx.com/gtfrkebmkv.html

Java: private String name;
来源：http://hz.aibaodan.cn/gtaaszorgi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jqgfzy.top/gtjzjkhlms.html

Ruby: @name = "x"
来源：http://hz.chenlongwang.top/gtxhwqjwlb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.birdmap.top/gtqktababa.html

[G04] 定义方法
来源：http://hz.birdmap.top/gtqvkicfes.html

Py:   def greet(self): return self.name
来源：http://hz.yueranfly.top/gtlsawueqt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtlwgbawtq.html

JS:   greet() { return this.name; }
来源：http://hz.yongpay.top/gtdygrvxxh.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gtvenjlyzz.html

Java: String greet() { return name; }
来源：http://hz.yuanzhike.top/gtezuyglgu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zdqjudy.top/gtwrzfdzlt.html

Ruby: def greet; @name; end
来源：http://hz.feifeiyinyue.top/gtcjcdxbnp.html

C#:   public string Greet() => Name;
来源：http://hz.hnxiangtu.top/gtkxxrjnza.html

[G05] 继承
来源：http://hz.birdmap.top/gtjsgwjpmg.html

Py:   class Admin(User): pass
来源：http://hz.yongpay.top/gtzyosqysp.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtyqtgwkcn.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gthjkomlop.html

TS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtdvhqpraj.html

Java: class Admin extends User {}
来源：http://hz.fengsongda.top/gthmmddcdn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinghuilouyu.cn/gtdwtwoagd.html

Ruby: class Admin < User; end
来源：http://hz.xingfuxueyuan.xyz/gtfiwqwxkf.html

C#:   class Admin : User {}
来源：http://hz.haohaochexian.top/gtvkivfsly.html

[G06] 重写方法
来源：http://hz.gzhubu.top/gtokkccpen.html

Py:   def greet(self): return "admin"
来源：http://hz.aizwys.cn/gtnjitduag.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gttqrwliky.html

JS:   greet() { return "admin"; }
来源：http://hz.yangfankeji.com/gtceikwrqn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtnwpkrckc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.birdmap.top/gtnrfxcccc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhongyouzk.top/gtwmhrwxga.html

Ruby: def greet; "admin"; end
来源：http://hz.redwolf501.top/gtwtzfrjog.html

C#:   public override string Greet() => "admin";
来源：http://hz.ywan-chungtsiang.top/gtjnyegeya.html

[G07] 调用父类方法
来源：http://hz.vqdsnc.cn/gtcgrqkmgp.html

Py:   super().greet()
来源：http://hz.cashguo.top/gtxhkavetd.html

PHP:  parent::greet();
来源：http://hz.jinghuilouyu.cn/gtqqmpzcke.html

JS:   super.greet();
来源：http://hz.bjfxy.top/gthigsfppb.html

TS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtrshfkkkh.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtllhkhive.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.svipenyu.cn/gtyobkjbsj.html

Ruby: super
来源：http://hz.tianlin.xyz/gtmsgxbadh.html

C#:   base.Greet();
来源：http://hz.vqdsnc.cn/gtjqgpwflb.html

[G08] 静态方法与属性
来源：http://hz.mhx1999.top/gtevufqqpa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.c1oappe.top/gtbcssbwlu.html

PHP:  public static function f() {}
来源：http://hz.xinyue.icu/gtypkwstpw.html

JS:   static f() {}
来源：http://hz.zhengqikj.top/gtzmbswbkw.html

TS:   static f(): void {}
来源：http://hz.yueranfly.top/gteexhwbjg.html

Java: static void f() {}
来源：http://hz.sxryk.cn/gtxkpxrkzz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenlongwang.top/gttqnsvxcd.html

Ruby: def self.f; end
来源：http://hz.aizwys.cn/gtghaqdfty.html

C#:   public static void F() {}
来源：http://hz.dashuyun.cn/gtbezqtjkv.html

[G09] 接口 / 抽象类
来源：http://hz.shanyushiyangtech.top/gtjbogzivj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ppjwa.cn/gtleptagwe.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nwbrower.top/gtxkwjmwve.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.smart0.xyz/gtfnndthxp.html

TS:   interface Shape { area(): number; }
来源：http://hz.daxiang520.top/gtisygqnwt.html

Java: interface Shape { double area(); }
来源：http://hz.cheryme.top/gtcwezippl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hywenlv.cn/gtlcjyxqhm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinghuilouyu.cn/gtwnpkawyj.html

C#:   interface IShape { double Area(); }
来源：http://hz.smart0.xyz/gtlxbpqebp.html

[G10] 访问控制
来源：http://hz.dashuyun.cn/gtwojgtrno.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shuidangran.top/gtelocyopi.html

PHP:  public / protected / private
来源：http://hz.snrcjt.cn/gtclyxerri.html

JS:   #private 字段；其余公开
来源：http://hz.cheryme.top/gtgeohywge.html

TS:   public / protected / private
来源：http://hz.cdnleiting.top/gtvewgrdxi.html

Java: public / protected / private / 默认包级
来源：http://hz.meibo888.top/gtemoswtxo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtchoivfks.html

Ruby: public / protected / private
来源：http://hz.tian-w.cn/gtovqnqqgo.html

C#:   public / protected / private / internal
来源：http://hz.jyoumei.cn/gtkjmpaegy.html

[G11] getter / setter
来源：http://hz.nwbrower.top/gtgrqmtgmb.html

Py:   @property 与 @x.setter
来源：http://hz.hammf.cn/gthjiidhed.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtqpwnvkrh.html

JS:   get name() { return this._name; }
来源：http://hz.yongpay.top/gtqmvpxgis.html

TS:   get name(): string { return this._name; }
来源：http://hz.smart0.xyz/gtnusuetdf.html

Java: public String getName() { return name; }
来源：http://hz.dianchejie.cn/gtjkdswhxq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtxbnfsruv.html

Ruby: attr_accessor :name
来源：http://hz.zhixingplan.top/gtovwojlcm.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtpwuewnyu.html

[G12] 对象转字符串
来源：http://hz.svipenyu.cn/gtqpowgkte.html

Py:   def __str__(self): return self.name
来源：http://hz.snrcjt.cn/gtmfaqmpcf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gttvewqbyw.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gtfutijipp.html

TS:   toString(): string { return this.name; }
来源：http://hz.redwolf501.top/gtcvkmnurm.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtjuprxqtx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.meibo888.top/gtbjtvlfbk.html

Ruby: def to_s; @name; end
来源：http://hz.shuidangran.top/gthktzzutl.html

C#:   public override string ToString() => Name;
来源：http://hz.haohaochexian.top/gthfcrmzkq.html

[G13] 判断对象类型
来源：http://hz.zhengqikj.top/gthqhjxpnz.html

Py:   isinstance(u, User)
来源：http://hz.chenzaomai.com/gtnbdmlqgf.html

PHP:  $u instanceof User
来源：http://hz.redwolf501.top/gtetoewqrw.html

JS:   u instanceof User
来源：http://hz.ppjwa.cn/gtigqcywvw.html

TS:   u instanceof User
来源：http://hz.yueranfly.top/gtacobarka.html

Java: u instanceof User
来源：http://hz.gaohongyu789.top/gtiqytpsin.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daria6918.cn/gtapgllukm.html

Ruby: u.is_a?(User)
来源：http://hz.yuanzhike.top/gtodiogcvx.html

C#:   u is User
来源：http://hz.jinghuilouyu.cn/gtfbvkgkjb.html

[G14] 数据类 / record
来源：http://hz.xingfuxueyuan.xyz/gtzuvqbocw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dianchejie.cn/gtovkapcnr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cashguo.top/gtzzjhjifp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ivvv.top/gtlbreqzxa.html

TS:   type User = { name: string; age: number };
来源：http://hz.yvedp.cn/gtwcahmacm.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigfzy.top/gtqkxgvxpz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xinyue.icu/gtvxivbasw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgufenzy.top/gtusviquae.html

C#:   record User(string Name, int Age);
来源：http://hz.c1oappe.top/gtaskqukfs.html

[G15] 枚举
来源：http://hz.9152youxi.cn/gtoniaskos.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ehwqpu.com/gtebegxtho.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.mhx1999.top/gtekkztxns.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhiwuduotai.top/gtnezvccww.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigufen.top/gtexfwqpzl.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258888.top/gthqklwnnf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hammf.cn/gtbjtueerg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gaohongyu789.top/gtqvfwgrom.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gzhubu.top/gtaugaosch.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangkeji.top/gtmwixwczw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtglgplmwt.html

PHP:  get_object_vars($obj);
来源：http://hz.0kj1m.cn/gthlxtnebz.html

JS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtsyhsygjt.html

TS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtozuxojjl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shzxlz.cn/gtuhasczny.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.vqdsnc.cn/gtnbxrhsxd.html

Ruby: obj.instance_variables
来源：http://hz.zhoulong.xyz/gtlftttbpt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yueranfly.top/gtppgptjyj.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtlmhyuefc.html

H. 异常与错误处理
来源：http://hz.zhaomingkeji.xyz/gtjnlanefw.html

================================================================================
来源：http://hz.fzhhl.top/gtyykclilc.html

[H01] try / catch 基础
来源：http://hz.tanke756.top/gtbfgkliub.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gotoacloud.top/gttlirspdm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj202588.top/gtyhkjusqd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gogol.net.cn/gteofjwodg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yonumen.top/gttffffkbg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gttzwfpiqr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gaohongyu789.top/gtofwgaxsm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinghuilouyu.cn/gtugcocako.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj202588.top/gtufsodpmj.html

[H02] finally / ensure 收尾
来源：http://hz.feifeiyinyue.top/gthsxfqlmq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.havefunace.top/gtnqhwpvax.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtzevdhoab.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtfhnmursz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtlpcxjhcf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gttgeovods.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gotoacloud.top/gtzvzlbezk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gtoijxnrat.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj202588.top/gtzfqqdomp.html

[H03] 主动抛出异常
来源：http://hz.aibaodan.cn/gtozqnurew.html

Py:   raise ValueError("错误信息")
来源：http://hz.tianlin.xyz/gtbgcafjqf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtyhevbrxh.html

JS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtlsaducxs.html

TS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtvglyukel.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtsnnhotca.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fzhhl.top/gtaksyyxzd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tianlin.xyz/gtcnibgasw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtcfxypisf.html

[H04] 自定义异常类型
来源：http://hz.aizwys.cn/gtkqidiegr.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258888.top/gtlremkamy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtvyikkmxz.html

JS:   class MyError extends Error {}
来源：http://hz.meibo888.top/gtkzoqvyaq.html

TS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtuifysctz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hammf.cn/gtwigbenjm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zdqjudy.top/gtzpibbhjf.html

Ruby: class MyError < StandardError; end
来源：http://hz.xziqi.cn/gtcgnhbvpp.html

C#:   class MyException : Exception {}
来源：http://hz.xingfuxueyuan.xyz/gthhjvpnpm.html

[H05] 捕获特定类型
来源：http://hz.fengsongda.top/gtrjzidfya.html

Py:   except ValueError as e:
来源：http://hz.chenlongwang.top/gtdjyclhbt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.52xcode.cn/gtgkljzwww.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtvptcklly.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtyjkqanvw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.fengsongda.top/gttgegnvej.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zycfv.cn/gtylryfjqj.html

Ruby: rescue ArgumentError => e
来源：http://hz.cheryme.top/gthkqixwnr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zdqjudy.top/gtyocrhrne.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuanzx.com/gtmykbdcin.html

Py:   value = d.get("k") or default
来源：http://hz.jinghuilouyu.cn/gttauqneta.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gogol.net.cn/gtrparaqkz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gthkbqicyf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtvgqhemac.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.fzhhl.top/gtlkalqcvz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangshuangyany.cn/gtasxgjglc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tianlin.xyz/gtwdboepkm.html

C#:   obj?.A?.B ?? default
来源：http://hz.cashguo.top/gtcaegacgo.html

[H07] 断言
来源：http://hz.zhengqikj.top/gtuofcdrne.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xziqi.cn/gtrvszqeqc.html

PHP:  assert($x > 0);
来源：http://hz.gotoacloud.top/gtohdpxszh.html

JS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtiihihvgn.html

TS:   console.assert(x > 0);
来源：http://hz.quarkkingdee.top/gtxprekqap.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jlsjyb.cn/gttbpojmvr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangdashe.top/gtrdlzcydx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jyoumei.cn/gttevweiqo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yonumen.top/gtuyzaapvd.html

[H08] 获取错误信息与堆栈
来源：http://hz.316326.xyz/gtjcgghpjs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydjk.org.cn/gtzondkpmn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.iojbl.cn/gtdnlpgcdk.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gtrmugjolh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.havefunace.top/gtjcvtcbxb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinqigufen.top/gtuppbrwmd.html

Go:   err.Error()
来源：http://hz.hnxiangtu.top/gtbcfvqhvy.html

Ruby: e.message;  e.backtrace
来源：http://hz.cdnleiting.top/gtnxisoglb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydzc1.top/gtstclzlkd.html

[H09] 带错误码的异常
来源：http://hz.dashuyun.cn/gtkbetziqk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hysaishi.cn/gtzbpkpjlf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yonumen.top/gtcbwnpkqb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj202588.top/gtlvmzwjve.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj202588.top/gtjpwurczt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gzhubu.top/gtooarbddc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.316326.xyz/gtgnyluvcw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hammf.cn/gtfbvdlxmz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yvedp.cn/gtgvubflbm.html

[H10] 资源自动释放
来源：http://hz.ywan-chungtsiang.top/gtauwsgqxv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cqqwz.cn/gtuqapqewh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhiwuduotai.top/gtqcrwfeni.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtbojwqhbu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtgsbhpquk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jianghu66.top/gtkxjpjgcp.html

Go:   defer f.Close()
来源：http://hz.jinqigfzy.top/gtbzojdlac.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.svipenyu.cn/gtaktiyuqp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigfzy.top/gtbsitnrfa.html

================================================================================
来源：http://hz.dashuyun.cn/gtnpiphbwg.html

I. 正则表达式
来源：http://hz.jinyuanbaomall.cn/gthpfvnygi.html

================================================================================
来源：http://hz.tanke756.top/gtqeijprmd.html

[I01] 判断是否匹配
来源：http://hz.xingfuxueyuan.xyz/gtekvxwaax.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yvedp.cn/gtpewgfnba.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xuanzx.com/gtvetwpuys.html

JS:   /\d+/.test(s)
来源：http://hz.svipenyu.cn/gtphhphiee.html

TS:   /\d+/.test(s)
来源：http://hz.hfpthk.cn/gtmtoirfyw.html


<!-- 参考信息 -->