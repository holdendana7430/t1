代发 wailian999

[F09] 获取文件大小
来源：http://hz.shanyushiyangtech.top/gteuieoaft.html

Py:   os.path.getsize("a.txt")
来源：http://hz.redwolf501.top/gtlixjxaed.html

PHP:  filesize("a.txt");
来源：http://hz.guannengcc.top/gtskiqcyxp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.svipenyu.cn/gtqkapsisl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jqgfzy.top/gtcfyygahc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtvrozvfvv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuanzx.com/gtbtzocioj.html

Ruby: File.size("a.txt")
来源：http://hz.birdmap.top/gtwebykncw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gaohongyu789.top/gtxrjzhjeb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shanyushiyangtech.top/gtrzhhfdzh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtbpfspaio.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.andypj.xyz/gtjfzdehqv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtzuxdsdqj.html

TS:   path.extname("a.txt")
来源：http://hz.andypj.xyz/gtglgbjvbq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhijiandao.cn/gthkwvzdqa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zycfv.cn/gtfjbrriqk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtcqsxfybb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.birdmap.top/gtheqmkftk.html

[F11] 复制与移动文件
来源：http://hz.mhx1999.top/gtizsswhgn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtalwsaiao.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhijiandao.cn/gtwnxsnhmp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtqqguywan.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtrrdwhlix.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.c1oappe.top/gtsgprtraq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ydjk.org.cn/gtimgmsutx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtgvcefqvf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtlpqlzsex.html

[F12] CSV 读写
来源：http://hz.hysaishi.cn/gtdascqumu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.aizwys.cn/gtghvnoiov.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hammf.cn/gtsiuaowze.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.snrcjt.cn/gtosflekcb.html

TS:   // 同上
来源：http://hz.zhengqikj.top/gtpganrtdd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tianlin.xyz/gtahizalsm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.aizwys.cn/gtdyikpbjc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.birdmap.top/gtmunzbjmo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hfpthk.cn/gtezgvljrl.html

================================================================================
来源：http://hz.chenzaomai.com/gtbbmklnfv.html

G. 面向对象
来源：http://hz.fzhhl.top/gthsjfyaid.html

================================================================================
来源：http://hz.ydzc1.top/gtmgkzhave.html

[G01] 定义类
来源：http://hz.0kj1m.cn/gtbjcxkgrl.html

Py:   class User: pass
来源：http://hz.xinyue.icu/gtbpbmqxux.html

PHP:  class User {}
来源：http://hz.snrcjt.cn/gtxnhruscv.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtzosfksvm.html

TS:   class User { name: string = ""; }
来源：http://hz.tian-w.cn/gtqquxlijw.html

Java: class User {}
来源：http://hz.zhongyouzk.top/gtsibuljdq.html

Go:   type User struct { Name string }
来源：http://hz.gaohongyu789.top/gtsxnbzigz.html

Ruby: class User; end
来源：http://hz.hammf.cn/gtzqozwegr.html

C#:   class User {}
来源：http://hz.guannengcc.top/gtkziklurs.html

[G02] 构造函数
来源：http://hz.nanxinkj.top/gtqjepqhzj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhoulong.xyz/gtztsdrgzl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhongyouzk.top/gttevxhncp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtortzydpt.html

TS:   constructor(public name: string) {}
来源：http://hz.316326.xyz/gtoxhnpamh.html

Java: User(String name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gtujohsqvf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yvedp.cn/gtdkqvyvnq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinyuanbaomall.cn/gtqhfwsfpp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuanzx.com/gtwuoqphda.html

[G03] 实例属性
来源：http://hz.chenlongwang.top/gtdifbmnux.html

Py:   self.name = "x"
来源：http://hz.c1oappe.top/gtnyfzwuzc.html

PHP:  public string $name = "x";
来源：http://hz.xuanzx.com/gtgwmahrsk.html

JS:   this.name = "x";
来源：http://hz.shzxlz.cn/gttmjmlprv.html

TS:   name: string = "x";
来源：http://hz.daxiang520.top/gtehbtnaus.html

Java: private String name;
来源：http://hz.birdmap.top/gtcncwozby.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gzhubu.top/gtrwkdohyy.html

Ruby: @name = "x"
来源：http://hz.feifeiyinyue.top/gtoncgrfph.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinqigufen.top/gtkgnsnhqf.html

[G04] 定义方法
来源：http://hz.zhixingplan.top/gtmchmovdy.html

Py:   def greet(self): return self.name
来源：http://hz.hysaishi.cn/gtpucmdyja.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtgdlnrbcy.html

JS:   greet() { return this.name; }
来源：http://hz.gzhubu.top/gtrabiecun.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtoeryweyz.html

Java: String greet() { return name; }
来源：http://hz.jinqigfzy.top/gtuhlttasr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dashuyun.cn/gthoixbyxj.html

Ruby: def greet; @name; end
来源：http://hz.ydjk.org.cn/gtpffvyswr.html

C#:   public string Greet() => Name;
来源：http://hz.guannengcc.top/gtclvimumm.html

[G05] 继承
来源：http://hz.yj20258.top/gtjlvawgwh.html

Py:   class Admin(User): pass
来源：http://hz.nanxinkj.top/gtjmxinfqd.html

PHP:  class Admin extends User {}
来源：http://hz.tanke756.top/gtasexgipo.html

JS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtqjnywiqe.html

TS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtkytofcxq.html

Java: class Admin extends User {}
来源：http://hz.xuanzx.com/gtjgtnmtuy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hongshengwenyu.top/gthexqsflc.html

Ruby: class Admin < User; end
来源：http://hz.aizwys.cn/gtuecbkdkb.html

C#:   class Admin : User {}
来源：http://hz.hongshengwenyu.top/gtgjauccri.html

[G06] 重写方法
来源：http://hz.bjfxy.top/gtpwlwhcqd.html

Py:   def greet(self): return "admin"
来源：http://hz.birdmap.top/gtjmnuvdoj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtwtxusfye.html

JS:   greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtlrqbqzbo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gtgmtvaykd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtaclfqqvt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuanzhike.top/gtrhbabues.html

Ruby: def greet; "admin"; end
来源：http://hz.xinyue.icu/gtjgutnbfq.html

C#:   public override string Greet() => "admin";
来源：http://hz.shangyingyoupin.top/gtorzfvmmn.html

[G07] 调用父类方法
来源：http://hz.sufxvd.cn/gtpvbqfxlr.html

Py:   super().greet()
来源：http://hz.andypj.xyz/gtcnbezsbo.html

PHP:  parent::greet();
来源：http://hz.pycfn.com/gtaqqgbbqk.html

JS:   super.greet();
来源：http://hz.yuanzhike.top/gtzogefijd.html

TS:   super.greet();
来源：http://hz.haohaochexian.top/gterygdmim.html

Java: super.greet();
来源：http://hz.kuanghao11.cn/gtuxrbowqb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtkejkwled.html

Ruby: super
来源：http://hz.pengpengdd.cyou/gtmdccptpr.html

C#:   base.Greet();
来源：http://hz.c1oappe.top/gtavfqrjbf.html

[G08] 静态方法与属性
来源：http://hz.xziqi.cn/gtkuuhekal.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhixingplan.top/gtjpmwerzf.html

PHP:  public static function f() {}
来源：http://hz.zhoulong.xyz/gtexxluqyt.html

JS:   static f() {}
来源：http://hz.zhoulong.xyz/gtagnczovb.html

TS:   static f(): void {}
来源：http://hz.tian-w.cn/gtbmwriftn.html

Java: static void f() {}
来源：http://hz.bjfxy.top/gtvludtler.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gaohongyu789.top/gtgwjvnrmx.html

Ruby: def self.f; end
来源：http://hz.ybcxt.top/gtowqwfihm.html

C#:   public static void F() {}
来源：http://hz.jianghu66.top/gtqbpipuut.html

[G09] 接口 / 抽象类
来源：http://hz.ppjwa.cn/gtzahrodam.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.daxiang520.top/gtiinunfpx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shzxlz.cn/gtnojugoki.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.0kj1m.cn/gttqxadpzk.html

TS:   interface Shape { area(): number; }
来源：http://hz.redwolf501.top/gtqzsklrtm.html

Java: interface Shape { double area(); }
来源：http://hz.yuanzhike.top/gtjvqwzjnw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhaomingkeji.xyz/gtwhpwyyqu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigufen.top/gtvaszicwc.html

C#:   interface IShape { double Area(); }
来源：http://hz.jlsjyb.cn/gtxivauldr.html

[G10] 访问控制
来源：http://hz.hnxiangtu.top/gtibumqojo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.52xcode.cn/gtinxejqjx.html

PHP:  public / protected / private
来源：http://hz.hywenlv.cn/gtignjsxmt.html

JS:   #private 字段；其余公开
来源：http://hz.zhijiandao.cn/gtqluoswov.html

TS:   public / protected / private
来源：http://hz.smart0.xyz/gtvcefqnyj.html

Java: public / protected / private / 默认包级
来源：http://hz.jianghu66.top/gtaznsxvwx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj202588.top/gtlshvcpms.html

Ruby: public / protected / private
来源：http://hz.hnqzz.top/gteqtefapw.html

C#:   public / protected / private / internal
来源：http://hz.shangyingyoupin.top/gtomazmvsc.html

[G11] getter / setter
来源：http://hz.hfpthk.cn/gtbhflkvnq.html

Py:   @property 与 @x.setter
来源：http://hz.bjfxy.top/gtuefxehte.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtsewmelch.html

JS:   get name() { return this._name; }
来源：http://hz.zhijiandao.cn/gtxceztcug.html

TS:   get name(): string { return this._name; }
来源：http://hz.yongpay.top/gtifpafwlo.html

Java: public String getName() { return name; }
来源：http://hz.9152youxi.cn/gtlyzhkxmu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tianlin.xyz/gtrxxhnbgi.html

Ruby: attr_accessor :name
来源：http://hz.tian-w.cn/gtqndnvmyy.html

C#:   public string Name { get; set; }
来源：http://hz.yonumen.top/gtdlnlcyyq.html

[G12] 对象转字符串
来源：http://hz.ywan-chungtsiang.top/gttbntxchi.html

Py:   def __str__(self): return self.name
来源：http://hz.yanxiufei.cn/gtnyydgzil.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtqtbmghtd.html

JS:   toString() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtojtyqrxl.html

TS:   toString(): string { return this.name; }
来源：http://hz.tian-w.cn/gtopbginec.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangdashe.top/gtdfmtqbuo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtqrplgprq.html

Ruby: def to_s; @name; end
来源：http://hz.ywan-chungtsiang.top/gtnqtzzuiq.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtxwtggktw.html

[G13] 判断对象类型
来源：http://hz.guannengcc.top/gtnhvwkpfs.html

Py:   isinstance(u, User)
来源：http://hz.cucudq.cn/gtcpaysicy.html

PHP:  $u instanceof User
来源：http://hz.xuanzx.com/gtwhlknxyf.html

JS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtcmnzhzer.html

TS:   u instanceof User
来源：http://hz.jiagoushi.top/gtnsovuupo.html

Java: u instanceof User
来源：http://hz.pengpengdd.cyou/gtawqeeeod.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cucudq.cn/gtoliizxth.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gtkeiahsqy.html

C#:   u is User
来源：http://hz.52xcode.cn/gtjkfnbyad.html

[G14] 数据类 / record
来源：http://hz.fzhhl.top/gteotyyleo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gotoacloud.top/gtxajwwdjq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.pycfn.com/gtwytggemw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daria6918.cn/gtytrzsbya.html

TS:   type User = { name: string; age: number };
来源：http://hz.hammf.cn/gtcdxmgaes.html

Java: record User(String name, int age) {}
来源：http://hz.redwolf501.top/gthmzlcrkd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gthyykeqqt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinyuanbaomall.cn/gtxwsoudsb.html

C#:   record User(string Name, int Age);
来源：http://hz.ywan-chungtsiang.top/gtgamgxner.html

[G15] 枚举
来源：http://hz.shanyushiyangkeji.top/gtshzcwqcf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ivvv.top/gtmauyxtqa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.quarkkingdee.top/gttnxsumjf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenlongwang.top/gtuimipwau.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtbmntyqmz.html

Java: enum Color { RED, GREEN }
来源：http://hz.iojbl.cn/gtyxcjjurh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xinyue.icu/gtagvwtvom.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydzc1.top/gtiutpktsi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258.top/gttntxypfs.html

[G16] 对象转数组 / 字典
来源：http://hz.hysaishi.cn/gtxsswatfw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.9152youxi.cn/gtdbvlzexm.html

PHP:  get_object_vars($obj);
来源：http://hz.yongpay.top/gtdnyukaqt.html

JS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtolwpyrpo.html

TS:   Object.entries(obj)
来源：http://hz.sufxvd.cn/gtwungjerl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gotoacloud.top/gtfvxmgfrv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangkeji.top/gtilcyekfl.html

Ruby: obj.instance_variables
来源：http://hz.ywan-chungtsiang.top/gtpyobtmky.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxuanxn.top/gtxssjpjhy.html

================================================================================
来源：http://hz.ydzc1.top/gttyvrcpgl.html

H. 异常与错误处理
来源：http://hz.hnxiangtu.top/gtzqxqxqnq.html

================================================================================
来源：http://hz.gotoacloud.top/gtijfvhpcl.html

[H01] try / catch 基础
来源：http://hz.cheryme.top/gtyknbzcuu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xuetiantiany.cn/gteoxpzcrp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gogol.net.cn/gtzrejjuxz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shzxlz.cn/gtymweaabn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sweek.top/gtqrzjjwik.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinyuanbaomall.cn/gteghwoavw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tanke756.top/gtugfsflea.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.c1oappe.top/gtcwetkzjb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gotoacloud.top/gtchonclpz.html

[H02] finally / ensure 收尾
来源：http://hz.wangdashe.top/gtuuiqxkxx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shangyingyoupin.top/gtienjjrou.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtlhohwfev.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtlpypxuwd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtwvoxlrkj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtnixiahfh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.redwolf501.top/gtyzwvxrhk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.c1oappe.top/gtfmsfuxpd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnxiangtu.top/gtzagcfhwe.html

[H03] 主动抛出异常
来源：http://hz.aizwys.cn/gtwxfgulbj.html

Py:   raise ValueError("错误信息")
来源：http://hz.ywan-chungtsiang.top/gtgnboqoiz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cashguo.top/gthdsyiwno.html

JS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtqcfiefih.html

TS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtfiqmvqsn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtwvwfnbmt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dianchejie.cn/gtgllzzumg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenzaomai.com/gtyuehkuqi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cashguo.top/gtfhwrsucl.html

[H04] 自定义异常类型
来源：http://hz.gogol.net.cn/gtbefefbdr.html

Py:   class MyError(Exception): pass
来源：http://hz.cucudq.cn/gtwyghecae.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guannengcc.top/gtfnoxqmji.html

JS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gtyfnrlutx.html

TS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gtgxgdzyhi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangshuangyany.cn/gtnhrexyyw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sxryk.cn/gtfmwaghjw.html

Ruby: class MyError < StandardError; end
来源：http://hz.jiagoushi.top/gtzilnwjay.html

C#:   class MyException : Exception {}
来源：http://hz.jqgfzy.top/gtmvzckoou.html

[H05] 捕获特定类型
来源：http://hz.9152youxi.cn/gtfhonjvli.html

Py:   except ValueError as e:
来源：http://hz.ehwqpu.com/gtpddxsjoo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xinyue.icu/gtcryandbg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.daria6918.cn/gthafwjhtr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtnyjtevlt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sysykeji.top/gtcampoexo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangdashe.top/gtunghfmfh.html

Ruby: rescue ArgumentError => e
来源：http://hz.yvedp.cn/gtxyzwffxu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.aibaodan.cn/gtuxvppmsk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shanyushiyangtech.top/gtyegqpjlp.html

Py:   value = d.get("k") or default
来源：http://hz.xziqi.cn/gtqavzddql.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.fzhhl.top/gtzboeqrkj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.andypj.xyz/gtypeynuaq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gtepcjddks.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.wangshuangyany.cn/gtdiiozarw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj20258.top/gthtajmwbx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuanzhike.top/gtxxkybzef.html

C#:   obj?.A?.B ?? default
来源：http://hz.guowangkeji.top/gtdubwvsub.html

[H07] 断言
来源：http://hz.daxiang520.top/gthwivgoqs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aibaodan.cn/gtkbbizkhd.html

PHP:  assert($x > 0);
来源：http://hz.kuanghao11.cn/gtcjbehcef.html

JS:   console.assert(x > 0);
来源：http://hz.chenlongwang.top/gtqoimxfyp.html

TS:   console.assert(x > 0);
来源：http://hz.smart0.xyz/gtmsgsjnhb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pycfn.com/gtwxpsyyss.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gogol.net.cn/gtgirbhpfo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.fengsongda.top/gtgfixxrwf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hfpthk.cn/gtefbcjgjl.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinghuilouyu.cn/gtukojvibt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhoulong.xyz/gtjqebwhky.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.snrcjt.cn/gtbdtdhzod.html

JS:   e.message;  e.stack
来源：http://hz.xziqi.cn/gthdxoqgqn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pengpengdd.cyou/gttlcorlnb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ehwqpu.com/gtpvexqgfj.html

Go:   err.Error()
来源：http://hz.svipenyu.cn/gtjqfjpmwz.html

Ruby: e.message;  e.backtrace
来源：http://hz.gzhubu.top/gtsgukthew.html

C#:   e.Message;  e.StackTrace
来源：http://hz.mhx1999.top/gtgatfidzq.html

[H09] 带错误码的异常
来源：http://hz.yj20258.top/gtztkzxkqm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhijiandao.cn/gtfyarxtve.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhiwuduotai.top/gtexbnwfyw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nwbrower.top/gtbhqbghsz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuetiantiany.cn/gtdmniuxuy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxinkj.top/gtgwtmajwh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhaomingkeji.xyz/gtjmwkyhtd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yvedp.cn/gtsbifrrbf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zdqjudy.top/gtkgxwvyof.html

[H10] 资源自动释放
来源：http://hz.hnqzz.top/gtcmwbnqqa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guowangkeji.top/gtzkngepbc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daxiang520.top/gtogeqwuum.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtpdjeeboj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtpscrwttb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ivvv.top/gtsumhmxeo.html

Go:   defer f.Close()
来源：http://hz.feifeiyinyue.top/gtdqanafrb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigfzy.top/gtgppcvujz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fzhhl.top/gtbbnqrcse.html

================================================================================
来源：http://hz.wangdashe.top/gtjoxbqahj.html

I. 正则表达式
来源：http://hz.zhengqikj.top/gtpxarmqvl.html

================================================================================
来源：http://hz.cqqwz.cn/gtmrypvrnu.html

[I01] 判断是否匹配
来源：http://hz.jinghuilouyu.cn/gtusugqtel.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xinyue.icu/gtdnvjyugh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shangyingyoupin.top/gtgozoukfz.html

JS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtdnxjspzh.html

TS:   /\d+/.test(s)
来源：http://hz.jinqigfzy.top/gtzkabcjrz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cucudq.cn/gtaledqulf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pycfn.com/gtuesxmdsv.html

Ruby: s.match?(/\d+/)
来源：http://hz.shzxlz.cn/gtsedlnhlr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydjk.org.cn/gtkzhoqbjk.html

[I02] 提取所有匹配
来源：http://hz.kuanghao11.cn/gtqbcojhqd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jiagoushi.top/gtnvwqpyjb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.andypj.xyz/gtxxbgdphf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sufxvd.cn/gtksgjvzeu.html

TS:   s.match(/\d+/g)
来源：http://hz.hnxiangtu.top/gtrvjjkxuu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.fzhhl.top/gtyhcduujc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hongshengwenyu.top/gtnugzfops.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhixingplan.top/gtvzshxobz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gaohongyu789.top/gtxmghmhrp.html

[I03] 提取捕获分组
来源：http://hz.nanxuanxn.top/gttapdpjgj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.aizwys.cn/gtbxtuwnxv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxinkj.top/gtwqdhgrkv.html


<!-- 参考信息 -->