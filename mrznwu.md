代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xziqi.cn/gtvfnhywyo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258.top/gtuzsokuts.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuxming.cn/gtxpzkphji.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gotoacloud.top/gtzeatyjqs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhixingplan.top/gttavjtpcz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.wangdashe.top/gtvfhhidpx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daria6918.cn/gttpyvrocp.html

[F08] 遍历目录
来源：http://hz.daxiang520.top/gtgwcgduqs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cashguo.top/gtnnxzpebk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.guowangkeji.top/gtyajsysvb.html

JS:   fs.readdirSync("dir")
来源：http://hz.tian-w.cn/gtqnzcnorc.html

TS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtapokxxzd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258.top/gtlmoxjeli.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hywenlv.cn/gtsadqxqpb.html

Ruby: Dir.children("dir")
来源：http://hz.xylfe.cn/gthutfzgnn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cqqwz.cn/gtefckbcdz.html

[F09] 获取文件大小
来源：http://hz.xuanzx.com/gtunlktglz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.mhx1999.top/gtqatjiydz.html

PHP:  filesize("a.txt");
来源：http://hz.aizwys.cn/gtopigiilb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtebtwuwvb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.wangshuangyany.cn/gtyedtooon.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtpyrptrur.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ybcxt.top/gtpcvhvkkf.html

Ruby: File.size("a.txt")
来源：http://hz.havefunace.top/gtuobkgxoh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shuidangran.top/gtuecgnbob.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shangyingyoupin.top/gttcdfwywf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtyrbzvxhl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.snrcjt.cn/gtqlrjcekd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gotoacloud.top/gtejtisefg.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigfzy.top/gtuxfissai.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shzxlz.cn/gtbzxpocsf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aizwys.cn/gtzaskccww.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtjojsquav.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtstlmfubl.html

[F11] 复制与移动文件
来源：http://hz.fengsongda.top/gttklaxuvu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtlrwkxxwr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gtemsohjcl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtndsyllpw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtdeqzckru.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gaohongyu789.top/gtorkwohdo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhijiandao.cn/gtjheazofg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gteaztlfvp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pycfn.com/gthjwnpxlx.html

[F12] CSV 读写
来源：http://hz.jinyuanbaomall.cn/gtjxaaujdh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhengqikj.top/gtzyjkaafy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.bjfxy.top/gtdjcoybgq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.guowangkeji.top/gtkgmkmded.html

TS:   // 同上
来源：http://hz.hammf.cn/gtlykchkbv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.daxiang520.top/gttevgkfot.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gtsjeyurmw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xziqi.cn/gtrnfhvryo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangdashe.top/gtswnxigch.html

================================================================================
来源：http://hz.dianchejie.cn/gtkgktutok.html

G. 面向对象
来源：http://hz.shanyushiyangtech.top/gtlmpmcnsp.html

================================================================================
来源：http://hz.snrcjt.cn/gttgjytjlc.html

[G01] 定义类
来源：http://hz.shzxlz.cn/gttaaooqzk.html

Py:   class User: pass
来源：http://hz.cucudq.cn/gtmyiybdyw.html

PHP:  class User {}
来源：http://hz.yj202588.top/gtszvyedpv.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtkphewpqg.html

TS:   class User { name: string = ""; }
来源：http://hz.zhixingplan.top/gtawowpsjx.html

Java: class User {}
来源：http://hz.vqdsnc.cn/gtwbcdcjuj.html

Go:   type User struct { Name string }
来源：http://hz.fzhhl.top/gtjkesetxn.html

Ruby: class User; end
来源：http://hz.yj20258.top/gtobkrcbaz.html

C#:   class User {}
来源：http://hz.daxiang520.top/gtaozkyzlm.html

[G02] 构造函数
来源：http://hz.hysaishi.cn/gtpmsxyrer.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhoulong.xyz/gtqxctvhui.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxuanxn.top/gtkobxrgae.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.dashuyun.cn/gtwjilyyjt.html

TS:   constructor(public name: string) {}
来源：http://hz.jqgfzy.top/gtlyhjmnja.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj20258.top/gtgmqhqvfp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nwbrower.top/gtfsmbnpez.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gaohongyu789.top/gtynyuesvi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gaohongyu789.top/gtfwsttlwp.html

[G03] 实例属性
来源：http://hz.birdmap.top/gtmfploybe.html

Py:   self.name = "x"
来源：http://hz.yangfankeji.com/gtfmrqhyzy.html

PHP:  public string $name = "x";
来源：http://hz.cheryme.top/gtsrloqvea.html

JS:   this.name = "x";
来源：http://hz.zhaomingkeji.xyz/gthdlqyhlv.html

TS:   name: string = "x";
来源：http://hz.zhiwuduotai.top/gtfkygtodc.html

Java: private String name;
来源：http://hz.hywenlv.cn/gtpautqzmp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuanzhike.top/gtprdkvpuu.html

Ruby: @name = "x"
来源：http://hz.zhixingplan.top/gtyqxmpffs.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinqigfzy.top/gtaxmvxczh.html

[G04] 定义方法
来源：http://hz.chenlongwang.top/gtmqgezpjx.html

Py:   def greet(self): return self.name
来源：http://hz.guowangkeji.top/gtcpzwwyjj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtnsrglqqu.html

JS:   greet() { return this.name; }
来源：http://hz.iojbl.cn/gtjsfhazfz.html

TS:   greet(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtfglqezol.html

Java: String greet() { return name; }
来源：http://hz.quarkkingdee.top/gtsldskofv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shzxlz.cn/gteyzstxiq.html

Ruby: def greet; @name; end
来源：http://hz.jinqigufen.top/gtwyzhdqyn.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtmaimwsaj.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtlmrycgvd.html

Py:   class Admin(User): pass
来源：http://hz.jyoumei.cn/gtciltapgy.html

PHP:  class Admin extends User {}
来源：http://hz.aibaodan.cn/gtyxpuabon.html

JS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtzytkqxkp.html

TS:   class Admin extends User {}
来源：http://hz.cheryme.top/gtnmqdzkzr.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtaueaxpor.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yangfankeji.com/gtltzrmnjc.html

Ruby: class Admin < User; end
来源：http://hz.hywenlv.cn/gtnvwvrcqy.html

C#:   class Admin : User {}
来源：http://hz.pycfn.com/gtajikixur.html

[G06] 重写方法
来源：http://hz.bjfxy.top/gtyyravovj.html

Py:   def greet(self): return "admin"
来源：http://hz.shuidangran.top/gtmhkxsjvs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtlamrhcnt.html

JS:   greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gtxqlbizyl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.redwolf501.top/gtihsltzgm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtavybziea.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cashguo.top/gtoqbrpqgp.html

Ruby: def greet; "admin"; end
来源：http://hz.nwbrower.top/gtgdlsotib.html

C#:   public override string Greet() => "admin";
来源：http://hz.cqqwz.cn/gtjgdddjxi.html

[G07] 调用父类方法
来源：http://hz.vqdsnc.cn/gtxndfaord.html

Py:   super().greet()
来源：http://hz.wangdashe.top/gtnhtfdqqa.html

PHP:  parent::greet();
来源：http://hz.hfpthk.cn/gtswxndtcy.html

JS:   super.greet();
来源：http://hz.yongpay.top/gtdhwpqkly.html

TS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtlkxjekqy.html

Java: super.greet();
来源：http://hz.ehwqpu.com/gtgiytjbgk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tanke756.top/gtntnsjagl.html

Ruby: super
来源：http://hz.vqdsnc.cn/gtiurxzqil.html

C#:   base.Greet();
来源：http://hz.kuanghao11.cn/gtqrktpkyn.html

[G08] 静态方法与属性
来源：http://hz.316326.xyz/gtqlrdiaaa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guowangkeji.top/gtszviuvbq.html

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gtyfabpols.html

JS:   static f() {}
来源：http://hz.gotoacloud.top/gtnkdpqzcp.html

TS:   static f(): void {}
来源：http://hz.xylfe.cn/gtdxrcykjc.html

Java: static void f() {}
来源：http://hz.jinyuanbaomall.cn/gtthkvsbuv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nwbrower.top/gtqkdehsnd.html

Ruby: def self.f; end
来源：http://hz.dianchejie.cn/gtfzjfjbkl.html

C#:   public static void F() {}
来源：http://hz.hysaishi.cn/gtdvpleznb.html

[G09] 接口 / 抽象类
来源：http://hz.yangfankeji.com/gtuqsdeubb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinqigufen.top/gtdqtrdhqb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.smart0.xyz/gtxsulxqec.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.birdmap.top/gtfemmhpxp.html

TS:   interface Shape { area(): number; }
来源：http://hz.cqqwz.cn/gtytunwrpw.html

Java: interface Shape { double area(); }
来源：http://hz.zhiwuduotai.top/gtsmudawtp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.guowangkeji.top/gtrrzafemj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhiwuduotai.top/gtogpkbllu.html

C#:   interface IShape { double Area(); }
来源：http://hz.yonumen.top/gtiudnhmyz.html

[G10] 访问控制
来源：http://hz.ybcxt.top/gtbsnvoztt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.316326.xyz/gtopbozhkr.html

PHP:  public / protected / private
来源：http://hz.cqqwz.cn/gtfkasstdr.html

JS:   #private 字段；其余公开
来源：http://hz.gotoacloud.top/gtdujekruh.html

TS:   public / protected / private
来源：http://hz.pengpengdd.cyou/gtyshkhywt.html

Java: public / protected / private / 默认包级
来源：http://hz.kuanghao11.cn/gtfhsbtyhm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtscbpzhtl.html

Ruby: public / protected / private
来源：http://hz.birdmap.top/gtbyhcjbsw.html

C#:   public / protected / private / internal
来源：http://hz.sxryk.cn/gtljvhudnq.html

[G11] getter / setter
来源：http://hz.wangshuangyany.cn/gtmxpevfyf.html

Py:   @property 与 @x.setter
来源：http://hz.cheryme.top/gtpagtaffu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtuavtcrwi.html

JS:   get name() { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtetsluyem.html

TS:   get name(): string { return this._name; }
来源：http://hz.kuanghao11.cn/gtcpkllptl.html

Java: public String getName() { return name; }
来源：http://hz.jinghuilouyu.cn/gtgxuhhqvb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ybcxt.top/gtdjsspkbh.html

Ruby: attr_accessor :name
来源：http://hz.52xcode.cn/gtupwidqxm.html

C#:   public string Name { get; set; }
来源：http://hz.tian-w.cn/gtquoffijx.html

[G12] 对象转字符串
来源：http://hz.ydzc1.top/gtdgwurjlx.html

Py:   def __str__(self): return self.name
来源：http://hz.sxryk.cn/gtssimjnqn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtnnrplbxm.html

JS:   toString() { return this.name; }
来源：http://hz.xziqi.cn/gtrsjqqlmm.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtkiejawvi.html

Java: @Override public String toString() { return name; }
来源：http://hz.andypj.xyz/gtmcyznsoe.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.redwolf501.top/gtzyxhjuah.html

Ruby: def to_s; @name; end
来源：http://hz.wangshuangyany.cn/gtywbwamtp.html

C#:   public override string ToString() => Name;
来源：http://hz.ivvv.top/gtuuthnjed.html

[G13] 判断对象类型
来源：http://hz.meibo888.top/gttqpwvamd.html

Py:   isinstance(u, User)
来源：http://hz.quarkkingdee.top/gtconstgkt.html

PHP:  $u instanceof User
来源：http://hz.yuxming.cn/gtxybjeeuz.html

JS:   u instanceof User
来源：http://hz.tianlin.xyz/gtzjbakshr.html

TS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtizfxarar.html

Java: u instanceof User
来源：http://hz.yvedp.cn/gtdxmrjseo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangdashe.top/gtuqnujcgh.html

Ruby: u.is_a?(User)
来源：http://hz.aizwys.cn/gtnziohyom.html

C#:   u is User
来源：http://hz.jinyuanbaomall.cn/gtpznopann.html

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gtxtwdotds.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hywenlv.cn/gttglodtgl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sufxvd.cn/gttlenukme.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yvedp.cn/gtzgwjthgr.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigfzy.top/gttvtwubmm.html

Java: record User(String name, int age) {}
来源：http://hz.gogol.net.cn/gtdxgvrnwl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.svipenyu.cn/gtpddpebsy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.mhx1999.top/gtzqwlonnx.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gtdfvdhqiq.html

[G15] 枚举
来源：http://hz.sweek.top/gtmgqpftxq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yanxiufei.cn/gtgbvizocf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.c1oappe.top/gtqjhakiup.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgufenzy.top/gttupopfjz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtnrraukfo.html

Java: enum Color { RED, GREEN }
来源：http://hz.yueranfly.top/gtshnakxyh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hnxiangtu.top/gtjnrvuxph.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydzc1.top/gtjjprdnef.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtnftgaqoy.html

[G16] 对象转数组 / 字典
来源：http://hz.hywenlv.cn/gtflfthvnt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sweek.top/gtapsqfsfk.html

PHP:  get_object_vars($obj);
来源：http://hz.quarkkingdee.top/gtgelsljsw.html

JS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtqgrpezzw.html

TS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtddfiqplw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.svipenyu.cn/gtbkeoggpp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.9152youxi.cn/gtlxglylht.html

Ruby: obj.instance_variables
来源：http://hz.gzhubu.top/gtmlugpfua.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.iojbl.cn/gtlnjwxnmg.html

================================================================================
来源：http://hz.svipenyu.cn/gtwkyxrotx.html

H. 异常与错误处理
来源：http://hz.cucudq.cn/gtjllzlrbo.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtzxxnuune.html

[H01] try / catch 基础
来源：http://hz.316326.xyz/gtjgxtilnq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.daria6918.cn/gtwvdavslk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.bjfxy.top/gtwphbgdon.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sysykeji.top/gtfnlmwfmg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yongpay.top/gtquvvrohz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shuidangran.top/gtnytyzirn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258.top/gtpnqcpynr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xinyue.icu/gtxvoxfdfg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhoulong.xyz/gtwdzlhmri.html

[H02] finally / ensure 收尾
来源：http://hz.chenzaomai.com/gtcfuoafef.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuanzhike.top/gttpvrpvln.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtchuyhuqu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gthlqucztt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtddyrabhn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtmvaqrpje.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gteqccblju.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhongyouzk.top/gtyaemhtss.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.dashuyun.cn/gtopkpfico.html

[H03] 主动抛出异常
来源：http://hz.xingfuxueyuan.xyz/gtdrpxewcv.html

Py:   raise ValueError("错误信息")
来源：http://hz.gaohongyu789.top/gteuowcuaj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtizuckapd.html

JS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtvplsawwd.html

TS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtgsimubla.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtsslkhyzq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinyuanbaomall.cn/gttlmiebod.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aizwys.cn/gtgsksonlr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtdroptjwd.html

[H04] 自定义异常类型
来源：http://hz.yangfankeji.com/gtzdcnrobq.html

Py:   class MyError(Exception): pass
来源：http://hz.yongpay.top/gtyllzehig.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daxiang520.top/gtahkqzmpa.html

JS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gtcrlyyemt.html

TS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gtkxyguvap.html

Java: class MyException extends RuntimeException {}
来源：http://hz.mhx1999.top/gtwplezljw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.52xcode.cn/gttopvisaf.html

Ruby: class MyError < StandardError; end
来源：http://hz.cheryme.top/gthfyhavzy.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtuxejdtyu.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangkeji.top/gtekelahfu.html

Py:   except ValueError as e:
来源：http://hz.xylfe.cn/gtienhatao.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dashuyun.cn/gtdcbmwxag.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yangfankeji.com/gtjbcoedev.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtecfpkvka.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gtemeadvhe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258888.top/gtksbugswl.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxuanxn.top/gtdbwemorm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pengpengdd.cyou/gttkjfnqkq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yanxiufei.cn/gtljtjidgo.html

Py:   value = d.get("k") or default
来源：http://hz.quarkkingdee.top/gtvvesmpfl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangshuangyany.cn/gtwqhbfxqp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtigakypaz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtggbokvlj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj202588.top/gtfdgjubgx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.52xcode.cn/gtozdoqdya.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hongshengwenyu.top/gthgvdoxii.html

C#:   obj?.A?.B ?? default
来源：http://hz.jianghu66.top/gtwrljerqa.html

[H07] 断言
来源：http://hz.quarkkingdee.top/gtxgfvzisi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.daxiang520.top/gtzxyksqqz.html

PHP:  assert($x > 0);
来源：http://hz.ehwqpu.com/gtsfdfdeat.html

JS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gtsrzdgejl.html

TS:   console.assert(x > 0);
来源：http://hz.smart0.xyz/gtexpkxqlb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yonumen.top/gtmbzzyzxi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jlsjyb.cn/gtoozxmibi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cheryme.top/gthhjidqej.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shuidangran.top/gtlnxmsuku.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenlongwang.top/gtpjmttmza.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yanxiufei.cn/gtqajpsufv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.316326.xyz/gtrgugqemz.html

JS:   e.message;  e.stack
来源：http://hz.smart0.xyz/gtrvsfegyc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.52xcode.cn/gtavaojdov.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yonumen.top/gtbamhlgbu.html

Go:   err.Error()
来源：http://hz.jqgfzy.top/gtylfpaqyl.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gtredwbpok.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jlsjyb.cn/gtpvcgrkrg.html

[H09] 带错误码的异常
来源：http://hz.haohaochexian.top/gtfcgwltka.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuanzhike.top/gtwztptdrb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxuanxn.top/gtxllkqavw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fengsongda.top/gtofyxscsx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xingfuxueyuan.xyz/gtblpaisgb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zycfv.cn/gtbnhrrspg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhongyouzk.top/gtxesstjvr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.9152youxi.cn/gttozbpslw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.guowangkeji.top/gtdplmmwko.html

[H10] 资源自动释放
来源：http://hz.hongshengwenyu.top/gtticihipy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnxiangtu.top/gtttjdbyqr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydjk.org.cn/gtektzlnye.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gtiexmhzag.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtwishwred.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sufxvd.cn/gtwtubfcvn.html

Go:   defer f.Close()
来源：http://hz.yj202588.top/gtkomacckd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sxryk.cn/gtcvkpmhmq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhongyouzk.top/gtgqhuxfle.html

================================================================================
来源：http://hz.chenzaomai.com/gtcamnnqmw.html

I. 正则表达式
来源：http://hz.yongpay.top/gtyqentvvw.html

================================================================================
来源：http://hz.nanxuanxn.top/gtxeyulrwd.html

[I01] 判断是否匹配
来源：http://hz.zdqjudy.top/gtkdwqwlei.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zycfv.cn/gtqcljaixf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hammf.cn/gtrictiyho.html

JS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtkbnxtjrl.html

TS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtdjbmnlxv.html


<!-- 参考信息 -->