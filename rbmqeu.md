代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.smart0.xyz/gtcdbliooj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtxrjatitl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtfctxtpgv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.snrcjt.cn/gtvzayyyje.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jiagoushi.top/gtgpskotwb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sweek.top/gtklyazajw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zycfv.cn/gtbobzikxk.html

[F12] CSV 读写
来源：http://hz.fzhhl.top/gtucvoxhiq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ppjwa.cn/gtwomneqyb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnqzz.top/gtzfsaiqpc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.pengpengdd.cyou/gtssaqfkyc.html

TS:   // 同上
来源：http://hz.havefunace.top/gtcefuenwq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhongyouzk.top/gtwjohtahp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ivvv.top/gtxhnqapul.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.haohaochexian.top/gtileekczn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhengqikj.top/gtajjidaun.html

================================================================================
来源：http://hz.fengsongda.top/gtojwafhwz.html

G. 面向对象
来源：http://hz.shanyushiyangtech.top/gtsasifvxy.html

================================================================================
来源：http://hz.daria6918.cn/gtzckshdjp.html

[G01] 定义类
来源：http://hz.tianlin.xyz/gtxyzbkfvz.html

Py:   class User: pass
来源：http://hz.wangdashe.top/gtjxhvxsvb.html

PHP:  class User {}
来源：http://hz.andypj.xyz/gtfxhgwgwy.html

JS:   class User {}
来源：http://hz.fengsongda.top/gtjpsoerdm.html

TS:   class User { name: string = ""; }
来源：http://hz.yangfankeji.com/gtwtmxmqgk.html

Java: class User {}
来源：http://hz.shangyingyoupin.top/gtlmqtqtzg.html

Go:   type User struct { Name string }
来源：http://hz.pengpengdd.cyou/gtmmhoixqm.html

Ruby: class User; end
来源：http://hz.xuetiantiany.cn/gtomecevfc.html

C#:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtoolybtet.html

[G02] 构造函数
来源：http://hz.cdnleiting.top/gtybegoaky.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hongshengwenyu.top/gtivhytipn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinyuanbaomall.cn/gtpaefhclc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gttiszkxqn.html

TS:   constructor(public name: string) {}
来源：http://hz.guannengcc.top/gtvstdcatp.html

Java: User(String name) { this.name = name; }
来源：http://hz.tianlin.xyz/gtjhmaeihs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258888.top/gtnhdlavbd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tianlin.xyz/gtfglumnbn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.meibo888.top/gtyipgiwvs.html

[G03] 实例属性
来源：http://hz.bjfxy.top/gtsyanxpul.html

Py:   self.name = "x"
来源：http://hz.aizwys.cn/gtkjdtkxyr.html

PHP:  public string $name = "x";
来源：http://hz.sufxvd.cn/gtvjlwufgw.html

JS:   this.name = "x";
来源：http://hz.jinyuanbaomall.cn/gtwhembzkd.html

TS:   name: string = "x";
来源：http://hz.hongshengwenyu.top/gtdwipsgka.html

Java: private String name;
来源：http://hz.ybcxt.top/gtkjzlmuql.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jqgfzy.top/gtbaflwvgg.html

Ruby: @name = "x"
来源：http://hz.wangdashe.top/gtvspxeqwe.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cqqwz.cn/gtaghqorqu.html

[G04] 定义方法
来源：http://hz.jlsjyb.cn/gtzolrdqxn.html

Py:   def greet(self): return self.name
来源：http://hz.yueranfly.top/gttywndumt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtyortxrgg.html

JS:   greet() { return this.name; }
来源：http://hz.wangdashe.top/gtswbhmhgp.html

TS:   greet(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtbllcilxb.html

Java: String greet() { return name; }
来源：http://hz.andypj.xyz/gtpcsqivyk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.haohaochexian.top/gtiyascafc.html

Ruby: def greet; @name; end
来源：http://hz.pycfn.com/gtylvzhahb.html

C#:   public string Greet() => Name;
来源：http://hz.yj20258.top/gtmqmjocvx.html

[G05] 继承
来源：http://hz.fzhhl.top/gtcflrfdss.html

Py:   class Admin(User): pass
来源：http://hz.fengsongda.top/gtvrvbcnhy.html

PHP:  class Admin extends User {}
来源：http://hz.yj20258.top/gtlczswuuy.html

JS:   class Admin extends User {}
来源：http://hz.yuxming.cn/gtoeizksua.html

TS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtdttnhhbl.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtkgzywqwc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.snrcjt.cn/gtcqssniso.html

Ruby: class Admin < User; end
来源：http://hz.gzhubu.top/gtavtixyyp.html

C#:   class Admin : User {}
来源：http://hz.aizwys.cn/gtwelqkijs.html

[G06] 重写方法
来源：http://hz.iojbl.cn/gtcnwprrmh.html

Py:   def greet(self): return "admin"
来源：http://hz.sufxvd.cn/gtghoubrsc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtafhcacvy.html

JS:   greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gtrwwojlis.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gthuguvxyx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtkzlqooql.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gtpjsijync.html

Ruby: def greet; "admin"; end
来源：http://hz.yongpay.top/gtzuqqajfc.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgufenzy.top/gtanpxetvf.html

[G07] 调用父类方法
来源：http://hz.cashguo.top/gtevdjmvta.html

Py:   super().greet()
来源：http://hz.shuidangran.top/gtrkeosclz.html

PHP:  parent::greet();
来源：http://hz.bjfxy.top/gtcmedhvjt.html

JS:   super.greet();
来源：http://hz.cucudq.cn/gtviaftmsd.html

TS:   super.greet();
来源：http://hz.zdqjudy.top/gtodfwbjrx.html

Java: super.greet();
来源：http://hz.ehwqpu.com/gtvwaumirf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gotoacloud.top/gtwnkwdmzt.html

Ruby: super
来源：http://hz.hywenlv.cn/gthlwykxdk.html

C#:   base.Greet();
来源：http://hz.yj202588.top/gtfrzfxfxd.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gtwdljvwkh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.316326.xyz/gtqnlzhfjr.html

PHP:  public static function f() {}
来源：http://hz.xziqi.cn/gtdhnlgohr.html

JS:   static f() {}
来源：http://hz.tanke756.top/gthgcurqqd.html

TS:   static f(): void {}
来源：http://hz.quarkkingdee.top/gtdfypmxsl.html

Java: static void f() {}
来源：http://hz.chenlongwang.top/gtanrdgfns.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.quarkkingdee.top/gtwkjnerig.html

Ruby: def self.f; end
来源：http://hz.hammf.cn/gthbjhwtbh.html

C#:   public static void F() {}
来源：http://hz.andypj.xyz/gtuihxmrqi.html

[G09] 接口 / 抽象类
来源：http://hz.guowangkeji.top/gtedaztqdf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.feifeiyinyue.top/gtzkrjryun.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtpdifxhii.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhiwuduotai.top/gtvqlfenqq.html

TS:   interface Shape { area(): number; }
来源：http://hz.sufxvd.cn/gtfkzqrzrt.html

Java: interface Shape { double area(); }
来源：http://hz.guowangkeji.top/gtbvlsqszp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yanxiufei.cn/gtyrfjnksi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.quarkkingdee.top/gtmlizbztn.html

C#:   interface IShape { double Area(); }
来源：http://hz.fengsongda.top/gtkujidsue.html

[G10] 访问控制
来源：http://hz.jianghu66.top/gttqwocowe.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258.top/gtmytfbovz.html

PHP:  public / protected / private
来源：http://hz.yongpay.top/gtgxzbpcpw.html

JS:   #private 字段；其余公开
来源：http://hz.9152youxi.cn/gtiasxexhv.html

TS:   public / protected / private
来源：http://hz.yj202588.top/gtaqylhkqb.html

Java: public / protected / private / 默认包级
来源：http://hz.pycfn.com/gtylfypaqe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.c1oappe.top/gtiqpqbivn.html

Ruby: public / protected / private
来源：http://hz.aizwys.cn/gtizqrmrhs.html

C#:   public / protected / private / internal
来源：http://hz.aibaodan.cn/gtyeaigcqs.html

[G11] getter / setter
来源：http://hz.shanyushiyangtech.top/gtlrxardvz.html

Py:   @property 与 @x.setter
来源：http://hz.cucudq.cn/gtqarfftur.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtffnapbof.html

JS:   get name() { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtcgjwbfvt.html

TS:   get name(): string { return this._name; }
来源：http://hz.yanxiufei.cn/gtucnqxigz.html

Java: public String getName() { return name; }
来源：http://hz.xuanzx.com/gtvfvdusch.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gthkedfldv.html

Ruby: attr_accessor :name
来源：http://hz.quarkkingdee.top/gtwcpydsyt.html

C#:   public string Name { get; set; }
来源：http://hz.redwolf501.top/gtzyuzrrey.html

[G12] 对象转字符串
来源：http://hz.zhijiandao.cn/gthukzvzyr.html

Py:   def __str__(self): return self.name
来源：http://hz.xylfe.cn/gtcjolrdap.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtaluhoqnd.html

JS:   toString() { return this.name; }
来源：http://hz.hywenlv.cn/gtfpmefdup.html

TS:   toString(): string { return this.name; }
来源：http://hz.sxryk.cn/gttmkuarby.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuxming.cn/gtxdbhkswl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yangfankeji.com/gtvcyzxqkh.html

Ruby: def to_s; @name; end
来源：http://hz.ydzc1.top/gtkrxdroey.html

C#:   public override string ToString() => Name;
来源：http://hz.chenlongwang.top/gtryagmwbu.html

[G13] 判断对象类型
来源：http://hz.wangshuangyany.cn/gtturmwafe.html

Py:   isinstance(u, User)
来源：http://hz.kuanghao11.cn/gtgrniivcn.html

PHP:  $u instanceof User
来源：http://hz.yangfankeji.com/gttxkotxih.html

JS:   u instanceof User
来源：http://hz.cheryme.top/gthxcxvnfs.html

TS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtyqgaaftw.html

Java: u instanceof User
来源：http://hz.tianlin.xyz/gtkmfezdyl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinghuilouyu.cn/gtlorgzmmz.html

Ruby: u.is_a?(User)
来源：http://hz.tian-w.cn/gtpnymzrqb.html

C#:   u is User
来源：http://hz.mhx1999.top/gtuavackdk.html

[G14] 数据类 / record
来源：http://hz.gzhubu.top/gttghwalzs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jiagoushi.top/gtunevmbof.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.smart0.xyz/gtuzvxgivt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnqzz.top/gthysciyit.html

TS:   type User = { name: string; age: number };
来源：http://hz.redwolf501.top/gtioijtmyr.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangtech.top/gtglqdoluu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.andypj.xyz/gteisywjsc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.dianchejie.cn/gtupokwgrz.html

C#:   record User(string Name, int Age);
来源：http://hz.dashuyun.cn/gtnxfksfax.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gtluktudok.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.havefunace.top/gtihxxjoje.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nanxuanxn.top/gtoiakhjsq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.9152youxi.cn/gtzkxhvnvy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxuanxn.top/gtwbxptdce.html

Java: enum Color { RED, GREEN }
来源：http://hz.gzhubu.top/gtcaehrrmj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.bjfxy.top/gtkxrawqvz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gotoacloud.top/gtyjohnvhi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gtaropwibd.html

[G16] 对象转数组 / 字典
来源：http://hz.quarkkingdee.top/gtwsvvmahc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.meibo888.top/gtuqbdijno.html

PHP:  get_object_vars($obj);
来源：http://hz.shanyushiyangtech.top/gtpogcxgvg.html

JS:   Object.entries(obj)
来源：http://hz.nanxuanxn.top/gtuubxasqh.html

TS:   Object.entries(obj)
来源：http://hz.yuanzhike.top/gtieeubqdv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gzhubu.top/gtvxlzbvpo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.52xcode.cn/gtsprtqoln.html

Ruby: obj.instance_variables
来源：http://hz.nanxinkj.top/gtzyownxlh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxinkj.top/gttnwmunag.html

================================================================================
来源：http://hz.sxryk.cn/gtreyjxrxh.html

H. 异常与错误处理
来源：http://hz.tian-w.cn/gtmxdzsols.html

================================================================================
来源：http://hz.hnxiangtu.top/gtocgjhjjp.html

[H01] try / catch 基础
来源：http://hz.316326.xyz/gtrdlwdhxk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigufen.top/gteblhagjv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gzhubu.top/gtefeeqtqv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtnenjtjxi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.aibaodan.cn/gttunfpmla.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daria6918.cn/gthliaryyi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.vqdsnc.cn/gttozpudlf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yueranfly.top/gtuisyyhnp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xinyue.icu/gtobtpfnay.html

[H02] finally / ensure 收尾
来源：http://hz.shanyushiyangtech.top/gtcrvwyrho.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sxryk.cn/gtistkmjob.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtqygybgus.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtnflnozfr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtnkuyeizr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtlvshxira.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sysykeji.top/gteuedigtz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.quarkkingdee.top/gtbwotfmwt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hywenlv.cn/gtuwwrpmlh.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gtpjlyvgnb.html

Py:   raise ValueError("错误信息")
来源：http://hz.316326.xyz/gtgtjmulls.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtqyppmqlw.html

JS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gtwcxnucry.html

TS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtamwkwosu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gttuhrqitv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jyoumei.cn/gtotiampao.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxuanxn.top/gtcpzjbgum.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtbmxxnwvi.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtzswonvkw.html

Py:   class MyError(Exception): pass
来源：http://hz.hnxiangtu.top/gtkgjkvbts.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtdglxjbzv.html

JS:   class MyError extends Error {}
来源：http://hz.chenjidiqi.icu/gtiuexhzeq.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtvjzkwvph.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gtrfslfcoy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.mhx1999.top/gtxifrskek.html

Ruby: class MyError < StandardError; end
来源：http://hz.xinyue.icu/gtqvmtcbzp.html

C#:   class MyException : Exception {}
来源：http://hz.nanxuanxn.top/gtricatynx.html

[H05] 捕获特定类型
来源：http://hz.smart0.xyz/gtgdtjwmxd.html

Py:   except ValueError as e:
来源：http://hz.ydjk.org.cn/gtfrolattv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hammf.cn/gttyzffnzs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gtbizdcdip.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtzxwgiazv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhaomingkeji.xyz/gtijvkslqy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangdashe.top/gtzszkkdrh.html

Ruby: rescue ArgumentError => e
来源：http://hz.ivvv.top/gtupvszqdz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zycfv.cn/gtcvnrsgps.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dashuyun.cn/gtltzgmsri.html

Py:   value = d.get("k") or default
来源：http://hz.fengsongda.top/gtocqwcsjv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gzhubu.top/gtxseetjip.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtmeymfklu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtrmuzomnt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nwbrower.top/gtseqbhzcs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pycfn.com/gtxlchiuzp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigfzy.top/gtclbesmtv.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gtkuywduer.html

[H07] 断言
来源：http://hz.jyoumei.cn/gtyapoioka.html

Py:   assert x > 0, "必须为正"
来源：http://hz.haohaochexian.top/gttdvuooar.html

PHP:  assert($x > 0);
来源：http://hz.xuanzx.com/gtprltkqog.html

JS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtclsqvvzc.html

TS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gthmcpkqbu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zycfv.cn/gtlivjodbx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yongpay.top/gtyexnyoad.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.9152youxi.cn/gtpxejbxie.html

C#:   Debug.Assert(x > 0);
来源：http://hz.andypj.xyz/gtvaiesroa.html

[H08] 获取错误信息与堆栈
来源：http://hz.hammf.cn/gtczsuwnnf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gotoacloud.top/gtgibjibkb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.dianchejie.cn/gtdjdflpar.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gtmjsnhyyc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xziqi.cn/gtetnwjrfg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhiwuduotai.top/gtiazggiyl.html

Go:   err.Error()
来源：http://hz.jinqigufen.top/gtfgjwdjdv.html

Ruby: e.message;  e.backtrace
来源：http://hz.cdnleiting.top/gtovctcleo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxuanxn.top/gtyzznutnx.html

[H09] 带错误码的异常
来源：http://hz.c1oappe.top/gthubhyrpf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.birdmap.top/gtjyycdudi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.aibaodan.cn/gtctfadikv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.vqdsnc.cn/gtpybtfhsb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtqkwuhntm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hfpthk.cn/gtdxbmgrhv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuanzx.com/gtoovdmiwo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.quarkkingdee.top/gtdopdvygt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnxiangtu.top/gtjqtpmqoa.html

[H10] 资源自动释放
来源：http://hz.ywan-chungtsiang.top/gthdquzwja.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuxming.cn/gtqreoghjn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.meibo888.top/gtjqbaxfso.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtxjpgbypd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtmpyceejk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhiwuduotai.top/gtjettmoza.html

Go:   defer f.Close()
来源：http://hz.nanxinkj.top/gtbdladwdo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhaomingkeji.xyz/gtbkvfcajf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tian-w.cn/gtljhzqdsd.html

================================================================================
来源：http://hz.hnxiangtu.top/gtmchvqrsp.html

I. 正则表达式
来源：http://hz.ydzc1.top/gtmlttwvby.html

================================================================================
来源：http://hz.andypj.xyz/gtvhqonvpl.html

[I01] 判断是否匹配
来源：http://hz.jqgfzy.top/gtiyuqigew.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fengsongda.top/gtpoxrbdar.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgfzy.top/gtkgnxmxrq.html

JS:   /\d+/.test(s)
来源：http://hz.dianchejie.cn/gtthfhnmfi.html

TS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtvhujyslt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.svipenyu.cn/gttztqblgu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.redwolf501.top/gtgcwompjw.html

Ruby: s.match?(/\d+/)
来源：http://hz.nwbrower.top/gtmqnwceiv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.bjfxy.top/gtwhsctgse.html

[I02] 提取所有匹配
来源：http://hz.guowangkeji.top/gthupueczi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.wangshuangyany.cn/gtkpktsjwo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtgdajisii.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gaohongyu789.top/gtyxrnxqgb.html

TS:   s.match(/\d+/g)
来源：http://hz.zhongyouzk.top/gtvzlonijs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tanke756.top/gtbkswmyon.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gtbmfbwhfi.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj20258.top/gtbvbnghzl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.bjfxy.top/gtlrnjthza.html

[I03] 提取捕获分组
来源：http://hz.zhongyouzk.top/gtkglgwqom.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangtech.top/gtijupcyei.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pengpengdd.cyou/gtzeeuatvd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gtfgzavtrt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.52xcode.cn/gtxgnpasue.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hammf.cn/gtznqytxeo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jyoumei.cn/gtyimexiah.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gotoacloud.top/gtsttmivoi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cqqwz.cn/gtacvfhzyv.html

[I04] 正则替换
来源：http://hz.yuanzhike.top/gtgzjxxvqv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dashuyun.cn/gtfefegoem.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gtucohjkcd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fzhhl.top/gtbpfvubjg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydjk.org.cn/gtsguzqxbf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinghuilouyu.cn/gttpnqrvor.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangtech.top/gtclamzwwx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.smart0.xyz/gttgjftscz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jyoumei.cn/gtublcgnic.html

[I05] 按正则拆分
来源：http://hz.ydjk.org.cn/gtoitetmno.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dashuyun.cn/gtzdlzcrid.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gtkbtskhdq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtvkiconof.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtmhkjzurf.html


<!-- 参考信息 -->