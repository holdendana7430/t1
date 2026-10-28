代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtekygtcht.html

[G03] 实例属性
来源：http://hz.shangyingyoupin.top/gtaplevudr.html

Py:   self.name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtcobqkkmc.html

PHP:  public string $name = "x";
来源：http://hz.dianchejie.cn/gttjmrntoc.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gttyfynxju.html

TS:   name: string = "x";
来源：http://hz.quarkkingdee.top/gtrczcnpna.html

Java: private String name;
来源：http://hz.smart0.xyz/gtsgrjdwqo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.redwolf501.top/gthtfcflca.html

Ruby: @name = "x"
来源：http://hz.feifeiyinyue.top/gtlcprztty.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yanxiufei.cn/gtqxwikgkm.html

[G04] 定义方法
来源：http://hz.hammf.cn/gtpagpcmkt.html

Py:   def greet(self): return self.name
来源：http://hz.sweek.top/gtxvwjbkwo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.316326.xyz/gtfanhkitg.html

JS:   greet() { return this.name; }
来源：http://hz.svipenyu.cn/gtnpcxygln.html

TS:   greet(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gtiuxlfljm.html

Java: String greet() { return name; }
来源：http://hz.xziqi.cn/gtlecbxnat.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.aibaodan.cn/gtbvqicjrp.html

Ruby: def greet; @name; end
来源：http://hz.yangfankeji.com/gtrgnebnxv.html

C#:   public string Greet() => Name;
来源：http://hz.havefunace.top/gtsivxtqmw.html

[G05] 继承
来源：http://hz.cheryme.top/gtnlwpvfds.html

Py:   class Admin(User): pass
来源：http://hz.hnqzz.top/gtbbjhobpl.html

PHP:  class Admin extends User {}
来源：http://hz.chenzaomai.com/gtlgqbntds.html

JS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtcjrmnywr.html

TS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtxggvstrm.html

Java: class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtfkggubtf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.52xcode.cn/gtgyjmkujq.html

Ruby: class Admin < User; end
来源：http://hz.hywenlv.cn/gtjmouuxfx.html

C#:   class Admin : User {}
来源：http://hz.fzhhl.top/gtfwipofdc.html

[G06] 重写方法
来源：http://hz.hysaishi.cn/gthfuxkgai.html

Py:   def greet(self): return "admin"
来源：http://hz.gaohongyu789.top/gtncpkouua.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yueranfly.top/gtkrrxbvpv.html

JS:   greet() { return "admin"; }
来源：http://hz.52xcode.cn/gtyamnwhkk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxuanxn.top/gtahxcrowx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtijkvugml.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hysaishi.cn/gtuyddctgg.html

Ruby: def greet; "admin"; end
来源：http://hz.nwbrower.top/gtlldsatpp.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenjidiqi.icu/gtcyuslpkh.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtblvrndpr.html

Py:   super().greet()
来源：http://hz.shuidangran.top/gttrztgsyx.html

PHP:  parent::greet();
来源：http://hz.daria6918.cn/gtsgealeqb.html

JS:   super.greet();
来源：http://hz.hnqzz.top/gtsqicpapy.html

TS:   super.greet();
来源：http://hz.jqgfzy.top/gtwthjracy.html

Java: super.greet();
来源：http://hz.ydzc1.top/gtjalidjhg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtewyvbtun.html

Ruby: super
来源：http://hz.hywenlv.cn/gtzbhkiugm.html

C#:   base.Greet();
来源：http://hz.sweek.top/gtcoykvlnd.html

[G08] 静态方法与属性
来源：http://hz.jinqigfzy.top/gtjdzsogeq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnqzz.top/gtrzsrwzvj.html

PHP:  public static function f() {}
来源：http://hz.shzxlz.cn/gtokmzgdyi.html

JS:   static f() {}
来源：http://hz.cqqwz.cn/gtnrpgvknd.html

TS:   static f(): void {}
来源：http://hz.sufxvd.cn/gtulkucbti.html

Java: static void f() {}
来源：http://hz.hfpthk.cn/gtkcjtdhfd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258.top/gtaonikiql.html

Ruby: def self.f; end
来源：http://hz.yj20258888.top/gtjdnnengv.html

C#:   public static void F() {}
来源：http://hz.aibaodan.cn/gtlanlrlyb.html

[G09] 接口 / 抽象类
来源：http://hz.aibaodan.cn/gtnnjawtdz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.daxiang520.top/gttggrnvpz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxuanxn.top/gtlnxefbcf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hongshengwenyu.top/gtvymmpemv.html

TS:   interface Shape { area(): number; }
来源：http://hz.tianlin.xyz/gtayrzyygz.html

Java: interface Shape { double area(); }
来源：http://hz.zdqjudy.top/gtmlzdnrbt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.feifeiyinyue.top/gtpzonujfi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jiagoushi.top/gtpbsgidkh.html

C#:   interface IShape { double Area(); }
来源：http://hz.ehwqpu.com/gtvihowtva.html

[G10] 访问控制
来源：http://hz.jlsjyb.cn/gtzrcurdzs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.snrcjt.cn/gtedsskgod.html

PHP:  public / protected / private
来源：http://hz.ppjwa.cn/gtcmyullab.html

JS:   #private 字段；其余公开
来源：http://hz.yj202588.top/gtpczzynnl.html

TS:   public / protected / private
来源：http://hz.yj202588.top/gtnpckgvmo.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtyeyinpkz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daxiang520.top/gtqvrenmcv.html

Ruby: public / protected / private
来源：http://hz.cqqwz.cn/gtxggvozvj.html

C#:   public / protected / private / internal
来源：http://hz.jlsjyb.cn/gtzjvzawee.html

[G11] getter / setter
来源：http://hz.yj202588.top/gtbeyqeyaz.html

Py:   @property 与 @x.setter
来源：http://hz.zhongyouzk.top/gtdtqpwuyt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258.top/gtubkegsas.html

JS:   get name() { return this._name; }
来源：http://hz.yangfankeji.com/gtluhllbia.html

TS:   get name(): string { return this._name; }
来源：http://hz.shangyingyoupin.top/gtawaqrswv.html

Java: public String getName() { return name; }
来源：http://hz.cashguo.top/gthnferdqt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258888.top/gtmkfduhrx.html

Ruby: attr_accessor :name
来源：http://hz.sxryk.cn/gtftgmmwgy.html

C#:   public string Name { get; set; }
来源：http://hz.jlsjyb.cn/gtelajirgv.html

[G12] 对象转字符串
来源：http://hz.snrcjt.cn/gthchyldix.html

Py:   def __str__(self): return self.name
来源：http://hz.xuetiantiany.cn/gtiaukcnzi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtkjhdtpop.html

JS:   toString() { return this.name; }
来源：http://hz.wangshuangyany.cn/gtwexebeli.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gtstqfxele.html

Java: @Override public String toString() { return name; }
来源：http://hz.0kj1m.cn/gtmmprdnvn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.c1oappe.top/gtordawfyv.html

Ruby: def to_s; @name; end
来源：http://hz.gaohongyu789.top/gtqcmdcwqn.html

C#:   public override string ToString() => Name;
来源：http://hz.zhoulong.xyz/gtcjrqmpct.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gtpnsyzkwr.html

Py:   isinstance(u, User)
来源：http://hz.ehwqpu.com/gtyqloactw.html

PHP:  $u instanceof User
来源：http://hz.chenjidiqi.icu/gtsrrnijsp.html

JS:   u instanceof User
来源：http://hz.hnqzz.top/gtzvmnjqjm.html

TS:   u instanceof User
来源：http://hz.gaohongyu789.top/gtjfmrctrd.html

Java: u instanceof User
来源：http://hz.wangdashe.top/gtrcqfmiwi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xziqi.cn/gtnkciicoj.html

Ruby: u.is_a?(User)
来源：http://hz.yvedp.cn/gtwstcvcsr.html

C#:   u is User
来源：http://hz.zhoulong.xyz/gtywdhhjxi.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtcejwmyny.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yvedp.cn/gtuwuppdoc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yonumen.top/gtspkpewfa.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hongshengwenyu.top/gtdjvajktp.html

TS:   type User = { name: string; age: number };
来源：http://hz.svipenyu.cn/gtnuoyodem.html

Java: record User(String name, int age) {}
来源：http://hz.316326.xyz/gtunozgnkc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigfzy.top/gtebptiaed.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xylfe.cn/gtjicovcfi.html

C#:   record User(string Name, int Age);
来源：http://hz.wangdashe.top/gtvoflpwdv.html

[G15] 枚举
来源：http://hz.shanyushiyangtech.top/gtqvvmanum.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangkeji.top/gtndcncztb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.birdmap.top/gtgpixjhvz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yonumen.top/gtrwxqokid.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenzaomai.com/gtkypcyywk.html

Java: enum Color { RED, GREEN }
来源：http://hz.meibo888.top/gtdpxkopln.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhaomingkeji.xyz/gtlsbsiuyo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydzc1.top/gtkukmgdjz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtccqbglyy.html

[G16] 对象转数组 / 字典
来源：http://hz.cucudq.cn/gtxykresun.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhongyouzk.top/gtozhjktle.html

PHP:  get_object_vars($obj);
来源：http://hz.shzxlz.cn/gthdwlaqkh.html

JS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtqepytxps.html

TS:   Object.entries(obj)
来源：http://hz.feifeiyinyue.top/gtpbgkyvfk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yonumen.top/gtkrzefwnx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenlongwang.top/gtqlfokkjx.html

Ruby: obj.instance_variables
来源：http://hz.yj20258.top/gtfqrrpeiy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuanzx.com/gtkvnwbnfk.html

================================================================================
来源：http://hz.zhoulong.xyz/gtmogephht.html

H. 异常与错误处理
来源：http://hz.andypj.xyz/gtxtemucwl.html

================================================================================
来源：http://hz.xylfe.cn/gtbfttltdg.html

[H01] try / catch 基础
来源：http://hz.yj20258.top/gtbmwwkwoh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fengsongda.top/gtvgfzlckm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.snrcjt.cn/gtqpcymadd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtqjlecwow.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.bjfxy.top/gtcmfzjavu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cqqwz.cn/gtwlcqpjka.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gzhubu.top/gtijjnotpt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.wangshuangyany.cn/gtmyloxhxx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.havefunace.top/gtwcogzidn.html

[H02] finally / ensure 收尾
来源：http://hz.gzhubu.top/gtxeiozwkv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnxiangtu.top/gtsdquamzc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtbckwganq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtoolkfeda.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtchwzsutj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gthqsuocln.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tanke756.top/gtuyiwuxaq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxuanxn.top/gtfchujirz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hammf.cn/gtfgwkkmyz.html

[H03] 主动抛出异常
来源：http://hz.hywenlv.cn/gtllpwlxnl.html

Py:   raise ValueError("错误信息")
来源：http://hz.hywenlv.cn/gtpfuvyrmf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtilmndddh.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtusczauaj.html

TS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtyialmlqk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtsfiyudqv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gaohongyu789.top/gtvhegkaxx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yueranfly.top/gtadztzrww.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtofjlqhde.html

[H04] 自定义异常类型
来源：http://hz.sysykeji.top/gtfhyqwfsv.html

Py:   class MyError(Exception): pass
来源：http://hz.nanxuanxn.top/gtddrvjiqk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtpfkajese.html

JS:   class MyError extends Error {}
来源：http://hz.shuidangran.top/gtabznqqxo.html

TS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gtzgsbrkts.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtjghtywzx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aizwys.cn/gtmfvbokme.html

Ruby: class MyError < StandardError; end
来源：http://hz.ivvv.top/gtjmsceafg.html

C#:   class MyException : Exception {}
来源：http://hz.jinqigfzy.top/gtptkxbzqk.html

[H05] 捕获特定类型
来源：http://hz.zdqjudy.top/gtfujxsrbw.html

Py:   except ValueError as e:
来源：http://hz.tianlin.xyz/gtrqqtdkmc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuetiantiany.cn/gtakapzglr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gtzelogtlh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtifzfuvmi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yvedp.cn/gtxyckrvqt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xziqi.cn/gtqggskdam.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtjozyuedi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.birdmap.top/gtremzqokp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ehwqpu.com/gtlwoispjx.html

Py:   value = d.get("k") or default
来源：http://hz.haohaochexian.top/gtycmfzglj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuxming.cn/gttwxwgbrk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtgrshzpot.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.c1oappe.top/gtcvlxhlaw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xziqi.cn/gtbweikgxs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dianchejie.cn/gtiggvercz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtaeopcjae.html

C#:   obj?.A?.B ?? default
来源：http://hz.yonumen.top/gtbpekibul.html

[H07] 断言
来源：http://hz.jqgufenzy.top/gtrfjivzot.html

Py:   assert x > 0, "必须为正"
来源：http://hz.smart0.xyz/gtkzhpcncn.html

PHP:  assert($x > 0);
来源：http://hz.yanxiufei.cn/gtepucwsuu.html

JS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtsnepwcae.html

TS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gtcrvvjqqk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ywan-chungtsiang.top/gtjoxrldzb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xinyue.icu/gttalgznwk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yuanzhike.top/gtsgredydi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hammf.cn/gtfbocguoe.html

[H08] 获取错误信息与堆栈
来源：http://hz.guannengcc.top/gtnpihjoat.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.snrcjt.cn/gtphvrfjvb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.snrcjt.cn/gtspwwjcni.html

JS:   e.message;  e.stack
来源：http://hz.smart0.xyz/gtowaewyvl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.wangshuangyany.cn/gtdunowmxy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenzaomai.com/gtwxijaxki.html

Go:   err.Error()
来源：http://hz.sweek.top/gtzebbarxt.html

Ruby: e.message;  e.backtrace
来源：http://hz.zycfv.cn/gtzgzrqqmn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhaomingkeji.xyz/gtztldlhxm.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtqxdcuafz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.bjfxy.top/gtrrgalcxh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zycfv.cn/gtifxhwdtz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jiagoushi.top/gthjnrrtod.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnqzz.top/gtihubxpzr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.svipenyu.cn/gtgddhxpsp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuanzhike.top/gtdkbuemja.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ybcxt.top/gtksdwyseo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.daxiang520.top/gteagaoolg.html

[H10] 资源自动释放
来源：http://hz.gzhubu.top/gtuqekkodk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shangyingyoupin.top/gtnskpcxkx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fengsongda.top/gtwqpxjzkh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtzvdkrkmd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtrsckpoll.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ehwqpu.com/gtituscisv.html

Go:   defer f.Close()
来源：http://hz.bjfxy.top/gtemjjjjrn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.bjfxy.top/gtbleqptuf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgufenzy.top/gtnpzftqtx.html

================================================================================
来源：http://hz.cucudq.cn/gtlilcmkce.html

I. 正则表达式
来源：http://hz.fzhhl.top/gtysrvbtyn.html

================================================================================
来源：http://hz.hysaishi.cn/gtxfwwbdnh.html

[I01] 判断是否匹配
来源：http://hz.yj202588.top/gtmitijnvx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gotoacloud.top/gtsoicukus.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gaohongyu789.top/gtvssmpulh.html

JS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtbvwebiec.html

TS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtsxcyytfd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yonumen.top/gteuavutud.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenzaomai.com/gtrddtaqls.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgufenzy.top/gtakwlhpri.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xylfe.cn/gtjorzflmm.html

[I02] 提取所有匹配
来源：http://hz.jlsjyb.cn/gtdinxoluv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fzhhl.top/gtcrgporcs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cdnleiting.top/gtqjsmuncb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yvedp.cn/gtxogkcwly.html

TS:   s.match(/\d+/g)
来源：http://hz.xziqi.cn/gtzhgtmuum.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shangyingyoupin.top/gtmmsjzzgm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gtmvhzoywc.html

Ruby: s.scan(/\d+/)
来源：http://hz.tanke756.top/gtpyseviid.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.andypj.xyz/gtiyrfbltc.html

[I03] 提取捕获分组
来源：http://hz.sysykeji.top/gtvixldvjl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shangyingyoupin.top/gtzhwfmzqq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtibleqhcq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.aizwys.cn/gtgbvyotax.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.redwolf501.top/gtfhluitjc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj20258.top/gtohnxrzib.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.smart0.xyz/gtyrgfenao.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtaiywqtfb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinyuanbaomall.cn/gtjbgnuhqr.html

[I04] 正则替换
来源：http://hz.havefunace.top/gtoxzbdfxd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daria6918.cn/gtxcsumslw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.birdmap.top/gtunjaaach.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtyahdxzyh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtaxbtdyqv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.bjfxy.top/gtspjnplbq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.iojbl.cn/gthloozagd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sufxvd.cn/gtdqcxtuwi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxinkj.top/gtrlxnfvir.html

[I05] 按正则拆分
来源：http://hz.jyoumei.cn/gtlluukenq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenzaomai.com/gtwauppfmb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtngkbmvvq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtdzywvxil.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtxphhymmr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.316326.xyz/gtjzsmmiuu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtfblpxlta.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtjozaqdbr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxinkj.top/gtbynbkapo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.dashuyun.cn/gtsxaswyvm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gtdcqrfums.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shanyushiyangtech.top/gtdpyapcjr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gteidqkjkb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtpggyftdr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tanke756.top/gtksynpisa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangdashe.top/gtteckwpnf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gtfthcxdhq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtfqzriijt.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenzaomai.com/gtoogobeuh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxuanxn.top/gttkvxcbyh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnqzz.top/gtbsljvnso.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhoulong.xyz/gtlhweebyy.html

TS:   /error/gim
来源：http://hz.gzhubu.top/gtrezguxis.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.wangdashe.top/gtygecymdc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.vqdsnc.cn/gtmdbxzlxx.html

Ruby: s.scan(/error/i)
来源：http://hz.xziqi.cn/gtjxjavvng.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dashuyun.cn/gtjkfgcxbk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zdqjudy.top/gtypgnvftx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xylfe.cn/gtewclfaib.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yuxming.cn/gtbfnfmfth.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.9152youxi.cn/gtecqstirn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtzgeiqvjk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.havefunace.top/gtzuvzpzpa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhixingplan.top/gtenxrxgkp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.birdmap.top/gtejgzgysz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtswcsttgu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtougdoydz.html

J. 日期与时间
来源：http://hz.zdqjudy.top/gtkjqpkwbw.html

================================================================================
来源：http://hz.yuanzhike.top/gtfzzealop.html

[J01] 获取当前时间
来源：http://hz.jlsjyb.cn/gtlfinltsg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shuidangran.top/gtqvhdzacz.html


<!-- 参考信息 -->