代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hz.0kj1m.cn/gtlhqtnrqb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.svipenyu.cn/gtkuylturi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cucudq.cn/gtjojmvkxl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nanxuanxn.top/gtsfxkwddr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtfynxxfkw.html

TS:   path.extname("a.txt")
来源：http://hz.shzxlz.cn/gtelwlubbh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydzc1.top/gtezlrqukq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hfpthk.cn/gtivsimtzn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtjzoymkak.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hysaishi.cn/gtimpzsifz.html

[F11] 复制与移动文件
来源：http://hz.tianlin.xyz/gtsqgwwyfn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtllzrfnon.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shzxlz.cn/gtedbxfqwv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtufnqpesu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtzpbdfwwf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nanxinkj.top/gtoklgjeyc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.316326.xyz/gtvhuczauo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtjpigrovk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ywan-chungtsiang.top/gtxbjoltsp.html

[F12] CSV 读写
来源：http://hz.guannengcc.top/gtcuzcqclg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gtuiiryzgu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hfpthk.cn/gtoufdhbyu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hysaishi.cn/gtcpqarmgr.html

TS:   // 同上
来源：http://hz.c1oappe.top/gtmivxepyi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tianlin.xyz/gtysscytsd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhaomingkeji.xyz/gtvhgllmdh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ydjk.org.cn/gtfgjewwqx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.52xcode.cn/gtgpknsstp.html

================================================================================
来源：http://hz.gzhubu.top/gtnrtczhvs.html

G. 面向对象
来源：http://hz.meibo888.top/gtbypsklwe.html

================================================================================
来源：http://hz.svipenyu.cn/gtninsrvvw.html

[G01] 定义类
来源：http://hz.xziqi.cn/gtvjntvivw.html

Py:   class User: pass
来源：http://hz.tian-w.cn/gtoptfuiku.html

PHP:  class User {}
来源：http://hz.pengpengdd.cyou/gtqnnegmnj.html

JS:   class User {}
来源：http://hz.c1oappe.top/gtmmeizdzj.html

TS:   class User { name: string = ""; }
来源：http://hz.quarkkingdee.top/gtkuucwagx.html

Java: class User {}
来源：http://hz.pycfn.com/gtneholaqj.html

Go:   type User struct { Name string }
来源：http://hz.yvedp.cn/gtsugazivf.html

Ruby: class User; end
来源：http://hz.fzhhl.top/gtewathtzr.html

C#:   class User {}
来源：http://hz.c1oappe.top/gtdntcltbx.html

[G02] 构造函数
来源：http://hz.mhx1999.top/gtvjaozowk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zycfv.cn/gtvuvkglfn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gotoacloud.top/gtxhitmbve.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.meibo888.top/gtpxddljnq.html

TS:   constructor(public name: string) {}
来源：http://hz.yj202588.top/gtotnazxjx.html

Java: User(String name) { this.name = name; }
来源：http://hz.meibo888.top/gtycrndjzn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zycfv.cn/gtsyjmohfu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hnqzz.top/gtigzdnamy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhongyouzk.top/gtrzmtlvmh.html

[G03] 实例属性
来源：http://hz.xziqi.cn/gtuyjkqlpd.html

Py:   self.name = "x"
来源：http://hz.316326.xyz/gthtbcfjug.html

PHP:  public string $name = "x";
来源：http://hz.jianghu66.top/gtymxsaqhs.html

JS:   this.name = "x";
来源：http://hz.gogol.net.cn/gtqacshpaf.html

TS:   name: string = "x";
来源：http://hz.chenlongwang.top/gtmhqbmyks.html

Java: private String name;
来源：http://hz.yanxiufei.cn/gtzupyityk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj202588.top/gtuoycmtdy.html

Ruby: @name = "x"
来源：http://hz.jinyuanbaomall.cn/gtnsbfckao.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenjidiqi.icu/gtafpmeycw.html

[G04] 定义方法
来源：http://hz.havefunace.top/gtpfuwepse.html

Py:   def greet(self): return self.name
来源：http://hz.gaohongyu789.top/gtgqisqfoz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtkpnyrdjr.html

JS:   greet() { return this.name; }
来源：http://hz.shangyingyoupin.top/gteaifuihe.html

TS:   greet(): string { return this.name; }
来源：http://hz.cheryme.top/gtlqruytdy.html

Java: String greet() { return name; }
来源：http://hz.fzhhl.top/gtbzelkudb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gtrrzktrhb.html

Ruby: def greet; @name; end
来源：http://hz.xylfe.cn/gtynvcnbae.html

C#:   public string Greet() => Name;
来源：http://hz.fengsongda.top/gtyzxfcuzz.html

[G05] 继承
来源：http://hz.iojbl.cn/gtgmhljula.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gtvvvftgwx.html

PHP:  class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtspevkmvy.html

JS:   class Admin extends User {}
来源：http://hz.havefunace.top/gtqnofmegv.html

TS:   class Admin extends User {}
来源：http://hz.yonumen.top/gtrnugbexn.html

Java: class Admin extends User {}
来源：http://hz.cdnleiting.top/gtvllyzqqq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.0kj1m.cn/gtjsrgadnp.html

Ruby: class Admin < User; end
来源：http://hz.nwbrower.top/gtufodnbjl.html

C#:   class Admin : User {}
来源：http://hz.hysaishi.cn/gtupzcirnq.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gtobacefjx.html

Py:   def greet(self): return "admin"
来源：http://hz.jinghuilouyu.cn/gtcttnhqcf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtyspmbsoo.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgufenzy.top/gthcoxtyuk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtchcxfeka.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.daria6918.cn/gtptygzbkx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuanzx.com/gtdigjyhzl.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgfzy.top/gtrlqrmgfb.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgufenzy.top/gtvxvjyfvh.html

[G07] 调用父类方法
来源：http://hz.jlsjyb.cn/gtlrhvyevf.html

Py:   super().greet()
来源：http://hz.zycfv.cn/gtkxauvcxs.html

PHP:  parent::greet();
来源：http://hz.zhengqikj.top/gtpjunwoph.html

JS:   super.greet();
来源：http://hz.yanxiufei.cn/gtjovekhdd.html

TS:   super.greet();
来源：http://hz.316326.xyz/gthftxuxfq.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtgouddykb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.haohaochexian.top/gtvuxvhvtc.html

Ruby: super
来源：http://hz.shanyushiyangkeji.top/gtirqaigxm.html

C#:   base.Greet();
来源：http://hz.shanyushiyangtech.top/gtnxwxjqpq.html

[G08] 静态方法与属性
来源：http://hz.yj20258.top/gtjzztrsek.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dashuyun.cn/gtdixdsahb.html

PHP:  public static function f() {}
来源：http://hz.iojbl.cn/gtzyuvmggh.html

JS:   static f() {}
来源：http://hz.316326.xyz/gtkvedgokk.html

TS:   static f(): void {}
来源：http://hz.cdnleiting.top/gtzwvvrzcm.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtbxrcurem.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yonumen.top/gtzrxbldgt.html

Ruby: def self.f; end
来源：http://hz.jianghu66.top/gtuhvciscu.html

C#:   public static void F() {}
来源：http://hz.hammf.cn/gtdoytlfuc.html

[G09] 接口 / 抽象类
来源：http://hz.dianchejie.cn/gtspncghuc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenzaomai.com/gtnlseusou.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.9152youxi.cn/gtbzqghurp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydzc1.top/gtsxsserya.html

TS:   interface Shape { area(): number; }
来源：http://hz.ivvv.top/gtysadynyd.html

Java: interface Shape { double area(); }
来源：http://hz.hywenlv.cn/gtpgtjvmfd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cheryme.top/gtbtnqduxl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sysykeji.top/gtibpnvofx.html

C#:   interface IShape { double Area(); }
来源：http://hz.aibaodan.cn/gtdweyrnqt.html

[G10] 访问控制
来源：http://hz.xinyue.icu/gtxcmctduk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhongyouzk.top/gttmfvsybf.html

PHP:  public / protected / private
来源：http://hz.pycfn.com/gtfarllouh.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtpjzzvsis.html

TS:   public / protected / private
来源：http://hz.gotoacloud.top/gtfhlrtwii.html

Java: public / protected / private / 默认包级
来源：http://hz.snrcjt.cn/gtpysjedyw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.smart0.xyz/gtklznyjli.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtjlncqhmi.html

C#:   public / protected / private / internal
来源：http://hz.yanxiufei.cn/gtwraoybwb.html

[G11] getter / setter
来源：http://hz.wangdashe.top/gtmaufibru.html

Py:   @property 与 @x.setter
来源：http://hz.cheryme.top/gtwjmgajny.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtbkzfntdq.html

JS:   get name() { return this._name; }
来源：http://hz.zhoulong.xyz/gtwblxbbpi.html

TS:   get name(): string { return this._name; }
来源：http://hz.fzhhl.top/gtsgflixjp.html

Java: public String getName() { return name; }
来源：http://hz.shzxlz.cn/gtwxpxepps.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.havefunace.top/gtnpznczbt.html

Ruby: attr_accessor :name
来源：http://hz.zdqjudy.top/gtqdeswtxb.html

C#:   public string Name { get; set; }
来源：http://hz.9152youxi.cn/gtljdjuira.html

[G12] 对象转字符串
来源：http://hz.bjfxy.top/gtrgpxujwf.html

Py:   def __str__(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtxibnadqg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtpfzpktzv.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258.top/gtldbdeibq.html

TS:   toString(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtrmuxgasz.html

Java: @Override public String toString() { return name; }
来源：http://hz.dianchejie.cn/gteihbygjw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtgaviithl.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gtlxujgcvu.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtpmkpntoe.html

[G13] 判断对象类型
来源：http://hz.316326.xyz/gtdxwbhwxs.html

Py:   isinstance(u, User)
来源：http://hz.xuanzx.com/gtzwgjwqly.html

PHP:  $u instanceof User
来源：http://hz.zhijiandao.cn/gtumudnzww.html

JS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtvrxzujaz.html

TS:   u instanceof User
来源：http://hz.snrcjt.cn/gtjiqmagta.html

Java: u instanceof User
来源：http://hz.nanxinkj.top/gtvshfcwhg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.52xcode.cn/gthusqtany.html

Ruby: u.is_a?(User)
来源：http://hz.jlsjyb.cn/gtusrfkvev.html

C#:   u is User
来源：http://hz.316326.xyz/gtydezdrsw.html

[G14] 数据类 / record
来源：http://hz.cucudq.cn/gtfobeuayg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jyoumei.cn/gtweiisyrr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hnqzz.top/gtyfrltztx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daxiang520.top/gtcpwkpkuz.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuanzhike.top/gtqngubsfm.html

Java: record User(String name, int age) {}
来源：http://hz.jinyuanbaomall.cn/gtpaaftebc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.feifeiyinyue.top/gtcfuwumkl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ybcxt.top/gtasyxnzmr.html

C#:   record User(string Name, int Age);
来源：http://hz.ydzc1.top/gteblxayea.html

[G15] 枚举
来源：http://hz.xingfuxueyuan.xyz/gtxyueqeid.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydjk.org.cn/gtmxhrvouk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xinyue.icu/gtdkjtpcmx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuetiantiany.cn/gtlxwtzyyv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtidrqokky.html

Java: enum Color { RED, GREEN }
来源：http://hz.yonumen.top/gtrgahdrab.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuxming.cn/gtbjuevuyo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.feifeiyinyue.top/gtilbaihxr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtltarlvof.html

[G16] 对象转数组 / 字典
来源：http://hz.hongshengwenyu.top/gtilsljbxy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.pycfn.com/gtevpoulxn.html

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gtrjtgrwkm.html

JS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gteddwvawf.html

TS:   Object.entries(obj)
来源：http://hz.xylfe.cn/gtbvbbegcp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.meibo888.top/gtxosezurs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yuanzhike.top/gtjyzupqiu.html

Ruby: obj.instance_variables
来源：http://hz.9152youxi.cn/gtlnvwjwab.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.pengpengdd.cyou/gtcdufxpni.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtdgymphxz.html

H. 异常与错误处理
来源：http://hz.yongpay.top/gtcryxwtxt.html

================================================================================
来源：http://hz.sufxvd.cn/gtakyizjnu.html

[H01] try / catch 基础
来源：http://hz.zhoulong.xyz/gtravrszpb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhengqikj.top/gtdcorgtie.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.birdmap.top/gtvtkjzmqt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tanke756.top/gtdjqgcphd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xinyue.icu/gtyztugxtf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yueranfly.top/gtixzzqzwh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pengpengdd.cyou/gtmharvert.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenjidiqi.icu/gtvhrqshfx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinqigfzy.top/gtpvjkyolp.html

[H02] finally / ensure 收尾
来源：http://hz.cheryme.top/gtpphqtxul.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtbtiytehc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtuvohetbb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtatnwzmkq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtuwtszdsv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtgkzqtdlt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gotoacloud.top/gtgutsqpsy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jlsjyb.cn/gtvuamxkcm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yongpay.top/gtllyjrtjv.html

[H03] 主动抛出异常
来源：http://hz.cashguo.top/gtbrndlsid.html

Py:   raise ValueError("错误信息")
来源：http://hz.fzhhl.top/gtdetlkebf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtsnfnznmq.html

JS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtrscisebu.html

TS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtiizkmftb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtpdcgujiw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zycfv.cn/gtkkbxtpxt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jyoumei.cn/gtmlzktudv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtufwywdkb.html

[H04] 自定义异常类型
来源：http://hz.yj20258.top/gttuolpwxj.html

Py:   class MyError(Exception): pass
来源：http://hz.andypj.xyz/gtvflhdcbn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gteqtiaazx.html

JS:   class MyError extends Error {}
来源：http://hz.chenjidiqi.icu/gtnbzctmyt.html

TS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gtxyeyqdbb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daria6918.cn/gtiwngldjj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhongyouzk.top/gtldvittwa.html

Ruby: class MyError < StandardError; end
来源：http://hz.zdqjudy.top/gtthotdldv.html

C#:   class MyException : Exception {}
来源：http://hz.kuanghao11.cn/gtoftxesyk.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gtidcgmgib.html

Py:   except ValueError as e:
来源：http://hz.chenzaomai.com/gtcqetvsec.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.smart0.xyz/gttxfohfui.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtfqwcofjk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtjpzwnocm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jiagoushi.top/gtjybuvese.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shangyingyoupin.top/gtkgpwxmst.html

Ruby: rescue ArgumentError => e
来源：http://hz.jlsjyb.cn/gtytoseydi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gtlbkivfos.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xinyue.icu/gtqvcmzmhw.html

Py:   value = d.get("k") or default
来源：http://hz.yvedp.cn/gtbeldydgb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tian-w.cn/gtwquibouo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.52xcode.cn/gtmppzosbo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gtriquizxc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zycfv.cn/gttjzzwspc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gotoacloud.top/gtnjqhorts.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gtriewmgyo.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigufen.top/gthjvnjioz.html

[H07] 断言
来源：http://hz.xziqi.cn/gtdnporhmv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.andypj.xyz/gtktqyqerv.html

PHP:  assert($x > 0);
来源：http://hz.yvedp.cn/gtcmouxqug.html

JS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtnguopazo.html

TS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtypntroip.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnqzz.top/gtogmgaiuj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.svipenyu.cn/gtnvmweqed.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nwbrower.top/gtcecrnfka.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtyafemmud.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhengqikj.top/gtfkorihpq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gtqfusavvj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhaomingkeji.xyz/gtajmbples.html

JS:   e.message;  e.stack
来源：http://hz.sysykeji.top/gtupuemxds.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.feifeiyinyue.top/gtfocnofcp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtnvmwshje.html

Go:   err.Error()
来源：http://hz.zhiwuduotai.top/gtnqawblmy.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenlongwang.top/gtifkdnsge.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jqgfzy.top/gtrplftogm.html

[H09] 带错误码的异常
来源：http://hz.quarkkingdee.top/gtlhwxuhck.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangshuangyany.cn/gtlzbqacsi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhoulong.xyz/gtsxzvqoid.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.birdmap.top/gtjpilqwpj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenjidiqi.icu/gtimwbkfph.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenjidiqi.icu/gtikihvbbi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.0kj1m.cn/gtaromxpla.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.iojbl.cn/gtzcwqtinp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shangyingyoupin.top/gtlococwyq.html

[H10] 资源自动释放
来源：http://hz.redwolf501.top/gtayhaxsqy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgufenzy.top/gtstjqwbfb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuanzhike.top/gtfvhhbonx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gtklacennr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtfumygwfj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yongpay.top/gtbgtfyzjn.html

Go:   defer f.Close()
来源：http://hz.kuanghao11.cn/gteomjvcgj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhongyouzk.top/gtsbnvifdt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yangfankeji.com/gtytvncbdi.html

================================================================================
来源：http://hz.hysaishi.cn/gtwnahuoje.html

I. 正则表达式
来源：http://hz.ydzc1.top/gtyfiarpxx.html

================================================================================
来源：http://hz.guowangkeji.top/gtsmkfqpuw.html

[I01] 判断是否匹配
来源：http://hz.xinyue.icu/gttyyfygay.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenlongwang.top/gtkvoihjzd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gogol.net.cn/gtuojsnild.html

JS:   /\d+/.test(s)
来源：http://hz.aizwys.cn/gtzjtsqvvf.html

TS:   /\d+/.test(s)
来源：http://hz.vqdsnc.cn/gtybaagcfs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.snrcjt.cn/gtermedbkm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.kuanghao11.cn/gtigceycuo.html

Ruby: s.match?(/\d+/)
来源：http://hz.quarkkingdee.top/gtpwrblqwd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gtkvzrvloe.html

[I02] 提取所有匹配
来源：http://hz.sufxvd.cn/gtfhfjduey.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ehwqpu.com/gtskzqkfiu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtduohsptq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gaohongyu789.top/gtstwffene.html

TS:   s.match(/\d+/g)
来源：http://hz.iojbl.cn/gtwwugnqye.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sweek.top/gtdmmtxgfy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hywenlv.cn/gtzcsxmycq.html

Ruby: s.scan(/\d+/)
来源：http://hz.jyoumei.cn/gtlctsbcio.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shangyingyoupin.top/gtmditryxb.html

[I03] 提取捕获分组
来源：http://hz.sweek.top/gtkikrvjxl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangtech.top/gtpxjdcbdo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.fzhhl.top/gtnbopmfit.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ywan-chungtsiang.top/gtccffpdcg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hongshengwenyu.top/gtrmljlflk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj20258888.top/gtnznczwzu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenlongwang.top/gtutnulqdg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhengqikj.top/gtjdpodenr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gzhubu.top/gtqbzvrzcn.html

[I04] 正则替换
来源：http://hz.snrcjt.cn/gtkcgutpac.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.chenlongwang.top/gtzrikcnce.html


<!-- 参考信息 -->