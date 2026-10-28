代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gthvtmccdf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtssnhbwgk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jyoumei.cn/gtiahtnjsw.html

[F12] CSV 读写
来源：http://hz.chenzaomai.com/gtdmnllthp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuanzx.com/gtbinablmg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cashguo.top/gtxcvrgbeg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ppjwa.cn/gtflbgecri.html

TS:   // 同上
来源：http://hz.chenlongwang.top/gtdysawzan.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.bjfxy.top/gtiemwiigu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daxiang520.top/gtobwhsilo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aizwys.cn/gtbfofhhyo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sufxvd.cn/gtffiyoevu.html

================================================================================
来源：http://hz.yonumen.top/gtrusltuzi.html

G. 面向对象
来源：http://hz.pengpengdd.cyou/gtyxrlyewx.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtecigzbni.html

[G01] 定义类
来源：http://hz.jinghuilouyu.cn/gtjwqxcixi.html

Py:   class User: pass
来源：http://hz.xylfe.cn/gtgrmvntgw.html

PHP:  class User {}
来源：http://hz.jinqigufen.top/gtlhdfxzxa.html

JS:   class User {}
来源：http://hz.ppjwa.cn/gtvarquwyq.html

TS:   class User { name: string = ""; }
来源：http://hz.jqgufenzy.top/gtltpyqsld.html

Java: class User {}
来源：http://hz.yj202588.top/gtbtvucwxu.html

Go:   type User struct { Name string }
来源：http://hz.nanxinkj.top/gtddloycre.html

Ruby: class User; end
来源：http://hz.yj202588.top/gttgpuhjyf.html

C#:   class User {}
来源：http://hz.tian-w.cn/gtazoorjri.html

[G02] 构造函数
来源：http://hz.quarkkingdee.top/gtdnprkdso.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ywan-chungtsiang.top/gtozhezmcm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.birdmap.top/gtnmgrmjlw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tianlin.xyz/gtbkvsliug.html

TS:   constructor(public name: string) {}
来源：http://hz.xylfe.cn/gtikkebbfm.html

Java: User(String name) { this.name = name; }
来源：http://hz.jyoumei.cn/gtvqqexujn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.feifeiyinyue.top/gtisrbndsu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtrimutnkf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.meibo888.top/gtyffwjqdr.html

[G03] 实例属性
来源：http://hz.zhijiandao.cn/gtwvhndbtb.html

Py:   self.name = "x"
来源：http://hz.yj20258888.top/gtuhxavkod.html

PHP:  public string $name = "x";
来源：http://hz.hammf.cn/gtplquhzli.html

JS:   this.name = "x";
来源：http://hz.jinqigufen.top/gtrocrqilz.html

TS:   name: string = "x";
来源：http://hz.haohaochexian.top/gthldydmrb.html

Java: private String name;
来源：http://hz.chenlongwang.top/gtjwcbyoru.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258.top/gthxbkxtos.html

Ruby: @name = "x"
来源：http://hz.sufxvd.cn/gtnihculfc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.iojbl.cn/gtjqonflsj.html

[G04] 定义方法
来源：http://hz.feifeiyinyue.top/gttsqxxnpw.html

Py:   def greet(self): return self.name
来源：http://hz.iojbl.cn/gtuxtqyylj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtpobkkawx.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigufen.top/gtbutjafdv.html

TS:   greet(): string { return this.name; }
来源：http://hz.ybcxt.top/gtdaobfzry.html

Java: String greet() { return name; }
来源：http://hz.hysaishi.cn/gtrqbijdee.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuanzx.com/gtdiqgwaur.html

Ruby: def greet; @name; end
来源：http://hz.xuetiantiany.cn/gtufvrxowj.html

C#:   public string Greet() => Name;
来源：http://hz.zdqjudy.top/gtzdqhbadp.html

[G05] 继承
来源：http://hz.andypj.xyz/gtbtobytjg.html

Py:   class Admin(User): pass
来源：http://hz.gaohongyu789.top/gtuepvxmcg.html

PHP:  class Admin extends User {}
来源：http://hz.ppjwa.cn/gtcswduqak.html

JS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtcdsusrba.html

TS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtdspeqeiz.html

Java: class Admin extends User {}
来源：http://hz.chenlongwang.top/gtlbgqfkfd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shangyingyoupin.top/gtzcceczks.html

Ruby: class Admin < User; end
来源：http://hz.jlsjyb.cn/gtqaymarri.html

C#:   class Admin : User {}
来源：http://hz.yj20258888.top/gtyfswhkfh.html

[G06] 重写方法
来源：http://hz.bjfxy.top/gtbnleossa.html

Py:   def greet(self): return "admin"
来源：http://hz.gogol.net.cn/gtvdorjkhn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtbanzpzqj.html

JS:   greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtcayfajrf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtnoflixth.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gotoacloud.top/gtssbbrmwm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenjidiqi.icu/gtipozkdot.html

Ruby: def greet; "admin"; end
来源：http://hz.cashguo.top/gthepmglfr.html

C#:   public override string Greet() => "admin";
来源：http://hz.cdnleiting.top/gthwanwgpg.html

[G07] 调用父类方法
来源：http://hz.pengpengdd.cyou/gtfeahuvif.html

Py:   super().greet()
来源：http://hz.shanyushiyangtech.top/gtepoxkbyz.html

PHP:  parent::greet();
来源：http://hz.yanxiufei.cn/gttwqmsdlg.html

JS:   super.greet();
来源：http://hz.xuanzx.com/gtbzgloqva.html

TS:   super.greet();
来源：http://hz.gzhubu.top/gtpgtzjloc.html

Java: super.greet();
来源：http://hz.yj20258.top/gtduilgayl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xziqi.cn/gtrdniljrf.html

Ruby: super
来源：http://hz.havefunace.top/gtrqltvpec.html

C#:   base.Greet();
来源：http://hz.hongshengwenyu.top/gtayueyfeq.html

[G08] 静态方法与属性
来源：http://hz.jyoumei.cn/gtpdsoxjui.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daxiang520.top/gtrnzgutao.html

PHP:  public static function f() {}
来源：http://hz.xuetiantiany.cn/gtqgbggrsn.html

JS:   static f() {}
来源：http://hz.guannengcc.top/gtggiifjrv.html

TS:   static f(): void {}
来源：http://hz.zhaomingkeji.xyz/gtbgeawpzl.html

Java: static void f() {}
来源：http://hz.quarkkingdee.top/gtaqpefjhx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gtlkqegytf.html

Ruby: def self.f; end
来源：http://hz.0kj1m.cn/gtoszifsci.html

C#:   public static void F() {}
来源：http://hz.wangdashe.top/gtlknnszkt.html

[G09] 接口 / 抽象类
来源：http://hz.sysykeji.top/gtlhcmflyz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtkrpenspd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuetiantiany.cn/gtxjivygul.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jiagoushi.top/gtllvsbokx.html

TS:   interface Shape { area(): number; }
来源：http://hz.smart0.xyz/gtnzjqwgmc.html

Java: interface Shape { double area(); }
来源：http://hz.jqgfzy.top/gtutncfdod.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinghuilouyu.cn/gtglnyrkvx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxuanxn.top/gttlusbouj.html

C#:   interface IShape { double Area(); }
来源：http://hz.nwbrower.top/gtehiadbjz.html

[G10] 访问控制
来源：http://hz.gzhubu.top/gtsxqqpybd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yvedp.cn/gtedfdxban.html

PHP:  public / protected / private
来源：http://hz.cucudq.cn/gtewhvpbpg.html

JS:   #private 字段；其余公开
来源：http://hz.redwolf501.top/gtctacfaoq.html

TS:   public / protected / private
来源：http://hz.nanxuanxn.top/gtckhwtdxn.html

Java: public / protected / private / 默认包级
来源：http://hz.cashguo.top/gtghcvikbi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cheryme.top/gtjixoovoq.html

Ruby: public / protected / private
来源：http://hz.zhongyouzk.top/gtesdyjknw.html

C#:   public / protected / private / internal
来源：http://hz.andypj.xyz/gtphejdype.html

[G11] getter / setter
来源：http://hz.kuanghao11.cn/gtbfzoplbm.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtyeinsgkf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtaathmpkf.html

JS:   get name() { return this._name; }
来源：http://hz.hnxiangtu.top/gtdeuzcuxu.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gtpcwajong.html

Java: public String getName() { return name; }
来源：http://hz.smart0.xyz/gtmfsyfgnw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fengsongda.top/gtufnnhlye.html

Ruby: attr_accessor :name
来源：http://hz.birdmap.top/gtducmggww.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangkeji.top/gtnaozjych.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtjcihhyvr.html

Py:   def __str__(self): return self.name
来源：http://hz.zycfv.cn/gtfpixjxcf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtmtkhaaqu.html

JS:   toString() { return this.name; }
来源：http://hz.zhongyouzk.top/gtjjipmjlh.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj202588.top/gtkguszily.html

Java: @Override public String toString() { return name; }
来源：http://hz.cucudq.cn/gtuhtnudda.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jiagoushi.top/gtyqhckibj.html

Ruby: def to_s; @name; end
来源：http://hz.sysykeji.top/gtzkubkljl.html

C#:   public override string ToString() => Name;
来源：http://hz.hysaishi.cn/gtzhchzfwl.html

[G13] 判断对象类型
来源：http://hz.yj20258.top/gtrcohnnvn.html

Py:   isinstance(u, User)
来源：http://hz.birdmap.top/gtocnmyjgr.html

PHP:  $u instanceof User
来源：http://hz.zhixingplan.top/gtgqrrbhdl.html

JS:   u instanceof User
来源：http://hz.gotoacloud.top/gtmjjrzach.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtrkhggzhh.html

Java: u instanceof User
来源：http://hz.kuanghao11.cn/gtqbtupksv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenzaomai.com/gtxdmqbkxn.html

Ruby: u.is_a?(User)
来源：http://hz.zycfv.cn/gtjvgailyk.html

C#:   u is User
来源：http://hz.yonumen.top/gtyaienlbk.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtjwjqrrxe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hywenlv.cn/gtglraiksb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gotoacloud.top/gtuwbewtno.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhiwuduotai.top/gtuvxktifm.html

TS:   type User = { name: string; age: number };
来源：http://hz.birdmap.top/gtdxtdhazx.html

Java: record User(String name, int age) {}
来源：http://hz.yangfankeji.com/gtmljuywuv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xziqi.cn/gtbddqzepk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhoulong.xyz/gtcactqtzw.html

C#:   record User(string Name, int Age);
来源：http://hz.tanke756.top/gtemdmwxsc.html

[G15] 枚举
来源：http://hz.ydzc1.top/gttivmjkdh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dianchejie.cn/gtoluvsgvq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hnqzz.top/gticklzedh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shuidangran.top/gtotuulvgd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigfzy.top/gtetyssfko.html

Java: enum Color { RED, GREEN }
来源：http://hz.hammf.cn/gttutuzsft.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ybcxt.top/gtxlwbmucd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigufen.top/gtenlicewp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gtsbxpjtqc.html

[G16] 对象转数组 / 字典
来源：http://hz.ppjwa.cn/gtvgdntobf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dianchejie.cn/gtfbmrhojg.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gtlhrqfrqu.html

JS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtmvikgzqp.html

TS:   Object.entries(obj)
来源：http://hz.pycfn.com/gthybornqr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ybcxt.top/gtgswarzip.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtjjvdksmu.html

Ruby: obj.instance_variables
来源：http://hz.zhijiandao.cn/gtttdphzgr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.c1oappe.top/gtqqehttfc.html

================================================================================
来源：http://hz.jlsjyb.cn/gtsclqaksz.html

H. 异常与错误处理
来源：http://hz.ydjk.org.cn/gtyltxwqxm.html

================================================================================
来源：http://hz.ydzc1.top/gtvhibxjdi.html

[H01] try / catch 基础
来源：http://hz.yueranfly.top/gtmuwbnwmj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hysaishi.cn/gtmpcbawmk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinghuilouyu.cn/gthhqxnqgn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtephbnphm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtcqruaruq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sweek.top/gtbvswogyg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhoulong.xyz/gtjlqchofe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtxmaffcwj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hywenlv.cn/gtekewlfig.html

[H02] finally / ensure 收尾
来源：http://hz.gzhubu.top/gtstiyjxgk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gotoacloud.top/gtlfwiujin.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtisvqbmum.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtzapfclje.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtqzzpxylt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtdylpclud.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dianchejie.cn/gtooqlxhxo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shzxlz.cn/gtewwbnqkn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenzaomai.com/gtuujgwdmg.html

[H03] 主动抛出异常
来源：http://hz.havefunace.top/gtqzkoodeq.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhongyouzk.top/gturktvoov.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gtqlxrscnx.html

JS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtfoeigbfn.html

TS:   throw new Error("错误信息");
来源：http://hz.yonumen.top/gtdtbjiuoi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtruicgkez.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gteteemoxa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.kuanghao11.cn/gtjurfeiot.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hammf.cn/gtdiajmtdk.html

[H04] 自定义异常类型
来源：http://hz.yongpay.top/gtymzfyeun.html

Py:   class MyError(Exception): pass
来源：http://hz.9152youxi.cn/gtztvnbkaj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gthubgidhl.html

JS:   class MyError extends Error {}
来源：http://hz.meibo888.top/gtunezwizs.html

TS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtwzvqrwox.html

Java: class MyException extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtdwdpygjr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhixingplan.top/gtjsssxehu.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtataomlid.html

C#:   class MyException : Exception {}
来源：http://hz.feifeiyinyue.top/gtvqxzhcqv.html

[H05] 捕获特定类型
来源：http://hz.sufxvd.cn/gthdnsamgo.html

Py:   except ValueError as e:
来源：http://hz.zhaomingkeji.xyz/gtgawsucwd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ehwqpu.com/gtgyfrxery.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shzxlz.cn/gtzlrtelah.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtqabhiwng.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sufxvd.cn/gtssopagbp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.pycfn.com/gtbucndpbk.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258888.top/gtkfuocjib.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ybcxt.top/gtjjndtcmp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yuxming.cn/gtbtrerjpb.html

Py:   value = d.get("k") or default
来源：http://hz.ppjwa.cn/gtdqbwkais.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.havefunace.top/gtrohrkkzx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtstixqabi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtbpbzvvfw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhixingplan.top/gtjuctmqgj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guowangkeji.top/gtroavokat.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangkeji.top/gtrykihkdg.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtwifkamys.html

[H07] 断言
来源：http://hz.hongshengwenyu.top/gtcnylobjn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nwbrower.top/gtcejuvrff.html

PHP:  assert($x > 0);
来源：http://hz.smart0.xyz/gtwjuatydi.html

JS:   console.assert(x > 0);
来源：http://hz.jqgufenzy.top/gtlktvzwva.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtytrggwao.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangkeji.top/gtzqcrydtv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hysaishi.cn/gttzoralou.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxuanxn.top/gtadfrmdxd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ehwqpu.com/gtbgtfxgvy.html

[H08] 获取错误信息与堆栈
来源：http://hz.birdmap.top/gtuldegglo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgufenzy.top/gtljdkgxoi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhengqikj.top/gtcjrhutua.html

JS:   e.message;  e.stack
来源：http://hz.yj20258.top/gtjtmcoela.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigfzy.top/gtfkhqiows.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yonumen.top/gtnvmmlvkg.html

Go:   err.Error()
来源：http://hz.cucudq.cn/gtvnkrtdgv.html

Ruby: e.message;  e.backtrace
来源：http://hz.zycfv.cn/gtgnzlvrka.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cqqwz.cn/gtvxueyykm.html

[H09] 带错误码的异常
来源：http://hz.shuidangran.top/gtbuslgbrk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangkeji.top/gtrjbxufzy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhengqikj.top/gtgmaukjcj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ivvv.top/gttlksmjfg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cdnleiting.top/gtmlhfgnmp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhongyouzk.top/gtkjwqlyts.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuanzhike.top/gtnfcxdhtr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jiagoushi.top/gthdpcrtkf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aibaodan.cn/gtpcvldudw.html

[H10] 资源自动释放
来源：http://hz.jinqigufen.top/gthzwxnzfh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jyoumei.cn/gtaxuntrdt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daria6918.cn/gtizlnciwh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtxtqodaao.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtucmthjhp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guannengcc.top/gtktukmjbb.html

Go:   defer f.Close()
来源：http://hz.daxiang520.top/gtuecjqpej.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hfpthk.cn/gtqymoseko.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.316326.xyz/gtieblokez.html

================================================================================
来源：http://hz.cucudq.cn/gtitjekiur.html

I. 正则表达式
来源：http://hz.shuidangran.top/gtcofhtbra.html

================================================================================
来源：http://hz.dashuyun.cn/gtpuebmgvj.html

[I01] 判断是否匹配
来源：http://hz.zhengqikj.top/gtywniczeq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yanxiufei.cn/gtnwrvxojf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.mhx1999.top/gtsgikpnwu.html

JS:   /\d+/.test(s)
来源：http://hz.feifeiyinyue.top/gtriykrmjn.html

TS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtecjbkmxv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sxryk.cn/gtygelfzdz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenzaomai.com/gtckpvgubx.html

Ruby: s.match?(/\d+/)
来源：http://hz.316326.xyz/gtlyrrxnxk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gtbmblrknm.html

[I02] 提取所有匹配
来源：http://hz.ppjwa.cn/gtxymfrxqa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cashguo.top/gtodtbqzmw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuxming.cn/gtwqavddof.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pengpengdd.cyou/gtusktlcku.html

TS:   s.match(/\d+/g)
来源：http://hz.ehwqpu.com/gtyrsoxuza.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jiagoushi.top/gtqnwnvprr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.svipenyu.cn/gtlbiqmpeh.html

Ruby: s.scan(/\d+/)
来源：http://hz.shuidangran.top/gtzsbvhsfu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xziqi.cn/gtdahignse.html

[I03] 提取捕获分组
来源：http://hz.jyoumei.cn/gtozthoclf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shzxlz.cn/gtwffzlfor.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hnqzz.top/gtfmaqfzye.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhaomingkeji.xyz/gtkqxzzoqv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigfzy.top/gtmzakrvrx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guowangkeji.top/gtnpbywbgn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tanke756.top/gtrkvjvjph.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shzxlz.cn/gtjboczboo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tian-w.cn/gtmuxtkhtt.html

[I04] 正则替换
来源：http://hz.jyoumei.cn/gtilpwtddb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dashuyun.cn/gtxlcosmor.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jiagoushi.top/gtpfzwwxnn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gtjsorjosc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtwiuuytnc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jianghu66.top/gtzjtgmljs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgfzy.top/gtorfvmuky.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dianchejie.cn/gtidpbenmq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ehwqpu.com/gtyqglwopv.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtftxqodwd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.mhx1999.top/gtcqfgzlyw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sxryk.cn/gtaicppvlp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtvhnawvvc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtwgwfqsbn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yj20258.top/gtqzhmqucz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ppjwa.cn/gtlrgeqesh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gteaxjxpfo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigfzy.top/gttmuelfwl.html


<!-- 参考信息 -->