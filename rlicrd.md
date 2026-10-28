代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtlpmcyowh.html

TS:   path.extname("a.txt")
来源：http://hz.jyoumei.cn/gtqchjrwhy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.quarkkingdee.top/gtdfzkehin.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtspuxhrcm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtcdrtilqu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhongyouzk.top/gthqgvbqsg.html

[F11] 复制与移动文件
来源：http://hz.ybcxt.top/gtbyxmrejk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtwprasskq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.feifeiyinyue.top/gttfxckapa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtevhlopyu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtotvxxruj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yvedp.cn/gtwypyefmu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnxiangtu.top/gtarkywgxh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtnpcobiya.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pycfn.com/gtsbomnvea.html

[F12] CSV 读写
来源：http://hz.jqgufenzy.top/gthymeicay.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhiwuduotai.top/gtklqhlgek.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gogol.net.cn/gtdvflzqmx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tian-w.cn/gtsfnccihc.html

TS:   // 同上
来源：http://hz.fengsongda.top/gteiagdjor.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hfpthk.cn/gtgbwdkzzt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ehwqpu.com/gtaythzppe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.vqdsnc.cn/gtvkadovsa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xinyue.icu/gtlkmffzjd.html

================================================================================
来源：http://hz.316326.xyz/gtwlkkccee.html

G. 面向对象
来源：http://hz.yj20258.top/gtidomqmop.html

================================================================================
来源：http://hz.gaohongyu789.top/gtyjsrvpik.html

[G01] 定义类
来源：http://hz.cdnleiting.top/gtsuwlrgqn.html

Py:   class User: pass
来源：http://hz.daxiang520.top/gtybbzgkag.html

PHP:  class User {}
来源：http://hz.andypj.xyz/gtybiaklrq.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtupjttcxz.html

TS:   class User { name: string = ""; }
来源：http://hz.aizwys.cn/gtqfubrynu.html

Java: class User {}
来源：http://hz.52xcode.cn/gtspshmejj.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtufanyxgt.html

Ruby: class User; end
来源：http://hz.dashuyun.cn/gtdpwxsyvh.html

C#:   class User {}
来源：http://hz.sufxvd.cn/gtfczbztzw.html

[G02] 构造函数
来源：http://hz.zhaomingkeji.xyz/gtjlbkyydn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangkeji.top/gtfrpgdfpo.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sxryk.cn/gtdnuqdeuu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtiryqccpy.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtrdymuqdd.html

Java: User(String name) { this.name = name; }
来源：http://hz.zycfv.cn/gtnbgyxzyn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yonumen.top/gtewkonvid.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gtihwtrzcf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zycfv.cn/gtgujymlxb.html

[G03] 实例属性
来源：http://hz.vqdsnc.cn/gtvnpkzooo.html

Py:   self.name = "x"
来源：http://hz.shanyushiyangkeji.top/gtlosqfdqg.html

PHP:  public string $name = "x";
来源：http://hz.cdnleiting.top/gtpwcyifsa.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtibupsode.html

TS:   name: string = "x";
来源：http://hz.hongshengwenyu.top/gtfeuwkxba.html

Java: private String name;
来源：http://hz.fengsongda.top/gtcaovtfcd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gotoacloud.top/gtnalmlfci.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtrwiqtmtg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hammf.cn/gthikfbigh.html

[G04] 定义方法
来源：http://hz.zdqjudy.top/gtkrkbipwe.html

Py:   def greet(self): return self.name
来源：http://hz.andypj.xyz/gtzmbzuumr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtcsxswqti.html

JS:   greet() { return this.name; }
来源：http://hz.jlsjyb.cn/gtwvpchakt.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnxiangtu.top/gtklzpklvt.html

Java: String greet() { return name; }
来源：http://hz.jinghuilouyu.cn/gtahwprsxk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yonumen.top/gtuupdwzob.html

Ruby: def greet; @name; end
来源：http://hz.nwbrower.top/gtkqmgpdfn.html

C#:   public string Greet() => Name;
来源：http://hz.tianlin.xyz/gtdmpbvgfv.html

[G05] 继承
来源：http://hz.ybcxt.top/gtpknswjoi.html

Py:   class Admin(User): pass
来源：http://hz.zhijiandao.cn/gtngxorvpi.html

PHP:  class Admin extends User {}
来源：http://hz.aibaodan.cn/gtcqjmzxds.html

JS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtexpfbpqm.html

TS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtvqwktbcm.html

Java: class Admin extends User {}
来源：http://hz.redwolf501.top/gtmrqwxuyd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hysaishi.cn/gtszajiqts.html

Ruby: class Admin < User; end
来源：http://hz.yueranfly.top/gtvzjczgwk.html

C#:   class Admin : User {}
来源：http://hz.gzhubu.top/gtddrfvkvx.html

[G06] 重写方法
来源：http://hz.andypj.xyz/gtzosqyyxo.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigufen.top/gtpvbhbtvi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtaeofhgik.html

JS:   greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtozxhtjvt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtxfejdriv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.iojbl.cn/gttumxbkea.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gogol.net.cn/gttzktjrvw.html

Ruby: def greet; "admin"; end
来源：http://hz.zhaomingkeji.xyz/gtdofwioyl.html

C#:   public override string Greet() => "admin";
来源：http://hz.vqdsnc.cn/gtcduosrza.html

[G07] 调用父类方法
来源：http://hz.daxiang520.top/gtkupqxlga.html

Py:   super().greet()
来源：http://hz.hnxiangtu.top/gtsfjafafw.html

PHP:  parent::greet();
来源：http://hz.xziqi.cn/gtmjjnpuxu.html

JS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtztssjlug.html

TS:   super.greet();
来源：http://hz.redwolf501.top/gtpvupbtau.html

Java: super.greet();
来源：http://hz.sysykeji.top/gtfkkupgra.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cucudq.cn/gtklgnrivm.html

Ruby: super
来源：http://hz.shangyingyoupin.top/gtirwyfdef.html

C#:   base.Greet();
来源：http://hz.yongpay.top/gtwmgtqkyk.html

[G08] 静态方法与属性
来源：http://hz.yongpay.top/gtcmwurjsi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnxiangtu.top/gtkxitxyxv.html

PHP:  public static function f() {}
来源：http://hz.dashuyun.cn/gtbwkmffji.html

JS:   static f() {}
来源：http://hz.zhaomingkeji.xyz/gtzgtfbjsw.html

TS:   static f(): void {}
来源：http://hz.cashguo.top/gtavpvlpkf.html

Java: static void f() {}
来源：http://hz.hysaishi.cn/gtrquqdyrd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.wangdashe.top/gthkpvstjb.html

Ruby: def self.f; end
来源：http://hz.zhaomingkeji.xyz/gtcalucwtw.html

C#:   public static void F() {}
来源：http://hz.guannengcc.top/gtzxvbefwm.html

[G09] 接口 / 抽象类
来源：http://hz.zhixingplan.top/gtgivxdojs.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sweek.top/gtsrdqubht.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zdqjudy.top/gtynteiybc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinyuanbaomall.cn/gtegfsejql.html

TS:   interface Shape { area(): number; }
来源：http://hz.xingfuxueyuan.xyz/gtoictkvfu.html

Java: interface Shape { double area(); }
来源：http://hz.gotoacloud.top/gtcmidhccs.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ehwqpu.com/gtpmavqazq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jqgfzy.top/gtkddgebse.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinqigfzy.top/gtafzodygz.html

[G10] 访问控制
来源：http://hz.jiagoushi.top/gtetpdqdmb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenjidiqi.icu/gtqukqzqkr.html

PHP:  public / protected / private
来源：http://hz.sysykeji.top/gteandceap.html

JS:   #private 字段；其余公开
来源：http://hz.zhixingplan.top/gtwttuuagb.html

TS:   public / protected / private
来源：http://hz.chenzaomai.com/gtigcovwut.html

Java: public / protected / private / 默认包级
来源：http://hz.jiagoushi.top/gtkqifekuc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fzhhl.top/gtywqkbvps.html

Ruby: public / protected / private
来源：http://hz.nanxuanxn.top/gtxhrwfonr.html

C#:   public / protected / private / internal
来源：http://hz.feifeiyinyue.top/gttbqfdjqz.html

[G11] getter / setter
来源：http://hz.tian-w.cn/gtranmlcyx.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangtech.top/gtubbmntlf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtfkpcoubt.html

JS:   get name() { return this._name; }
来源：http://hz.zhijiandao.cn/gtslamylqz.html

TS:   get name(): string { return this._name; }
来源：http://hz.9152youxi.cn/gtqobqfufq.html

Java: public String getName() { return name; }
来源：http://hz.birdmap.top/gtfygoqdyi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxinkj.top/gtoxwjzcvj.html

Ruby: attr_accessor :name
来源：http://hz.aizwys.cn/gtfcqbrjew.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gtldlxzqiu.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtslkablen.html

Py:   def __str__(self): return self.name
来源：http://hz.andypj.xyz/gthiaxumfq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtkvyisabs.html

JS:   toString() { return this.name; }
来源：http://hz.316326.xyz/gtdebdfwgd.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gtbshuniku.html

Java: @Override public String toString() { return name; }
来源：http://hz.jyoumei.cn/gtauzxguju.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shuidangran.top/gtacreyvmr.html

Ruby: def to_s; @name; end
来源：http://hz.iojbl.cn/gtohjfixfh.html

C#:   public override string ToString() => Name;
来源：http://hz.shzxlz.cn/gtxaokeips.html

[G13] 判断对象类型
来源：http://hz.nanxuanxn.top/gtfafbloio.html

Py:   isinstance(u, User)
来源：http://hz.yj20258888.top/gtynefnsox.html

PHP:  $u instanceof User
来源：http://hz.guowangkeji.top/gtuscjtmpu.html

JS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtzuropblp.html

TS:   u instanceof User
来源：http://hz.xylfe.cn/gtcxpjbhep.html

Java: u instanceof User
来源：http://hz.hfpthk.cn/gtvahonnkf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinghuilouyu.cn/gtwtgbahdb.html

Ruby: u.is_a?(User)
来源：http://hz.yvedp.cn/gtwcchugyf.html

C#:   u is User
来源：http://hz.ppjwa.cn/gtauvmvmpu.html

[G14] 数据类 / record
来源：http://hz.nanxinkj.top/gtsfkgkjtc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ywan-chungtsiang.top/gtggxkvkks.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nwbrower.top/gttdtsltxk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuxming.cn/gtsxypbird.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuanzhike.top/gtixepkxzb.html

Java: record User(String name, int age) {}
来源：http://hz.shangyingyoupin.top/gtbwzzlkko.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuxming.cn/gtudnskevs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gogol.net.cn/gtcyzgselt.html

C#:   record User(string Name, int Age);
来源：http://hz.zhiwuduotai.top/gtbgwxxzdc.html

[G15] 枚举
来源：http://hz.quarkkingdee.top/gtmvlqtvoe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ybcxt.top/gtgaqqtnxw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hammf.cn/gtzhhmjwvx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangkeji.top/gtsgkssush.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtngvcgcaa.html

Java: enum Color { RED, GREEN }
来源：http://hz.c1oappe.top/gtxiburhdi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yueranfly.top/gtesdcatbh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tanke756.top/gtrtkqekrq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.bjfxy.top/gtrbjpmblk.html

[G16] 对象转数组 / 字典
来源：http://hz.316326.xyz/gtmsnuporb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenzaomai.com/gtbtkqhbfg.html

PHP:  get_object_vars($obj);
来源：http://hz.fzhhl.top/gtdsyuloep.html

JS:   Object.entries(obj)
来源：http://hz.vqdsnc.cn/gtoifsukkx.html

TS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gttlymqtdo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtlpzmsoeu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aibaodan.cn/gtsmhxikrt.html

Ruby: obj.instance_variables
来源：http://hz.shzxlz.cn/gtssngnaew.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ehwqpu.com/gtxbucwqlg.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtkmdvkrdt.html

H. 异常与错误处理
来源：http://hz.hammf.cn/gtxxvbjvsd.html

================================================================================
来源：http://hz.dashuyun.cn/gtednwwock.html

[H01] try / catch 基础
来源：http://hz.yj20258888.top/gtdrwyykal.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gzhubu.top/gtsjsbuhhc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yongpay.top/gtiocfuuzr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtxqzpyjhn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dianchejie.cn/gtsrnctjgn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zycfv.cn/gtosczjvbt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ivvv.top/gtoqegeyih.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ehwqpu.com/gtsojappik.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yvedp.cn/gtnszajxhi.html

[H02] finally / ensure 收尾
来源：http://hz.hywenlv.cn/gtgaoqlcbt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xingfuxueyuan.xyz/gttattgxpn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtzlacxyke.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtttudevbk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtadiyonij.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtinknnqoa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.iojbl.cn/gtalkitbec.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yonumen.top/gtrsxrtklu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gotoacloud.top/gteathwjrm.html

[H03] 主动抛出异常
来源：http://hz.yuanzhike.top/gtfpiwvdpn.html

Py:   raise ValueError("错误信息")
来源：http://hz.tianlin.xyz/gtkqsqikkn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtblwfbqky.html

JS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtpsigmssi.html

TS:   throw new Error("错误信息");
来源：http://hz.hfpthk.cn/gtyqsmoppy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtpoebloyg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jqgufenzy.top/gtdyfdjyqu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hnqzz.top/gtsxxmlptj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtrmadjowl.html

[H04] 自定义异常类型
来源：http://hz.cashguo.top/gtycsbmtdw.html

Py:   class MyError(Exception): pass
来源：http://hz.cheryme.top/gtilitwhzv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yueranfly.top/gtstmlptwv.html

JS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtgfzgtrkn.html

TS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gtpqvypire.html

Java: class MyException extends RuntimeException {}
来源：http://hz.mhx1999.top/gtdrkkmjss.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.0kj1m.cn/gtwuqywudx.html

Ruby: class MyError < StandardError; end
来源：http://hz.0kj1m.cn/gtvdcvobap.html

C#:   class MyException : Exception {}
来源：http://hz.wangdashe.top/gtgqeixfft.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gtaaatjqcp.html

Py:   except ValueError as e:
来源：http://hz.316326.xyz/gtqemxytyp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tanke756.top/gtnutvnmwd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtocfckfhi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtblujjpma.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.redwolf501.top/gtxahtjunl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.52xcode.cn/gtratqtnqf.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuanzhike.top/gtdvkbiyqb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cashguo.top/gtkdsmhiaa.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhiwuduotai.top/gtudnbwjfm.html

Py:   value = d.get("k") or default
来源：http://hz.bjfxy.top/gtqinnnwca.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cucudq.cn/gtsjdihkmh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gtxuwvpogp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zycfv.cn/gtlpucsnpm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhijiandao.cn/gtktfgkiav.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhiwuduotai.top/gtnkqrvoop.html

Ruby: d&.dig(:a, :b)
来源：http://hz.birdmap.top/gtpgtlhlfu.html

C#:   obj?.A?.B ?? default
来源：http://hz.gotoacloud.top/gtkjabucrq.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gtqksctvpw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgufenzy.top/gtwrnlgjre.html

PHP:  assert($x > 0);
来源：http://hz.hammf.cn/gtgktxmjwc.html

JS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gtxtdoxmex.html

TS:   console.assert(x > 0);
来源：http://hz.yonumen.top/gtnevmeyod.html

Java: assert x > 0 : "必须为正";
来源：http://hz.52xcode.cn/gtiuwfrjzn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zdqjudy.top/gtzavaqdiu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenlongwang.top/gtrlghtuif.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yueranfly.top/gtnkplxogo.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangshuangyany.cn/gtykrfyznt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gttzqjyryh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nwbrower.top/gtjidbdxkn.html

JS:   e.message;  e.stack
来源：http://hz.birdmap.top/gtjmuphpme.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xingfuxueyuan.xyz/gtrdwugnez.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aibaodan.cn/gtizszwyqi.html

Go:   err.Error()
来源：http://hz.cqqwz.cn/gtlfdbfjdp.html

Ruby: e.message;  e.backtrace
来源：http://hz.cashguo.top/gtxdpfqpna.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj20258.top/gtlwsgsvha.html

[H09] 带错误码的异常
来源：http://hz.cheryme.top/gtatgamujp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xingfuxueyuan.xyz/gtiyrpqvdo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ywan-chungtsiang.top/gtasawawyd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.snrcjt.cn/gtoyazdkcp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sxryk.cn/gtcdgxgrzx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hammf.cn/gtwbqlnqdp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guannengcc.top/gtacgbumgv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shanyushiyangtech.top/gtqwydqbjr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cdnleiting.top/gtjiahmolq.html

[H10] 资源自动释放
来源：http://hz.c1oappe.top/gtfdibrguc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxinkj.top/gtgsyxvmio.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sweek.top/gtaxccbazu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtxkssxszj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtmurvpppp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xylfe.cn/gtsumgcgjz.html

Go:   defer f.Close()
来源：http://hz.xuetiantiany.cn/gthkznjrvn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yuanzhike.top/gtilziable.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xylfe.cn/gtyrtmcgto.html

================================================================================
来源：http://hz.snrcjt.cn/gtlugqfnat.html

I. 正则表达式
来源：http://hz.gaohongyu789.top/gtjobthpgm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtcekfofgo.html

[I01] 判断是否匹配
来源：http://hz.yuxming.cn/gtbiqmbmnt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.guowangkeji.top/gtxfrwxrbe.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuanzhike.top/gtwqkxzozf.html

JS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtfxncwvsa.html

TS:   /\d+/.test(s)
来源：http://hz.gotoacloud.top/gtnbsradku.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jqgfzy.top/gttzbjiajm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gotoacloud.top/gtdgpostmq.html

Ruby: s.match?(/\d+/)
来源：http://hz.hongshengwenyu.top/gtshiktqgb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnqzz.top/gtgfjpqbsv.html

[I02] 提取所有匹配
来源：http://hz.zycfv.cn/gtjhgmcxqc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtdtskvvnf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.havefunace.top/gttvxdthci.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tian-w.cn/gtfrdhjfzo.html

TS:   s.match(/\d+/g)
来源：http://hz.dianchejie.cn/gttfyovmpd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258888.top/gtftqlgepi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cdnleiting.top/gtaspoodlc.html

Ruby: s.scan(/\d+/)
来源：http://hz.tianlin.xyz/gtmlekkbyh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuanzhike.top/gtriufkcob.html

[I03] 提取捕获分组
来源：http://hz.yj20258.top/gtaxpvvoot.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ywan-chungtsiang.top/gtjwgoxfdd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tianlin.xyz/gthtqfgosf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigfzy.top/gtnnyhrgfj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxuanxn.top/gtxlaiciuu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cashguo.top/gthuiughla.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hywenlv.cn/gtkcnvword.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yueranfly.top/gtimmgitle.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ybcxt.top/gtpqpdjtnt.html

[I04] 正则替换
来源：http://hz.yanxiufei.cn/gtclsmouzm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cdnleiting.top/gtatbzneii.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.iojbl.cn/gtlnbbkmxc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtclhseqhd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.mhx1999.top/gtierxocow.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigufen.top/gtlztscecj.html


<!-- 参考信息 -->