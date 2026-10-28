代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xuanzx.com/gtoguvgpyw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtdwofqdqg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydzc1.top/gtexhjcxhw.html

[F12] CSV 读写
来源：http://hz.birdmap.top/gtwyvzbnxl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sysykeji.top/gtyjmauvoe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnxiangtu.top/gtbnrkjrnw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.meibo888.top/gtrlpmftlz.html

TS:   // 同上
来源：http://hz.daxiang520.top/gthupirksy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.kuanghao11.cn/gtmeenoivo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.bjfxy.top/gtbwydaboo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jyoumei.cn/gtziqqlkgk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tianlin.xyz/gtjjaokqhh.html

================================================================================
来源：http://hz.sufxvd.cn/gtsknvgwaw.html

G. 面向对象
来源：http://hz.ppjwa.cn/gtqbklvasc.html

================================================================================
来源：http://hz.yuxming.cn/gtbbwsywfw.html

[G01] 定义类
来源：http://hz.yangfankeji.com/gtcjujxgkg.html

Py:   class User: pass
来源：http://hz.zhengqikj.top/gtfpxjhjei.html

PHP:  class User {}
来源：http://hz.yueranfly.top/gtjznqbxlv.html

JS:   class User {}
来源：http://hz.redwolf501.top/gtaodskilb.html

TS:   class User { name: string = ""; }
来源：http://hz.yonumen.top/gtzhdcyuck.html

Java: class User {}
来源：http://hz.zdqjudy.top/gtiajizgvo.html

Go:   type User struct { Name string }
来源：http://hz.xuetiantiany.cn/gtsqvxhldh.html

Ruby: class User; end
来源：http://hz.snrcjt.cn/gtysstlhig.html

C#:   class User {}
来源：http://hz.pycfn.com/gtqlrwiqgw.html

[G02] 构造函数
来源：http://hz.daria6918.cn/gtexitvexh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fengsongda.top/gtzipqcsix.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gzhubu.top/gtzckoebws.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.9152youxi.cn/gtxhlocgev.html

TS:   constructor(public name: string) {}
来源：http://hz.jyoumei.cn/gtrgybxkwj.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtmtdxpvor.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hongshengwenyu.top/gtfceiosqg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yonumen.top/gtmkrlwwaf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ydzc1.top/gtamxdaclf.html

[G03] 实例属性
来源：http://hz.ydjk.org.cn/gtmceuotzr.html

Py:   self.name = "x"
来源：http://hz.shzxlz.cn/gtvwctagxa.html

PHP:  public string $name = "x";
来源：http://hz.birdmap.top/gthbiwbypv.html

JS:   this.name = "x";
来源：http://hz.chenzaomai.com/gttkhacjvb.html

TS:   name: string = "x";
来源：http://hz.c1oappe.top/gtteejqozm.html

Java: private String name;
来源：http://hz.redwolf501.top/gtjmnnqpet.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zycfv.cn/gtfriclbnt.html

Ruby: @name = "x"
来源：http://hz.zhixingplan.top/gtyknmzgno.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.vqdsnc.cn/gtvksvuszi.html

[G04] 定义方法
来源：http://hz.meibo888.top/gtobriuqid.html

Py:   def greet(self): return self.name
来源：http://hz.nanxinkj.top/gtthvyvpsg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtzckioylw.html

JS:   greet() { return this.name; }
来源：http://hz.feifeiyinyue.top/gtpmwttdeb.html

TS:   greet(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gtaxybefeq.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gtgnbijdop.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.meibo888.top/gtqwruborm.html

Ruby: def greet; @name; end
来源：http://hz.dianchejie.cn/gtztpabdkg.html

C#:   public string Greet() => Name;
来源：http://hz.yangfankeji.com/gtkkccyefe.html

[G05] 继承
来源：http://hz.wangdashe.top/gtgmlqxuwz.html

Py:   class Admin(User): pass
来源：http://hz.gotoacloud.top/gttityqprc.html

PHP:  class Admin extends User {}
来源：http://hz.birdmap.top/gtzgjnznym.html

JS:   class Admin extends User {}
来源：http://hz.xinyue.icu/gtdacnkvwf.html

TS:   class Admin extends User {}
来源：http://hz.svipenyu.cn/gtwjmdyvla.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtibylnqez.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.haohaochexian.top/gtpfswblfz.html

Ruby: class Admin < User; end
来源：http://hz.jinqigufen.top/gtubydagsu.html

C#:   class Admin : User {}
来源：http://hz.0kj1m.cn/gtmpgohnpc.html

[G06] 重写方法
来源：http://hz.redwolf501.top/gtsuuqmvlh.html

Py:   def greet(self): return "admin"
来源：http://hz.chenlongwang.top/gtnzfknztc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhengqikj.top/gtpbvspcow.html

JS:   greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtahutsyyr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tianlin.xyz/gterqltcvy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fengsongda.top/gtuqtjpfsh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ywan-chungtsiang.top/gtcpyagmew.html

Ruby: def greet; "admin"; end
来源：http://hz.zhiwuduotai.top/gtisckuqyq.html

C#:   public override string Greet() => "admin";
来源：http://hz.jlsjyb.cn/gtdidyveci.html

[G07] 调用父类方法
来源：http://hz.tian-w.cn/gtnetvanqx.html

Py:   super().greet()
来源：http://hz.xylfe.cn/gtebnovxjb.html

PHP:  parent::greet();
来源：http://hz.fengsongda.top/gtucylxqim.html

JS:   super.greet();
来源：http://hz.mhx1999.top/gtpcjvepoo.html

TS:   super.greet();
来源：http://hz.gzhubu.top/gtwodrcckb.html

Java: super.greet();
来源：http://hz.sufxvd.cn/gthafrhorl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.feifeiyinyue.top/gtptjtnuhw.html

Ruby: super
来源：http://hz.meibo888.top/gteubjeiid.html

C#:   base.Greet();
来源：http://hz.zycfv.cn/gtzafgcioa.html

[G08] 静态方法与属性
来源：http://hz.yuxming.cn/gtxbgyteay.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenjidiqi.icu/gtddgrrthq.html

PHP:  public static function f() {}
来源：http://hz.nwbrower.top/gtmwjxufus.html

JS:   static f() {}
来源：http://hz.shangyingyoupin.top/gtqjysenuk.html

TS:   static f(): void {}
来源：http://hz.cqqwz.cn/gtcfpfdebf.html

Java: static void f() {}
来源：http://hz.xuanzx.com/gttyafsjzm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.snrcjt.cn/gtrdurtnqe.html

Ruby: def self.f; end
来源：http://hz.zhijiandao.cn/gtcxuylnfh.html

C#:   public static void F() {}
来源：http://hz.yj20258888.top/gtkfwvtxfb.html

[G09] 接口 / 抽象类
来源：http://hz.52xcode.cn/gtfaibokth.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ehwqpu.com/gtiybffncy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tanke756.top/gtvxdfjwte.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gtwxdtedds.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinyuanbaomall.cn/gtimttldmw.html

Java: interface Shape { double area(); }
来源：http://hz.hongshengwenyu.top/gtqztsilyn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jlsjyb.cn/gtovtbutzn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.havefunace.top/gtkmuggbbm.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinghuilouyu.cn/gtnwzhrvel.html

[G10] 访问控制
来源：http://hz.sysykeji.top/gtrkdtpdws.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sysykeji.top/gtwjbdxsnq.html

PHP:  public / protected / private
来源：http://hz.haohaochexian.top/gtryowmwen.html

JS:   #private 字段；其余公开
来源：http://hz.jinqigufen.top/gtzzxnivaw.html

TS:   public / protected / private
来源：http://hz.vqdsnc.cn/gtmzgdgveg.html

Java: public / protected / private / 默认包级
来源：http://hz.jiagoushi.top/gtuahxzeed.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydjk.org.cn/gtpcvtdndo.html

Ruby: public / protected / private
来源：http://hz.hnxiangtu.top/gtztrjzant.html

C#:   public / protected / private / internal
来源：http://hz.iojbl.cn/gtlukhlldk.html

[G11] getter / setter
来源：http://hz.shanyushiyangkeji.top/gtpuyrmugr.html

Py:   @property 与 @x.setter
来源：http://hz.yuxming.cn/gtgxephlhy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtxqqrwebh.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigufen.top/gtxsasxcqd.html

TS:   get name(): string { return this._name; }
来源：http://hz.haohaochexian.top/gtombrzrbz.html

Java: public String getName() { return name; }
来源：http://hz.yj20258.top/gtdqagrrbj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtaiwckvmh.html

Ruby: attr_accessor :name
来源：http://hz.zycfv.cn/gtuwfqdsfl.html

C#:   public string Name { get; set; }
来源：http://hz.sxryk.cn/gtwtxuqtce.html

[G12] 对象转字符串
来源：http://hz.quarkkingdee.top/gtzrfmjnau.html

Py:   def __str__(self): return self.name
来源：http://hz.sweek.top/gtprgwnbbm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtvechhfeu.html

JS:   toString() { return this.name; }
来源：http://hz.meibo888.top/gtxbpmsviq.html

TS:   toString(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtpjtovbjb.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhongyouzk.top/gtwioyjmhe.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xziqi.cn/gtenrepprm.html

Ruby: def to_s; @name; end
来源：http://hz.tianlin.xyz/gtvqxggsig.html

C#:   public override string ToString() => Name;
来源：http://hz.jinyuanbaomall.cn/gteokqjpsk.html

[G13] 判断对象类型
来源：http://hz.aizwys.cn/gtmoolcfpb.html

Py:   isinstance(u, User)
来源：http://hz.andypj.xyz/gtcayhvsmf.html

PHP:  $u instanceof User
来源：http://hz.xuetiantiany.cn/gtgiyazskz.html

JS:   u instanceof User
来源：http://hz.zhijiandao.cn/gtzlfezdqb.html

TS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtajrbuocg.html

Java: u instanceof User
来源：http://hz.yonumen.top/gtewjqwxzu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenjidiqi.icu/gtdrbqwhpa.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtnqtpdstf.html

C#:   u is User
来源：http://hz.jqgufenzy.top/gtrjvmvflg.html

[G14] 数据类 / record
来源：http://hz.daria6918.cn/gtpyfkdsot.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pengpengdd.cyou/gtvbjvawpn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj20258888.top/gtpydcvxqp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258.top/gtedppmfub.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhoulong.xyz/gtylqemtzc.html

Java: record User(String name, int age) {}
来源：http://hz.52xcode.cn/gthshbhrlh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jianghu66.top/gtoskfryhj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuanzx.com/gtjegyqcnw.html

C#:   record User(string Name, int Age);
来源：http://hz.zhixingplan.top/gtjtpwbklq.html

[G15] 枚举
来源：http://hz.yuanzhike.top/gtqbhxczkz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cheryme.top/gtxwqruggk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.andypj.xyz/gthkylimzb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xingfuxueyuan.xyz/gtnonkkwrc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.meibo888.top/gtixwpttox.html

Java: enum Color { RED, GREEN }
来源：http://hz.havefunace.top/gtxofixkuf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shuidangran.top/gtehithxea.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydjk.org.cn/gtgdkdtzbb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cucudq.cn/gtvrxrwbbj.html

[G16] 对象转数组 / 字典
来源：http://hz.yuxming.cn/gtppwjqgnx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhengqikj.top/gthqjwmony.html

PHP:  get_object_vars($obj);
来源：http://hz.daxiang520.top/gtyelxuzql.html

JS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtubyvcnoo.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtckpddksi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yangfankeji.com/gtfukjmdbp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yanxiufei.cn/gthtiiftib.html

Ruby: obj.instance_variables
来源：http://hz.52xcode.cn/gtzefldmjl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nwbrower.top/gtoxcgdbdo.html

================================================================================
来源：http://hz.yuanzhike.top/gtyjtgchdr.html

H. 异常与错误处理
来源：http://hz.hongshengwenyu.top/gtlbyfmekr.html

================================================================================
来源：http://hz.dashuyun.cn/gtsveeqjlg.html

[H01] try / catch 基础
来源：http://hz.yuxming.cn/gtcujbyszw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.birdmap.top/gtpdfmchgy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuxming.cn/gtgtkaxbvw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.birdmap.top/gthctyxohj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnqzz.top/gtmxfafjcq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shuidangran.top/gtqjrmlxur.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.vqdsnc.cn/gtasnufvqi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydzc1.top/gtuxcvjnrh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sufxvd.cn/gtvucltyrp.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtzgqqrwqk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinyuanbaomall.cn/gtykqwvrjz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtsjmezdoh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtomkjqrur.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtlsdmxppo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtioylkted.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yongpay.top/gtiiuuofaa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhongyouzk.top/gtxlenhcir.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ybcxt.top/gtgwoigplc.html

[H03] 主动抛出异常
来源：http://hz.hongshengwenyu.top/gtvhqgpfzl.html

Py:   raise ValueError("错误信息")
来源：http://hz.ybcxt.top/gtndnbxuem.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtmtaxvvvn.html

JS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtztkhzmdi.html

TS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtydnixber.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtsftcetgp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cucudq.cn/gtrztpdmny.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinqigufen.top/gtxyfpbkwu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtehzirquk.html

[H04] 自定义异常类型
来源：http://hz.daxiang520.top/gtsthbpamd.html

Py:   class MyError(Exception): pass
来源：http://hz.zycfv.cn/gtmuxaywgo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhengqikj.top/gtzwjdmvdk.html

JS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gtlvaxsrdh.html

TS:   class MyError extends Error {}
来源：http://hz.xuetiantiany.cn/gtyxaordvg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258.top/gtksgcqaen.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hongshengwenyu.top/gtxhdjbinm.html

Ruby: class MyError < StandardError; end
来源：http://hz.quarkkingdee.top/gtwyletlyu.html

C#:   class MyException : Exception {}
来源：http://hz.iojbl.cn/gtfejhxmzj.html

[H05] 捕获特定类型
来源：http://hz.wangshuangyany.cn/gtckdatfpj.html

Py:   except ValueError as e:
来源：http://hz.havefunace.top/gtosujcaol.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhongyouzk.top/gtfigztwkt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtbyivrbap.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtyfjqkkds.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.birdmap.top/gtctasksuv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.quarkkingdee.top/gtffleojff.html

Ruby: rescue ArgumentError => e
来源：http://hz.gotoacloud.top/gthswajcpu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jiagoushi.top/gtzbwziqfp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.birdmap.top/gtwjiouzrt.html

Py:   value = d.get("k") or default
来源：http://hz.hnqzz.top/gtcxsmiiec.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.c1oappe.top/gttunflloe.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigufen.top/gtbnifjvwe.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtkeeokzwx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ydzc1.top/gtavwrebag.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj202588.top/gtoiizbkul.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtrdyetuua.html

C#:   obj?.A?.B ?? default
来源：http://hz.feifeiyinyue.top/gtajcjitut.html

[H07] 断言
来源：http://hz.ywan-chungtsiang.top/gthnoastap.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cheryme.top/gtosqrdvwi.html

PHP:  assert($x > 0);
来源：http://hz.xziqi.cn/gtzoovsoeo.html

JS:   console.assert(x > 0);
来源：http://hz.jlsjyb.cn/gtxkdbfqfe.html

TS:   console.assert(x > 0);
来源：http://hz.svipenyu.cn/gthcsltgxd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj202588.top/gtlzkotjdg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cucudq.cn/gthqjgsevz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.snrcjt.cn/gtvatatyjs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.c1oappe.top/gtgijjdjwz.html

[H08] 获取错误信息与堆栈
来源：http://hz.vqdsnc.cn/gtvwxzbucy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xinyue.icu/gtccohprng.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigfzy.top/gtffymfsjg.html

JS:   e.message;  e.stack
来源：http://hz.haohaochexian.top/gtzcvjfdeo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xylfe.cn/gtuleutmst.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jlsjyb.cn/gtcnyohnah.html

Go:   err.Error()
来源：http://hz.tianlin.xyz/gthikecnsz.html

Ruby: e.message;  e.backtrace
来源：http://hz.c1oappe.top/gtvbuysgjq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yueranfly.top/gtcftcmpjq.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gtouhiyfxe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hysaishi.cn/gtjgvzketl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxuanxn.top/gtmovprmyg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dianchejie.cn/gtmhlrykcm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xingfuxueyuan.xyz/gtnftgytwp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.svipenyu.cn/gtrgswjaty.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuxming.cn/gtljdfgjwh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.daxiang520.top/gtdyjkslxt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.c1oappe.top/gtblnnzjro.html

[H10] 资源自动释放
来源：http://hz.cheryme.top/gtbamvbxmm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinyuanbaomall.cn/gtcfxaqfpd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.svipenyu.cn/gtaaerpfui.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daxiang520.top/gtmvibiicr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtcyrewuwn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydzc1.top/gteouyskrj.html

Go:   defer f.Close()
来源：http://hz.wangdashe.top/gtridrjwjx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xinyue.icu/gtuuvjxiwp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hfpthk.cn/gtovepijpf.html

================================================================================
来源：http://hz.yj20258888.top/gtghxkhtgi.html

I. 正则表达式
来源：http://hz.xylfe.cn/gtjgpcewnp.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtpvreqhro.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtaniofuuh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sweek.top/gtqqgysyrv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenjidiqi.icu/gtnmcpfzgm.html

JS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtgdksxglw.html

TS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtdlgvgjyd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guannengcc.top/gtflinuacj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ywan-chungtsiang.top/gtexqsrrfq.html

Ruby: s.match?(/\d+/)
来源：http://hz.xingfuxueyuan.xyz/gttfyxakbe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtthvdclxl.html

[I02] 提取所有匹配
来源：http://hz.iojbl.cn/gtpbzhokwe.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuetiantiany.cn/gthoisrcxv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ehwqpu.com/gtjhsizwaq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.andypj.xyz/gtzmlfukly.html

TS:   s.match(/\d+/g)
来源：http://hz.316326.xyz/gtmnuvhtwt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nanxinkj.top/gtjdsirbev.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guannengcc.top/gtpbldsnrh.html

Ruby: s.scan(/\d+/)
来源：http://hz.iojbl.cn/gttbpiaojk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangkeji.top/gticsphflj.html

[I03] 提取捕获分组
来源：http://hz.vqdsnc.cn/gtwxbdilku.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuetiantiany.cn/gtzufrmyxz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.kuanghao11.cn/gtdlsgodsn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxinkj.top/gtpybzghcz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hongshengwenyu.top/gtduvhteuh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhoulong.xyz/gtiiwnakyi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhongyouzk.top/gtszomnfmk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnqzz.top/gtriiuucpa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hammf.cn/gtcavtwxcr.html

[I04] 正则替换
来源：http://hz.fzhhl.top/gtohbznyvm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgufenzy.top/gtrbqioyub.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yongpay.top/gtvnjjmybc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gtefjjnapa.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtdubhfyyu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.iojbl.cn/gtbtjqhvst.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.kuanghao11.cn/gtaekhtqfa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yangfankeji.com/gtlczadbbq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigfzy.top/gtbskldtyi.html

[I05] 按正则拆分
来源：http://hz.jqgfzy.top/gtskvvxcap.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cashguo.top/gtvsqwjkyt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daria6918.cn/gtwbbelzgs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtnawbocua.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtxglhxijw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ybcxt.top/gtsnywarim.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenjidiqi.icu/gtofikxgyi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtchozeuxl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jiagoushi.top/gtidrlknuq.html


<!-- 参考信息 -->