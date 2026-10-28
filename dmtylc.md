代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://hz.haohaochexian.top/gtfotfkovt.html

[G03] 实例属性
来源：http://hz.daxiang520.top/gtblzxnjjk.html

Py:   self.name = "x"
来源：http://hz.birdmap.top/gtxozpktxh.html

PHP:  public string $name = "x";
来源：http://hz.hnxiangtu.top/gtxkcxreki.html

JS:   this.name = "x";
来源：http://hz.hnqzz.top/gtrykmzdvw.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtiajdsuud.html

Java: private String name;
来源：http://hz.xziqi.cn/gtrlqhqufz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydzc1.top/gtqfablapt.html

Ruby: @name = "x"
来源：http://hz.iojbl.cn/gtxezvirff.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.kuanghao11.cn/gtfurvqqfv.html

[G04] 定义方法
来源：http://hz.xziqi.cn/gtnrwjhnkc.html

Py:   def greet(self): return self.name
来源：http://hz.zhixingplan.top/gtebazhgns.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yongpay.top/gtugxzdqlg.html

JS:   greet() { return this.name; }
来源：http://hz.havefunace.top/gtcsjlntzh.html

TS:   greet(): string { return this.name; }
来源：http://hz.pycfn.com/gtnbwepshf.html

Java: String greet() { return name; }
来源：http://hz.zhiwuduotai.top/gtdifvybha.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ehwqpu.com/gtkmgxapyj.html

Ruby: def greet; @name; end
来源：http://hz.guannengcc.top/gtpzxyqvnd.html

C#:   public string Greet() => Name;
来源：http://hz.ydjk.org.cn/gtfcndyzyd.html

[G05] 继承
来源：http://hz.jlsjyb.cn/gtmrxuakqa.html

Py:   class Admin(User): pass
来源：http://hz.gogol.net.cn/gtgebqhavo.html

PHP:  class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtfsepqlpu.html

JS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtgpbbtipb.html

TS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtspjrrfbp.html

Java: class Admin extends User {}
来源：http://hz.yj20258888.top/gtxwqykaar.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.haohaochexian.top/gtaxdgylqt.html

Ruby: class Admin < User; end
来源：http://hz.shuidangran.top/gtznwxkesj.html

C#:   class Admin : User {}
来源：http://hz.smart0.xyz/gttdhdutrw.html

[G06] 重写方法
来源：http://hz.chenzaomai.com/gtckfmfveu.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxinkj.top/gtxqxmtglh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtydtqfrdq.html

JS:   greet() { return "admin"; }
来源：http://hz.pycfn.com/gtimnezgov.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gtmwykfrvp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zycfv.cn/gtteuyokiz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangtech.top/gtgirferrn.html

Ruby: def greet; "admin"; end
来源：http://hz.9152youxi.cn/gthmmchuwi.html

C#:   public override string Greet() => "admin";
来源：http://hz.c1oappe.top/gtjnznzpiy.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangtech.top/gtegyxcquo.html

Py:   super().greet()
来源：http://hz.gotoacloud.top/gtrxgwtzfc.html

PHP:  parent::greet();
来源：http://hz.nwbrower.top/gtplwhyesp.html

JS:   super.greet();
来源：http://hz.9152youxi.cn/gtimexfztt.html

TS:   super.greet();
来源：http://hz.0kj1m.cn/gtncjrjbqp.html

Java: super.greet();
来源：http://hz.daxiang520.top/gtctltrmio.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.havefunace.top/gtgxjlwmlu.html

Ruby: super
来源：http://hz.dianchejie.cn/gtorurszuu.html

C#:   base.Greet();
来源：http://hz.hywenlv.cn/gtoxquyktu.html

[G08] 静态方法与属性
来源：http://hz.tanke756.top/gtykytginz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinyuanbaomall.cn/gtyzdsdehy.html

PHP:  public static function f() {}
来源：http://hz.dianchejie.cn/gtmyfncusc.html

JS:   static f() {}
来源：http://hz.fengsongda.top/gtuzovpdrf.html

TS:   static f(): void {}
来源：http://hz.cdnleiting.top/gtqgcqgrwi.html

Java: static void f() {}
来源：http://hz.jinqigufen.top/gtmsjhbuzh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.guannengcc.top/gtbcpharyd.html

Ruby: def self.f; end
来源：http://hz.wangshuangyany.cn/gtcjacsyis.html

C#:   public static void F() {}
来源：http://hz.sufxvd.cn/gtvpadsldh.html

[G09] 接口 / 抽象类
来源：http://hz.nwbrower.top/gtfreqzvdd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangkeji.top/gtlzoodwhe.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.bjfxy.top/gtkxmiljio.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinghuilouyu.cn/gtpmaqnchh.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxuanxn.top/gtoqbotnkf.html

Java: interface Shape { double area(); }
来源：http://hz.andypj.xyz/gtnigoqsoo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jiagoushi.top/gtjjeiwaks.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenlongwang.top/gtgqimfalk.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgufenzy.top/gtrndzqbez.html

[G10] 访问控制
来源：http://hz.shanyushiyangkeji.top/gtickxtfao.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hongshengwenyu.top/gtvgbwstms.html

PHP:  public / protected / private
来源：http://hz.kuanghao11.cn/gtiqtyrsdj.html

JS:   #private 字段；其余公开
来源：http://hz.hysaishi.cn/gtcvdnqnca.html

TS:   public / protected / private
来源：http://hz.snrcjt.cn/gtkrllkask.html

Java: public / protected / private / 默认包级
来源：http://hz.ybcxt.top/gtzhsoyldl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.smart0.xyz/gtirnlrmth.html

Ruby: public / protected / private
来源：http://hz.hnxiangtu.top/gtotvwmxeg.html

C#:   public / protected / private / internal
来源：http://hz.yanxiufei.cn/gtmvytbuun.html

[G11] getter / setter
来源：http://hz.shuidangran.top/gtjynyfpek.html

Py:   @property 与 @x.setter
来源：http://hz.cucudq.cn/gtpgvwivre.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gteunsjato.html

JS:   get name() { return this._name; }
来源：http://hz.fzhhl.top/gtwnymggjo.html

TS:   get name(): string { return this._name; }
来源：http://hz.yuxming.cn/gtgmpzfcok.html

Java: public String getName() { return name; }
来源：http://hz.hnqzz.top/gtpwwmxqnb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ehwqpu.com/gtdqjxthjd.html

Ruby: attr_accessor :name
来源：http://hz.cucudq.cn/gtdzttjnux.html

C#:   public string Name { get; set; }
来源：http://hz.yuanzhike.top/gtazruglzt.html

[G12] 对象转字符串
来源：http://hz.sxryk.cn/gtzgcyessk.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangtech.top/gtefxtwhad.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtserumllm.html

JS:   toString() { return this.name; }
来源：http://hz.jinqigfzy.top/gtxmefepup.html

TS:   toString(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtjxhomedm.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigufen.top/gtvbkmhvoc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.0kj1m.cn/gtnkbyreft.html

Ruby: def to_s; @name; end
来源：http://hz.jlsjyb.cn/gtnhmivskx.html

C#:   public override string ToString() => Name;
来源：http://hz.jinqigufen.top/gtwmomisuc.html

[G13] 判断对象类型
来源：http://hz.tianlin.xyz/gtxswaxwbu.html

Py:   isinstance(u, User)
来源：http://hz.redwolf501.top/gtenuqbuet.html

PHP:  $u instanceof User
来源：http://hz.yangfankeji.com/gtpopdomfp.html

JS:   u instanceof User
来源：http://hz.redwolf501.top/gtfmgwszot.html

TS:   u instanceof User
来源：http://hz.yangfankeji.com/gtktpfomqi.html

Java: u instanceof User
来源：http://hz.haohaochexian.top/gtpflbniwi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258888.top/gtsagcaneg.html

Ruby: u.is_a?(User)
来源：http://hz.zhoulong.xyz/gtofzghqyl.html

C#:   u is User
来源：http://hz.sufxvd.cn/gtqiydyfch.html

[G14] 数据类 / record
来源：http://hz.yj20258.top/gtxnentlxv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jlsjyb.cn/gtflsmlkjc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.bjfxy.top/gtgltztdhw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jlsjyb.cn/gtmyrkmtqg.html

TS:   type User = { name: string; age: number };
来源：http://hz.ppjwa.cn/gtyvaoqsha.html

Java: record User(String name, int age) {}
来源：http://hz.jqgufenzy.top/gtuogmkkzw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.c1oappe.top/gtxshbjuhy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnxiangtu.top/gtjsgldquj.html

C#:   record User(string Name, int Age);
来源：http://hz.yuanzhike.top/gtvjdistli.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gtzmlugnoj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cheryme.top/gttvcdwhxa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenlongwang.top/gtxgegepgw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydjk.org.cn/gtuumieega.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtnrsbwdrd.html

Java: enum Color { RED, GREEN }
来源：http://hz.ehwqpu.com/gtpsgocqpc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zdqjudy.top/gtsisetbyo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.feifeiyinyue.top/gthdjaoxxx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtctwanqsx.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangtech.top/gtjivixhkk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yueranfly.top/gtlvjyxvwg.html

PHP:  get_object_vars($obj);
来源：http://hz.ppjwa.cn/gtbasfihoo.html

JS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtxwideans.html

TS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtjemzhyrt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinghuilouyu.cn/gtizntmior.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.svipenyu.cn/gtzapfojqy.html

Ruby: obj.instance_variables
来源：http://hz.hongshengwenyu.top/gtonycxunc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxinkj.top/gtskykmxxb.html

================================================================================
来源：http://hz.ydzc1.top/gthktaolil.html

H. 异常与错误处理
来源：http://hz.cashguo.top/gtwxvtyett.html

================================================================================
来源：http://hz.sufxvd.cn/gtywgnnnep.html

[H01] try / catch 基础
来源：http://hz.tianlin.xyz/gtvnmeoaxq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.havefunace.top/gtcxjjkmkz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinyuanbaomall.cn/gthcrnweln.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtpezedfnd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.birdmap.top/gtibneelwd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pycfn.com/gttuwejxsi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.guannengcc.top/gtwaiekudb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yonumen.top/gtaesptftp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gtroozpbry.html

[H02] finally / ensure 收尾
来源：http://hz.zhoulong.xyz/gtzgzdedse.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ybcxt.top/gtotcshxbc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtvgtbeywt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtbxhegylv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtozzxdrod.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtcqglioqj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj202588.top/gtlswpcnvq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jlsjyb.cn/gtexzohxvo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cucudq.cn/gtcpiqfetu.html

[H03] 主动抛出异常
来源：http://hz.hongshengwenyu.top/gtgjzapila.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhixingplan.top/gtyxeckpku.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtilwhihjc.html

JS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gtlfszuoyi.html

TS:   throw new Error("错误信息");
来源：http://hz.birdmap.top/gturbdomjx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtulwkfhmf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jqgufenzy.top/gtlvdbehtx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinyuanbaomall.cn/gtwlmdizmm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtvclzxfpg.html

[H04] 自定义异常类型
来源：http://hz.316326.xyz/gtpbdjsxrn.html

Py:   class MyError(Exception): pass
来源：http://hz.guannengcc.top/gtsyjmudkr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgfzy.top/gtpxrmzxef.html

JS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtnukyeiom.html

TS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtsxaealld.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtyzblvepn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sysykeji.top/gtmzhedpij.html

Ruby: class MyError < StandardError; end
来源：http://hz.jianghu66.top/gtmxjijaik.html

C#:   class MyException : Exception {}
来源：http://hz.hongshengwenyu.top/gthinweuzx.html

[H05] 捕获特定类型
来源：http://hz.jiagoushi.top/gtwiaaaqig.html

Py:   except ValueError as e:
来源：http://hz.cashguo.top/gtvdajzvqj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hysaishi.cn/gtussyvmew.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aizwys.cn/gtxkabmnrf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yongpay.top/gtmgadmkoh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258.top/gtkbpgnhxv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yongpay.top/gtrjpbnxqb.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhixingplan.top/gtqppzmfos.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shanyushiyangkeji.top/gtlwsmwkic.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenjidiqi.icu/gtujfnegib.html

Py:   value = d.get("k") or default
来源：http://hz.zhijiandao.cn/gteleyspmi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnxiangtu.top/gtlwbvbver.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.bjfxy.top/gtkhqhhkdk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtsasthcnu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sufxvd.cn/gthmuxmqcc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ehwqpu.com/gtedkpfqpv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yongpay.top/gtiwpxzpjz.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangshuangyany.cn/gtgecxpexw.html

[H07] 断言
来源：http://hz.chenzaomai.com/gtbawvohhk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.c1oappe.top/gthnxqliwe.html

PHP:  assert($x > 0);
来源：http://hz.feifeiyinyue.top/gtrjghrfsk.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtxqoltcjp.html

TS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gtqgrnqpyx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.havefunace.top/gtmmbqefcl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zycfv.cn/gtevbuxtmi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtfajzykiv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.kuanghao11.cn/gtrswyawtk.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuxming.cn/gtryzhasex.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ppjwa.cn/gtlusgzvef.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.meibo888.top/gtqfowhjvp.html

JS:   e.message;  e.stack
来源：http://hz.redwolf501.top/gtdcnmclhl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigfzy.top/gttnlqpoyo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.52xcode.cn/gtusqwsdkz.html

Go:   err.Error()
来源：http://hz.tianlin.xyz/gtwshojulj.html

Ruby: e.message;  e.backtrace
来源：http://hz.tian-w.cn/gtnhopdubx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jqgufenzy.top/gtcqornias.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtkiwlawcv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shangyingyoupin.top/gtxutnrmzk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yangfankeji.com/gtinxzgbcv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenlongwang.top/gttonscvrk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gzhubu.top/gtrkwvlzhv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhiwuduotai.top/gtxmrutzdd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gtnuudquwp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nwbrower.top/gtpesqysyt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangkeji.top/gthsxtctil.html

[H10] 资源自动释放
来源：http://hz.zhaomingkeji.xyz/gtxcbbrrqt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtbedvcrmn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.svipenyu.cn/gtuioqchol.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtzunmofsj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ivvv.top/gtuuhitabd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shuidangran.top/gttcizfyma.html

Go:   defer f.Close()
来源：http://hz.cqqwz.cn/gtfchnjema.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ydjk.org.cn/gtzpovqnvz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.quarkkingdee.top/gtyzhjtgaw.html

================================================================================
来源：http://hz.yvedp.cn/gtsiqogiwl.html

I. 正则表达式
来源：http://hz.havefunace.top/gtcyllhyla.html

================================================================================
来源：http://hz.sxryk.cn/gtgbudqezl.html

[I01] 判断是否匹配
来源：http://hz.cheryme.top/gtmcskqwow.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ivvv.top/gtinnjaaqz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hammf.cn/gtsesyhasg.html

JS:   /\d+/.test(s)
来源：http://hz.tianlin.xyz/gtkfwbirno.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtnnidhebv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shangyingyoupin.top/gtwjhzuvnd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangdashe.top/gtoijecffd.html

Ruby: s.match?(/\d+/)
来源：http://hz.birdmap.top/gtwbnxmwrc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sweek.top/gtqcefibaj.html

[I02] 提取所有匹配
来源：http://hz.shzxlz.cn/gtexftfzqj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.kuanghao11.cn/gtwhmovntc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhijiandao.cn/gtubcikbog.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ybcxt.top/gtbfjsovja.html

TS:   s.match(/\d+/g)
来源：http://hz.snrcjt.cn/gtigrujsui.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhongyouzk.top/gtdvcksjkc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tanke756.top/gtaenpewbh.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhaomingkeji.xyz/gtaebzsiaz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xylfe.cn/gttksuhbzy.html

[I03] 提取捕获分组
来源：http://hz.nwbrower.top/gtvwtcjmmh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhengqikj.top/gtjmhbfcha.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.0kj1m.cn/gtsyyvbzuz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.iojbl.cn/gtuyvpwunu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ivvv.top/gtzvezoecc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xingfuxueyuan.xyz/gtnptkmsno.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gotoacloud.top/gtypmwjnyf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ydzc1.top/gtpwxtexvu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nwbrower.top/gtztdcuozq.html

[I04] 正则替换
来源：http://hz.hnxiangtu.top/gtbzfiyzfn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgfzy.top/gtzbgxlvoo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtuamszbvr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtlyfjrtdh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gtdezojqco.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jiagoushi.top/gtxpiacjnh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hammf.cn/gtkjhqlega.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shuidangran.top/gtfyrhynmd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jianghu66.top/gtwcrvbjdb.html

[I05] 按正则拆分
来源：http://hz.yonumen.top/gtljykrvay.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhoulong.xyz/gtjlegalvi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hfpthk.cn/gtomywrchn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtahpquhxd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtnsruqyxr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.meibo888.top/gtodltdrhq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shzxlz.cn/gtesxjxaao.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtoubstwum.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gzhubu.top/gtubmjknrc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuxming.cn/gthqttppou.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtuqmelqvk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuanzhike.top/gtkscwupds.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shzxlz.cn/gtaoxundil.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.meibo888.top/gtfpehbgjc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtsojeefux.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258888.top/gtoxlyjbzi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gtiopaceua.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtsvifltrn.html

[I07] 忽略大小写与多行模式
来源：http://hz.cheryme.top/gtgkrybisx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydzc1.top/gtjeacbfec.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.birdmap.top/gtahddfmmx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hysaishi.cn/gtbynzinkf.html

TS:   /error/gim
来源：http://hz.c1oappe.top/gtossfwtqw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigufen.top/gtgnqprthz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hysaishi.cn/gtszdplqox.html

Ruby: s.scan(/error/i)
来源：http://hz.birdmap.top/gtczcwocmg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258888.top/gtnhmdppss.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xziqi.cn/gtlbwrkskg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.daria6918.cn/gtoizthbsu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fengsongda.top/gtkxdieehg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gthuneegfk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhongyouzk.top/gtgjpbvkcz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yangfankeji.com/gtcqxqztbj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yvedp.cn/gtujijnimb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hammf.cn/gtbebgmwxb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yvedp.cn/gtpbuwlznc.html

================================================================================
来源：http://hz.pycfn.com/gtmnncytsk.html

J. 日期与时间
来源：http://hz.redwolf501.top/gtywfadjxx.html

================================================================================
来源：http://hz.tian-w.cn/gtnnigcejh.html

[J01] 获取当前时间
来源：http://hz.cqqwz.cn/gttygpiwsj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.andypj.xyz/gtbnvbrvrk.html


<!-- 参考信息 -->