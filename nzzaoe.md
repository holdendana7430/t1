代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtmmwyccye.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xziqi.cn/gtmqyxgmvz.html

[F11] 复制与移动文件
来源：http://hz.9152youxi.cn/gtyumhrici.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtxeqkbflj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jiagoushi.top/gtkzpanrso.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtkskzqbna.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtlqeglhsi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tanke756.top/gtcgbxmxkc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tanke756.top/gtbcwkfllc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtbczhjnpe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.kuanghao11.cn/gtcrfjdchm.html

[F12] CSV 读写
来源：http://hz.wangshuangyany.cn/gthshcfaqk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhaomingkeji.xyz/gthlgvffis.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangtech.top/gtpuncnikp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yonumen.top/gtlnvnncyi.html

TS:   // 同上
来源：http://hz.zhongyouzk.top/gthznwiojp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cucudq.cn/gtjovtncbq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ybcxt.top/gtdwwwjdei.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shzxlz.cn/gtlrufrmgh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhixingplan.top/gtgkhhrcqg.html

================================================================================
来源：http://hz.sxryk.cn/gtshxjbdjb.html

G. 面向对象
来源：http://hz.chenzaomai.com/gtbczzykco.html

================================================================================
来源：http://hz.yangfankeji.com/gtxovyrbak.html

[G01] 定义类
来源：http://hz.ehwqpu.com/gtavsghcbj.html

Py:   class User: pass
来源：http://hz.jianghu66.top/gtpnjfbima.html

PHP:  class User {}
来源：http://hz.xuetiantiany.cn/gtsffruptb.html

JS:   class User {}
来源：http://hz.shuidangran.top/gtnqdjgpnj.html

TS:   class User { name: string = ""; }
来源：http://hz.dashuyun.cn/gtvujfmxet.html

Java: class User {}
来源：http://hz.cashguo.top/gtptodmpug.html

Go:   type User struct { Name string }
来源：http://hz.nanxinkj.top/gtlgzmuqop.html

Ruby: class User; end
来源：http://hz.birdmap.top/gtbdyihcjj.html

C#:   class User {}
来源：http://hz.pengpengdd.cyou/gtkylsudfd.html

[G02] 构造函数
来源：http://hz.jinghuilouyu.cn/gtnvodejmh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtewwvkpxw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fengsongda.top/gtmygokylx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gtnyrsftui.html

TS:   constructor(public name: string) {}
来源：http://hz.yvedp.cn/gtmmoudkwu.html

Java: User(String name) { this.name = name; }
来源：http://hz.cashguo.top/gtzoddouov.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shzxlz.cn/gtyicmsfob.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fengsongda.top/gtmbujcdvr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtvhynumyz.html

[G03] 实例属性
来源：http://hz.gotoacloud.top/gtdtsvqqwo.html

Py:   self.name = "x"
来源：http://hz.zhoulong.xyz/gtevtnjprw.html

PHP:  public string $name = "x";
来源：http://hz.shzxlz.cn/gtuyuhrwvq.html

JS:   this.name = "x";
来源：http://hz.c1oappe.top/gtylggztwu.html

TS:   name: string = "x";
来源：http://hz.aibaodan.cn/gtyjciobaq.html

Java: private String name;
来源：http://hz.shangyingyoupin.top/gtkhakvair.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.smart0.xyz/gtehlmdcyr.html

Ruby: @name = "x"
来源：http://hz.zhiwuduotai.top/gtgaxrqspd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.iojbl.cn/gtcifjylvn.html

[G04] 定义方法
来源：http://hz.zdqjudy.top/gtebzkapwq.html

Py:   def greet(self): return self.name
来源：http://hz.yvedp.cn/gtsjelqqpg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtqbrtqmxo.html

JS:   greet() { return this.name; }
来源：http://hz.feifeiyinyue.top/gtrbzlgxca.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtvdsfqkpn.html

Java: String greet() { return name; }
来源：http://hz.chenjidiqi.icu/gtlmdzooto.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yuxming.cn/gtwgykxfit.html

Ruby: def greet; @name; end
来源：http://hz.chenlongwang.top/gtzifbxlxo.html

C#:   public string Greet() => Name;
来源：http://hz.52xcode.cn/gtqpbuinnt.html

[G05] 继承
来源：http://hz.wangshuangyany.cn/gtvexkofxj.html

Py:   class Admin(User): pass
来源：http://hz.wangshuangyany.cn/gtucmadvaa.html

PHP:  class Admin extends User {}
来源：http://hz.hywenlv.cn/gtylmlocvn.html

JS:   class Admin extends User {}
来源：http://hz.daxiang520.top/gtamhkadcu.html

TS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtnnxdoujg.html

Java: class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtrneupftn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cqqwz.cn/gtjtdoxxgo.html

Ruby: class Admin < User; end
来源：http://hz.xylfe.cn/gtkrngfcgb.html

C#:   class Admin : User {}
来源：http://hz.ywan-chungtsiang.top/gtdapqnfmx.html

[G06] 重写方法
来源：http://hz.shzxlz.cn/gtuydijqrh.html

Py:   def greet(self): return "admin"
来源：http://hz.chenjidiqi.icu/gtlaqqpexz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtkllkestr.html

JS:   greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtpiahljrs.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtpzamkpst.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hammf.cn/gtopxyjcxy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zycfv.cn/gtfafvzywx.html

Ruby: def greet; "admin"; end
来源：http://hz.fzhhl.top/gturdywuxi.html

C#:   public override string Greet() => "admin";
来源：http://hz.guannengcc.top/gtfytjinko.html

[G07] 调用父类方法
来源：http://hz.zhiwuduotai.top/gtahcyndab.html

Py:   super().greet()
来源：http://hz.yuanzhike.top/gtzaevvxmw.html

PHP:  parent::greet();
来源：http://hz.yj20258.top/gtdplfciyq.html

JS:   super.greet();
来源：http://hz.hywenlv.cn/gtdmsuvgvg.html

TS:   super.greet();
来源：http://hz.ivvv.top/gtonpwgwwa.html

Java: super.greet();
来源：http://hz.shangyingyoupin.top/gtdoskqmhy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.smart0.xyz/gtvuatohez.html

Ruby: super
来源：http://hz.svipenyu.cn/gtfdenkcqa.html

C#:   base.Greet();
来源：http://hz.yangfankeji.com/gtzyxnzqwk.html

[G08] 静态方法与属性
来源：http://hz.aibaodan.cn/gtcdksatos.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jianghu66.top/gtlcqjswnv.html

PHP:  public static function f() {}
来源：http://hz.yj202588.top/gtcvsavcbf.html

JS:   static f() {}
来源：http://hz.kuanghao11.cn/gtqvgteeti.html

TS:   static f(): void {}
来源：http://hz.xinyue.icu/gttbwsjtqp.html

Java: static void f() {}
来源：http://hz.sweek.top/gtgprmwouo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yonumen.top/gtatdrlkuo.html

Ruby: def self.f; end
来源：http://hz.cqqwz.cn/gteqyacmlo.html

C#:   public static void F() {}
来源：http://hz.hywenlv.cn/gtfsttjhym.html

[G09] 接口 / 抽象类
来源：http://hz.jianghu66.top/gtlmuqzdmq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.9152youxi.cn/gtsfegdcnr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.haohaochexian.top/gtepdlxdwx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yanxiufei.cn/gtcxlrjxiv.html

TS:   interface Shape { area(): number; }
来源：http://hz.daria6918.cn/gtoxytyhhd.html

Java: interface Shape { double area(); }
来源：http://hz.aizwys.cn/gtuhhgmywj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yongpay.top/gthyxeyrpw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.pycfn.com/gtxpxnhdbi.html

C#:   interface IShape { double Area(); }
来源：http://hz.zdqjudy.top/gtehqmtgpt.html

[G10] 访问控制
来源：http://hz.cashguo.top/gtixmkvhfm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nanxinkj.top/gtyzrftimn.html

PHP:  public / protected / private
来源：http://hz.ydjk.org.cn/gtdhbjmtng.html

JS:   #private 字段；其余公开
来源：http://hz.zhoulong.xyz/gtkwhhtlsm.html

TS:   public / protected / private
来源：http://hz.ydzc1.top/gtcxfhhrnm.html

Java: public / protected / private / 默认包级
来源：http://hz.guowangkeji.top/gtywoslhqp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhongyouzk.top/gtdxgqpktv.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtwfogwisr.html

C#:   public / protected / private / internal
来源：http://hz.hnqzz.top/gtywtfzqpo.html

[G11] getter / setter
来源：http://hz.ydjk.org.cn/gtcuovappq.html

Py:   @property 与 @x.setter
来源：http://hz.zdqjudy.top/gtpgbwnfzp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtpfbymeen.html

JS:   get name() { return this._name; }
来源：http://hz.andypj.xyz/gtunvgkwuz.html

TS:   get name(): string { return this._name; }
来源：http://hz.pengpengdd.cyou/gtqggxngxi.html

Java: public String getName() { return name; }
来源：http://hz.kuanghao11.cn/gtvitapptj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtgbmdhqko.html

Ruby: attr_accessor :name
来源：http://hz.hfpthk.cn/gtzvafyuvv.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gtipwphnha.html

[G12] 对象转字符串
来源：http://hz.pengpengdd.cyou/gtabeurisg.html

Py:   def __str__(self): return self.name
来源：http://hz.nwbrower.top/gtysgxjkci.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtsreogmqn.html

JS:   toString() { return this.name; }
来源：http://hz.ppjwa.cn/gtixjwuwie.html

TS:   toString(): string { return this.name; }
来源：http://hz.feifeiyinyue.top/gtfhuvrwal.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258888.top/gtpdhmpibv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtvtlwrzdg.html

Ruby: def to_s; @name; end
来源：http://hz.zhaomingkeji.xyz/gttdnzzsdx.html

C#:   public override string ToString() => Name;
来源：http://hz.jianghu66.top/gtesjmrxdt.html

[G13] 判断对象类型
来源：http://hz.redwolf501.top/gtnjvqcqck.html

Py:   isinstance(u, User)
来源：http://hz.aizwys.cn/gtnekzaayw.html

PHP:  $u instanceof User
来源：http://hz.vqdsnc.cn/gtvotmuntd.html

JS:   u instanceof User
来源：http://hz.daria6918.cn/gtvhbukyax.html

TS:   u instanceof User
来源：http://hz.chenzaomai.com/gtjtuacpev.html

Java: u instanceof User
来源：http://hz.9152youxi.cn/gtirkapzzn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtbvxohaoc.html

Ruby: u.is_a?(User)
来源：http://hz.aibaodan.cn/gtvxqeotfb.html

C#:   u is User
来源：http://hz.jqgufenzy.top/gtwwqucfmg.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtqffqzuzc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.andypj.xyz/gtzzqxeibz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hammf.cn/gtieihanoh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xziqi.cn/gtzoxjszvr.html

TS:   type User = { name: string; age: number };
来源：http://hz.ppjwa.cn/gtopouokim.html

Java: record User(String name, int age) {}
来源：http://hz.xuanzx.com/gtimzmsqgn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gtzvrirkgg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hammf.cn/gtjothcjkk.html

C#:   record User(string Name, int Age);
来源：http://hz.yanxiufei.cn/gtaoubkfnz.html

[G15] 枚举
来源：http://hz.jinqigfzy.top/gtlboasqzo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yongpay.top/gtiypvgpoy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.52xcode.cn/gtswuexqof.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hongshengwenyu.top/gtqwsvqgsd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gthqfxcncx.html

Java: enum Color { RED, GREEN }
来源：http://hz.guowangkeji.top/gtjrahpnol.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhoulong.xyz/gtpvzzalse.html

Ruby: Color = %i[red green].freeze
来源：http://hz.smart0.xyz/gtnymxjqrq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.bjfxy.top/gtxxbtkasm.html

[G16] 对象转数组 / 字典
来源：http://hz.yvedp.cn/gtivyfchiz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.9152youxi.cn/gtzsskqwgp.html

PHP:  get_object_vars($obj);
来源：http://hz.mhx1999.top/gtsvynkirg.html

JS:   Object.entries(obj)
来源：http://hz.guowangkeji.top/gtjaokgtfw.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtuyutwbyk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hysaishi.cn/gtorojedrq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ybcxt.top/gtiioclkfv.html

Ruby: obj.instance_variables
来源：http://hz.wangdashe.top/gtfafdfblh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sysykeji.top/gtnklaalug.html

================================================================================
来源：http://hz.aibaodan.cn/gtvygtyivn.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gtpwvelcax.html

================================================================================
来源：http://hz.gzhubu.top/gtttghvyej.html

[H01] try / catch 基础
来源：http://hz.tanke756.top/gtbgjmzfdr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.snrcjt.cn/gtglbjbmal.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.meibo888.top/gtgjirbyfp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zycfv.cn/gtsniqtata.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtlrxrjafq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.fengsongda.top/gtamjdhqkp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258.top/gtnkzxtslb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.iojbl.cn/gtvghdfeco.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.haohaochexian.top/gtiesjbgib.html

[H02] finally / ensure 收尾
来源：http://hz.c1oappe.top/gtxrsxdxtu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhoulong.xyz/gtyvqewjbo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtvjhbztdk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtcrtntqoo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtntsphuhq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtjpvoinaz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnxiangtu.top/gthldwyrxa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258888.top/gtgtmtxwtw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.smart0.xyz/gtyssnjldr.html

[H03] 主动抛出异常
来源：http://hz.xingfuxueyuan.xyz/gtbkaszmvv.html

Py:   raise ValueError("错误信息")
来源：http://hz.52xcode.cn/gtxlhrybhb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtgwvscxkq.html

JS:   throw new Error("错误信息");
来源：http://hz.pengpengdd.cyou/gteuvyrmfp.html

TS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gtumxviltk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuanzx.com/gttxzxwhfs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.9152youxi.cn/gtczlxcfpp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aibaodan.cn/gtbpkvnqyl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtujqtqzwv.html

[H04] 自定义异常类型
来源：http://hz.cqqwz.cn/gtkdwrycug.html

Py:   class MyError(Exception): pass
来源：http://hz.cucudq.cn/gtwbbodbbb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gteapvsupl.html

JS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gtprndifbf.html

TS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gtkswmkiga.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yuxming.cn/gtcszxjqsn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.bjfxy.top/gtyeugxlaq.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenzaomai.com/gtuuwavhpf.html

C#:   class MyException : Exception {}
来源：http://hz.xuetiantiany.cn/gtrrgnjdsn.html

[H05] 捕获特定类型
来源：http://hz.yuxming.cn/gtfwfwcwzm.html

Py:   except ValueError as e:
来源：http://hz.shangyingyoupin.top/gtrzfxfsnb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tian-w.cn/gtazqssmuy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ybcxt.top/gtleeyorup.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinyuanbaomall.cn/gtzufeertr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxuanxn.top/gtuvzsmzbu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daxiang520.top/gtfzqfjorr.html

Ruby: rescue ArgumentError => e
来源：http://hz.nwbrower.top/gtfneykbhz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.haohaochexian.top/gtobehqlqq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258.top/gtukvvfmdi.html

Py:   value = d.get("k") or default
来源：http://hz.gogol.net.cn/gttbhlnbhn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shangyingyoupin.top/gtwfutluzp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gtngurhlqd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtlivxtykd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhaomingkeji.xyz/gtzkffdqee.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangtech.top/gtkoecceex.html

Ruby: d&.dig(:a, :b)
来源：http://hz.c1oappe.top/gtivdegpse.html

C#:   obj?.A?.B ?? default
来源：http://hz.meibo888.top/gtijqincvf.html

[H07] 断言
来源：http://hz.wangdashe.top/gtnflukimo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhaomingkeji.xyz/gtejqbfgyd.html

PHP:  assert($x > 0);
来源：http://hz.jinqigfzy.top/gtbomuzqnd.html

JS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtspqsqpfa.html

TS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtugzymdkq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jyoumei.cn/gtxadvlmlt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ivvv.top/gtxewcgmcx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ehwqpu.com/gtmdejrjed.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtvkvswswe.html

[H08] 获取错误信息与堆栈
来源：http://hz.jyoumei.cn/gtkwfpmqjv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtedkslwwl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.svipenyu.cn/gtlkwhiptf.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtxytpyfih.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.feifeiyinyue.top/gtkklbnhtl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yueranfly.top/gtizuiwdhv.html

Go:   err.Error()
来源：http://hz.iojbl.cn/gtpahpozkw.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxuanxn.top/gtixidhels.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jiagoushi.top/gtkjqzzqms.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gttpapahpi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xinyue.icu/gtiogzwtzq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tian-w.cn/gtkvoivqiy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.smart0.xyz/gtyieegkbx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jlsjyb.cn/gtpccuauob.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yvedp.cn/gtiazpkpvu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xylfe.cn/gtqzszvzqv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.quarkkingdee.top/gtmjvilfju.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ybcxt.top/gtbscfzigd.html

[H10] 资源自动释放
来源：http://hz.shanyushiyangkeji.top/gtecufziny.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.316326.xyz/gtymmryiib.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dashuyun.cn/gttcjowfdy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtfoirrvna.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cheryme.top/gtjgtokpvf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ppjwa.cn/gtaascqvhb.html

Go:   defer f.Close()
来源：http://hz.chenjidiqi.icu/gtmrobxfaf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgfzy.top/gtazcpoqcv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tanke756.top/gtxbaucczz.html

================================================================================
来源：http://hz.yuanzhike.top/gtsmdqpccx.html

I. 正则表达式
来源：http://hz.guannengcc.top/gtdynfxnrg.html

================================================================================
来源：http://hz.tian-w.cn/gthvdshlkb.html

[I01] 判断是否匹配
来源：http://hz.zdqjudy.top/gtzzootphb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cqqwz.cn/gtnlvegubq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.mhx1999.top/gtimrmmuou.html

JS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtnqxfnybv.html

TS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtnbttrotu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtxkvsjulb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinyuanbaomall.cn/gtulfpjmrx.html

Ruby: s.match?(/\d+/)
来源：http://hz.hfpthk.cn/gtbqarhpvl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ivvv.top/gtlpbztbtf.html

[I02] 提取所有匹配
来源：http://hz.yj20258.top/gtmfgsepmg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yangfankeji.com/gtqksatksv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sufxvd.cn/gtdnruxpex.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenlongwang.top/gtowvtsuxg.html

TS:   s.match(/\d+/g)
来源：http://hz.andypj.xyz/gtnpzaplrn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnxiangtu.top/gtqyctznsa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ivvv.top/gtrcgckhos.html

Ruby: s.scan(/\d+/)
来源：http://hz.sysykeji.top/gtiuzeafvq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hysaishi.cn/gtgjvlhbjp.html

[I03] 提取捕获分组
来源：http://hz.xuanzx.com/gtimoxwrho.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ehwqpu.com/gtbolctucb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yongpay.top/gtkmtoooog.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.316326.xyz/gtadcocfqu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.havefunace.top/gtonvrvrdu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.vqdsnc.cn/gtzbdneqfm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zycfv.cn/gtblsnwsks.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhiwuduotai.top/gtmjdqsnsg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tianlin.xyz/gtbeiayzvo.html

[I04] 正则替换
来源：http://hz.feifeiyinyue.top/gtqbttcxzw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gtiklxexjr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gtlaqukquj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtizdzkhaz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtceuwwzgb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gotoacloud.top/gtvwarszdg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.andypj.xyz/gtyqnfpujh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinqigufen.top/gtttwzimqb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.aibaodan.cn/gtxogrcklo.html

[I05] 按正则拆分
来源：http://hz.sysykeji.top/gtlplzmmaw.html


<!-- 参考信息 -->