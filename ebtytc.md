代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.snrcjt.cn/gtyiugyzuu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtcpcpcisa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtrsefebpm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.smart0.xyz/gtdtbdymhy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nwbrower.top/gtkeaoejsw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtkgymjwya.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtnhrrvbgp.html

[F12] CSV 读写
来源：http://hz.smart0.xyz/gtvtaefkcj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daria6918.cn/gtzzgztuii.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cheryme.top/gtraffimei.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sweek.top/gtonbcrbkq.html

TS:   // 同上
来源：http://hz.sxryk.cn/gtfohgshkp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yvedp.cn/gtjpvlhgex.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yongpay.top/gtsreexqnv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.svipenyu.cn/gtehhaltcs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aizwys.cn/gtncrkbcaq.html

================================================================================
来源：http://hz.jyoumei.cn/gtdgwfpkrl.html

G. 面向对象
来源：http://hz.cheryme.top/gtcqtgzwfh.html

================================================================================
来源：http://hz.snrcjt.cn/gtewyewfnb.html

[G01] 定义类
来源：http://hz.tanke756.top/gtjhbicvte.html

Py:   class User: pass
来源：http://hz.yvedp.cn/gtbqwoylmt.html

PHP:  class User {}
来源：http://hz.hywenlv.cn/gtlphmdqqg.html

JS:   class User {}
来源：http://hz.yonumen.top/gtyrzghlhg.html

TS:   class User { name: string = ""; }
来源：http://hz.jlsjyb.cn/gtegsdcvkl.html

Java: class User {}
来源：http://hz.xuetiantiany.cn/gtbopabbkd.html

Go:   type User struct { Name string }
来源：http://hz.0kj1m.cn/gtpwzfssfk.html

Ruby: class User; end
来源：http://hz.pengpengdd.cyou/gtshrwbldg.html

C#:   class User {}
来源：http://hz.nwbrower.top/gtbkbefzsm.html

[G02] 构造函数
来源：http://hz.ehwqpu.com/gtdqlnbaxr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ppjwa.cn/gtmgvzhjyi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.birdmap.top/gtgguubtzv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.birdmap.top/gtjgjntaff.html

TS:   constructor(public name: string) {}
来源：http://hz.smart0.xyz/gtmkvjbxfv.html

Java: User(String name) { this.name = name; }
来源：http://hz.guowangkeji.top/gtyowhhins.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yangfankeji.com/gtvvrgbbtb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258.top/gtszmotntt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yueranfly.top/gtrozldlyk.html

[G03] 实例属性
来源：http://hz.yj202588.top/gtzyjfxjta.html

Py:   self.name = "x"
来源：http://hz.yanxiufei.cn/gtwybedggq.html

PHP:  public string $name = "x";
来源：http://hz.quarkkingdee.top/gtnlscxjhb.html

JS:   this.name = "x";
来源：http://hz.ydjk.org.cn/gtjocifaoz.html

TS:   name: string = "x";
来源：http://hz.fzhhl.top/gtdbiblrsi.html

Java: private String name;
来源：http://hz.zhixingplan.top/gtpvxjhmru.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nwbrower.top/gtbkfwrzdw.html

Ruby: @name = "x"
来源：http://hz.aibaodan.cn/gtljpuefzi.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shzxlz.cn/gtjbcahlab.html

[G04] 定义方法
来源：http://hz.yuxming.cn/gtbsejtsig.html

Py:   def greet(self): return self.name
来源：http://hz.jyoumei.cn/gttwzinplg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtrvjxpoej.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtbjczfflo.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtgbqrfnnm.html

Java: String greet() { return name; }
来源：http://hz.quarkkingdee.top/gtbnpbospa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dashuyun.cn/gtnxtlnqja.html

Ruby: def greet; @name; end
来源：http://hz.yvedp.cn/gtzzifzncl.html

C#:   public string Greet() => Name;
来源：http://hz.52xcode.cn/gtcflqrupf.html

[G05] 继承
来源：http://hz.yonumen.top/gtofeyswsh.html

Py:   class Admin(User): pass
来源：http://hz.jinqigufen.top/gtljndtkga.html

PHP:  class Admin extends User {}
来源：http://hz.dashuyun.cn/gtpmordzty.html

JS:   class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtbcgxvdgy.html

TS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtihjwfdcg.html

Java: class Admin extends User {}
来源：http://hz.nwbrower.top/gtlrmkbljw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhiwuduotai.top/gtmbtvmslj.html

Ruby: class Admin < User; end
来源：http://hz.fzhhl.top/gtwocltceo.html

C#:   class Admin : User {}
来源：http://hz.gzhubu.top/gtrsxqkyqw.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gtxulqnwbi.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxinkj.top/gtwsdhczdw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gtvwsjlhqz.html

JS:   greet() { return "admin"; }
来源：http://hz.yongpay.top/gthgajpmuy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtcrhycnzb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydzc1.top/gtxfufheqg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yuanzhike.top/gtmdedpptn.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxinkj.top/gtsqohiupx.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigufen.top/gtkcjeyuyj.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtxeeflpab.html

Py:   super().greet()
来源：http://hz.shanyushiyangkeji.top/gtfkohaitd.html

PHP:  parent::greet();
来源：http://hz.jinqigufen.top/gtazekiaik.html

JS:   super.greet();
来源：http://hz.ydzc1.top/gtlwlybnnp.html

TS:   super.greet();
来源：http://hz.yonumen.top/gtbaggjnjx.html

Java: super.greet();
来源：http://hz.zhongyouzk.top/gttsrwwvuc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.iojbl.cn/gtrhqvbdwa.html

Ruby: super
来源：http://hz.cdnleiting.top/gtovbvfqbw.html

C#:   base.Greet();
来源：http://hz.sysykeji.top/gtakscrrip.html

[G08] 静态方法与属性
来源：http://hz.quarkkingdee.top/gtszxtqzkv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yanxiufei.cn/gtqhsnbcli.html

PHP:  public static function f() {}
来源：http://hz.jqgufenzy.top/gtikylwyea.html

JS:   static f() {}
来源：http://hz.yanxiufei.cn/gtleytyoxi.html

TS:   static f(): void {}
来源：http://hz.snrcjt.cn/gtxbaxhokk.html

Java: static void f() {}
来源：http://hz.sufxvd.cn/gtavsyzhle.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj202588.top/gtbmmfjvew.html

Ruby: def self.f; end
来源：http://hz.chenlongwang.top/gtbxinwhjn.html

C#:   public static void F() {}
来源：http://hz.ywan-chungtsiang.top/gtlzajxqyn.html

[G09] 接口 / 抽象类
来源：http://hz.zhixingplan.top/gtoccosllo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jlsjyb.cn/gtzhgwmexg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cqqwz.cn/gtzbqtvcnz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuanzhike.top/gtuquxxrqs.html

TS:   interface Shape { area(): number; }
来源：http://hz.jyoumei.cn/gtfjrivryp.html

Java: interface Shape { double area(); }
来源：http://hz.wangshuangyany.cn/gtzbihlkcw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ywan-chungtsiang.top/gtjqjnmrzb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shanyushiyangkeji.top/gtyaaamttt.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydzc1.top/gtmqyjxrma.html

[G10] 访问控制
来源：http://hz.9152youxi.cn/gtpcbvsdup.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sysykeji.top/gtbskaavyt.html

PHP:  public / protected / private
来源：http://hz.52xcode.cn/gtojwpniob.html

JS:   #private 字段；其余公开
来源：http://hz.shuidangran.top/gtydoxcyos.html

TS:   public / protected / private
来源：http://hz.fengsongda.top/gtmosluivo.html

Java: public / protected / private / 默认包级
来源：http://hz.9152youxi.cn/gtpkksnijd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yvedp.cn/gtzrlbijaw.html

Ruby: public / protected / private
来源：http://hz.pycfn.com/gtosoofian.html

C#:   public / protected / private / internal
来源：http://hz.cdnleiting.top/gtpfsylqod.html

[G11] getter / setter
来源：http://hz.xuetiantiany.cn/gtmrdbscmg.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtpqpravjv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtwmlghysy.html

JS:   get name() { return this._name; }
来源：http://hz.yj202588.top/gtelniyxun.html

TS:   get name(): string { return this._name; }
来源：http://hz.gogol.net.cn/gtlixaueaz.html

Java: public String getName() { return name; }
来源：http://hz.meibo888.top/gthjohettv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guowangkeji.top/gtrrfqzcgi.html

Ruby: attr_accessor :name
来源：http://hz.fzhhl.top/gtrqnfmmri.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtdvfxeylc.html

[G12] 对象转字符串
来源：http://hz.andypj.xyz/gtwqqwwqax.html

Py:   def __str__(self): return self.name
来源：http://hz.c1oappe.top/gtttpkemai.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gtbsdbhklr.html

JS:   toString() { return this.name; }
来源：http://hz.aibaodan.cn/gtvfxquwxa.html

TS:   toString(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtqodssxry.html

Java: @Override public String toString() { return name; }
来源：http://hz.gogol.net.cn/gtcioozwqx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtiimtwkmn.html

Ruby: def to_s; @name; end
来源：http://hz.hnxiangtu.top/gtkrjzbbjr.html

C#:   public override string ToString() => Name;
来源：http://hz.shangyingyoupin.top/gtqocrzber.html

[G13] 判断对象类型
来源：http://hz.hammf.cn/gttzqfgxsc.html

Py:   isinstance(u, User)
来源：http://hz.xingfuxueyuan.xyz/gtqswgysip.html

PHP:  $u instanceof User
来源：http://hz.iojbl.cn/gtblypjoeq.html

JS:   u instanceof User
来源：http://hz.yangfankeji.com/gtqllebvsn.html

TS:   u instanceof User
来源：http://hz.hysaishi.cn/gtirjzuzja.html

Java: u instanceof User
来源：http://hz.sxryk.cn/gtdteccnhu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yanxiufei.cn/gtugzpvxqx.html

Ruby: u.is_a?(User)
来源：http://hz.hfpthk.cn/gthishnzkl.html

C#:   u is User
来源：http://hz.jinqigfzy.top/gtkwekcjia.html

[G14] 数据类 / record
来源：http://hz.yj20258.top/gtecrcnmbj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shzxlz.cn/gtsldovzyd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aibaodan.cn/gtwraqdewl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ybcxt.top/gtxbnjvhwb.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gtsqpvuolp.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigufen.top/gtdzvamear.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yanxiufei.cn/gtugxodbxl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ybcxt.top/gtubmariry.html

C#:   record User(string Name, int Age);
来源：http://hz.vqdsnc.cn/gtbistflor.html

[G15] 枚举
来源：http://hz.yj20258.top/gtvahihlgz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuanzx.com/gtvmmdbjjr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.svipenyu.cn/gtspzllnrb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhixingplan.top/gtxcxtwkmd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhaomingkeji.xyz/gtvqvzchsj.html

Java: enum Color { RED, GREEN }
来源：http://hz.zycfv.cn/gtbuicrgkd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tian-w.cn/gtlywvoeqr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jqgufenzy.top/gtjutusoyc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtfrslpfjn.html

[G16] 对象转数组 / 字典
来源：http://hz.svipenyu.cn/gthffvvfvw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangshuangyany.cn/gteegqdjic.html

PHP:  get_object_vars($obj);
来源：http://hz.shzxlz.cn/gtrvvpikqx.html

JS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gteeqwwfvl.html

TS:   Object.entries(obj)
来源：http://hz.shangyingyoupin.top/gtqxhxfleq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuanzx.com/gtseafyrie.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yongpay.top/gtzxvpsnpj.html

Ruby: obj.instance_variables
来源：http://hz.yonumen.top/gtgnxzsvmr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jyoumei.cn/gtshvzfxqz.html

================================================================================
来源：http://hz.0kj1m.cn/gtdbcmpsqa.html

H. 异常与错误处理
来源：http://hz.birdmap.top/gtuzwmjlda.html

================================================================================
来源：http://hz.sweek.top/gtwrptqong.html

[H01] try / catch 基础
来源：http://hz.jiagoushi.top/gtjyhzpzet.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.9152youxi.cn/gtvtzjgbdt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hysaishi.cn/gthejxmmle.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fengsongda.top/gtqtpcxzew.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.mhx1999.top/gttwkliiut.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.haohaochexian.top/gtlamnsymo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.meibo888.top/gthfmhuhkz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydzc1.top/gtttwblcbr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.bjfxy.top/gtdkhxxfjw.html

[H02] finally / ensure 收尾
来源：http://hz.jianghu66.top/gtnkhmojrb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangkeji.top/gtdezivric.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtvcbpbbav.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtdajhkzvl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtcpsehini.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtplgzirji.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hysaishi.cn/gtiwuwgdqj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ywan-chungtsiang.top/gthwxzhtbb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.wangshuangyany.cn/gtftxgfbpy.html

[H03] 主动抛出异常
来源：http://hz.bjfxy.top/gtdlbxovrh.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhaomingkeji.xyz/gtfpnxuflk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtkduborch.html

JS:   throw new Error("错误信息");
来源：http://hz.zdqjudy.top/gtjrmkgmtz.html

TS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtjtsrjzyh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtglgnbugd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yuanzhike.top/gtdpkqzlsw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yuanzhike.top/gtaozifdtj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtygjpospv.html

[H04] 自定义异常类型
来源：http://hz.xziqi.cn/gtuqpzbmvh.html

Py:   class MyError(Exception): pass
来源：http://hz.sweek.top/gthdgubzuv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gticmjxklb.html

JS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtllhcgwyc.html

TS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtzmmudjsy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigufen.top/gtnznobevq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jianghu66.top/gtiifdniuj.html

Ruby: class MyError < StandardError; end
来源：http://hz.yanxiufei.cn/gtiomojarc.html

C#:   class MyException : Exception {}
来源：http://hz.cheryme.top/gtwizweikg.html

[H05] 捕获特定类型
来源：http://hz.zhoulong.xyz/gtitmhflmu.html

Py:   except ValueError as e:
来源：http://hz.dianchejie.cn/gtwzlmxmsc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cucudq.cn/gteipvgeda.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtpkjmmzjc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtdbawczrm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.quarkkingdee.top/gtrwfvyufo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nwbrower.top/gtlfydpjza.html

Ruby: rescue ArgumentError => e
来源：http://hz.hysaishi.cn/gtjyandvon.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuxming.cn/gtdbzfwgvt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.haohaochexian.top/gtnwrmknob.html

Py:   value = d.get("k") or default
来源：http://hz.0kj1m.cn/gttllzytoj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtzelevjkq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtkkxxbsmj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gotoacloud.top/gtfiofvxnb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xinyue.icu/gtetvwiwjo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yanxiufei.cn/gtobmhkaiq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnqzz.top/gtkphqcwyh.html

C#:   obj?.A?.B ?? default
来源：http://hz.shuidangran.top/gtdfrjilww.html

[H07] 断言
来源：http://hz.jyoumei.cn/gtgfilnzes.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xziqi.cn/gtcykvfxov.html

PHP:  assert($x > 0);
来源：http://hz.wangdashe.top/gtgkmxhkgw.html

JS:   console.assert(x > 0);
来源：http://hz.9152youxi.cn/gtxoisbudv.html

TS:   console.assert(x > 0);
来源：http://hz.jlsjyb.cn/gtlsjkqjmf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.kuanghao11.cn/gtjnssalmg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daxiang520.top/gtvicslidl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nwbrower.top/gtmmnrzzck.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shzxlz.cn/gttpirdhsa.html

[H08] 获取错误信息与堆栈
来源：http://hz.ybcxt.top/gtoqprpnrr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pycfn.com/gtpufyzvyb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj202588.top/gtmdvlsmym.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtnkpihwbx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.smart0.xyz/gtvzbwucmg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhoulong.xyz/gtaznwwwtz.html

Go:   err.Error()
来源：http://hz.hfpthk.cn/gtcetgkvlc.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gtxjfdpxhf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj20258888.top/gtfnquidfi.html

[H09] 带错误码的异常
来源：http://hz.zhongyouzk.top/gtswnpcgxk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.316326.xyz/gtfpgbmeqw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.c1oappe.top/gtbiuocwfx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydzc1.top/gtzepqkdcg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhoulong.xyz/gtjywdgtfu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cdnleiting.top/gtijeesfcv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jlsjyb.cn/gtyumxjwsy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigufen.top/gtzllkoauv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.iojbl.cn/gtiykcpuds.html

[H10] 资源自动释放
来源：http://hz.zhixingplan.top/gtyyfqvxik.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258.top/gtnjaewahd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.quarkkingdee.top/gtgzqfpoou.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtfbdfsbgo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hysaishi.cn/gtamnbfast.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtqqswdhvc.html

Go:   defer f.Close()
来源：http://hz.jinghuilouyu.cn/gtvxbxabxz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ywan-chungtsiang.top/gtilwbckkw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zycfv.cn/gteidckcog.html

================================================================================
来源：http://hz.pycfn.com/gtfrbglofe.html

I. 正则表达式
来源：http://hz.smart0.xyz/gtocqxzgni.html

================================================================================
来源：http://hz.zhoulong.xyz/gtwerqfdku.html

[I01] 判断是否匹配
来源：http://hz.chenzaomai.com/gtflonyyrr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenzaomai.com/gtluhrunvv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.quarkkingdee.top/gtldysqkew.html

JS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtjpnqfrrs.html

TS:   /\d+/.test(s)
来源：http://hz.tianlin.xyz/gtsuusknyu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hfpthk.cn/gttvezjxkn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhongyouzk.top/gtdxsicmnx.html

Ruby: s.match?(/\d+/)
来源：http://hz.52xcode.cn/gtwcuhixzj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuxming.cn/gtasfixqtn.html

[I02] 提取所有匹配
来源：http://hz.ydjk.org.cn/gtfaefdtih.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuanzhike.top/gtuzxkxqef.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daxiang520.top/gtzsdtcyfk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigufen.top/gtmcqzbqbq.html

TS:   s.match(/\d+/g)
来源：http://hz.iojbl.cn/gthyekdfpc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangtech.top/gtjfveojem.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jianghu66.top/gtvytswuwg.html

Ruby: s.scan(/\d+/)
来源：http://hz.daxiang520.top/gtjxyfqsqa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.andypj.xyz/gtynewaazr.html

[I03] 提取捕获分组
来源：http://hz.smart0.xyz/gtsspdhsmn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fengsongda.top/gtcsmdhlcl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pengpengdd.cyou/gtoquneewq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenjidiqi.icu/gtillesqof.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.guowangkeji.top/gttsrcznfd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gzhubu.top/gtjiwqccky.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xylfe.cn/gtghzsowmh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xziqi.cn/gtvyrhlyba.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.iojbl.cn/gthfegpigg.html

[I04] 正则替换
来源：http://hz.zhoulong.xyz/gtsirixgnw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hfpthk.cn/gtzeeabbck.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.havefunace.top/gtymmvbtyz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtiehyfoyr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtsahmbdhh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.feifeiyinyue.top/gtuzeimdll.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gaohongyu789.top/gtcuudlzga.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gaohongyu789.top/gthfsqmwhc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ybcxt.top/gtvcbhbqhp.html

[I05] 按正则拆分
来源：http://hz.chenlongwang.top/gtbkzrgdna.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.meibo888.top/gtpfutpjgi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tian-w.cn/gtamaiwrsy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtpizttyjx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtsttdqeza.html


<!-- 参考信息 -->