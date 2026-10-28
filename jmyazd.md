代发 wailian999

TS:   constructor(public name: string) {}
来源：http://hz.jqgufenzy.top/gtzkdtmazk.html

Java: User(String name) { this.name = name; }
来源：http://hz.smart0.xyz/gtnxormzji.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangdashe.top/gtsufieawl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gtfslnjzvd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shuidangran.top/gtvbrpcyzp.html

[G03] 实例属性
来源：http://hz.xuetiantiany.cn/gtmqofccwi.html

Py:   self.name = "x"
来源：http://hz.sweek.top/gtpnljoyuv.html

PHP:  public string $name = "x";
来源：http://hz.cdnleiting.top/gtvgcpdxtk.html

JS:   this.name = "x";
来源：http://hz.hongshengwenyu.top/gtutcdhttn.html

TS:   name: string = "x";
来源：http://hz.redwolf501.top/gtaqdxwutu.html

Java: private String name;
来源：http://hz.wangdashe.top/gtnyegxjwt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jqgufenzy.top/gtplanrfwk.html

Ruby: @name = "x"
来源：http://hz.fengsongda.top/gtcuuverlh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yonumen.top/gttreletad.html

[G04] 定义方法
来源：http://hz.jyoumei.cn/gtupnyobee.html

Py:   def greet(self): return self.name
来源：http://hz.yonumen.top/gtupoxykwd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sweek.top/gtugkxiqzd.html

JS:   greet() { return this.name; }
来源：http://hz.quarkkingdee.top/gtbkknxssx.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuanzhike.top/gtxvgykedh.html

Java: String greet() { return name; }
来源：http://hz.chenjidiqi.icu/gtkeilqpzl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yangfankeji.com/gtwvxtddbi.html

Ruby: def greet; @name; end
来源：http://hz.dashuyun.cn/gtootierfy.html

C#:   public string Greet() => Name;
来源：http://hz.c1oappe.top/gtcvadngyc.html

[G05] 继承
来源：http://hz.yuxming.cn/gtegtgxeoi.html

Py:   class Admin(User): pass
来源：http://hz.gzhubu.top/gtptjvpren.html

PHP:  class Admin extends User {}
来源：http://hz.yangfankeji.com/gtntlltkjb.html

JS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtgizksled.html

TS:   class Admin extends User {}
来源：http://hz.dashuyun.cn/gtdflijpgz.html

Java: class Admin extends User {}
来源：http://hz.gogol.net.cn/gtlzuemvac.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.iojbl.cn/gtnuoqzjdo.html

Ruby: class Admin < User; end
来源：http://hz.kuanghao11.cn/gtjrnljhed.html

C#:   class Admin : User {}
来源：http://hz.gotoacloud.top/gtwxxfrhhv.html

[G06] 重写方法
来源：http://hz.zhengqikj.top/gtoimoqgoo.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigufen.top/gtbvkfcram.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gtkhoflwtg.html

JS:   greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gtshkhilwd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtoyiygcdd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gteonkkuld.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xziqi.cn/gtanfjieqk.html

Ruby: def greet; "admin"; end
来源：http://hz.cqqwz.cn/gtbxqyrawk.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtodcfknlg.html

[G07] 调用父类方法
来源：http://hz.xylfe.cn/gtgpgywnuc.html

Py:   super().greet()
来源：http://hz.c1oappe.top/gtmiyqlxuo.html

PHP:  parent::greet();
来源：http://hz.zhoulong.xyz/gtpdzinztk.html

JS:   super.greet();
来源：http://hz.shzxlz.cn/gtpggomqpe.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtbvzibrgq.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtiqfkwaiu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shuidangran.top/gtjoacqbvo.html

Ruby: super
来源：http://hz.9152youxi.cn/gtefvdvrct.html

C#:   base.Greet();
来源：http://hz.jinqigfzy.top/gtrudcczwy.html

[G08] 静态方法与属性
来源：http://hz.sxryk.cn/gtdjvbdkkh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhiwuduotai.top/gthczxvsxi.html

PHP:  public static function f() {}
来源：http://hz.ivvv.top/gtuznebmao.html

JS:   static f() {}
来源：http://hz.sweek.top/gtydsxmwlj.html

TS:   static f(): void {}
来源：http://hz.hfpthk.cn/gttnfpqkca.html

Java: static void f() {}
来源：http://hz.fengsongda.top/gtiegwupsv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj202588.top/gtfgslmpta.html

Ruby: def self.f; end
来源：http://hz.hnxiangtu.top/gtxiuwrxgl.html

C#:   public static void F() {}
来源：http://hz.c1oappe.top/gtmowqweoa.html

[G09] 接口 / 抽象类
来源：http://hz.yonumen.top/gtcmdbnxny.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xingfuxueyuan.xyz/gtnsyfbuhs.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hfpthk.cn/gtikckuuwo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhoulong.xyz/gtkcynskft.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigufen.top/gtrzfhhvji.html

Java: interface Shape { double area(); }
来源：http://hz.fengsongda.top/gtxcgdhnxi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhongyouzk.top/gtrvgpkbyu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sweek.top/gtpgpggiwl.html

C#:   interface IShape { double Area(); }
来源：http://hz.smart0.xyz/gthavkezyd.html

[G10] 访问控制
来源：http://hz.nanxinkj.top/gtkhhavdqz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.0kj1m.cn/gtnwfmdeuj.html

PHP:  public / protected / private
来源：http://hz.nanxuanxn.top/gtqtrubnie.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258888.top/gtrbvgfoie.html

TS:   public / protected / private
来源：http://hz.ppjwa.cn/gtcizqsbzl.html

Java: public / protected / private / 默认包级
来源：http://hz.svipenyu.cn/gtwczznijw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhoulong.xyz/gtndkujefa.html

Ruby: public / protected / private
来源：http://hz.smart0.xyz/gtrljvmsmp.html

C#:   public / protected / private / internal
来源：http://hz.zhaomingkeji.xyz/gtihjowbcn.html

[G11] getter / setter
来源：http://hz.gzhubu.top/gteikfcpxd.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtyfkiqqlo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtbszblqkn.html

JS:   get name() { return this._name; }
来源：http://hz.jyoumei.cn/gtqcgrqted.html

TS:   get name(): string { return this._name; }
来源：http://hz.yonumen.top/gtyjhzhrbn.html

Java: public String getName() { return name; }
来源：http://hz.chenzaomai.com/gtrdmyspuq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtsalflxvr.html

Ruby: attr_accessor :name
来源：http://hz.xziqi.cn/gtsmygovnv.html

C#:   public string Name { get; set; }
来源：http://hz.yangfankeji.com/gtlooqsztn.html

[G12] 对象转字符串
来源：http://hz.jinqigufen.top/gtwjbknrgq.html

Py:   def __str__(self): return self.name
来源：http://hz.hongshengwenyu.top/gtethaulqi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtgmjaywna.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtkxgbalxf.html

TS:   toString(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gtioaljiwd.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhiwuduotai.top/gtmkdwumjw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuanzx.com/gtthywfrmi.html

Ruby: def to_s; @name; end
来源：http://hz.jqgfzy.top/gthvcusvcp.html

C#:   public override string ToString() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtctkkcsml.html

[G13] 判断对象类型
来源：http://hz.mhx1999.top/gtnzcjslml.html

Py:   isinstance(u, User)
来源：http://hz.fzhhl.top/gtbdyhpdes.html

PHP:  $u instanceof User
来源：http://hz.guannengcc.top/gtepkwkutz.html

JS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtujofzaqt.html

TS:   u instanceof User
来源：http://hz.meibo888.top/gtgwxierbw.html

Java: u instanceof User
来源：http://hz.dianchejie.cn/gthdmtwmvl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yanxiufei.cn/gtdxaffhky.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtbdptfpbi.html

C#:   u is User
来源：http://hz.xingfuxueyuan.xyz/gtrtvrivep.html

[G14] 数据类 / record
来源：http://hz.cashguo.top/gtrcvoibcm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhongyouzk.top/gtrsmuphdj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ivvv.top/gtwlovrfju.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yangfankeji.com/gtemwdwjyz.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinghuilouyu.cn/gtvkhdemue.html

Java: record User(String name, int age) {}
来源：http://hz.meibo888.top/gtlaphcnck.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hammf.cn/gthlfnzsnh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gotoacloud.top/gtbmirgoly.html

C#:   record User(string Name, int Age);
来源：http://hz.ydjk.org.cn/gtdbqixjdq.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtgvmiesnk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zycfv.cn/gtqovgbtkh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.feifeiyinyue.top/gtpouxkyhc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.daria6918.cn/gtmxgalxxi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtnnlosmwq.html

Java: enum Color { RED, GREEN }
来源：http://hz.ybcxt.top/gtkafwmgev.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cdnleiting.top/gtcemqwtbz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ehwqpu.com/gtzcecodyy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gttmlppoke.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gtgwwvapzb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinqigfzy.top/gtjbqsndek.html

PHP:  get_object_vars($obj);
来源：http://hz.52xcode.cn/gtudsieykq.html

JS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gtbhcnxrja.html

TS:   Object.entries(obj)
来源：http://hz.feifeiyinyue.top/gtiptqmjsl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgfzy.top/gtnqeeucao.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yonumen.top/gtooprqkzg.html

Ruby: obj.instance_variables
来源：http://hz.c1oappe.top/gteqbngyeu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dashuyun.cn/gtwsqrnbsx.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtkdvhlpkg.html

H. 异常与错误处理
来源：http://hz.zhongyouzk.top/gtfgibamsd.html

================================================================================
来源：http://hz.daxiang520.top/gteetsiocp.html

[H01] try / catch 基础
来源：http://hz.daria6918.cn/gthylthziu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhengqikj.top/gtoclkvoja.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hammf.cn/gtsyfudzfv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.havefunace.top/gtlmiryvhr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shuidangran.top/gtdvfjsquc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shangyingyoupin.top/gtlpumqcsw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shanyushiyangtech.top/gtqhqbbzkz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xuanzx.com/gtxmzzqgtd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gtgepwlzts.html

[H02] finally / ensure 收尾
来源：http://hz.chenlongwang.top/gtzpwcsbso.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aibaodan.cn/gthjbngvkd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtnujcsdhj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtitajyzxj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtqnuonpkc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtozxabxrj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangdashe.top/gtuobcqngh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.iojbl.cn/gtxitvtwlo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ybcxt.top/gtsirgvihx.html

[H03] 主动抛出异常
来源：http://hz.havefunace.top/gtfiqjhosa.html

Py:   raise ValueError("错误信息")
来源：http://hz.yueranfly.top/gthtqhjtap.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtgdzzfreb.html

JS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gtgdzdukes.html

TS:   throw new Error("错误信息");
来源：http://hz.zhongyouzk.top/gtusqjbrjv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtqygydeph.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.feifeiyinyue.top/gtecwxcems.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.iojbl.cn/gtjzjtsigc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258.top/gtfzkmiwjg.html

[H04] 自定义异常类型
来源：http://hz.cqqwz.cn/gtwosdpwpl.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258.top/gtmwmpyedb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sweek.top/gtiigxmdjr.html

JS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtbefhmrvo.html

TS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gtajlsxqws.html

Java: class MyException extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtavxvcqlo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tian-w.cn/gtcbnrwnjr.html

Ruby: class MyError < StandardError; end
来源：http://hz.meibo888.top/gtqxvgjsiw.html

C#:   class MyException : Exception {}
来源：http://hz.9152youxi.cn/gtnikqfsxr.html

[H05] 捕获特定类型
来源：http://hz.quarkkingdee.top/gteliqjwng.html

Py:   except ValueError as e:
来源：http://hz.zhiwuduotai.top/gtjdxwgybk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jiagoushi.top/gtetaqicwj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.meibo888.top/gtkwblwumb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtaxzfoclu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gttmmtqeaf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ehwqpu.com/gttafsmilj.html

Ruby: rescue ArgumentError => e
来源：http://hz.aizwys.cn/gttomtptnf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tianlin.xyz/gtjlgzkcfx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guowangkeji.top/gtqkncupvf.html

Py:   value = d.get("k") or default
来源：http://hz.cdnleiting.top/gtduowztgc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gtqgsvermz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtiqcnszja.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gtegdosaix.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtwrfjjfub.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cheryme.top/gtfdqzjaav.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jianghu66.top/gtcrjkuzph.html

C#:   obj?.A?.B ?? default
来源：http://hz.sweek.top/gthoiervhu.html

[H07] 断言
来源：http://hz.svipenyu.cn/gtunvfucqz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shanyushiyangkeji.top/gtziahemez.html

PHP:  assert($x > 0);
来源：http://hz.ybcxt.top/gtvnlsirec.html

JS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtwhytamxw.html

TS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtvqirkblm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.redwolf501.top/gtoejozvpv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenlongwang.top/gtihvztcug.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xingfuxueyuan.xyz/gtwpwjputi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.haohaochexian.top/gtxzwkjhjm.html

[H08] 获取错误信息与堆栈
来源：http://hz.sxryk.cn/gtmhehoedt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guannengcc.top/gtwqscvhnx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yanxiufei.cn/gtdxljdyiy.html

JS:   e.message;  e.stack
来源：http://hz.mhx1999.top/gtuuiayoxv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hysaishi.cn/gtvfxtipxh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinqigufen.top/gtxrtomzbc.html

Go:   err.Error()
来源：http://hz.iojbl.cn/gtyvroundu.html

Ruby: e.message;  e.backtrace
来源：http://hz.jyoumei.cn/gtwoyoqhna.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xylfe.cn/gtvxpkqakz.html

[H09] 带错误码的异常
来源：http://hz.xuetiantiany.cn/gtscgtsxzj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhixingplan.top/gtgemamdvm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangkeji.top/gtpglpstup.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sweek.top/gtrqhuhjib.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnqzz.top/gtmqdizuxl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhijiandao.cn/gtmbcpotld.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.meibo888.top/gtnixaextj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.havefunace.top/gttrutnzjz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.birdmap.top/gthlmxnebi.html

[H10] 资源自动释放
来源：http://hz.aibaodan.cn/gtvxwzgrmv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.feifeiyinyue.top/gtevlvjzjp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ivvv.top/gtdysblgfz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gaohongyu789.top/gtwkurdusu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtdfdizuel.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gtkrtjajgw.html

Go:   defer f.Close()
来源：http://hz.hammf.cn/gtizkwefjm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhiwuduotai.top/gtfjpnfsbk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sweek.top/gtdeyegffs.html

================================================================================
来源：http://hz.havefunace.top/gtljsrnydl.html

I. 正则表达式
来源：http://hz.tianlin.xyz/gtjkawcnwy.html

================================================================================
来源：http://hz.yueranfly.top/gtggordwob.html

[I01] 判断是否匹配
来源：http://hz.fzhhl.top/gtxyeyryft.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.smart0.xyz/gtsxlzmtvh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.vqdsnc.cn/gtuqpwaaly.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtslbvclsd.html

TS:   /\d+/.test(s)
来源：http://hz.mhx1999.top/gtwvlyuedc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.iojbl.cn/gtkyqpshio.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.kuanghao11.cn/gtladswowf.html

Ruby: s.match?(/\d+/)
来源：http://hz.52xcode.cn/gtzqwromix.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cheryme.top/gtaksonyiw.html

[I02] 提取所有匹配
来源：http://hz.fengsongda.top/gtwilbqrgh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.wangshuangyany.cn/gtsgrhtslf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtdzjuidbi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhijiandao.cn/gtplbtupzz.html

TS:   s.match(/\d+/g)
来源：http://hz.shuidangran.top/gtlcerbewf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gotoacloud.top/gttfubqtmd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenlongwang.top/gtoylkqaww.html

Ruby: s.scan(/\d+/)
来源：http://hz.guowangkeji.top/gtgiogloih.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinyuanbaomall.cn/gtkgmswics.html

[I03] 提取捕获分组
来源：http://hz.yuanzhike.top/gtgrelowwb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gtjgpfpvzn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daxiang520.top/gtlooxausy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhengqikj.top/gtstxntxch.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangshuangyany.cn/gtikbdcxvt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgfzy.top/gtdnpduvlv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tanke756.top/gtsmvzdaiv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pengpengdd.cyou/gtypakvgsu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuanzx.com/gtbzprxirg.html

[I04] 正则替换
来源：http://hz.cashguo.top/gtilhdhgsm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.snrcjt.cn/gthtfytcsq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtywrxhelv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtjaewlugj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gtcvamrnfn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hywenlv.cn/gtrxlqknfi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shangyingyoupin.top/gtewflqsxv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgufenzy.top/gttvmwphtm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.birdmap.top/gtrkesixjf.html

[I05] 按正则拆分
来源：http://hz.gogol.net.cn/gtbmmukevd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258888.top/gtnqcpvwdy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.havefunace.top/gthflhhygt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtwfxvbecb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtzbnbthfl.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zdqjudy.top/gtmoxnalam.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guannengcc.top/gttwowonae.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtbyxbgwtg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gzhubu.top/gtbglqwbvy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ybcxt.top/gtqiwedjlp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtdopkefvj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.52xcode.cn/gtzsbmcnvq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.52xcode.cn/gtecixsraw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gtzrowgtfk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.havefunace.top/gtybghbpiz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cqqwz.cn/gtguliovav.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ppjwa.cn/gtwtgzjtwb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gtydlyfkex.html

[I07] 忽略大小写与多行模式
来源：http://hz.hongshengwenyu.top/gtltygppdp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nwbrower.top/gtctvorork.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.wangshuangyany.cn/gtlpdsfbhd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aibaodan.cn/gtpxarkkfn.html

TS:   /error/gim
来源：http://hz.zhixingplan.top/gtaruhxzzo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.haohaochexian.top/gtewqbuncx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cheryme.top/gtgrkbqrma.html

Ruby: s.scan(/error/i)
来源：http://hz.fengsongda.top/gtywvvioun.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hnqzz.top/gtywvdkotg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.0kj1m.cn/gtsgezmlmt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.52xcode.cn/gtknduovjp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.bjfxy.top/gtwlbndowi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtxdbddmtv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtrzlfdiku.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jianghu66.top/gtokqjfgva.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.c1oappe.top/gtmcdhppyz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yangfankeji.com/gtkuuegktz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtfhwlfdks.html

================================================================================
来源：http://hz.ppjwa.cn/gtffxkgcvj.html


<!-- 参考信息 -->