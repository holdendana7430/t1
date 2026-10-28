代发 wailian999

Java: class User {}
来源：http://hz.hfpthk.cn/gtfzroutgf.html

Go:   type User struct { Name string }
来源：http://hz.jinghuilouyu.cn/gtczlzafyt.html

Ruby: class User; end
来源：http://hz.nanxinkj.top/gtofxkzccr.html

C#:   class User {}
来源：http://hz.dianchejie.cn/gtpkuzidpl.html

[G02] 构造函数
来源：http://hz.zhengqikj.top/gtlgazshzk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuetiantiany.cn/gtoyhtgsga.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shangyingyoupin.top/gtmjeoualk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.svipenyu.cn/gtfatcvclb.html

TS:   constructor(public name: string) {}
来源：http://hz.xylfe.cn/gtyrtvrftw.html

Java: User(String name) { this.name = name; }
来源：http://hz.birdmap.top/gtbxyovdqf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jiagoushi.top/gtkcolcdyi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guannengcc.top/gtjzgxvlbt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ppjwa.cn/gtngsmhbhu.html

[G03] 实例属性
来源：http://hz.hnxiangtu.top/gtbeyejytr.html

Py:   self.name = "x"
来源：http://hz.hfpthk.cn/gtxkgpniee.html

PHP:  public string $name = "x";
来源：http://hz.yueranfly.top/gtwfufwtps.html

JS:   this.name = "x";
来源：http://hz.cqqwz.cn/gtoijknuya.html

TS:   name: string = "x";
来源：http://hz.fengsongda.top/gthaualhkn.html

Java: private String name;
来源：http://hz.chenzaomai.com/gtkafuoymg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.birdmap.top/gtezjjmkyr.html

Ruby: @name = "x"
来源：http://hz.xylfe.cn/gteqhwznuw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj202588.top/gtfthwvwlk.html

[G04] 定义方法
来源：http://hz.yongpay.top/gtcvsngmrx.html

Py:   def greet(self): return self.name
来源：http://hz.pengpengdd.cyou/gtxllivans.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtiiblnkjt.html

JS:   greet() { return this.name; }
来源：http://hz.snrcjt.cn/gtghnnqxnw.html

TS:   greet(): string { return this.name; }
来源：http://hz.hammf.cn/gtopmztkgg.html

Java: String greet() { return name; }
来源：http://hz.yangfankeji.com/gtwowwlvgq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guannengcc.top/gtxfsgkczh.html

Ruby: def greet; @name; end
来源：http://hz.0kj1m.cn/gtmaeqienu.html

C#:   public string Greet() => Name;
来源：http://hz.ehwqpu.com/gtprkupydq.html

[G05] 继承
来源：http://hz.meibo888.top/gtbchipexg.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gtmjdaytxv.html

PHP:  class Admin extends User {}
来源：http://hz.svipenyu.cn/gtbtowacvk.html

JS:   class Admin extends User {}
来源：http://hz.cashguo.top/gtejzbdynj.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtjwoccbnu.html

Java: class Admin extends User {}
来源：http://hz.hywenlv.cn/gtjhgenvtu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydzc1.top/gtkdsoqcbx.html

Ruby: class Admin < User; end
来源：http://hz.yongpay.top/gtioockwgk.html

C#:   class Admin : User {}
来源：http://hz.kuanghao11.cn/gtadrsxvqv.html

[G06] 重写方法
来源：http://hz.vqdsnc.cn/gtczlzzyih.html

Py:   def greet(self): return "admin"
来源：http://hz.daxiang520.top/gthyhlwxqt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtswivkhzk.html

JS:   greet() { return "admin"; }
来源：http://hz.cucudq.cn/gteiqogeyb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gttnbvusxj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtzxnazjaw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.kuanghao11.cn/gtpaqgesid.html

Ruby: def greet; "admin"; end
来源：http://hz.kuanghao11.cn/gtudbhndou.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenlongwang.top/gtiekotjnk.html

[G07] 调用父类方法
来源：http://hz.wangshuangyany.cn/gtgdbqdqfy.html

Py:   super().greet()
来源：http://hz.zycfv.cn/gttmqsbtrm.html

PHP:  parent::greet();
来源：http://hz.xziqi.cn/gtctgzbqcs.html

JS:   super.greet();
来源：http://hz.chenjidiqi.icu/gtcisljebw.html

TS:   super.greet();
来源：http://hz.sweek.top/gtousdlpku.html

Java: super.greet();
来源：http://hz.birdmap.top/gtqujhtkcs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.mhx1999.top/gtesiscssc.html

Ruby: super
来源：http://hz.chenlongwang.top/gtruhjkygw.html

C#:   base.Greet();
来源：http://hz.gaohongyu789.top/gtipgpmezu.html

[G08] 静态方法与属性
来源：http://hz.nanxuanxn.top/gtkwfjmfmx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydjk.org.cn/gtvevpzaxi.html

PHP:  public static function f() {}
来源：http://hz.jlsjyb.cn/gtpppmqiur.html

JS:   static f() {}
来源：http://hz.shanyushiyangtech.top/gteylpiylt.html

TS:   static f(): void {}
来源：http://hz.hammf.cn/gtffjzkhzw.html

Java: static void f() {}
来源：http://hz.redwolf501.top/gtqaruyeko.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hfpthk.cn/gtkfcgexlg.html

Ruby: def self.f; end
来源：http://hz.ybcxt.top/gtkbeasyrf.html

C#:   public static void F() {}
来源：http://hz.jyoumei.cn/gtsdgkhkss.html

[G09] 接口 / 抽象类
来源：http://hz.chenjidiqi.icu/gtnodfckqt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xinyue.icu/gtmoemflrx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.aibaodan.cn/gtlgiwimfy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dianchejie.cn/gtnmsdtwxj.html

TS:   interface Shape { area(): number; }
来源：http://hz.zdqjudy.top/gtsyrjepjx.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtugkdqaie.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.c1oappe.top/gtjhvaeaav.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhixingplan.top/gtrflkixmd.html

C#:   interface IShape { double Area(); }
来源：http://hz.tanke756.top/gtnemiiqbv.html

[G10] 访问控制
来源：http://hz.tanke756.top/gttevipghs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.wangshuangyany.cn/gtybjgvfbo.html

PHP:  public / protected / private
来源：http://hz.hfpthk.cn/gtbnsaxzfz.html

JS:   #private 字段；其余公开
来源：http://hz.pengpengdd.cyou/gtlbckkclr.html

TS:   public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtlmqdewkg.html

Java: public / protected / private / 默认包级
来源：http://hz.jinyuanbaomall.cn/gtmggicinx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gtuvtuzbcp.html

Ruby: public / protected / private
来源：http://hz.zycfv.cn/gtdfefscuq.html

C#:   public / protected / private / internal
来源：http://hz.ehwqpu.com/gtalzcoxel.html

[G11] getter / setter
来源：http://hz.dashuyun.cn/gtrhrtwunz.html

Py:   @property 与 @x.setter
来源：http://hz.sweek.top/gtvmaqzwis.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.316326.xyz/gtwhsrwlxb.html

JS:   get name() { return this._name; }
来源：http://hz.xuanzx.com/gtqjjgxgha.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gtvlogotii.html

Java: public String getName() { return name; }
来源：http://hz.daxiang520.top/gtndeoznnp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtsrcqhnax.html

Ruby: attr_accessor :name
来源：http://hz.zhoulong.xyz/gtxymrthsj.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigufen.top/gtxrickmbd.html

[G12] 对象转字符串
来源：http://hz.sysykeji.top/gtuaimlomx.html

Py:   def __str__(self): return self.name
来源：http://hz.guannengcc.top/gtleczeuqm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtmbokqftp.html

JS:   toString() { return this.name; }
来源：http://hz.hfpthk.cn/gteiizmiev.html

TS:   toString(): string { return this.name; }
来源：http://hz.redwolf501.top/gtejjegupc.html

Java: @Override public String toString() { return name; }
来源：http://hz.yongpay.top/gtzdmrgcnd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ybcxt.top/gtlgtzaclo.html

Ruby: def to_s; @name; end
来源：http://hz.redwolf501.top/gtzuearcyv.html

C#:   public override string ToString() => Name;
来源：http://hz.yonumen.top/gtebbnecwz.html

[G13] 判断对象类型
来源：http://hz.hongshengwenyu.top/gtwnwqguvr.html

Py:   isinstance(u, User)
来源：http://hz.dashuyun.cn/gttzxdxztl.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtkpzpbgjq.html

JS:   u instanceof User
来源：http://hz.jqgfzy.top/gtzbrsktsy.html

TS:   u instanceof User
来源：http://hz.iojbl.cn/gtejuhmrhp.html

Java: u instanceof User
来源：http://hz.snrcjt.cn/gtgltgoylt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daria6918.cn/gtdocwuecv.html

Ruby: u.is_a?(User)
来源：http://hz.zhaomingkeji.xyz/gtonqllhiz.html

C#:   u is User
来源：http://hz.chenzaomai.com/gtsgfhkoib.html

[G14] 数据类 / record
来源：http://hz.zhaomingkeji.xyz/gtaotbbfxh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhijiandao.cn/gtrsuzgvxl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aizwys.cn/gttzbqsdbq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xinyue.icu/gtvelknuvy.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenzaomai.com/gtyjuqpfec.html

Java: record User(String name, int age) {}
来源：http://hz.quarkkingdee.top/gtuhbyokig.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nwbrower.top/gtwessxcmm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gogol.net.cn/gtuttrqwok.html

C#:   record User(string Name, int Age);
来源：http://hz.0kj1m.cn/gtfhmcesjd.html

[G15] 枚举
来源：http://hz.ydzc1.top/gttayqwpff.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xinyue.icu/gtiggbqwid.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gogol.net.cn/gtuvyxboih.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ywan-chungtsiang.top/gthpfcwmpc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtbhudfotk.html

Java: enum Color { RED, GREEN }
来源：http://hz.hysaishi.cn/gthkrikgky.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pycfn.com/gtyegmcuoy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhiwuduotai.top/gtfcgbgufy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtizgymuoc.html

[G16] 对象转数组 / 字典
来源：http://hz.iojbl.cn/gtbscxxnri.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shangyingyoupin.top/gtoxzltlre.html

PHP:  get_object_vars($obj);
来源：http://hz.dianchejie.cn/gtacrauerd.html

JS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtidwkzwvk.html

TS:   Object.entries(obj)
来源：http://hz.vqdsnc.cn/gtyxeqzdds.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.quarkkingdee.top/gthjezhgdj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenjidiqi.icu/gteemjzzcp.html

Ruby: obj.instance_variables
来源：http://hz.pengpengdd.cyou/gthyjgjefh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fengsongda.top/gtqooxpvbx.html

================================================================================
来源：http://hz.mhx1999.top/gtpspdxdqm.html

H. 异常与错误处理
来源：http://hz.9152youxi.cn/gtnvbiyjxn.html

================================================================================
来源：http://hz.fzhhl.top/gtatjfchgi.html

[H01] try / catch 基础
来源：http://hz.guowangkeji.top/gtidykgcfn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.quarkkingdee.top/gtzgjboklk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinyuanbaomall.cn/gtvgzwvgwo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.0kj1m.cn/gtglmqtpkd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.havefunace.top/gtcolksumy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxuanxn.top/gtwtvfaevz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tanke756.top/gtujfiowxj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.daria6918.cn/gtdeuksahf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ywan-chungtsiang.top/gtsycffsfb.html

[H02] finally / ensure 收尾
来源：http://hz.jianghu66.top/gtthctsjvd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.fengsongda.top/gtnomooins.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtgfqqdbfv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtcwqwbluc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtqukexbdu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtiggxajze.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhaomingkeji.xyz/gtsutmdqlu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnxiangtu.top/gtxvzqnfxv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xylfe.cn/gttlxtenqi.html

[H03] 主动抛出异常
来源：http://hz.nwbrower.top/gthuqwpgog.html

Py:   raise ValueError("错误信息")
来源：http://hz.svipenyu.cn/gtdjtvnegv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtdttfjkzg.html

JS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gthwxgnfay.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtzdxrvbua.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gaohongyu789.top/gtuajbjfgc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.birdmap.top/gthjwphrov.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.52xcode.cn/gtywqxfydy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtybhqqvga.html

[H04] 自定义异常类型
来源：http://hz.zycfv.cn/gtfwrmypyl.html

Py:   class MyError(Exception): pass
来源：http://hz.quarkkingdee.top/gthgwuizxq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtiqzpmieb.html

JS:   class MyError extends Error {}
来源：http://hz.cashguo.top/gtivtmwctc.html

TS:   class MyError extends Error {}
来源：http://hz.aizwys.cn/gtmpybeaxv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtjhmywqeu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jianghu66.top/gtytnvyxmg.html

Ruby: class MyError < StandardError; end
来源：http://hz.gaohongyu789.top/gtxxlzinpr.html

C#:   class MyException : Exception {}
来源：http://hz.nanxinkj.top/gtbzudujpy.html

[H05] 捕获特定类型
来源：http://hz.yuxming.cn/gtdnhrjrky.html

Py:   except ValueError as e:
来源：http://hz.feifeiyinyue.top/gtkmrcebhi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.birdmap.top/gtcpksvhnq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtjhgzrguq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cdnleiting.top/gtirgbihzb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gogol.net.cn/gtpaxqiyhs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.pengpengdd.cyou/gtqaieiqmp.html

Ruby: rescue ArgumentError => e
来源：http://hz.smart0.xyz/gtrvgpbwaj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tianlin.xyz/gtbegtuyen.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhixingplan.top/gtwvrvtsnb.html

Py:   value = d.get("k") or default
来源：http://hz.aizwys.cn/gtcvzworvl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gttdzyztth.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtezykjcnb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtsfgoufne.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuxming.cn/gtxxpwseec.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cqqwz.cn/gttuhbknoc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhijiandao.cn/gtyrbjdaqh.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtgmdlvnmk.html

[H07] 断言
来源：http://hz.jqgufenzy.top/gtzcdbpwez.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gzhubu.top/gteicqeycz.html

PHP:  assert($x > 0);
来源：http://hz.yvedp.cn/gtcbnlnhes.html

JS:   console.assert(x > 0);
来源：http://hz.sxryk.cn/gtmuefamhu.html

TS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gtyvnbwtpp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gogol.net.cn/gtejnohwjw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daxiang520.top/gtiwuzgdib.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.snrcjt.cn/gtqmpxaxpf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xinyue.icu/gtiagmxuuq.html

[H08] 获取错误信息与堆栈
来源：http://hz.hnqzz.top/gthywjkwfz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gogol.net.cn/gtpebiozds.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yangfankeji.com/gtrgcxcbkr.html

JS:   e.message;  e.stack
来源：http://hz.xinyue.icu/gtaihcvaph.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinghuilouyu.cn/gtorkzsxuj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.pengpengdd.cyou/gturxqrtul.html

Go:   err.Error()
来源：http://hz.jyoumei.cn/gtbehckskt.html

Ruby: e.message;  e.backtrace
来源：http://hz.tianlin.xyz/gtifuojjsh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj20258.top/gtinkjgixk.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gtwesaayof.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fzhhl.top/gtqfiouqbt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydzc1.top/gtvjnemosi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cqqwz.cn/gtbfeuoruz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.c1oappe.top/gtpqltjkzb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jlsjyb.cn/gtlppecqin.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.316326.xyz/gtznkugehx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jianghu66.top/gtokrvjssh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinghuilouyu.cn/gthjtabcje.html

[H10] 资源自动释放
来源：http://hz.haohaochexian.top/gtlkbjymli.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnxiangtu.top/gttwovqelx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hysaishi.cn/gtoxymqklc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtgejowmxm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cheryme.top/gtoblwdhrr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yueranfly.top/gtrgatvgwl.html

Go:   defer f.Close()
来源：http://hz.dashuyun.cn/gtrwtmbrcu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hywenlv.cn/gttgvezhph.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenzaomai.com/gtlfgazfxl.html

================================================================================
来源：http://hz.zhixingplan.top/gtuxnnaczf.html

I. 正则表达式
来源：http://hz.sysykeji.top/gtzkdjqkqi.html

================================================================================
来源：http://hz.chenlongwang.top/gteeobpggy.html

[I01] 判断是否匹配
来源：http://hz.yongpay.top/gtugdrkoua.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dianchejie.cn/gtxxwuauwc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258888.top/gtgznztxjt.html

JS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtztnmxbji.html

TS:   /\d+/.test(s)
来源：http://hz.zycfv.cn/gtvqtwmqye.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.mhx1999.top/gtrljiamcs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangdashe.top/gtgbvoreag.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgfzy.top/gtnxzknkvy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydjk.org.cn/gtlauisaha.html

[I02] 提取所有匹配
来源：http://hz.svipenyu.cn/gtafxlorhp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nwbrower.top/gtulffqoop.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ydzc1.top/gtulhjwdqn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.quarkkingdee.top/gtvhfvtwct.html

TS:   s.match(/\d+/g)
来源：http://hz.redwolf501.top/gtnqrjifyd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.birdmap.top/gtvnhujlma.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nwbrower.top/gtqxyjiiuy.html

Ruby: s.scan(/\d+/)
来源：http://hz.aizwys.cn/gtmaytokyk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shuidangran.top/gtzytirmgo.html

[I03] 提取捕获分组
来源：http://hz.hnqzz.top/gthmuztgkk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuanzhike.top/gtqvbgafzv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.quarkkingdee.top/gtzlzaljol.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shuidangran.top/gtbepsljql.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtzabkgbhh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yvedp.cn/gtjsmltnim.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zycfv.cn/gtvjmzksvm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xinyue.icu/gtvesnrwej.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgfzy.top/gtlqwfxzgd.html

[I04] 正则替换
来源：http://hz.havefunace.top/gtkowqfnqb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigufen.top/gtcyknnnbj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shuidangran.top/gtcabnujpo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.mhx1999.top/gtjiycybgb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtyhaxdveq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xylfe.cn/gtctzfpyat.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258888.top/gtvpkcsdln.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.feifeiyinyue.top/gtoiajdgck.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtlyktseeb.html

[I05] 按正则拆分
来源：http://hz.birdmap.top/gthgmdhsub.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sufxvd.cn/gtqvdwbgbp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ywan-chungtsiang.top/gtplljrbjb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtqqeqosku.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtnyduzuuy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhiwuduotai.top/gtzvdxyafr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydzc1.top/gtnczsiwkx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtmicrixsg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gtptyiugqg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuxming.cn/gtpjtdkxth.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhixingplan.top/gttsuiawcq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhongyouzk.top/gtxsmgywhp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtvqheohqg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtptksgsrk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258.top/gtwrwpaljw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ivvv.top/gtqjunjvoc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ppjwa.cn/gtvgneoiyt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtiohkdamz.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhiwuduotai.top/gtypetrkrl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.52xcode.cn/gthbsiajhb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gzhubu.top/gtjlucozcu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jianghu66.top/gtjddxgyac.html

TS:   /error/gim
来源：http://hz.xinyue.icu/gtootjccls.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yanxiufei.cn/gtbqrcpxae.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.guowangkeji.top/gtoqnrinvx.html

Ruby: s.scan(/error/i)
来源：http://hz.fzhhl.top/gtcgqftcoo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinghuilouyu.cn/gtaopgproe.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.9152youxi.cn/gtvoxlbmix.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yangfankeji.com/gtanpdpgiu.html


<!-- 参考信息 -->