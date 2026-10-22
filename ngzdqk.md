代发 wailian999

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ouvbdmwt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ldnvqgye.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tbmlyaqu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qmxfnxkt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2smzniwaa.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eddjhbjw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ylngkphz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hxuaigck.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2umpjctuh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dluhaznm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uufuxbbp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbghagqh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qxbtcdqy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dfvnkxkb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uipbmppd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rhebvshn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zabogvhs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nljrlaqy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2uxthzrlt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzokifde.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxxzcktv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ktidewyr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2doyubwwo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2aztaelhb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2gpbavkqj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2upjtvzjt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xipaxdmz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2vgnfhmkk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2trvevlio.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bjjvhxis.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ktnojptz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jautoksc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wtbxrwot.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vwixbxzn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2nwsmobld.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vvrymzla.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dimyvnhs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lcklecjf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyubhorl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tsbusxzt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ydoqzpvt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2sawvldqb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jrwqulzz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2duhllsbj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnvxddrc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2stzcxycw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2whxxznmy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kecesgut.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mkrmuhcd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lzgbawfs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2npnjkzxq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rxazyiio.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2aabnyler.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2abkjlkua.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sszvgxje.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bmjxufym.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dxzpxyyz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qybuerlw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ztppfdvy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vvvyhqyr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wigqybho.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ubywxkve.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qllbwztm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2iminyhzm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rmdytmlw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgwlztyn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ownijame.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2sfjcwpuz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ecbbbzmh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ivvazbdt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xmyeqbrm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tybgcwmn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2oscpsjur.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xuhdduvc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qasztuac.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ufqscqpk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2fczmtyjw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhxgobhl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2nhjwfwbr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2frrhdaun.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2kpgkdjsx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lforzeno.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ccnepljj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qalrahnr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2whbhwqim.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zbtlqsnc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2uzmkbefq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgjptlmk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ftbwgwud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdhzrmrf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2jrijwcjv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ojejbmnv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yauasofb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hrljyipe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmvfzsxv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxyfpybl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2pzjbkeaz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hnwqfsuu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2yoaebntt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2nehzqtpt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2byjcblhk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dmjmwlzu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ajmnnmek.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkbieaej.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2utveijqq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2cwzjsxnl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gwnkzyyf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zynztvbc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kelctesk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2lodxysot.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vfvkydmr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kqzjqlvu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ehrgiavb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lsisndud.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2irhwcksc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xucojpul.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uvfkhfhi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2lfjkqnpi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qtyxmjme.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vafbytcx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qaspdpqe.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bymxzjra.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wuusrlox.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2lydtuwma.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2jfavangv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2waoxhsjy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2nwmtehwu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kxzqbtjw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2qwghmaod.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2bqnuzwmk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rybnvbzc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvohzvwr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2iknopmzt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2fclqpeti.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2lhefokru.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jqkjuihw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2hgkluety.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2itcuuuov.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2oijdrudi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hcrzhsyc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2mffxxyeu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2gikslgyn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2olnnhxgr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vjixuckc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2krjgqypv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wwpaocbe.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2llwcjmov.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tlntwibd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ucbxsjje.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2xffesjbx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2iriikmcf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2mhbizhcb.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fundjzgi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2aouqzgue.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2twnygrfz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2jabhzlpk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2mosjzqtb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yrzsnawb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2thlzrlow.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2qaxjybcz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jxknhctu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2aqkapwwx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2fmanonaz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2eiknbxgj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2prfpxbyg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2xwfdfizi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2advoehsj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2rmbdadkq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2txxjgaxw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2bmjazyeu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2dqfsgatu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2tugdvrga.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ucjolesj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2jdixulqy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ocobjtvt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vhhruioy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2cyfibpej.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2vlkqnfyj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2iwtukgsu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2auoorchw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amrnnfex.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mbxkzdua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppgtoaaf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vpnjjxsk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bkqzxeqr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cfqaergb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qblsxkut.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgrwgrja.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ovzfntzz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2lrqqpbcb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wkmakdtw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fueiexpi.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rqojdsyo.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2eskmdiql.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2uzfuhlji.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2pvoungoq.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2rzqbtbwe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2nhggqklf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2azvwjwsf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2iohfssjt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2webmbgcu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2oyuvoufh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ngulgudh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2adoubyak.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hmjaczjd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2unjkcnsv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vumjcatn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2jbcptukj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uercqsjv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2dbhudojr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2pnyobixx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yccjkaaz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lbvjxedh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hcoxsfkc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mmmcugjr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cehnyckt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bfiulwan.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2okeroeih.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uiwiiiuu.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2rdgnoxlr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2cfrprczq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kbjfqryx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2aeszeipf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ljhmksrr.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2oqocxnng.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lwhdodne.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tquotyzw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ipgczjvu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2xtqypeef.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bdfwzalt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2bqgxaglx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2btihtskf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2jcxvozeh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rydwuqtz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2znsdvxvx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2tkeocdkf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ssfmxxjv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2mysihnba.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2wbnewxzv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2slkwxnya.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2lqchvats.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2tteytuqc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2nceclnji.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2dotqvrre.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2zkvjyrsp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2rfpkddrl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wvjnbhkw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2foincxmb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qjvzgadh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bfpmuvcb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2rusodkqj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2okjarpww.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2huypholj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2iwotdxhi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2lllucywi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhjwqnbh.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2aijulsjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbxoyfhy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2nbnmihgg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2wzxpihdu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2gafwtksu.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ecrnyyfz.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jeffeowm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fiodcyzp.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ytqsxiep.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2nzstqslh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2lewkkvul.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zvowlvbk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2wjydrtht.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2joecdlnb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2dlxryslw.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2qiqkljsw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2mrnqurvs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2xhnjrvue.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2oezlammg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2dqlxbnis.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2yxqhgtce.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2piaqvbmk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2bygdariy.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qjidtrdy.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qdlpymvo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2netysoqt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mdxnmjuu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2piyxdrse.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2nngktkmq.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2gqetrrlp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2eniffvcq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2sbtcneyx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2iyejrgjr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2vgwcuxpj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2enlddwql.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2kabfxboq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hsvrdglg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2oszrqjpx.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2fzfmxzrl.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2hnckemqi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2jljrzmrv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2inlyuyff.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2piqecpwa.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2aiqngzbv.html


<!-- 参考信息 -->