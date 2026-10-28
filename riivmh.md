代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj20258.top/gtwhzdzrdc.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtoqfzppus.html

C#:   public string Greet() => Name;
来源：http://hz.chenzaomai.com/gttczmjxlv.html

[G05] 继承
来源：http://hz.birdmap.top/gtaczrgxpf.html

Py:   class Admin(User): pass
来源：http://hz.shuidangran.top/gtbgaivxdu.html

PHP:  class Admin extends User {}
来源：http://hz.jqgfzy.top/gtzkahmhjb.html

JS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtgmqiwigq.html

TS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtciqvvgrd.html

Java: class Admin extends User {}
来源：http://hz.tianlin.xyz/gtripwltrm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zycfv.cn/gtipckktfi.html

Ruby: class Admin < User; end
来源：http://hz.yuanzhike.top/gtgfjmvgmp.html

C#:   class Admin : User {}
来源：http://hz.iojbl.cn/gtlaeyhcfo.html

[G06] 重写方法
来源：http://hz.sxryk.cn/gtklsnxxgv.html

Py:   def greet(self): return "admin"
来源：http://hz.52xcode.cn/gtwqrixjeg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtbggqiiig.html

JS:   greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtayrdwewo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtlriwtxod.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gteqfrtjic.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cdnleiting.top/gtrhgpjwyf.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigufen.top/gtxycbrdyd.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenlongwang.top/gtygzewqlq.html

[G07] 调用父类方法
来源：http://hz.pycfn.com/gtzwndtqgq.html

Py:   super().greet()
来源：http://hz.meibo888.top/gtztldbate.html

PHP:  parent::greet();
来源：http://hz.zhongyouzk.top/gtwfeonfsr.html

JS:   super.greet();
来源：http://hz.guannengcc.top/gtigjflhlk.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtffdykosj.html

Java: super.greet();
来源：http://hz.guannengcc.top/gtadammtwe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.316326.xyz/gttwwmikts.html

Ruby: super
来源：http://hz.zhongyouzk.top/gtolxhygph.html

C#:   base.Greet();
来源：http://hz.jyoumei.cn/gtqkaokbgp.html

[G08] 静态方法与属性
来源：http://hz.shanyushiyangtech.top/gtifhxzndj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xziqi.cn/gtxigqketj.html

PHP:  public static function f() {}
来源：http://hz.yj20258.top/gtldzxgxdt.html

JS:   static f() {}
来源：http://hz.sweek.top/gtxinxtpjo.html

TS:   static f(): void {}
来源：http://hz.sxryk.cn/gtssoxmstn.html

Java: static void f() {}
来源：http://hz.svipenyu.cn/gtddytbydn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinyuanbaomall.cn/gtkgoheajc.html

Ruby: def self.f; end
来源：http://hz.pycfn.com/gtnwuslfve.html

C#:   public static void F() {}
来源：http://hz.yj20258888.top/gttszodydi.html

[G09] 接口 / 抽象类
来源：http://hz.aizwys.cn/gtyqivhljo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yueranfly.top/gtgvjlzcal.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ehwqpu.com/gtvmqhbkux.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hongshengwenyu.top/gtcnqpsmrd.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhaomingkeji.xyz/gtdcaukeht.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangkeji.top/gtltocbmcn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cucudq.cn/gtdarjvtmj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jiagoushi.top/gtcsqkwvri.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgfzy.top/gtolhrtfbb.html

[G10] 访问控制
来源：http://hz.yanxiufei.cn/gtaybdvdji.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sxryk.cn/gtxujfbtfv.html

PHP:  public / protected / private
来源：http://hz.zhijiandao.cn/gtglhgkcyr.html

JS:   #private 字段；其余公开
来源：http://hz.sufxvd.cn/gtrplyxpjl.html

TS:   public / protected / private
来源：http://hz.ehwqpu.com/gtksgrhwgc.html

Java: public / protected / private / 默认包级
来源：http://hz.shanyushiyangkeji.top/gtyyivohqy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hongshengwenyu.top/gtchhjlyhh.html

Ruby: public / protected / private
来源：http://hz.zhiwuduotai.top/gtcedmprdx.html

C#:   public / protected / private / internal
来源：http://hz.vqdsnc.cn/gtjdlptibt.html

[G11] getter / setter
来源：http://hz.yueranfly.top/gtzukuagen.html

Py:   @property 与 @x.setter
来源：http://hz.zhoulong.xyz/gtzrgzbzds.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cashguo.top/gtdwlprang.html

JS:   get name() { return this._name; }
来源：http://hz.smart0.xyz/gtvtwpzvtg.html

TS:   get name(): string { return this._name; }
来源：http://hz.ydzc1.top/gtiqdsnoeb.html

Java: public String getName() { return name; }
来源：http://hz.fengsongda.top/gteyqenwwx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhengqikj.top/gtkeqykurb.html

Ruby: attr_accessor :name
来源：http://hz.jinqigufen.top/gtxfpofpmr.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gtwrjfssuo.html

[G12] 对象转字符串
来源：http://hz.zycfv.cn/gtytweahdf.html

Py:   def __str__(self): return self.name
来源：http://hz.guannengcc.top/gtieowydpa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtgaqlrzxy.html

JS:   toString() { return this.name; }
来源：http://hz.gzhubu.top/gtqulyqqzx.html

TS:   toString(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtbutrybxr.html

Java: @Override public String toString() { return name; }
来源：http://hz.xinyue.icu/gtoksnllqp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cucudq.cn/gtncspvqlu.html

Ruby: def to_s; @name; end
来源：http://hz.haohaochexian.top/gtafslziga.html

C#:   public override string ToString() => Name;
来源：http://hz.hammf.cn/gtqggbjvdk.html

[G13] 判断对象类型
来源：http://hz.yanxiufei.cn/gtrcjhaocu.html

Py:   isinstance(u, User)
来源：http://hz.chenlongwang.top/gtppnzhnlp.html

PHP:  $u instanceof User
来源：http://hz.cucudq.cn/gtdqlvukvl.html

JS:   u instanceof User
来源：http://hz.pycfn.com/gtmhpzpwee.html

TS:   u instanceof User
来源：http://hz.cheryme.top/gtjicttxrl.html

Java: u instanceof User
来源：http://hz.xuanzx.com/gtwicfflwg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sufxvd.cn/gtxpqycxue.html

Ruby: u.is_a?(User)
来源：http://hz.gzhubu.top/gtfqdcjplv.html

C#:   u is User
来源：http://hz.ybcxt.top/gtoejoiijd.html

[G14] 数据类 / record
来源：http://hz.jinghuilouyu.cn/gtdxhbahjx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.quarkkingdee.top/gtmraazwov.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgufenzy.top/gtpxkiihws.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258.top/gthgskmaov.html

TS:   type User = { name: string; age: number };
来源：http://hz.shangyingyoupin.top/gthoelsdus.html

Java: record User(String name, int age) {}
来源：http://hz.redwolf501.top/gtcsiqkieg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhaomingkeji.xyz/gtcwzzewpz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zdqjudy.top/gtbnablxoa.html

C#:   record User(string Name, int Age);
来源：http://hz.cucudq.cn/gtoioqthyi.html

[G15] 枚举
来源：http://hz.316326.xyz/gtbabgpqjp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtbpzwozwg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yonumen.top/gtlnykfadv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yvedp.cn/gtrltxpebq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hammf.cn/gtemauhgnh.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangtech.top/gtadklopdx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.haohaochexian.top/gtrgfeknqa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxinkj.top/gtujrkfybt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.andypj.xyz/gttbocaqdz.html

[G16] 对象转数组 / 字典
来源：http://hz.cashguo.top/gtyvfickug.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhoulong.xyz/gtiztgbefs.html

PHP:  get_object_vars($obj);
来源：http://hz.shanyushiyangtech.top/gtmjgqgydu.html

JS:   Object.entries(obj)
来源：http://hz.svipenyu.cn/gtcvxixqnh.html

TS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gtgbpkjaes.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hnqzz.top/gtpzndguxh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dianchejie.cn/gtbydhyooh.html

Ruby: obj.instance_variables
来源：http://hz.ybcxt.top/gtkzrbibqj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtlrlfyeaj.html

================================================================================
来源：http://hz.52xcode.cn/gtyuvsdyff.html

H. 异常与错误处理
来源：http://hz.gzhubu.top/gtptjhqbcs.html

================================================================================
来源：http://hz.smart0.xyz/gtwejsreuc.html

[H01] try / catch 基础
来源：http://hz.ybcxt.top/gtoneoojqm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xuetiantiany.cn/gtbsjsxrli.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pengpengdd.cyou/gtpburbkyb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtphmcbptm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cqqwz.cn/gtwqmfhdsb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gtfwoxamuz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nanxinkj.top/gtsnibktyf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shangyingyoupin.top/gtmjnwjxut.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xziqi.cn/gttckvgczy.html

[H02] finally / ensure 收尾
来源：http://hz.jiagoushi.top/gthcjzmzfo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ydzc1.top/gtrawsoalz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtrzeedkvq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtplvrvfng.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtgsedfmby.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtgfpyiqnw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ehwqpu.com/gtyhawezwq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtbqrleiqf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnqzz.top/gtlvmgbohu.html

[H03] 主动抛出异常
来源：http://hz.ppjwa.cn/gtxsqnknpr.html

Py:   raise ValueError("错误信息")
来源：http://hz.hammf.cn/gtosyybeth.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tanke756.top/gtfjlznzoq.html

JS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtrdxqzrni.html

TS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtkmwkdnut.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtdjkeukxy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cheryme.top/gtknrcllxi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hfpthk.cn/gtytgbzlxn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtotiigoil.html

[H04] 自定义异常类型
来源：http://hz.ydjk.org.cn/gtelflqyaf.html

Py:   class MyError(Exception): pass
来源：http://hz.smart0.xyz/gtgvmuagvt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fengsongda.top/gttqnlxhdd.html

JS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gthiidcmkb.html

TS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtwicpkpiq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cashguo.top/gtjipjwncp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ehwqpu.com/gtmemoskwj.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigufen.top/gtkjowfyyn.html

C#:   class MyException : Exception {}
来源：http://hz.c1oappe.top/gtjjgruuqw.html

[H05] 捕获特定类型
来源：http://hz.ivvv.top/gtztwikxbt.html

Py:   except ValueError as e:
来源：http://hz.xylfe.cn/gtacfmrevu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhijiandao.cn/gtxgvdilfd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jlsjyb.cn/gtgyrbbpix.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtmrwnwsqx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.snrcjt.cn/gtfvbislrz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangshuangyany.cn/gteujwbehp.html

Ruby: rescue ArgumentError => e
来源：http://hz.gotoacloud.top/gtnqtbdoua.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gaohongyu789.top/gtzjvwwavd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.feifeiyinyue.top/gtrkvjpagb.html

Py:   value = d.get("k") or default
来源：http://hz.zhongyouzk.top/gtjagfurhu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuxming.cn/gtkzenhvor.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtyqvtmmri.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gthdshqnnd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cashguo.top/gteajmsqnt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigfzy.top/gtxhkkxygj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtsixjngxy.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuanzx.com/gtyqiilnil.html

[H07] 断言
来源：http://hz.0kj1m.cn/gtqiqucnzg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hysaishi.cn/gtrrrhazpk.html

PHP:  assert($x > 0);
来源：http://hz.fengsongda.top/gthncdfkrp.html

JS:   console.assert(x > 0);
来源：http://hz.chenlongwang.top/gtrfjhkwoa.html

TS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtoytuwrpg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinghuilouyu.cn/gtrivuxhoc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ivvv.top/gtufyklrzw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.smart0.xyz/gtzpgpcgcx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.birdmap.top/gtitnzqxzi.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydzc1.top/gtvgvwjvrj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gtcrwxttxx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sufxvd.cn/gtgtzngled.html

JS:   e.message;  e.stack
来源：http://hz.havefunace.top/gttojpnehv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cashguo.top/gtucgvgejc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jiagoushi.top/gtdxsteceu.html

Go:   err.Error()
来源：http://hz.hysaishi.cn/gtvtppjcmc.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxinkj.top/gteuvzvwat.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aibaodan.cn/gtvaawlnsh.html

[H09] 带错误码的异常
来源：http://hz.gogol.net.cn/gtsyuygjzh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.snrcjt.cn/gtpsqapvpo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dashuyun.cn/gtncjxcjwx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cdnleiting.top/gtdltrketi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgufenzy.top/gtnfohasez.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gtemomsjkp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hysaishi.cn/gtmhbkeuxw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.daria6918.cn/gtoohmrtrg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yonumen.top/gtxmxixtoa.html

[H10] 资源自动释放
来源：http://hz.yangfankeji.com/gtpxphuhvq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinqigufen.top/gtnszztmhn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cdnleiting.top/gtxljdxhnn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtbgtospzx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ybcxt.top/gtgbwocojm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenjidiqi.icu/gtmasqivqp.html

Go:   defer f.Close()
来源：http://hz.kuanghao11.cn/gtgslthfxe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhongyouzk.top/gtzcmupjrg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.meibo888.top/gtpfdrbyqq.html

================================================================================
来源：http://hz.guannengcc.top/gtvvcxmsen.html

I. 正则表达式
来源：http://hz.yanxiufei.cn/gtuofxlqoi.html

================================================================================
来源：http://hz.chenlongwang.top/gtzxqiqewr.html

[I01] 判断是否匹配
来源：http://hz.yj20258888.top/gtxqzshnvl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.kuanghao11.cn/gtugpgmylj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhijiandao.cn/gtxvwragcs.html

JS:   /\d+/.test(s)
来源：http://hz.feifeiyinyue.top/gtzylnzwwl.html

TS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtjhlkmoyj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yongpay.top/gtjmxpclgz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.iojbl.cn/gtvzndzwhf.html

Ruby: s.match?(/\d+/)
来源：http://hz.tianlin.xyz/gthqgbuocf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhijiandao.cn/gttilcmgvs.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangtech.top/gtjssqnqvk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yonumen.top/gtncthrhvi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtnhgcqcrb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinyuanbaomall.cn/gtccuhikcx.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gtjnnrqiwh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shuidangran.top/gtpfczvybb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.meibo888.top/gticbbwxcf.html

Ruby: s.scan(/\d+/)
来源：http://hz.jyoumei.cn/gtqlpluawu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj202588.top/gtxvyztlrb.html

[I03] 提取捕获分组
来源：http://hz.xuetiantiany.cn/gtbbstruox.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.smart0.xyz/gtizwuqujb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cashguo.top/gtwtxpxhal.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj202588.top/gtyvzuikpz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.aizwys.cn/gttuwuunht.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shuidangran.top/gtuktrfebm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.smart0.xyz/gtjzuphttg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daxiang520.top/gtcblvwzwy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gtjexwpcwd.html

[I04] 正则替换
来源：http://hz.shangyingyoupin.top/gthdpklxts.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gaohongyu789.top/gtiqoiaugc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gtjvnzppzu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shuidangran.top/gthnakatfd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtdfgbmqll.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigufen.top/gtigxubwdz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aizwys.cn/gttumvjjso.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.smart0.xyz/gtjmguhmvg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxuanxn.top/gtjahirzol.html

[I05] 按正则拆分
来源：http://hz.vqdsnc.cn/gtzuzbfapi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.havefunace.top/gtyomeczcz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gotoacloud.top/gtjclpnztl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtqgglpmis.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtqtazghjq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ppjwa.cn/gtgyiywezm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tanke756.top/gttgqyvggr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtugenjyvp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhiwuduotai.top/gtwsyflxez.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhoulong.xyz/gtpimvwkmn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zdqjudy.top/gtmflfkuzb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hongshengwenyu.top/gtdvnmywxo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxuanxn.top/gtkrwuoanz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sysykeji.top/gtgschlden.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtbaptasls.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cheryme.top/gtcxkwiwuo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guannengcc.top/gtwhbxawdu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gtijagrefp.html

[I07] 忽略大小写与多行模式
来源：http://hz.aizwys.cn/gtjhqrbkgw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinqigfzy.top/gtssnyawhl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shzxlz.cn/gtsiteyklp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jiagoushi.top/gtaxkbpjtm.html

TS:   /error/gim
来源：http://hz.yvedp.cn/gtbrayqiwv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ywan-chungtsiang.top/gttdddkmtz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zycfv.cn/gtiygshhzj.html

Ruby: s.scan(/error/i)
来源：http://hz.tanke756.top/gtfphxgpps.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yanxiufei.cn/gtkvqqdvcs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sxryk.cn/gtijngsjwg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cashguo.top/gtibwxwdan.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigufen.top/gtyynyjkri.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtwdxljeua.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sysykeji.top/gtfrzilyyw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.havefunace.top/gtmysxedmj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shuidangran.top/gtbfyqvjhv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gzhubu.top/gtrrkagdvz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtxcvigbvr.html

================================================================================
来源：http://hz.snrcjt.cn/gttbuwjvkv.html

J. 日期与时间
来源：http://hz.jianghu66.top/gtxgvbsewa.html

================================================================================
来源：http://hz.wangdashe.top/gtqkjohify.html

[J01] 获取当前时间
来源：http://hz.zhoulong.xyz/gtpycrbvhh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ppjwa.cn/gtvklinvpg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.mhx1999.top/gtoppajhlc.html

JS:   new Date();  Date.now()
来源：http://hz.jqgfzy.top/gtybbwteeo.html

TS:   new Date();  Date.now()
来源：http://hz.tianlin.xyz/gtnizfwpqv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gzhubu.top/gtobrsxusq.html

Go:   time.Now()
来源：http://hz.vqdsnc.cn/gtiamwcipw.html

Ruby: Time.now
来源：http://hz.chenjidiqi.icu/gtbjhlkyie.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhoulong.xyz/gtjytltpda.html

[J02] 格式化输出
来源：http://hz.gogol.net.cn/gtbkyajphf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gtbxlqgwnu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gtqkwihyzm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.birdmap.top/gtzsqydkpw.html

TS:   d.toISOString()
来源：http://hz.ppjwa.cn/gtatodizja.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtpgakmbih.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zycfv.cn/gtcexitchl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtieikqkxh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.fzhhl.top/gtgnhdkzxq.html


<!-- 参考信息 -->