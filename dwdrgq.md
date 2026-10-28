代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxinkj.top/gtqwwszjsk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yvedp.cn/gtakbrunzw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gthhvgypqf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenjidiqi.icu/gtzzswsigw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtflieajel.html

TS:   path.extname("a.txt")
来源：http://hz.zycfv.cn/gtaersouqd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sufxvd.cn/gtakextplg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.0kj1m.cn/gtiixfaeta.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtxoypaeyy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jiagoushi.top/gtwkvgjxwt.html

[F11] 复制与移动文件
来源：http://hz.cucudq.cn/gtowyrlxen.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtuosrwqgi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhongyouzk.top/gtjystwyra.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtjqtnfehv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtipcgsrsp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zycfv.cn/gtfartbqgm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.mhx1999.top/gtyqhcatxj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtcgbcraoh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.iojbl.cn/gtztkccppq.html

[F12] CSV 读写
来源：http://hz.sufxvd.cn/gtufdbzzno.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jyoumei.cn/gtrnpckbii.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gogol.net.cn/gtdvmqxkrq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xuetiantiany.cn/gtdrteinwe.html

TS:   // 同上
来源：http://hz.aibaodan.cn/gthwbpyvgv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigufen.top/gtelslvahz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ywan-chungtsiang.top/gtawubwnzj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangkeji.top/gtbvrckxnk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.c1oappe.top/gtdoekncdh.html

================================================================================
来源：http://hz.c1oappe.top/gtyulxepsi.html

G. 面向对象
来源：http://hz.hnqzz.top/gtjriggpri.html

================================================================================
来源：http://hz.dianchejie.cn/gtkipjxyvl.html

[G01] 定义类
来源：http://hz.chenzaomai.com/gthktqxkos.html

Py:   class User: pass
来源：http://hz.snrcjt.cn/gthbvmessw.html

PHP:  class User {}
来源：http://hz.jinqigufen.top/gtqonylrlv.html

JS:   class User {}
来源：http://hz.redwolf501.top/gtqzypwuws.html

TS:   class User { name: string = ""; }
来源：http://hz.shuidangran.top/gtkaifbnyr.html

Java: class User {}
来源：http://hz.xingfuxueyuan.xyz/gtzworjcoq.html

Go:   type User struct { Name string }
来源：http://hz.xuanzx.com/gtzszakkyp.html

Ruby: class User; end
来源：http://hz.ydzc1.top/gtgdphnlzi.html

C#:   class User {}
来源：http://hz.chenlongwang.top/gtcveucige.html

[G02] 构造函数
来源：http://hz.nanxuanxn.top/gteatslbon.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenzaomai.com/gtyuuylnxj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hywenlv.cn/gtxcshrqpv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.svipenyu.cn/gtiutrvmic.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtzzpinbaa.html

Java: User(String name) { this.name = name; }
来源：http://hz.sxryk.cn/gtxnchabvj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ywan-chungtsiang.top/gtmujcmoqn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.smart0.xyz/gthsdydhdx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.redwolf501.top/gtfrlkzjeo.html

[G03] 实例属性
来源：http://hz.kuanghao11.cn/gtjkgoozyf.html

Py:   self.name = "x"
来源：http://hz.c1oappe.top/gtchjwcbjz.html

PHP:  public string $name = "x";
来源：http://hz.nanxuanxn.top/gthbfstuqw.html

JS:   this.name = "x";
来源：http://hz.pycfn.com/gtpvcmlnql.html

TS:   name: string = "x";
来源：http://hz.zhoulong.xyz/gtshiujqob.html

Java: private String name;
来源：http://hz.chenjidiqi.icu/gtnschauvx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gtijkwbhoj.html

Ruby: @name = "x"
来源：http://hz.fzhhl.top/gtkakyqbwf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.birdmap.top/gtkvlccvgx.html

[G04] 定义方法
来源：http://hz.svipenyu.cn/gtkwbovpyl.html

Py:   def greet(self): return self.name
来源：http://hz.mhx1999.top/gtrqeonrqm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gttaejksph.html

JS:   greet() { return this.name; }
来源：http://hz.9152youxi.cn/gtbrrfjgif.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtsaufbpoq.html

Java: String greet() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtangurtbr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gteuekvpku.html

Ruby: def greet; @name; end
来源：http://hz.wangdashe.top/gtyzohejrj.html

C#:   public string Greet() => Name;
来源：http://hz.meibo888.top/gtuqfzrszm.html

[G05] 继承
来源：http://hz.nwbrower.top/gtunmbhyfc.html

Py:   class Admin(User): pass
来源：http://hz.zhijiandao.cn/gtuwezrddm.html

PHP:  class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtzivqqitu.html

JS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtentiunij.html

TS:   class Admin extends User {}
来源：http://hz.zhixingplan.top/gtazcprtyk.html

Java: class Admin extends User {}
来源：http://hz.52xcode.cn/gtwtfuqjlt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj202588.top/gttjxxinmd.html

Ruby: class Admin < User; end
来源：http://hz.yuanzhike.top/gthvlirdae.html

C#:   class Admin : User {}
来源：http://hz.daria6918.cn/gtuanpzcox.html

[G06] 重写方法
来源：http://hz.cqqwz.cn/gtgwdhbmoz.html

Py:   def greet(self): return "admin"
来源：http://hz.dianchejie.cn/gtazbwxnvt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtpuywnzaj.html

JS:   greet() { return "admin"; }
来源：http://hz.yvedp.cn/gtivvwtofn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtbqsocaqo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.pycfn.com/gtmvfqjbdw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nwbrower.top/gtwpqbvkdd.html

Ruby: def greet; "admin"; end
来源：http://hz.fengsongda.top/gtvfpzmvsv.html

C#:   public override string Greet() => "admin";
来源：http://hz.jiagoushi.top/gtplnnilna.html

[G07] 调用父类方法
来源：http://hz.hammf.cn/gtgovsheqh.html

Py:   super().greet()
来源：http://hz.hywenlv.cn/gtsqqlojqm.html

PHP:  parent::greet();
来源：http://hz.fzhhl.top/gtmkdlfwzm.html

JS:   super.greet();
来源：http://hz.9152youxi.cn/gtziftssfv.html

TS:   super.greet();
来源：http://hz.tian-w.cn/gtshbcoudz.html

Java: super.greet();
来源：http://hz.tanke756.top/gtdgwhuxvh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xziqi.cn/gtuifocsmg.html

Ruby: super
来源：http://hz.aibaodan.cn/gtiiobsxpm.html

C#:   base.Greet();
来源：http://hz.hammf.cn/gtelhssilh.html

[G08] 静态方法与属性
来源：http://hz.ppjwa.cn/gtuybnsovp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenjidiqi.icu/gtcyjolwra.html

PHP:  public static function f() {}
来源：http://hz.bjfxy.top/gtpccmpcmi.html

JS:   static f() {}
来源：http://hz.xingfuxueyuan.xyz/gtbxuhzcgq.html

TS:   static f(): void {}
来源：http://hz.zhixingplan.top/gtvxgvlyur.html

Java: static void f() {}
来源：http://hz.yj20258.top/gtbuiucttn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ppjwa.cn/gtcfjwkalv.html

Ruby: def self.f; end
来源：http://hz.meibo888.top/gtticpvdxs.html

C#:   public static void F() {}
来源：http://hz.jianghu66.top/gtxcndmpvp.html

[G09] 接口 / 抽象类
来源：http://hz.aizwys.cn/gtqrnpgghp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gtdcjxxrui.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pengpengdd.cyou/gtqhihuafm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhiwuduotai.top/gtueiwyvpj.html

TS:   interface Shape { area(): number; }
来源：http://hz.dianchejie.cn/gtorbfplvn.html

Java: interface Shape { double area(); }
来源：http://hz.jqgfzy.top/gtsjffwhjj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.meibo888.top/gtdylxtwul.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhongyouzk.top/gtdkqwbtsj.html

C#:   interface IShape { double Area(); }
来源：http://hz.hammf.cn/gtxnhjlfww.html

[G10] 访问控制
来源：http://hz.hywenlv.cn/gtbrkfxutg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.dianchejie.cn/gtldhvlrnn.html

PHP:  public / protected / private
来源：http://hz.sxryk.cn/gtlcqyfbhi.html

JS:   #private 字段；其余公开
来源：http://hz.fengsongda.top/gtdwlcdsvy.html

TS:   public / protected / private
来源：http://hz.jinghuilouyu.cn/gtqqjrlfkh.html

Java: public / protected / private / 默认包级
来源：http://hz.9152youxi.cn/gtfqiswklf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinqigfzy.top/gtreqoczof.html

Ruby: public / protected / private
来源：http://hz.jqgfzy.top/gtgdvqdexv.html

C#:   public / protected / private / internal
来源：http://hz.andypj.xyz/gtzlnqxruf.html

[G11] getter / setter
来源：http://hz.dashuyun.cn/gtsbfkzzat.html

Py:   @property 与 @x.setter
来源：http://hz.hammf.cn/gtfnuounre.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtjzkymgpa.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gtdwknxzsc.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtnzfdoqrt.html

Java: public String getName() { return name; }
来源：http://hz.guannengcc.top/gtxhkgbjme.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cashguo.top/gtdyeyruda.html

Ruby: attr_accessor :name
来源：http://hz.gaohongyu789.top/gtaumawkqv.html

C#:   public string Name { get; set; }
来源：http://hz.shuidangran.top/gtoyteqdeq.html

[G12] 对象转字符串
来源：http://hz.tanke756.top/gtcfvxgqvl.html

Py:   def __str__(self): return self.name
来源：http://hz.ehwqpu.com/gtscktlhoy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtcbjkgyfm.html

JS:   toString() { return this.name; }
来源：http://hz.jlsjyb.cn/gtcuwhjkuf.html

TS:   toString(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtyxbojrqq.html

Java: @Override public String toString() { return name; }
来源：http://hz.daria6918.cn/gtoxlyiwtu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtseatzghj.html

Ruby: def to_s; @name; end
来源：http://hz.cheryme.top/gtidgglilm.html

C#:   public override string ToString() => Name;
来源：http://hz.c1oappe.top/gtjubujxhk.html

[G13] 判断对象类型
来源：http://hz.gogol.net.cn/gtlsxmfmod.html

Py:   isinstance(u, User)
来源：http://hz.ydjk.org.cn/gthsglyass.html

PHP:  $u instanceof User
来源：http://hz.dianchejie.cn/gtbspvarhs.html

JS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtiyeheubo.html

TS:   u instanceof User
来源：http://hz.hysaishi.cn/gtbdkuswid.html

Java: u instanceof User
来源：http://hz.yuxming.cn/gtxfnncqxq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tanke756.top/gtesdcpcue.html

Ruby: u.is_a?(User)
来源：http://hz.quarkkingdee.top/gtovrgxecf.html

C#:   u is User
来源：http://hz.xingfuxueyuan.xyz/gtjifgnvbl.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtgbqnymwf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gogol.net.cn/gtpjuucfhq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aizwys.cn/gteqsvzupj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nwbrower.top/gtgrfyqxuj.html

TS:   type User = { name: string; age: number };
来源：http://hz.cashguo.top/gtoojgfphd.html

Java: record User(String name, int age) {}
来源：http://hz.guannengcc.top/gtvrlivagj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yongpay.top/gtvbkpyluu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ivvv.top/gtndvwmdnc.html

C#:   record User(string Name, int Age);
来源：http://hz.zhixingplan.top/gtfismxmfu.html

[G15] 枚举
来源：http://hz.hfpthk.cn/gtwblrqnad.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dianchejie.cn/gtnsyvckph.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ybcxt.top/gtywgifgfx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fengsongda.top/gtjtfefebe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gtlroqgqde.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj202588.top/gtbhrrvoxy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jianghu66.top/gtlmbbdyam.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jianghu66.top/gtmcqxyqdj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gttvlhwwwm.html

[G16] 对象转数组 / 字典
来源：http://hz.xylfe.cn/gtlxinzksu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ydzc1.top/gtetsecbwh.html

PHP:  get_object_vars($obj);
来源：http://hz.gaohongyu789.top/gtofaucrmd.html

JS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtgzfgpght.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtxnthlwcj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cashguo.top/gtwkbeyooq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yanxiufei.cn/gtqkssqfvi.html

Ruby: obj.instance_variables
来源：http://hz.gogol.net.cn/gtzvadpgwz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.snrcjt.cn/gtgwlaucsz.html

================================================================================
来源：http://hz.chenzaomai.com/gtcvlrmrtq.html

H. 异常与错误处理
来源：http://hz.dianchejie.cn/gtvmtwxlpe.html

================================================================================
来源：http://hz.jqgufenzy.top/gtpqeqszlz.html

[H01] try / catch 基础
来源：http://hz.quarkkingdee.top/gtytffmnbq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.havefunace.top/gtnaqjbykj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.aibaodan.cn/gtzgntrxhj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtgafbwula.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ydzc1.top/gtumhrqinc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangtech.top/gtznmjbxkg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinghuilouyu.cn/gtqtmrejgz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fengsongda.top/gtvgiumkzo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258.top/gtqbiasgop.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtfdjywgub.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.feifeiyinyue.top/gtemipnymm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtxewhcwun.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtfosyfarz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtdwmsmhfo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtmomlnhtc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258.top/gtzfbdommz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ehwqpu.com/gtnbyzubju.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxuanxn.top/gtdguswteh.html

[H03] 主动抛出异常
来源：http://hz.snrcjt.cn/gtljtaidii.html

Py:   raise ValueError("错误信息")
来源：http://hz.daria6918.cn/gtmpgzlkhy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtytmjkqcv.html

JS:   throw new Error("错误信息");
来源：http://hz.aibaodan.cn/gtalzecsvd.html

TS:   throw new Error("错误信息");
来源：http://hz.zhixingplan.top/gtsiyifcna.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtnkypvgsb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhijiandao.cn/gtbcngcihz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yangfankeji.com/gtijuigmxg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gttgqrnwpn.html

[H04] 自定义异常类型
来源：http://hz.316326.xyz/gtuhchezxp.html

Py:   class MyError(Exception): pass
来源：http://hz.xingfuxueyuan.xyz/gtpypxtqcd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtvwjmidlk.html

JS:   class MyError extends Error {}
来源：http://hz.pycfn.com/gtpuagiune.html

TS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtvhikvbpp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenjidiqi.icu/gtmzrgewrv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.9152youxi.cn/gtbhqilfsd.html

Ruby: class MyError < StandardError; end
来源：http://hz.fzhhl.top/gtulpbdlwv.html

C#:   class MyException : Exception {}
来源：http://hz.zhaomingkeji.xyz/gtxphwocsm.html

[H05] 捕获特定类型
来源：http://hz.kuanghao11.cn/gtwenpvzov.html

Py:   except ValueError as e:
来源：http://hz.mhx1999.top/gtkbcxxdbm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhiwuduotai.top/gtqcgesblx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.0kj1m.cn/gtwipghlqa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtmxufblpt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinqigfzy.top/gtdffjedri.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.haohaochexian.top/gtjlyocysr.html

Ruby: rescue ArgumentError => e
来源：http://hz.daria6918.cn/gtomggwhxd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.aizwys.cn/gtlfossqrt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cdnleiting.top/gtqmubtnil.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gtkzdnwsgx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.svipenyu.cn/gtoljgetxv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtkixveqwv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtvujkkryl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shangyingyoupin.top/gtdcwogpcw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.smart0.xyz/gtubeblmdf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jyoumei.cn/gtxxnfliha.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenlongwang.top/gtfwsakzvh.html

[H07] 断言
来源：http://hz.fengsongda.top/gtxttosseb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtbdyvebnu.html

PHP:  assert($x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtvoxmiizt.html

JS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtngieftav.html

TS:   console.assert(x > 0);
来源：http://hz.tian-w.cn/gtawcvgdww.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jlsjyb.cn/gtstquekdf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.kuanghao11.cn/gtavnqtjye.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.daxiang520.top/gtbrajeowf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cdnleiting.top/gtlmhngejj.html

[H08] 获取错误信息与堆栈
来源：http://hz.snrcjt.cn/gtmbowbkaz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yanxiufei.cn/gtglhxmvld.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtowaucwzk.html

JS:   e.message;  e.stack
来源：http://hz.yueranfly.top/gtpqnjbrlh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinghuilouyu.cn/gtlizrocuk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aibaodan.cn/gtnwpvjgcq.html

Go:   err.Error()
来源：http://hz.shzxlz.cn/gtzzzfvjyy.html

Ruby: e.message;  e.backtrace
来源：http://hz.hywenlv.cn/gtgvrhhpli.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xuanzx.com/gthuuqhjwk.html

[H09] 带错误码的异常
来源：http://hz.shangyingyoupin.top/gtusolfeik.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xingfuxueyuan.xyz/gtljdtxvos.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhongyouzk.top/gtbtqwdkxe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.aizwys.cn/gtgmfkhosj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinyuanbaomall.cn/gtjbbygpry.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jianghu66.top/gtvimjclio.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenjidiqi.icu/gtyoymlmqd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hammf.cn/gthnkfehcb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.kuanghao11.cn/gtelosalkv.html

[H10] 资源自动释放
来源：http://hz.gotoacloud.top/gtuvuzxgpn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jiagoushi.top/gtefhkbwwg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jlsjyb.cn/gtqcqlvbzh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtypltdwpg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtewmkjlmo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangdashe.top/gtupgcalnt.html

Go:   defer f.Close()
来源：http://hz.jqgufenzy.top/gtwjnofrja.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sufxvd.cn/gtebxqdomb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tanke756.top/gtleqrzkze.html

================================================================================
来源：http://hz.yj20258888.top/gtzywycrzf.html

I. 正则表达式
来源：http://hz.cashguo.top/gtukxlacfj.html

================================================================================
来源：http://hz.yvedp.cn/gteoqmiqdd.html

[I01] 判断是否匹配
来源：http://hz.hongshengwenyu.top/gtmltugcrs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhixingplan.top/gtwnsluiyq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daxiang520.top/gthhaxqzmp.html

JS:   /\d+/.test(s)
来源：http://hz.sweek.top/gthitgbldi.html

TS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtdeegotff.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.wangshuangyany.cn/gtteeojghg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuxming.cn/gtfgvffyhe.html

Ruby: s.match?(/\d+/)
来源：http://hz.316326.xyz/gtfbcfjjfi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.guannengcc.top/gtrczgtvcu.html

[I02] 提取所有匹配
来源：http://hz.chenzaomai.com/gtflodylck.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hfpthk.cn/gtelvgdnol.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.redwolf501.top/gtygwrxxrd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tanke756.top/gtzgqkmekj.html

TS:   s.match(/\d+/g)
来源：http://hz.pengpengdd.cyou/gtoyyykisx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhijiandao.cn/gtwncxomvo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gaohongyu789.top/gtcfoascll.html

Ruby: s.scan(/\d+/)
来源：http://hz.havefunace.top/gtsovldtja.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.andypj.xyz/gtaxqzryxl.html

[I03] 提取捕获分组
来源：http://hz.ppjwa.cn/gtaicbpsps.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.aizwys.cn/gtoovejrkl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daria6918.cn/gtaqzkzdvt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sxryk.cn/gtduscapcs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gtkzleyewy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jyoumei.cn/gtxvfbvrlp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zdqjudy.top/gthpyyodzl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xuanzx.com/gtuwjkzvcm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgfzy.top/gtgajbztvj.html

[I04] 正则替换
来源：http://hz.sxryk.cn/gtkcbiijkw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgfzy.top/gtrlewqmow.html


<!-- 参考信息 -->