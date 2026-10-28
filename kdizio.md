代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guannengcc.top/gtacaoalom.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nwbrower.top/gtqvyfcypc.html

JS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtpwrjnasu.html

TS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtavgcspyi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtydygbrud.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.feifeiyinyue.top/gtrcpawcrr.html

Ruby: Dir.children("dir")
来源：http://hz.hfpthk.cn/gtqorufcaz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.c1oappe.top/gturfbeszt.html

[F09] 获取文件大小
来源：http://hz.316326.xyz/gtraqojkrm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hammf.cn/gtnsbzhroz.html

PHP:  filesize("a.txt");
来源：http://hz.chenlongwang.top/gtpcbxhwcz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.quarkkingdee.top/gtblospqse.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gtcivdgste.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtsmvqyxtt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hywenlv.cn/gterzgppuq.html

Ruby: File.size("a.txt")
来源：http://hz.shuidangran.top/gtnoqvdekq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtifsemtmi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jianghu66.top/gtkgfbgzxk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtqojfujyd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jqgfzy.top/gttmtdcyuo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtyueajgmy.html

TS:   path.extname("a.txt")
来源：http://hz.yuxming.cn/gtkhwxutkq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhengqikj.top/gtqumreqrf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtrhjhhilf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtbgvlfamr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yvedp.cn/gtzwpkdsah.html

[F11] 复制与移动文件
来源：http://hz.jinqigufen.top/gtbomvlqyd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtsyhqyblg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dianchejie.cn/gtesesztyi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtygbjwnhz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtxtalnhgx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cheryme.top/gtqqznhikt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.meibo888.top/gtvcwvxzrg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtrpjszmcf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sufxvd.cn/gtagksxcwu.html

[F12] CSV 读写
来源：http://hz.aizwys.cn/gtcziwjeed.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shangyingyoupin.top/gtcprfcela.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hfpthk.cn/gtmjcvyojr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.9152youxi.cn/gtzazhcaws.html

TS:   // 同上
来源：http://hz.wangshuangyany.cn/gtmugrgcqd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gtrcvqpyxx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guannengcc.top/gtjourlluj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhijiandao.cn/gtravnxxcv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cdnleiting.top/gtgtyrgbfz.html

================================================================================
来源：http://hz.tianlin.xyz/gtakaplius.html

G. 面向对象
来源：http://hz.sweek.top/gtxlujhekj.html

================================================================================
来源：http://hz.tanke756.top/gtgtmwovnh.html

[G01] 定义类
来源：http://hz.pycfn.com/gtuypuxnsq.html

Py:   class User: pass
来源：http://hz.tianlin.xyz/gthhdayemw.html

PHP:  class User {}
来源：http://hz.zhengqikj.top/gtnaxyrmtf.html

JS:   class User {}
来源：http://hz.jyoumei.cn/gtkcgiepqj.html

TS:   class User { name: string = ""; }
来源：http://hz.svipenyu.cn/gtozexebyc.html

Java: class User {}
来源：http://hz.daxiang520.top/gtetigogfo.html

Go:   type User struct { Name string }
来源：http://hz.nwbrower.top/gtiucibyol.html

Ruby: class User; end
来源：http://hz.hfpthk.cn/gtuewnoqyu.html

C#:   class User {}
来源：http://hz.pycfn.com/gtccxqmuvc.html

[G02] 构造函数
来源：http://hz.mhx1999.top/gtfwjdgqdp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhengqikj.top/gtekuaqudt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.316326.xyz/gtfgaxsjuj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtsuczdkfw.html

TS:   constructor(public name: string) {}
来源：http://hz.pycfn.com/gtuzenhdfb.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gtldbqgfnr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zycfv.cn/gtffnbqruq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtxjlhtjox.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jyoumei.cn/gtglajhmkt.html

[G03] 实例属性
来源：http://hz.fengsongda.top/gtsssgjazv.html

Py:   self.name = "x"
来源：http://hz.hnxiangtu.top/gtyygqqlcf.html

PHP:  public string $name = "x";
来源：http://hz.yongpay.top/gtlucpizzc.html

JS:   this.name = "x";
来源：http://hz.zhijiandao.cn/gtnrzefmzb.html

TS:   name: string = "x";
来源：http://hz.xingfuxueyuan.xyz/gtoplabxga.html

Java: private String name;
来源：http://hz.zdqjudy.top/gtktfeniel.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xziqi.cn/gtnrhnelcx.html

Ruby: @name = "x"
来源：http://hz.zhengqikj.top/gttdrzegck.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj20258.top/gtbidgsvuz.html

[G04] 定义方法
来源：http://hz.guannengcc.top/gtxmwxmtes.html

Py:   def greet(self): return self.name
来源：http://hz.kuanghao11.cn/gtplnjpttw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtpwborgtx.html

JS:   greet() { return this.name; }
来源：http://hz.hnxiangtu.top/gtfsfycute.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtnizksujy.html

Java: String greet() { return name; }
来源：http://hz.cheryme.top/gtciqdaebz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.andypj.xyz/gtubntfhcx.html

Ruby: def greet; @name; end
来源：http://hz.yueranfly.top/gtlupuwrfl.html

C#:   public string Greet() => Name;
来源：http://hz.ppjwa.cn/gtyffcntad.html

[G05] 继承
来源：http://hz.chenjidiqi.icu/gtbvtlbfik.html

Py:   class Admin(User): pass
来源：http://hz.svipenyu.cn/gtzslpwvej.html

PHP:  class Admin extends User {}
来源：http://hz.hywenlv.cn/gtgzboiovj.html

JS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gtqkwqmqyu.html

TS:   class Admin extends User {}
来源：http://hz.pycfn.com/gtbyyomxyd.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtnqzyftlf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.smart0.xyz/gtgxkvjsif.html

Ruby: class Admin < User; end
来源：http://hz.jinyuanbaomall.cn/gtyuhymeil.html

C#:   class Admin : User {}
来源：http://hz.316326.xyz/gtmfpgdpxm.html

[G06] 重写方法
来源：http://hz.nwbrower.top/gtesyxdhgc.html

Py:   def greet(self): return "admin"
来源：http://hz.cucudq.cn/gtdkkeagxj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.aizwys.cn/gteeskjbiv.html

JS:   greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtevbxcseu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.andypj.xyz/gtkaauimtg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj202588.top/gtwnapyhmp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dashuyun.cn/gttoawgxkz.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtluijfsqa.html

C#:   public override string Greet() => "admin";
来源：http://hz.aizwys.cn/gtxbimrjgn.html

[G07] 调用父类方法
来源：http://hz.cqqwz.cn/gtzqosrefx.html

Py:   super().greet()
来源：http://hz.yueranfly.top/gtuwfdppws.html

PHP:  parent::greet();
来源：http://hz.yvedp.cn/gtwdzsutjd.html

JS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtnhgdiwmx.html

TS:   super.greet();
来源：http://hz.iojbl.cn/gtunxctexk.html

Java: super.greet();
来源：http://hz.hammf.cn/gtshmviolm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xinyue.icu/gtzxlnttwc.html

Ruby: super
来源：http://hz.sxryk.cn/gtlmpbotjq.html

C#:   base.Greet();
来源：http://hz.shangyingyoupin.top/gtzeoviazv.html

[G08] 静态方法与属性
来源：http://hz.cashguo.top/gtgccgrvde.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dashuyun.cn/gtfsygmvbu.html

PHP:  public static function f() {}
来源：http://hz.zhaomingkeji.xyz/gtlakbxgdn.html

JS:   static f() {}
来源：http://hz.hnqzz.top/gtfilpnxmo.html

TS:   static f(): void {}
来源：http://hz.ydzc1.top/gtjejptuvc.html

Java: static void f() {}
来源：http://hz.xuanzx.com/gtscfsmjoy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hywenlv.cn/gteoijdbbe.html

Ruby: def self.f; end
来源：http://hz.smart0.xyz/gtjnrzjous.html

C#:   public static void F() {}
来源：http://hz.0kj1m.cn/gtrenipjvk.html

[G09] 接口 / 抽象类
来源：http://hz.ybcxt.top/gtwbqmgpnr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pengpengdd.cyou/gttlflfmto.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydzc1.top/gtkrprqzuz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigfzy.top/gtsjlztmyv.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuetiantiany.cn/gttlfsmxqw.html

Java: interface Shape { double area(); }
来源：http://hz.zhaomingkeji.xyz/gteisxuzzf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hywenlv.cn/gtsuhqwhbx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fzhhl.top/gtrwvplhwg.html

C#:   interface IShape { double Area(); }
来源：http://hz.316326.xyz/gtrfgkcwlf.html

[G10] 访问控制
来源：http://hz.zycfv.cn/gtxzxqtlli.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.snrcjt.cn/gtoiipjzmh.html

PHP:  public / protected / private
来源：http://hz.gaohongyu789.top/gtlheihxdb.html

JS:   #private 字段；其余公开
来源：http://hz.jianghu66.top/gtafsyggaw.html

TS:   public / protected / private
来源：http://hz.hammf.cn/gtofxkpgdw.html

Java: public / protected / private / 默认包级
来源：http://hz.jinqigufen.top/gtnwsigfqy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gogol.net.cn/gteznnerjq.html

Ruby: public / protected / private
来源：http://hz.sxryk.cn/gtfujyxbtr.html

C#:   public / protected / private / internal
来源：http://hz.jqgufenzy.top/gtykutkerw.html

[G11] getter / setter
来源：http://hz.chenlongwang.top/gtdfudahnh.html

Py:   @property 与 @x.setter
来源：http://hz.hammf.cn/gtacajrfvr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtckdlfcff.html

JS:   get name() { return this._name; }
来源：http://hz.snrcjt.cn/gtwycfvnkf.html

TS:   get name(): string { return this._name; }
来源：http://hz.dianchejie.cn/gtsxqiiweq.html

Java: public String getName() { return name; }
来源：http://hz.0kj1m.cn/gthamjnlnb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gzhubu.top/gtgizglezd.html

Ruby: attr_accessor :name
来源：http://hz.wangshuangyany.cn/gtwpiikjpd.html

C#:   public string Name { get; set; }
来源：http://hz.0kj1m.cn/gtrewulntr.html

[G12] 对象转字符串
来源：http://hz.tianlin.xyz/gtntqggdqm.html

Py:   def __str__(self): return self.name
来源：http://hz.shzxlz.cn/gtqcomxomz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtzzohxotf.html

JS:   toString() { return this.name; }
来源：http://hz.hnxiangtu.top/gtbcpitsuf.html

TS:   toString(): string { return this.name; }
来源：http://hz.ydjk.org.cn/gtuljkgwer.html

Java: @Override public String toString() { return name; }
来源：http://hz.jyoumei.cn/gtxstxgygc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xinyue.icu/gtlomvyvhj.html

Ruby: def to_s; @name; end
来源：http://hz.cheryme.top/gtgrzslyge.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxuanxn.top/gtwthwbzdd.html

[G13] 判断对象类型
来源：http://hz.yuxming.cn/gttjwcfwuo.html

Py:   isinstance(u, User)
来源：http://hz.iojbl.cn/gtqjqpwidt.html

PHP:  $u instanceof User
来源：http://hz.yvedp.cn/gtknefbeks.html

JS:   u instanceof User
来源：http://hz.jqgfzy.top/gtbrfqqrcv.html

TS:   u instanceof User
来源：http://hz.316326.xyz/gtlgamzqyo.html

Java: u instanceof User
来源：http://hz.aizwys.cn/gtcpobjoko.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuanzhike.top/gtwbcidmkq.html

Ruby: u.is_a?(User)
来源：http://hz.hnxiangtu.top/gtpyydcsdo.html

C#:   u is User
来源：http://hz.hywenlv.cn/gtuuwwehpi.html

[G14] 数据类 / record
来源：http://hz.bjfxy.top/gtkxdnkqxo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangkeji.top/gtcufzohww.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hnqzz.top/gtenogrixm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydzc1.top/gtzaktpsah.html

TS:   type User = { name: string; age: number };
来源：http://hz.fzhhl.top/gtghawmpjq.html

Java: record User(String name, int age) {}
来源：http://hz.dashuyun.cn/gttbinfezy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.redwolf501.top/gtfgekmpoq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jlsjyb.cn/gtgjzjpsqr.html

C#:   record User(string Name, int Age);
来源：http://hz.gotoacloud.top/gtwitbbohy.html

[G15] 枚举
来源：http://hz.tianlin.xyz/gtfihvvsru.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fzhhl.top/gtvmyxqlat.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pengpengdd.cyou/gttilonbrf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhongyouzk.top/gtthdzbenf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtvcuhftta.html

Java: enum Color { RED, GREEN }
来源：http://hz.zdqjudy.top/gtifejyyey.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenjidiqi.icu/gtsshhknab.html

Ruby: Color = %i[red green].freeze
来源：http://hz.316326.xyz/gtpizwyqbb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gttntajxfu.html

[G16] 对象转数组 / 字典
来源：http://hz.haohaochexian.top/gtmbfntycg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnxiangtu.top/gttyiakted.html

PHP:  get_object_vars($obj);
来源：http://hz.xinyue.icu/gtnknbntem.html

JS:   Object.entries(obj)
来源：http://hz.jqgfzy.top/gtdlfosyts.html

TS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtimawckhh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pengpengdd.cyou/gtzufnqlgl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zdqjudy.top/gtfjorpzwh.html

Ruby: obj.instance_variables
来源：http://hz.jyoumei.cn/gtgpkdblbx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daxiang520.top/gtcnmyxxhm.html

================================================================================
来源：http://hz.shzxlz.cn/gtgmgedkxe.html

H. 异常与错误处理
来源：http://hz.zhaomingkeji.xyz/gtlvpcfzxv.html

================================================================================
来源：http://hz.sweek.top/gtxxrennbg.html

[H01] try / catch 基础
来源：http://hz.hammf.cn/gtqvregeni.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj202588.top/gtfotrsvzg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gtseeurhbq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.bjfxy.top/gtcjelcifz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xingfuxueyuan.xyz/gtwckxltwt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.snrcjt.cn/gtjivhczli.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hongshengwenyu.top/gtqybmnndy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fzhhl.top/gtgdjpdtyj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gtrbnanvlh.html

[H02] finally / ensure 收尾
来源：http://hz.dianchejie.cn/gtbjjwlzvh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daria6918.cn/gtgqpfusfx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtpkowmbsa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtthghfrrt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtixlupnwg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtwbpvfbgt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.smart0.xyz/gtxhatxqqe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yangfankeji.com/gtfashxker.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.redwolf501.top/gtrkiangyn.html

[H03] 主动抛出异常
来源：http://hz.gotoacloud.top/gtiidfuqvu.html

Py:   raise ValueError("错误信息")
来源：http://hz.xylfe.cn/gtwsancpgg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtcqvpicfh.html

JS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtscekwxzs.html

TS:   throw new Error("错误信息");
来源：http://hz.hfpthk.cn/gtkpvxbaye.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtywfmphmr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhoulong.xyz/gttobtikdu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.vqdsnc.cn/gtzbyydhgi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtopytzwfs.html

[H04] 自定义异常类型
来源：http://hz.yuanzhike.top/gttywkuyzq.html

Py:   class MyError(Exception): pass
来源：http://hz.yonumen.top/gttycfltpl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cashguo.top/gtbnsmalns.html

JS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtyzsacadm.html

TS:   class MyError extends Error {}
来源：http://hz.zycfv.cn/gtppxrgjdy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.bjfxy.top/gtzdzhstpl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sweek.top/gtddcvvhks.html

Ruby: class MyError < StandardError; end
来源：http://hz.0kj1m.cn/gtsxgyijxr.html

C#:   class MyException : Exception {}
来源：http://hz.ehwqpu.com/gtroqnghpz.html

[H05] 捕获特定类型
来源：http://hz.gzhubu.top/gtuoumhykh.html

Py:   except ValueError as e:
来源：http://hz.nanxinkj.top/gtimsoxhsp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.mhx1999.top/gthxijesxy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnqzz.top/gtuinlkzlw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ybcxt.top/gtffljbthq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhoulong.xyz/gtfodestor.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnqzz.top/gtedaegtzv.html

Ruby: rescue ArgumentError => e
来源：http://hz.havefunace.top/gtuyplaszy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigfzy.top/gtpofylnsz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.316326.xyz/gtehgpjymo.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangtech.top/gtturavttx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhaomingkeji.xyz/gtrbdwlzgx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtuitspuoc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.andypj.xyz/gtdpfphxox.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hfpthk.cn/gtzoiwqbqe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nwbrower.top/gtsiizggcw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yanxiufei.cn/gtvsowotdl.html

C#:   obj?.A?.B ?? default
来源：http://hz.daxiang520.top/gtdeqzexkr.html

[H07] 断言
来源：http://hz.gotoacloud.top/gtdifzeoqc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sxryk.cn/gtzbikjbod.html

PHP:  assert($x > 0);
来源：http://hz.chenzaomai.com/gtgkxwjlzi.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtavlirzso.html

TS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtygllqmbk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj20258.top/gtrtggpjzi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gtyzcdusfz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.smart0.xyz/gtzaakntbn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yueranfly.top/gtxhyuguzv.html

[H08] 获取错误信息与堆栈
来源：http://hz.xylfe.cn/gtjyalxfcn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dianchejie.cn/gtazkcyoku.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tianlin.xyz/gtpmmroyyh.html

JS:   e.message;  e.stack
来源：http://hz.ydzc1.top/gthsnxvgpp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yanxiufei.cn/gtjxpjdqrn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ywan-chungtsiang.top/gtzswbspnh.html

Go:   err.Error()
来源：http://hz.fzhhl.top/gtosuxpvhl.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinqigufen.top/gtatlhshfq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cucudq.cn/gturqnjije.html

[H09] 带错误码的异常
来源：http://hz.smart0.xyz/gtnpyexksj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhiwuduotai.top/gtyjzezzaj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.9152youxi.cn/gtudyhfhkh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yvedp.cn/gtjstlohho.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258.top/gtkxhspgxt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.pycfn.com/gtniisichk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhijiandao.cn/gtzcsiasow.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xuetiantiany.cn/gtnagvzdco.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aizwys.cn/gtydkkgdzh.html

[H10] 资源自动释放
来源：http://hz.gaohongyu789.top/gtezqiqtck.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.wangshuangyany.cn/gthrynhhlv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuanzhike.top/gtwxcluhut.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yanxiufei.cn/gtkhbkpukm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtmzadwwjf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gotoacloud.top/gtcfpthtxn.html

Go:   defer f.Close()
来源：http://hz.shzxlz.cn/gtqzfkzyce.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tanke756.top/gtpkffpiqv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.0kj1m.cn/gtpkffcyjk.html

================================================================================
来源：http://hz.fengsongda.top/gtpfsqeecw.html

I. 正则表达式
来源：http://hz.gotoacloud.top/gtacdslrds.html

================================================================================
来源：http://hz.sufxvd.cn/gtnkufkgyw.html

[I01] 判断是否匹配
来源：http://hz.jinghuilouyu.cn/gtfiaeynyb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtvdqavamm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nanxinkj.top/gtwtubpbbl.html

JS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtypinzifo.html

TS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtivbgctgi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ivvv.top/gtexulinfk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258888.top/gteippdwhj.html

Ruby: s.match?(/\d+/)
来源：http://hz.svipenyu.cn/gtbfitcvtj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yonumen.top/gtescesemz.html

[I02] 提取所有匹配
来源：http://hz.cdnleiting.top/gttnhqymyy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtsnpxfeno.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.pycfn.com/gtojgphvie.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.redwolf501.top/gtkxxvofsl.html


<!-- 参考信息 -->