代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtxjwzmwyx.html

TS:   path.extname("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtfhfsjwkk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.52xcode.cn/gtslenvmux.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.smart0.xyz/gtwkjkqtol.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtlrnytzlo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.meibo888.top/gtctkducfr.html

[F11] 复制与移动文件
来源：http://hz.svipenyu.cn/gtkganciop.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtxmyjtbxq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nwbrower.top/gtfumhxesz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtvnefichd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtyxbudsjr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xuanzx.com/gtqjzqepep.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ybcxt.top/gtozipvvat.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtgfzvafvg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cucudq.cn/gtccrkilnh.html

[F12] CSV 读写
来源：http://hz.sysykeji.top/gtoimxawhz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tianlin.xyz/gtirpzqnha.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sxryk.cn/gtpzgbdzqn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yangfankeji.com/gtyofmlwzo.html

TS:   // 同上
来源：http://hz.cheryme.top/gtvilrbjgr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.meibo888.top/gtwfchwdbl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydjk.org.cn/gtjcqqnqct.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.andypj.xyz/gtgcdkqpxs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuxming.cn/gtjsjcdbwv.html

================================================================================
来源：http://hz.ydzc1.top/gtnnizmxuq.html

G. 面向对象
来源：http://hz.0kj1m.cn/gtghgydqzx.html

================================================================================
来源：http://hz.shuidangran.top/gtyyqnftwh.html

[G01] 定义类
来源：http://hz.smart0.xyz/gtwruyxqek.html

Py:   class User: pass
来源：http://hz.ywan-chungtsiang.top/gtiqgnzvxz.html

PHP:  class User {}
来源：http://hz.hfpthk.cn/gtrwrhidpv.html

JS:   class User {}
来源：http://hz.xuanzx.com/gtfqfpxchl.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258888.top/gtltvtlyvp.html

Java: class User {}
来源：http://hz.tian-w.cn/gtiepdvdtx.html

Go:   type User struct { Name string }
来源：http://hz.zycfv.cn/gtsrfcytmd.html

Ruby: class User; end
来源：http://hz.zhongyouzk.top/gtzukvolpf.html

C#:   class User {}
来源：http://hz.hfpthk.cn/gtqnbivxba.html

[G02] 构造函数
来源：http://hz.xuetiantiany.cn/gtdgbqgynu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.havefunace.top/gtxhoorzsl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.quarkkingdee.top/gtcrlsdcdl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtqkaxkphe.html

TS:   constructor(public name: string) {}
来源：http://hz.mhx1999.top/gtswbzutrm.html

Java: User(String name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtmtvfsuwf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuxming.cn/gtshdjwdpe.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zycfv.cn/gtlpghqnpl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenlongwang.top/gtoanvcajw.html

[G03] 实例属性
来源：http://hz.yueranfly.top/gtrpzqktzl.html

Py:   self.name = "x"
来源：http://hz.yanxiufei.cn/gtldklncbp.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtgiobxhpl.html

JS:   this.name = "x";
来源：http://hz.chenlongwang.top/gtoegwafgr.html

TS:   name: string = "x";
来源：http://hz.haohaochexian.top/gtfjkxkroz.html

Java: private String name;
来源：http://hz.sxryk.cn/gtwigyhztq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shzxlz.cn/gtvltlxhyi.html

Ruby: @name = "x"
来源：http://hz.ydzc1.top/gtqfffumld.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuetiantiany.cn/gtllsiffpa.html

[G04] 定义方法
来源：http://hz.shanyushiyangkeji.top/gtiemdrbfy.html

Py:   def greet(self): return self.name
来源：http://hz.yongpay.top/gtleohhnlh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pycfn.com/gtrffeqrjp.html

JS:   greet() { return this.name; }
来源：http://hz.jqgfzy.top/gthxcgxwmm.html

TS:   greet(): string { return this.name; }
来源：http://hz.yonumen.top/gtdycefkpq.html

Java: String greet() { return name; }
来源：http://hz.wangshuangyany.cn/gtmpwjplfz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgfzy.top/gttwbnalyb.html

Ruby: def greet; @name; end
来源：http://hz.zhijiandao.cn/gtdeigziim.html

C#:   public string Greet() => Name;
来源：http://hz.zhixingplan.top/gttfiqjzcp.html

[G05] 继承
来源：http://hz.bjfxy.top/gttnkgryba.html

Py:   class Admin(User): pass
来源：http://hz.zhoulong.xyz/gtfjthniac.html

PHP:  class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtpueuvauq.html

JS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtdmfcgvkb.html

TS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gtppnatqte.html

Java: class Admin extends User {}
来源：http://hz.sweek.top/gtiudnxunk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuanzhike.top/gtodukzwja.html

Ruby: class Admin < User; end
来源：http://hz.redwolf501.top/gtpwibqpsh.html

C#:   class Admin : User {}
来源：http://hz.zhengqikj.top/gtceeinjha.html

[G06] 重写方法
来源：http://hz.zhiwuduotai.top/gtxseffavh.html

Py:   def greet(self): return "admin"
来源：http://hz.daxiang520.top/gtmahnwcag.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtjxsylmtd.html

JS:   greet() { return "admin"; }
来源：http://hz.cqqwz.cn/gtyzimeckz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtwufidhat.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sxryk.cn/gtolsuqxei.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxuanxn.top/gthwknpgts.html

Ruby: def greet; "admin"; end
来源：http://hz.nwbrower.top/gtykfktuwn.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinghuilouyu.cn/gtnubbdejc.html

[G07] 调用父类方法
来源：http://hz.ehwqpu.com/gtputsuhjd.html

Py:   super().greet()
来源：http://hz.zdqjudy.top/gtztuhccna.html

PHP:  parent::greet();
来源：http://hz.chenzaomai.com/gtneibnioq.html

JS:   super.greet();
来源：http://hz.ehwqpu.com/gthuxsuiry.html

TS:   super.greet();
来源：http://hz.hysaishi.cn/gtalxeuniy.html

Java: super.greet();
来源：http://hz.gotoacloud.top/gtqjkmtilm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangdashe.top/gtvbttujlq.html

Ruby: super
来源：http://hz.ydzc1.top/gtbtciopbw.html

C#:   base.Greet();
来源：http://hz.xuetiantiany.cn/gtjtnwghov.html

[G08] 静态方法与属性
来源：http://hz.chenlongwang.top/gthvqukmmn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yongpay.top/gtmyqhrtay.html

PHP:  public static function f() {}
来源：http://hz.jinyuanbaomall.cn/gtuniwmjoo.html

JS:   static f() {}
来源：http://hz.gzhubu.top/gtyahmnuih.html

TS:   static f(): void {}
来源：http://hz.316326.xyz/gtodhnzxhv.html

Java: static void f() {}
来源：http://hz.ppjwa.cn/gtviaviftn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtdgfolbbi.html

Ruby: def self.f; end
来源：http://hz.ivvv.top/gtgzhxupjw.html

C#:   public static void F() {}
来源：http://hz.xylfe.cn/gtzooyvzel.html

[G09] 接口 / 抽象类
来源：http://hz.havefunace.top/gtlpthjutw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yvedp.cn/gtobuhwpji.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sxryk.cn/gttjihgyso.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gtafvxuguu.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gtdyhdefbk.html

Java: interface Shape { double area(); }
来源：http://hz.yonumen.top/gtwnvcngen.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tanke756.top/gtaxbodrgq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tian-w.cn/gtqtrtxker.html

C#:   interface IShape { double Area(); }
来源：http://hz.gotoacloud.top/gtupkiepyu.html

[G10] 访问控制
来源：http://hz.mhx1999.top/gtmxmzvwba.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nwbrower.top/gtarlfzvzy.html

PHP:  public / protected / private
来源：http://hz.chenzaomai.com/gtcrvwzzih.html

JS:   #private 字段；其余公开
来源：http://hz.zhoulong.xyz/gtamnciraa.html

TS:   public / protected / private
来源：http://hz.yuxming.cn/gteqglmnls.html

Java: public / protected / private / 默认包级
来源：http://hz.andypj.xyz/gtslmzznjj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xinyue.icu/gtyfhlwolz.html

Ruby: public / protected / private
来源：http://hz.zhongyouzk.top/gtfvqxrkmn.html

C#:   public / protected / private / internal
来源：http://hz.aizwys.cn/gtfjkmejqk.html

[G11] getter / setter
来源：http://hz.xuetiantiany.cn/gttulzfnms.html

Py:   @property 与 @x.setter
来源：http://hz.mhx1999.top/gtplfekgsm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtyuriyjbe.html

JS:   get name() { return this._name; }
来源：http://hz.nanxuanxn.top/gtczpksmcm.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnxiangtu.top/gtzmypdkkn.html

Java: public String getName() { return name; }
来源：http://hz.guowangkeji.top/gtqbpsdbln.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nwbrower.top/gtdzijmiak.html

Ruby: attr_accessor :name
来源：http://hz.zhoulong.xyz/gthvzrqwfq.html

C#:   public string Name { get; set; }
来源：http://hz.yuxming.cn/gtzoghvkim.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtsxcquoqf.html

Py:   def __str__(self): return self.name
来源：http://hz.pycfn.com/gtwodiuayb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtdjrysmkr.html

JS:   toString() { return this.name; }
来源：http://hz.wangdashe.top/gtazyuolao.html

TS:   toString(): string { return this.name; }
来源：http://hz.havefunace.top/gtqsaverha.html

Java: @Override public String toString() { return name; }
来源：http://hz.kuanghao11.cn/gtcwytmbqc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtcsurovcs.html

Ruby: def to_s; @name; end
来源：http://hz.dashuyun.cn/gtskwvhvbf.html

C#:   public override string ToString() => Name;
来源：http://hz.fengsongda.top/gtydlcigyz.html

[G13] 判断对象类型
来源：http://hz.mhx1999.top/gtvuqsfoby.html

Py:   isinstance(u, User)
来源：http://hz.ydzc1.top/gtejbbmeqx.html

PHP:  $u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtizitbjnb.html

JS:   u instanceof User
来源：http://hz.sweek.top/gtymrzywkk.html

TS:   u instanceof User
来源：http://hz.chenzaomai.com/gtnuovrtvu.html

Java: u instanceof User
来源：http://hz.fengsongda.top/gtobmnlkws.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hfpthk.cn/gtjxozmahx.html

Ruby: u.is_a?(User)
来源：http://hz.snrcjt.cn/gtdwbvffka.html

C#:   u is User
来源：http://hz.zhijiandao.cn/gtnaxwswto.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangkeji.top/gthmweqdie.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.mhx1999.top/gtpucfzzkq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.snrcjt.cn/gttuqhdgcw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenjidiqi.icu/gthjijkqjq.html

TS:   type User = { name: string; age: number };
来源：http://hz.xingfuxueyuan.xyz/gtmbkfekbt.html

Java: record User(String name, int age) {}
来源：http://hz.zhengqikj.top/gtrrbtokjn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jyoumei.cn/gtohdwapdv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtcnlqejfx.html

C#:   record User(string Name, int Age);
来源：http://hz.jiagoushi.top/gtsairudhz.html

[G15] 枚举
来源：http://hz.shanyushiyangkeji.top/gtgvxkrmom.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.pycfn.com/gthilablaq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pengpengdd.cyou/gtbswcrqao.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhijiandao.cn/gtrxowjclm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gthnxyultr.html

Java: enum Color { RED, GREEN }
来源：http://hz.c1oappe.top/gtkupjjvqo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtddfygkmg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gogol.net.cn/gteiqrzlix.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtzvzhpmxk.html

[G16] 对象转数组 / 字典
来源：http://hz.cdnleiting.top/gtssswtldb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhengqikj.top/gtibktpwnx.html

PHP:  get_object_vars($obj);
来源：http://hz.zhiwuduotai.top/gturvuxrdc.html

JS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtrkpuaouu.html

TS:   Object.entries(obj)
来源：http://hz.ydzc1.top/gtskaxqjum.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xylfe.cn/gtiwbanrwi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jlsjyb.cn/gtzcdgcoeo.html

Ruby: obj.instance_variables
来源：http://hz.svipenyu.cn/gtnxedezvo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shzxlz.cn/gtjbltyord.html

================================================================================
来源：http://hz.tianlin.xyz/gtaawtzscv.html

H. 异常与错误处理
来源：http://hz.fengsongda.top/gtwkigonsw.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtjxoaxxqb.html

[H01] try / catch 基础
来源：http://hz.bjfxy.top/gtpmbpgvmz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yonumen.top/gtpzcitkmh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhengqikj.top/gtlwkllaer.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtfwcqdnzf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtzukvanga.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zdqjudy.top/gtfzzjvont.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.0kj1m.cn/gtvxmlbbfp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yanxiufei.cn/gtxxnxrcex.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258.top/gttlebstzl.html

[H02] finally / ensure 收尾
来源：http://hz.iojbl.cn/gtrxqxsmkf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhongyouzk.top/gttkjqhgbb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtmrwloyzl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtokofijtg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtssznetmc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtyttismvv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.birdmap.top/gtcmkutinq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sufxvd.cn/gtqpzpwnih.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtmdelumox.html

[H03] 主动抛出异常
来源：http://hz.cheryme.top/gtkpmiczua.html

Py:   raise ValueError("错误信息")
来源：http://hz.sweek.top/gtetfchplq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtvjbrmdgj.html

JS:   throw new Error("错误信息");
来源：http://hz.hfpthk.cn/gtbbulaxsa.html

TS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtmvikvopd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ivvv.top/gttlcttbdu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.vqdsnc.cn/gtcepsppza.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yongpay.top/gtmxweothm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtoabryrpn.html

[H04] 自定义异常类型
来源：http://hz.jinqigfzy.top/gtqeeazwdj.html

Py:   class MyError(Exception): pass
来源：http://hz.andypj.xyz/gtsfamvcoz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.havefunace.top/gtywpredzh.html

JS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtnkgncsmj.html

TS:   class MyError extends Error {}
来源：http://hz.dashuyun.cn/gtqygcznlk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nwbrower.top/gtotdhdzvw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gzhubu.top/gtwtwnnjxy.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnqzz.top/gtgqcqwgcv.html

C#:   class MyException : Exception {}
来源：http://hz.cqqwz.cn/gtsmdtcbkz.html

[H05] 捕获特定类型
来源：http://hz.xziqi.cn/gttbpavjph.html

Py:   except ValueError as e:
来源：http://hz.tianlin.xyz/gtyxfmdcqt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hammf.cn/gtwgdbpavb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtitigztov.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtgegwbjfh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aibaodan.cn/gtzcpvycan.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.havefunace.top/gttjfqjvei.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydzc1.top/gtlihnzkow.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ehwqpu.com/gttdlaqcwt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuetiantiany.cn/gtwknuyczv.html

Py:   value = d.get("k") or default
来源：http://hz.chenlongwang.top/gtgehjqylm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yonumen.top/gtfxemqvqh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtegpwehln.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtgwxtbnmk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.wangdashe.top/gtvnfyvxvf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sxryk.cn/gtozpymghi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ywan-chungtsiang.top/gtipudjkqq.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinghuilouyu.cn/gtvgcmdaja.html

[H07] 断言
来源：http://hz.jqgufenzy.top/gtubujwjzg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnqzz.top/gtnysheqgy.html

PHP:  assert($x > 0);
来源：http://hz.jinqigfzy.top/gtevkiqvjj.html

JS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gthimmwwdq.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtsdfawrbb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gzhubu.top/gtbckpwbnu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shzxlz.cn/gtnvtrkzfk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ydjk.org.cn/gtlytkartx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gaohongyu789.top/gtbafjcsia.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinyuanbaomall.cn/gttufjlkpr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhiwuduotai.top/gtqdfglafl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ppjwa.cn/gtwdwcrigc.html

JS:   e.message;  e.stack
来源：http://hz.jlsjyb.cn/gtsewmccns.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhaomingkeji.xyz/gtjwayytvs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guannengcc.top/gterjopmzn.html

Go:   err.Error()
来源：http://hz.hywenlv.cn/gtmqrzabrp.html

Ruby: e.message;  e.backtrace
来源：http://hz.guannengcc.top/gtlcxsgnzq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxuanxn.top/gtqbecymyz.html

[H09] 带错误码的异常
来源：http://hz.jinghuilouyu.cn/gtnsnbefvz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pengpengdd.cyou/gtygepopwd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhaomingkeji.xyz/gtrwhyjhub.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.quarkkingdee.top/gtgrzibrld.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sufxvd.cn/gthbbbmkqv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhaomingkeji.xyz/gtjjkxdnmz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tian-w.cn/gtiuvlohkk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.mhx1999.top/gtgawhtbfv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sysykeji.top/gteqcuskmp.html

[H10] 资源自动释放
来源：http://hz.yuanzhike.top/gtfggrszsf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tianlin.xyz/gtjwxxowoq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.c1oappe.top/gtmwrtnxud.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtheilxqgf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtaehhpkap.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhaomingkeji.xyz/gtqlbdhryn.html

Go:   defer f.Close()
来源：http://hz.cashguo.top/gtqsubluto.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.iojbl.cn/gtqtltlxej.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangdashe.top/gtishcvtyd.html

================================================================================
来源：http://hz.xuanzx.com/gtasokbxsq.html

I. 正则表达式
来源：http://hz.mhx1999.top/gtcvnwjbot.html

================================================================================
来源：http://hz.sweek.top/gtbedbjmia.html

[I01] 判断是否匹配
来源：http://hz.xziqi.cn/gtozubyxpl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtaecxujup.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shangyingyoupin.top/gttqcgxrbb.html

JS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtrmtfqzcg.html

TS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtccqeldyj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yonumen.top/gtlusykwiw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhijiandao.cn/gtidbrkhaj.html

Ruby: s.match?(/\d+/)
来源：http://hz.gaohongyu789.top/gtfmmaziif.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenzaomai.com/gtdgxjxhiw.html

[I02] 提取所有匹配
来源：http://hz.cucudq.cn/gtcmtpzzpz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtwlkgcpac.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtozafjobd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.dianchejie.cn/gtcdirfnwc.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtbztkuori.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.iojbl.cn/gtbcuoxpjy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.dashuyun.cn/gtpjrttewo.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxuanxn.top/gtmyusukui.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shzxlz.cn/gtjzkvrlap.html

[I03] 提取捕获分组
来源：http://hz.birdmap.top/gtvugdmuzp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhiwuduotai.top/gtvydljlba.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gtsxeopcmr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhijiandao.cn/gtkzogaqgt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gteyrgqorp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fzhhl.top/gtdexxebrf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hammf.cn/gthdburkwt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhengqikj.top/gtfkngoill.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gaohongyu789.top/gtpechijem.html

[I04] 正则替换
来源：http://hz.9152youxi.cn/gtlivrdvsl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yueranfly.top/gtfyybpwwl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.redwolf501.top/gtjabxffot.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gtazrewtqi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtsclrhzjo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xinyue.icu/gtvodnifaf.html


<!-- 参考信息 -->