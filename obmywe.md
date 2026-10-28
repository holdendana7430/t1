代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtsonbtnpp.html

TS:   path.extname("a.txt")
来源：http://hz.jianghu66.top/gtpfcpmgmv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jianghu66.top/gtepiolocl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.nwbrower.top/gtvwfqxdmm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtorfvnxjd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtiugejiim.html

[F11] 复制与移动文件
来源：http://hz.nanxinkj.top/gtnnkgmmox.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhixingplan.top/gtmyregapx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuanzx.com/gtgllznyds.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtxdytgaqk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtgqxxyzpe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zdqjudy.top/gtxrizwolg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xingfuxueyuan.xyz/gtrsbglfbp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cheryme.top/gthkvwusww.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtwknfofxv.html

[F12] CSV 读写
来源：http://hz.wangshuangyany.cn/gtkrzhuzxe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigufen.top/gtzkmycjwm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nwbrower.top/gtrbokvcxl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.vqdsnc.cn/gtuqpdhuhz.html

TS:   // 同上
来源：http://hz.zhixingplan.top/gtgeapvezl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jyoumei.cn/gtgojtcqqy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tanke756.top/gtwoiuvyln.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.fzhhl.top/gtdesdgijg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tanke756.top/gtwvbtyupw.html

================================================================================
来源：http://hz.jyoumei.cn/gtcjmxhttu.html

G. 面向对象
来源：http://hz.9152youxi.cn/gtujaibmda.html

================================================================================
来源：http://hz.zycfv.cn/gtsbchublb.html

[G01] 定义类
来源：http://hz.tian-w.cn/gtjqulrviq.html

Py:   class User: pass
来源：http://hz.yangfankeji.com/gtdxhsrevw.html

PHP:  class User {}
来源：http://hz.jqgufenzy.top/gtdlnzwjic.html

JS:   class User {}
来源：http://hz.fengsongda.top/gtcdwxtixl.html

TS:   class User { name: string = ""; }
来源：http://hz.ivvv.top/gtrverqysx.html

Java: class User {}
来源：http://hz.jyoumei.cn/gtyjadtebe.html

Go:   type User struct { Name string }
来源：http://hz.havefunace.top/gtauiyslis.html

Ruby: class User; end
来源：http://hz.nwbrower.top/gtdkkskzkc.html

C#:   class User {}
来源：http://hz.xuetiantiany.cn/gtenxzefoi.html

[G02] 构造函数
来源：http://hz.jinghuilouyu.cn/gtcbeoryyl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shangyingyoupin.top/gtcxlmnuxa.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.316326.xyz/gtoternppd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tian-w.cn/gtevfodyto.html

TS:   constructor(public name: string) {}
来源：http://hz.yangfankeji.com/gtmlaesyyg.html

Java: User(String name) { this.name = name; }
来源：http://hz.sysykeji.top/gtvqcsmwpe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.feifeiyinyue.top/gtibmgiesz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxinkj.top/gtswsojklm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sweek.top/gtpxrobzjg.html

[G03] 实例属性
来源：http://hz.jinghuilouyu.cn/gtrgucdves.html

Py:   self.name = "x"
来源：http://hz.c1oappe.top/gtqxsgtuns.html

PHP:  public string $name = "x";
来源：http://hz.jinghuilouyu.cn/gtiozfnkjo.html

JS:   this.name = "x";
来源：http://hz.hongshengwenyu.top/gtdtewhkpu.html

TS:   name: string = "x";
来源：http://hz.meibo888.top/gthcydxxob.html

Java: private String name;
来源：http://hz.tian-w.cn/gtlnjyrnwo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cdnleiting.top/gtpxyxsjim.html

Ruby: @name = "x"
来源：http://hz.hywenlv.cn/gtnsernmov.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangtech.top/gtmfcqdlac.html

[G04] 定义方法
来源：http://hz.gaohongyu789.top/gtvejttrgf.html

Py:   def greet(self): return self.name
来源：http://hz.shanyushiyangtech.top/gtsydfvpuu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtqamceytv.html

JS:   greet() { return this.name; }
来源：http://hz.ivvv.top/gtilierbps.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenlongwang.top/gtldtgjkyu.html

Java: String greet() { return name; }
来源：http://hz.cucudq.cn/gtulzxubyl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtlvsrvzbg.html

Ruby: def greet; @name; end
来源：http://hz.jinqigfzy.top/gtpqjxxcwa.html

C#:   public string Greet() => Name;
来源：http://hz.jianghu66.top/gthmonklia.html

[G05] 继承
来源：http://hz.ppjwa.cn/gtulrdovnt.html

Py:   class Admin(User): pass
来源：http://hz.jyoumei.cn/gtymnzdfqc.html

PHP:  class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtjmaeqafu.html

JS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtsnqchgre.html

TS:   class Admin extends User {}
来源：http://hz.cheryme.top/gtfynazfwi.html

Java: class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtbtybmbmq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shzxlz.cn/gtrakmoqhk.html

Ruby: class Admin < User; end
来源：http://hz.ywan-chungtsiang.top/gtaqckhidw.html

C#:   class Admin : User {}
来源：http://hz.tianlin.xyz/gtlgijwgsn.html

[G06] 重写方法
来源：http://hz.xingfuxueyuan.xyz/gtpvzlhedt.html

Py:   def greet(self): return "admin"
来源：http://hz.cheryme.top/gtqmhwveqs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtsmayymjk.html

JS:   greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtqnaiduvy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtwpvrtqmc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtnagcampg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhengqikj.top/gtiljuawtl.html

Ruby: def greet; "admin"; end
来源：http://hz.guowangkeji.top/gthorimllq.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangkeji.top/gtxjbrfjjy.html

[G07] 调用父类方法
来源：http://hz.jinqigfzy.top/gtlfafrpex.html

Py:   super().greet()
来源：http://hz.gogol.net.cn/gthifmoqmw.html

PHP:  parent::greet();
来源：http://hz.meibo888.top/gtcpymzuzh.html

JS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtxxghjrnc.html

TS:   super.greet();
来源：http://hz.ydzc1.top/gtjijicpqa.html

Java: super.greet();
来源：http://hz.smart0.xyz/gtinzrjvjc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigfzy.top/gtxzxsjsii.html

Ruby: super
来源：http://hz.shanyushiyangkeji.top/gtnnlsnhli.html

C#:   base.Greet();
来源：http://hz.ybcxt.top/gttcbtwbgu.html

[G08] 静态方法与属性
来源：http://hz.guowangkeji.top/gtwmjfdrks.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhongyouzk.top/gtqqoflenf.html

PHP:  public static function f() {}
来源：http://hz.gotoacloud.top/gtpncqxwxm.html

JS:   static f() {}
来源：http://hz.gzhubu.top/gtozsadjqv.html

TS:   static f(): void {}
来源：http://hz.daxiang520.top/gtynosnznf.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtwrclztic.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.andypj.xyz/gtyyohkepr.html

Ruby: def self.f; end
来源：http://hz.zycfv.cn/gtdzsdltyg.html

C#:   public static void F() {}
来源：http://hz.jinghuilouyu.cn/gtdmbppiqc.html

[G09] 接口 / 抽象类
来源：http://hz.fzhhl.top/gtsfodkich.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gtfvroxkxg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daria6918.cn/gtzvdobzyv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fzhhl.top/gtgbtqshhu.html

TS:   interface Shape { area(): number; }
来源：http://hz.haohaochexian.top/gtvwyclvsc.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258.top/gtiladdwrr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daria6918.cn/gtmdituovj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ppjwa.cn/gtxxojdgod.html

C#:   interface IShape { double Area(); }
来源：http://hz.0kj1m.cn/gtmuxyuvzl.html

[G10] 访问控制
来源：http://hz.zhaomingkeji.xyz/gtydqxosww.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yonumen.top/gtkbamhlet.html

PHP:  public / protected / private
来源：http://hz.pycfn.com/gttrxfuehh.html

JS:   #private 字段；其余公开
来源：http://hz.zhijiandao.cn/gtojlltrhk.html

TS:   public / protected / private
来源：http://hz.gzhubu.top/gtirsitiks.html

Java: public / protected / private / 默认包级
来源：http://hz.meibo888.top/gtoerwtttq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fzhhl.top/gtndeqgjsd.html

Ruby: public / protected / private
来源：http://hz.xinyue.icu/gtfaojwxtd.html

C#:   public / protected / private / internal
来源：http://hz.zhoulong.xyz/gtykujxiuz.html

[G11] getter / setter
来源：http://hz.wangdashe.top/gtvtlhjyzi.html

Py:   @property 与 @x.setter
来源：http://hz.jlsjyb.cn/gtcukwaure.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cashguo.top/gtheklducp.html

JS:   get name() { return this._name; }
来源：http://hz.hysaishi.cn/gthicjtyis.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gtcjygobrs.html

Java: public String getName() { return name; }
来源：http://hz.zhongyouzk.top/gtlpsedfpk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tanke756.top/gtdonmgbod.html

Ruby: attr_accessor :name
来源：http://hz.feifeiyinyue.top/gtuwxknoym.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtibmukqfu.html

[G12] 对象转字符串
来源：http://hz.wangshuangyany.cn/gtqijnnrvf.html

Py:   def __str__(self): return self.name
来源：http://hz.fzhhl.top/gtilmejayh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtrrjxdnpv.html

JS:   toString() { return this.name; }
来源：http://hz.zhongyouzk.top/gtxcembxkc.html

TS:   toString(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gtaabewzka.html

Java: @Override public String toString() { return name; }
来源：http://hz.aibaodan.cn/gtyrtncsos.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yueranfly.top/gtnavplknp.html

Ruby: def to_s; @name; end
来源：http://hz.kuanghao11.cn/gtgfchmulv.html

C#:   public override string ToString() => Name;
来源：http://hz.gzhubu.top/gteneozwcy.html

[G13] 判断对象类型
来源：http://hz.nanxuanxn.top/gtmjdoduqh.html

Py:   isinstance(u, User)
来源：http://hz.fzhhl.top/gtzjvznlkf.html

PHP:  $u instanceof User
来源：http://hz.gotoacloud.top/gtvjjhozuj.html

JS:   u instanceof User
来源：http://hz.yuanzhike.top/gtfspwnasz.html

TS:   u instanceof User
来源：http://hz.hammf.cn/gtnbdmtpju.html

Java: u instanceof User
来源：http://hz.nanxuanxn.top/gtoeisiihg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jianghu66.top/gtrweoyiqf.html

Ruby: u.is_a?(User)
来源：http://hz.0kj1m.cn/gttzeqpgwn.html

C#:   u is User
来源：http://hz.ybcxt.top/gtrnsgomfm.html

[G14] 数据类 / record
来源：http://hz.smart0.xyz/gtzzehhrxh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258.top/gtakeqcgxy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yvedp.cn/gtxqdmwoas.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxuanxn.top/gtivfecrby.html

TS:   type User = { name: string; age: number };
来源：http://hz.aibaodan.cn/gtpmmpdwzg.html

Java: record User(String name, int age) {}
来源：http://hz.nwbrower.top/gteyxwqqzn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hnxiangtu.top/gtiqjsotwn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pengpengdd.cyou/gtousccarx.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgufenzy.top/gtzevqmmlm.html

[G15] 枚举
来源：http://hz.yangfankeji.com/gtubzxpkeq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shzxlz.cn/gtjhyqzrds.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gotoacloud.top/gtzswvokfy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.52xcode.cn/gtpigwptdg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hywenlv.cn/gtyjuptuus.html

Java: enum Color { RED, GREEN }
来源：http://hz.xylfe.cn/gtfkggvdls.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.dashuyun.cn/gtaovjoplk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cucudq.cn/gtauefotxo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtctvnusjz.html

[G16] 对象转数组 / 字典
来源：http://hz.fzhhl.top/gtcnldpkrr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dianchejie.cn/gtegpnufqw.html

PHP:  get_object_vars($obj);
来源：http://hz.ivvv.top/gtyfzscgxe.html

JS:   Object.entries(obj)
来源：http://hz.ydzc1.top/gtygfawuho.html

TS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtgjoikudt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ppjwa.cn/gtkmsgusik.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhaomingkeji.xyz/gtzdcsqqke.html

Ruby: obj.instance_variables
来源：http://hz.tianlin.xyz/gtckgtxnac.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jlsjyb.cn/gtlnhgxibq.html

================================================================================
来源：http://hz.hywenlv.cn/gtinjffqge.html

H. 异常与错误处理
来源：http://hz.quarkkingdee.top/gtlwlpucgt.html

================================================================================
来源：http://hz.snrcjt.cn/gthjouvevu.html

[H01] try / catch 基础
来源：http://hz.hfpthk.cn/gtwnxgczhz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.daxiang520.top/gtmoevzdyt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnqzz.top/gtoepcqwxt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258.top/gtdwjyuvwl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhixingplan.top/gtcptqrewx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhaomingkeji.xyz/gthurbudya.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shzxlz.cn/gtsppokldu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aizwys.cn/gtwsgcbvvi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guowangkeji.top/gtnomzgcvk.html

[H02] finally / ensure 收尾
来源：http://hz.gotoacloud.top/gttiyqyldy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.iojbl.cn/gtsvubiojt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtunojepuj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtqtdqfmlq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtwbgaxoho.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gttgxjtnln.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zycfv.cn/gthbuyewnb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.haohaochexian.top/gtvichnhju.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhijiandao.cn/gtqouxmqzu.html

[H03] 主动抛出异常
来源：http://hz.xuetiantiany.cn/gtntmfiyxr.html

Py:   raise ValueError("错误信息")
来源：http://hz.yanxiufei.cn/gtxmakshyc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtxgoowtzs.html

JS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtwwuenhoy.html

TS:   throw new Error("错误信息");
来源：http://hz.aibaodan.cn/gtddjgulbv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtccutwuks.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sweek.top/gtbhrwjtmo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guowangkeji.top/gtquxvdvye.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gtgtzlrmde.html

[H04] 自定义异常类型
来源：http://hz.9152youxi.cn/gtzrrqyaiy.html

Py:   class MyError(Exception): pass
来源：http://hz.feifeiyinyue.top/gtziogcgyr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuanzhike.top/gtxjoaiegw.html

JS:   class MyError extends Error {}
来源：http://hz.xuanzx.com/gtggboyfhp.html

TS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gterxejhpv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.bjfxy.top/gtwnurrvvc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xuanzx.com/gtjnhgkaqf.html

Ruby: class MyError < StandardError; end
来源：http://hz.tianlin.xyz/gtkeesqeuj.html

C#:   class MyException : Exception {}
来源：http://hz.redwolf501.top/gtnyqluuff.html

[H05] 捕获特定类型
来源：http://hz.fzhhl.top/gternehmap.html

Py:   except ValueError as e:
来源：http://hz.zhaomingkeji.xyz/gtgkiyokrm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dashuyun.cn/gtvzmrfvlr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.52xcode.cn/gtrnwndekb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.svipenyu.cn/gttqwefkfp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.pycfn.com/gtipjdhfst.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.snrcjt.cn/gtdqdtzwve.html

Ruby: rescue ArgumentError => e
来源：http://hz.daxiang520.top/gtbpayxvdg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.daria6918.cn/gtdmzgrrfq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jianghu66.top/gtyoizgowr.html

Py:   value = d.get("k") or default
来源：http://hz.jlsjyb.cn/gtzlwwxsug.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuxming.cn/gtqzsadqov.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.c1oappe.top/gtfxpawpvd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtgemrtgxb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.fzhhl.top/gtbyvoimum.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ppjwa.cn/gtfrtwckwp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shuidangran.top/gtakigyyit.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gttdjyvvvq.html

[H07] 断言
来源：http://hz.guannengcc.top/gtxzzmhmdm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zdqjudy.top/gtkbkeohwg.html

PHP:  assert($x > 0);
来源：http://hz.c1oappe.top/gtrdcddhkv.html

JS:   console.assert(x > 0);
来源：http://hz.sysykeji.top/gtgkykavrx.html

TS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtjtpkrzmc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangkeji.top/gteaocorry.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tianlin.xyz/gtsgpcgvod.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shanyushiyangtech.top/gtxaywsxep.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sweek.top/gtexyibogs.html

[H08] 获取错误信息与堆栈
来源：http://hz.shanyushiyangkeji.top/gthzeltiye.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhaomingkeji.xyz/gtslqhbnqr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pycfn.com/gtbywcjgnf.html

JS:   e.message;  e.stack
来源：http://hz.hammf.cn/gtftkvmssc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.mhx1999.top/gtyotucjsa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yanxiufei.cn/gtjibmltab.html

Go:   err.Error()
来源：http://hz.yj202588.top/gtkwywhivl.html

Ruby: e.message;  e.backtrace
来源：http://hz.sufxvd.cn/gtqitpgqqq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhixingplan.top/gtbikzbbem.html

[H09] 带错误码的异常
来源：http://hz.hnqzz.top/gtykagryie.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.iojbl.cn/gtyjwkrdhl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenjidiqi.icu/gtnshwmtkw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhengqikj.top/gtcuqzyuer.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sufxvd.cn/gtfrvixrwh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sweek.top/gtxwrpsnam.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yueranfly.top/gtpdoveoln.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hammf.cn/gtgdfmlfda.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dianchejie.cn/gtqekyuoiv.html

[H10] 资源自动释放
来源：http://hz.redwolf501.top/gtiavtpdpy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.iojbl.cn/gtfjigoelg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nwbrower.top/gtfetlwpzk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gtyecmuofy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtlcoqswgg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtpjihwjcm.html

Go:   defer f.Close()
来源：http://hz.chenlongwang.top/gtlnotjrgj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.snrcjt.cn/gtecumnnsm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jlsjyb.cn/gtelbbcvtj.html

================================================================================
来源：http://hz.cheryme.top/gtqlsiwggm.html

I. 正则表达式
来源：http://hz.feifeiyinyue.top/gtobyvczbv.html

================================================================================
来源：http://hz.daxiang520.top/gtgezcuiit.html

[I01] 判断是否匹配
来源：http://hz.ppjwa.cn/gtzwlvoehs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtqvhfupsg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dashuyun.cn/gtpcdygpgc.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigfzy.top/gtnbeafmzv.html

TS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtvcuilgir.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cashguo.top/gtrmwjhnja.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shuidangran.top/gtuqljltxs.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxinkj.top/gtklsfmcfj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jyoumei.cn/gtovtanxab.html

[I02] 提取所有匹配
来源：http://hz.zhengqikj.top/gtzybhozwa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shangyingyoupin.top/gtlomfqzku.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gtjywuehel.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gotoacloud.top/gtsfbiomvz.html

TS:   s.match(/\d+/g)
来源：http://hz.jiagoushi.top/gtdzckjkiz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jiagoushi.top/gtyiioerxx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sufxvd.cn/gtuhvndfuu.html

Ruby: s.scan(/\d+/)
来源：http://hz.daria6918.cn/gtsdbvwfdl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cucudq.cn/gttjhdnkwk.html

[I03] 提取捕获分组
来源：http://hz.52xcode.cn/gtemhwocly.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.smart0.xyz/gtmtobjdrc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shangyingyoupin.top/gtbwhfxwdz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jqgfzy.top/gthkcxzclb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigfzy.top/gtvgiaonte.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj20258.top/gtogeegymm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yuxming.cn/gtgpntafvr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.havefunace.top/gtlhteyugw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xinyue.icu/gtshqlbaos.html

[I04] 正则替换
来源：http://hz.sysykeji.top/gtslvokyxj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.quarkkingdee.top/gtmwtpigyx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tianlin.xyz/gtisldnkjg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.mhx1999.top/gtutqcslhc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gthryhssqt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gotoacloud.top/gtugeyegfm.html


<!-- 参考信息 -->