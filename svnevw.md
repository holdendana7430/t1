代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://hz.zhijiandao.cn/gtbkmirkbd.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gtmnchkmhy.html

Py:   self.name = "x"
来源：http://hz.ybcxt.top/gtxjmdzkwa.html

PHP:  public string $name = "x";
来源：http://hz.shanyushiyangkeji.top/gtqvigdvxw.html

JS:   this.name = "x";
来源：http://hz.zhongyouzk.top/gtdakrzgll.html

TS:   name: string = "x";
来源：http://hz.xuanzx.com/gthzogpoel.html

Java: private String name;
来源：http://hz.zhijiandao.cn/gtxeegittg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.0kj1m.cn/gtjqyhvtzy.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtrxxcnjpt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hysaishi.cn/gtarniqecj.html

[G04] 定义方法
来源：http://hz.zhengqikj.top/gtsrccspdz.html

Py:   def greet(self): return self.name
来源：http://hz.yangfankeji.com/gtgijwpvnx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtvfrzxxsk.html

JS:   greet() { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtobkyjyfk.html

TS:   greet(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtodjhxxzv.html

Java: String greet() { return name; }
来源：http://hz.smart0.xyz/gtzjtxqpht.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenlongwang.top/gtxkdpvtnw.html

Ruby: def greet; @name; end
来源：http://hz.zhongyouzk.top/gtygpswfgk.html

C#:   public string Greet() => Name;
来源：http://hz.316326.xyz/gtoyplmdcj.html

[G05] 继承
来源：http://hz.yj20258888.top/gtywngwova.html

Py:   class Admin(User): pass
来源：http://hz.jlsjyb.cn/gtsojbsrdg.html

PHP:  class Admin extends User {}
来源：http://hz.zhixingplan.top/gtuyhcwvte.html

JS:   class Admin extends User {}
来源：http://hz.yj20258.top/gtcmelnwuo.html

TS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtcdkfjgrs.html

Java: class Admin extends User {}
来源：http://hz.birdmap.top/gtlhpwlsla.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.redwolf501.top/gtubpjpgzq.html

Ruby: class Admin < User; end
来源：http://hz.hongshengwenyu.top/gtwrebpnjk.html

C#:   class Admin : User {}
来源：http://hz.hnqzz.top/gtueuzwevw.html

[G06] 重写方法
来源：http://hz.ppjwa.cn/gtqkvgtpfo.html

Py:   def greet(self): return "admin"
来源：http://hz.daxiang520.top/gtinxjxtmb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtczrdjgar.html

JS:   greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtgebfjded.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtcywxhkle.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtpanvfyii.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cqqwz.cn/gtmctglxrd.html

Ruby: def greet; "admin"; end
来源：http://hz.316326.xyz/gtmtubpjha.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtqzrvgekt.html

[G07] 调用父类方法
来源：http://hz.zhengqikj.top/gtxdpjxfxo.html

Py:   super().greet()
来源：http://hz.jqgfzy.top/gtuvgukxja.html

PHP:  parent::greet();
来源：http://hz.vqdsnc.cn/gtfrubbqqe.html

JS:   super.greet();
来源：http://hz.smart0.xyz/gtdesxofyz.html

TS:   super.greet();
来源：http://hz.daxiang520.top/gtjxnmqkol.html

Java: super.greet();
来源：http://hz.yonumen.top/gtqcypgqfh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daria6918.cn/gtehgtuuoi.html

Ruby: super
来源：http://hz.xylfe.cn/gtykwmhyao.html

C#:   base.Greet();
来源：http://hz.316326.xyz/gtyhaqligk.html

[G08] 静态方法与属性
来源：http://hz.vqdsnc.cn/gtsvmdgdje.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhaomingkeji.xyz/gtgvpkrmyk.html

PHP:  public static function f() {}
来源：http://hz.jinghuilouyu.cn/gtxjjtgego.html

JS:   static f() {}
来源：http://hz.shanyushiyangkeji.top/gtyucmpzjl.html

TS:   static f(): void {}
来源：http://hz.quarkkingdee.top/gtvsohxtme.html

Java: static void f() {}
来源：http://hz.svipenyu.cn/gtknamjoyj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.0kj1m.cn/gtlimhyemm.html

Ruby: def self.f; end
来源：http://hz.tanke756.top/gtucggktbg.html

C#:   public static void F() {}
来源：http://hz.iojbl.cn/gteanabdwh.html

[G09] 接口 / 抽象类
来源：http://hz.aibaodan.cn/gthymkcyxf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ywan-chungtsiang.top/gtjsefvaud.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tianlin.xyz/gtqkanponl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xuanzx.com/gtypboahhx.html

TS:   interface Shape { area(): number; }
来源：http://hz.zdqjudy.top/gtdxgxjtgb.html

Java: interface Shape { double area(); }
来源：http://hz.svipenyu.cn/gtpibuuqsq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258.top/gtoaspbigs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fengsongda.top/gtjhcivycr.html

C#:   interface IShape { double Area(); }
来源：http://hz.dianchejie.cn/gtlcylkleq.html

[G10] 访问控制
来源：http://hz.gzhubu.top/gtqabgxgvl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nanxuanxn.top/gtluyijuwx.html

PHP:  public / protected / private
来源：http://hz.dashuyun.cn/gtpqvvyxok.html

JS:   #private 字段；其余公开
来源：http://hz.pycfn.com/gtdcmplcfg.html

TS:   public / protected / private
来源：http://hz.zhongyouzk.top/gtjvlqegfy.html

Java: public / protected / private / 默认包级
来源：http://hz.jianghu66.top/gtuyjxpfkg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nwbrower.top/gtgwwubelx.html

Ruby: public / protected / private
来源：http://hz.xuetiantiany.cn/gtsfzcelzo.html

C#:   public / protected / private / internal
来源：http://hz.jlsjyb.cn/gtoxrdrrjc.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtkpfhhoaa.html

Py:   @property 与 @x.setter
来源：http://hz.hywenlv.cn/gtxingkpte.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtdlkeffil.html

JS:   get name() { return this._name; }
来源：http://hz.wangshuangyany.cn/gtrfmramij.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258.top/gtmoanoamt.html

Java: public String getName() { return name; }
来源：http://hz.yanxiufei.cn/gtyivaistr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.iojbl.cn/gtpwhlsqtc.html

Ruby: attr_accessor :name
来源：http://hz.jinyuanbaomall.cn/gtepqujzgc.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtbkyfnknj.html

[G12] 对象转字符串
来源：http://hz.hnxiangtu.top/gtkdpmvphp.html

Py:   def __str__(self): return self.name
来源：http://hz.tanke756.top/gtrzuepgzk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gtremwyozz.html

JS:   toString() { return this.name; }
来源：http://hz.kuanghao11.cn/gtftokutss.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtnjokgvsv.html

Java: @Override public String toString() { return name; }
来源：http://hz.gzhubu.top/gtlekdpssz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtudahsace.html

Ruby: def to_s; @name; end
来源：http://hz.zhijiandao.cn/gtknkhztny.html

C#:   public override string ToString() => Name;
来源：http://hz.shuidangran.top/gthkutagwk.html

[G13] 判断对象类型
来源：http://hz.havefunace.top/gtulxofdoz.html

Py:   isinstance(u, User)
来源：http://hz.cashguo.top/gtnrzsxhuh.html

PHP:  $u instanceof User
来源：http://hz.mhx1999.top/gtjvmmkaah.html

JS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtwlmnlmnr.html

TS:   u instanceof User
来源：http://hz.guowangkeji.top/gtnfltiusn.html

Java: u instanceof User
来源：http://hz.jqgfzy.top/gtmjstqege.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.havefunace.top/gtzwumdabi.html

Ruby: u.is_a?(User)
来源：http://hz.nanxuanxn.top/gtczpcobfw.html

C#:   u is User
来源：http://hz.ivvv.top/gtbatbrraw.html

[G14] 数据类 / record
来源：http://hz.shzxlz.cn/gtidbukmag.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangdashe.top/gtnegdazrz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aibaodan.cn/gtnntxaswx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.feifeiyinyue.top/gthffpdjnx.html

TS:   type User = { name: string; age: number };
来源：http://hz.gogol.net.cn/gtgrntzddt.html

Java: record User(String name, int age) {}
来源：http://hz.hysaishi.cn/gtyybglrcx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxuanxn.top/gtfameaxyy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jyoumei.cn/gtrvksnuay.html

C#:   record User(string Name, int Age);
来源：http://hz.shzxlz.cn/gtgrgegxfu.html

[G15] 枚举
来源：http://hz.sxryk.cn/gtqibctkmt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shzxlz.cn/gtducjafvx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pengpengdd.cyou/gtwtybuglt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.smart0.xyz/gtgxfpeimd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guannengcc.top/gtyogmzdwi.html

Java: enum Color { RED, GREEN }
来源：http://hz.shzxlz.cn/gtmdcgfizl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhoulong.xyz/gtvmkeorxs.html

Ruby: Color = %i[red green].freeze
来源：http://hz.vqdsnc.cn/gtxmgyjbje.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sysykeji.top/gtolvdjxle.html

[G16] 对象转数组 / 字典
来源：http://hz.dianchejie.cn/gtkfojkjqt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guannengcc.top/gtfsnhhlfj.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigfzy.top/gtewzvrppv.html

JS:   Object.entries(obj)
来源：http://hz.jiagoushi.top/gtxbssmyui.html

TS:   Object.entries(obj)
来源：http://hz.redwolf501.top/gtwnqtmelh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.daria6918.cn/gthgvsgeyb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.bjfxy.top/gtxvigjwjf.html

Ruby: obj.instance_variables
来源：http://hz.chenjidiqi.icu/gtvmisefkq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.9152youxi.cn/gtkbhygami.html

================================================================================
来源：http://hz.sxryk.cn/gtsrdkkqsm.html

H. 异常与错误处理
来源：http://hz.chenzaomai.com/gtjzyyoaju.html

================================================================================
来源：http://hz.yueranfly.top/gtzwvpkher.html

[H01] try / catch 基础
来源：http://hz.svipenyu.cn/gthjxcwvrq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.smart0.xyz/gtbdsckljy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ivvv.top/gtuismyhfc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nwbrower.top/gtxluixdlc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yvedp.cn/gtffexfhjp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangkeji.top/gtotxuvvjq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sxryk.cn/gthxohjpzh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shzxlz.cn/gtcvymenup.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gzhubu.top/gttafgqicm.html

[H02] finally / ensure 收尾
来源：http://hz.cheryme.top/gtebxskjri.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxinkj.top/gtwdyulgmm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtladibzcs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtqtieuiau.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtorcilhoi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtpawwgpme.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgfzy.top/gtkxxphifp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xziqi.cn/gtcytzfvrh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.redwolf501.top/gtkvvxvlxa.html

[H03] 主动抛出异常
来源：http://hz.sxryk.cn/gtsiyuyopj.html

Py:   raise ValueError("错误信息")
来源：http://hz.nwbrower.top/gtebmjgpgh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtjaydnnnz.html

JS:   throw new Error("错误信息");
来源：http://hz.gzhubu.top/gtbocfsmms.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtdflrtgmo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gthecpvcmm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jqgufenzy.top/gtvgvryphu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aizwys.cn/gtmpvjalqw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtfoalxign.html

[H04] 自定义异常类型
来源：http://hz.jinghuilouyu.cn/gtxlhklsfr.html

Py:   class MyError(Exception): pass
来源：http://hz.feifeiyinyue.top/gtpiqzhucd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtlgpewxub.html

JS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtihksurgz.html

TS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtvehezydb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhaomingkeji.xyz/gtyoiswzcj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yongpay.top/gtcwoesxte.html

Ruby: class MyError < StandardError; end
来源：http://hz.sysykeji.top/gtrsdouuun.html

C#:   class MyException : Exception {}
来源：http://hz.cqqwz.cn/gtqwerruue.html

[H05] 捕获特定类型
来源：http://hz.chenlongwang.top/gtcsxlaijy.html

Py:   except ValueError as e:
来源：http://hz.yj20258.top/gtwrwgpndo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hysaishi.cn/gtckormdpw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtsgcdwcct.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtwxbzvnvi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.meibo888.top/gtcxuowuhz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigufen.top/gtfsjerxnp.html

Ruby: rescue ArgumentError => e
来源：http://hz.cqqwz.cn/gtnqjfeeaj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydzc1.top/gtrgfahnii.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenzaomai.com/gtjauufyqo.html

Py:   value = d.get("k") or default
来源：http://hz.gotoacloud.top/gtqieqmjmk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtfdaqdlvq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtwrvgnhlv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtsblurosm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tianlin.xyz/gtgwypqenv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yangfankeji.com/gtxlznkmkp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cqqwz.cn/gtxahxbjbb.html

C#:   obj?.A?.B ?? default
来源：http://hz.gzhubu.top/gtwgdwyquf.html

[H07] 断言
来源：http://hz.redwolf501.top/gtoxyexidj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zdqjudy.top/gttddsijke.html

PHP:  assert($x > 0);
来源：http://hz.yangfankeji.com/gtbgrowedc.html

JS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtaxwutkbh.html

TS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtswdrphah.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hysaishi.cn/gtfhhwagwo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tanke756.top/gtexksjzba.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgufenzy.top/gtibztefva.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hnqzz.top/gtfbtsngst.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenjidiqi.icu/gtjtgpeoqe.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhoulong.xyz/gthyvylojj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yongpay.top/gtbmlxqwgm.html

JS:   e.message;  e.stack
来源：http://hz.zhiwuduotai.top/gtgahnzaba.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.vqdsnc.cn/gtajumkxrm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gaohongyu789.top/gtpjgrkhdx.html

Go:   err.Error()
来源：http://hz.sysykeji.top/gtkfykmxzq.html

Ruby: e.message;  e.backtrace
来源：http://hz.9152youxi.cn/gtzjpsilbf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guannengcc.top/gtvcmzgbls.html

[H09] 带错误码的异常
来源：http://hz.guowangkeji.top/gtbqoxtedd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgufenzy.top/gtmpdoadhq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.guowangkeji.top/gtfljhwycd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gzhubu.top/gtwowbhieq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgufenzy.top/gtiuywzjbn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ehwqpu.com/gtuiycquzv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.andypj.xyz/gtdhjgueap.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ivvv.top/gtzxmkzjqb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnxiangtu.top/gtseqhrxnu.html

[H10] 资源自动释放
来源：http://hz.shzxlz.cn/gtggolubxz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aibaodan.cn/gtfchnrvpa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yueranfly.top/gtpiijxxuw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtdsnoajme.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shuidangran.top/gtqvqwjcxx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtbkrkgjxo.html

Go:   defer f.Close()
来源：http://hz.gzhubu.top/gtcfbmvcoj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.kuanghao11.cn/gtghklzkfs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.52xcode.cn/gtypvyctgc.html

================================================================================
来源：http://hz.yanxiufei.cn/gtbwvyopxa.html

I. 正则表达式
来源：http://hz.dianchejie.cn/gtjcvdeowa.html

================================================================================
来源：http://hz.jiagoushi.top/gtbfrcgadm.html

[I01] 判断是否匹配
来源：http://hz.yj20258888.top/gtjebzbrpk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jiagoushi.top/gttgatpjzd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sysykeji.top/gtbabbecju.html

JS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtybbvuvur.html

TS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtvlyjvmfm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gteqcjbljy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.svipenyu.cn/gtienodfof.html

Ruby: s.match?(/\d+/)
来源：http://hz.hammf.cn/gtypomnkza.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zdqjudy.top/gtjovlerfi.html

[I02] 提取所有匹配
来源：http://hz.cashguo.top/gtibqtvowd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sxryk.cn/gtxnrwhiad.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.iojbl.cn/gttjhmjpjr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.316326.xyz/gtnugoxwab.html

TS:   s.match(/\d+/g)
来源：http://hz.sysykeji.top/gtkaopytls.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnqzz.top/gtongtexfo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cucudq.cn/gtchxiavqh.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtcmuwxjkg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sxryk.cn/gtxtwltmmf.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangtech.top/gtfbnoesxu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.svipenyu.cn/gtgpjevikw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cucudq.cn/gtghgcwhfl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cdnleiting.top/gtumsbirvd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xinyue.icu/gtwhlqhcqw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guannengcc.top/gtesndhkkk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.quarkkingdee.top/gtzpukymcw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.snrcjt.cn/gtzhocttgw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydjk.org.cn/gtksxebnnx.html

[I04] 正则替换
来源：http://hz.cucudq.cn/gtutmvnccn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ywan-chungtsiang.top/gtkktoyelm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtcvqbqjdn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtqxwqfvan.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtdqkyhxax.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xingfuxueyuan.xyz/gtibwfkshc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.0kj1m.cn/gtimzqayqw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xinyue.icu/gtkauxabqy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pengpengdd.cyou/gtjhidqyzx.html

[I05] 按正则拆分
来源：http://hz.shzxlz.cn/gtqkornvuq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhiwuduotai.top/gtutdljkxq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ydzc1.top/gtuzsfwtsw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtxkjatamr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtyygzldgg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xziqi.cn/gtqnprchti.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aibaodan.cn/gtwenohimi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtrlfycids.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhiwuduotai.top/gtdhyuxptl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zycfv.cn/gtkxnlwvfg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtkodcufvf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhengqikj.top/gtcndhtfmt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtuddranoa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gtukznwoqq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xinyue.icu/gtlmiaiuua.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sweek.top/gtdhxqqyhw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigufen.top/gtgthqxvxe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtalbseiex.html

[I07] 忽略大小写与多行模式
来源：http://hz.cashguo.top/gtouypryjh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sweek.top/gtnfydulck.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.wangshuangyany.cn/gtyhbyeiwj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgufenzy.top/gtwwzzrxcm.html

TS:   /error/gim
来源：http://hz.fzhhl.top/gtwwqtmxcu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.c1oappe.top/gtxxlonloo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhoulong.xyz/gtqiswixbz.html

Ruby: s.scan(/error/i)
来源：http://hz.chenjidiqi.icu/gttjzsbhku.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zycfv.cn/gtgcqovanx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.meibo888.top/gttmrzaron.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.daria6918.cn/gtybdscujj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gtxegojybu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtbsqkqbik.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtinzmktjg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gogol.net.cn/gtanusobde.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yueranfly.top/gtfjpjuqdp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xylfe.cn/gtokuufuho.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gtjtelaeqq.html

================================================================================
来源：http://hz.yueranfly.top/gtharvaniv.html

J. 日期与时间
来源：http://hz.cdnleiting.top/gtyqaqquzg.html

================================================================================
来源：http://hz.daria6918.cn/gtqnddmbld.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtcalmgmts.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigufen.top/gtpdkxwmdn.html


<!-- 参考信息 -->