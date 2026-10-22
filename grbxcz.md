代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vngqvulk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zxmmupgi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bgbguwxb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ywkllnzz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2diijzkpl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bugnlfgx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uxmfavyt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhexignq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vueefrbc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2aykntxfy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qacosnuz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ulpaaslz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mcffyjyk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjmoxdxb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2kplbmifa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2oljtfdla.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pppvkbmx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2injtpiya.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pbpsqecm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tuzkrwov.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2myhbzyhm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ogpcexep.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xkroksum.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jqstfxod.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qumibxej.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2znwcdtoi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jzcgiapi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lfynfdsl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mwiphaxw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wklaecxs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mfevqxvb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gtlnmefq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2crgxyuob.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqywexra.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ljfohkdt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mpirtgsa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uxynpwav.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2owblkfgq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2quptrosg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ukdcspwr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ypdezgoq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvmjmros.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2erixvvng.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qznwquxa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xqbhbouo.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpnjhmnz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2aoejcogi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2qrcpfnew.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ltleerqz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xiyykocn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2czttqtpj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tmyoyyba.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2drmbgnjd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ilftosbi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ogedsmek.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2elnspvrk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cdthowok.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ngjizzmr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2sriwcqre.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2stiygxvb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2spqusamo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2sstrudyw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tfgccrrm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2guovmkmo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2wnrtjfwx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rvpaegma.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2peygoppf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ozjlviwy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pzneecpd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pojbtcur.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2pudqpddq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2iqsrentz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zrjyiiqg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwxaquzl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2toywridm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2rwyyuwhh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nlvjauyw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tvlaottx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ihignzay.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2vfxtzqje.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jgaeopmm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2skjedpae.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rnwfriuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdlzzmve.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2whyfbbew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmnktsqu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2lplabwcv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2fipcknnu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wqrsujna.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlrtmigh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcudwsfh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ualwxbeg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2dxrrlgap.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2zwrpmznm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2okpzlldg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2nqeighrq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ugfmqjoi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzrmzwgy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xzbbanod.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eylcwnqv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2myyajbyl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2lqvvcxuv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jivqbnts.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfmolwzn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gfvqimdp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2eccyikla.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dzlykolk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eepvugnt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2atxvpsgc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2swcbcaui.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ueixogkv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2lvjvkqou.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sjlgjyow.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2lbidnxyf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xnxvmtsl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozzgpogl.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2emopazig.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuituocv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayppshoi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2oqewmsfp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2sfibvhto.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2cmrslgqx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2scyidptu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2nzwcmbjl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zjcbyryn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxrshjuw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgjjgxov.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbmnqfrr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qstdgayz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2oqtmrswa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlkbmbpr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2thxfyviq.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2zmenouhk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fwjtkjca.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yzhubkpa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mmwvurek.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2bonshsaw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2tqmcfdyu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2luqpvmii.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pagpbrrr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2scrxycgc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2yoypnmmn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aothupqo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zdhhffla.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cdxdnnqi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2igtkleyq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xnwclbzm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2rtrqpfrp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fcryyxtp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2kqinbvpe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2tswuuwti.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rvttqqyn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2irxymzxv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2coypenam.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2kbpevasp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2dhivjdib.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2nzenzuhx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ymdenbag.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2luxfgypr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jcohvabe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mpxegsrj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2aceacaxj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2cgeajpin.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzrpjzpe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2qmaesxym.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2dfvwylrx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2pgqbdwfr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2zmogezvx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ecuutkkc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2klpojsgm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mntjtrcy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vvoodpxz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2fguwdxqn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2rgljtkkn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2qtylofmd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nyqaeajc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtytyypp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2zbprmoel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkvkklbj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aktuvxhb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2bmnqibfp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2frfyesmo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrhfzssq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2eatkjdaa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2pvndeede.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2kjijdaih.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2dtovodug.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fkweavbn.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ozbgpvtv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2riwidawq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mzaotubu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2jaobjdgi.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ulnvnumd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2chcqnzik.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jogqhttl.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nqgnuwqu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vfdkyddr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ggbdpqad.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wwrfkxku.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pzgbywtl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2huqjddov.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jtszewgh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ujxiwaze.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2dzcjdlso.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2atauhfsk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2jziidqvu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dudljrvm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2xnhhkmwp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ovowmqww.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kzasvfqp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hyohmbop.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2kvhevlnx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2seylxehs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2hobpnmnc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jurcklmr.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uynryvem.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jbqfimyj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ktmvqovf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2juyxdcvh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2txkpmauq.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2sxxvvrxw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhrtsrxa.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2gbwijgul.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2bhwzowov.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2lvmlpmjs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2okcfnecv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2tzkiwzhg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2mdpjfoqy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kmjaizue.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tekbumon.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2iosczcfr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2pycpxtsw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xymgbpmr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2zkkxaowz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2phbmwezz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2hpnydfbi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2airbfwiz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2vhvuifqs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2pmywwyot.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2yiknmzlx.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2rqotuemc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2naudukpf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2udtzowoy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2wlqlwjda.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2abjghjsl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mkhxceop.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kkdxcivk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ocsgebwa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2uwkauero.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2wlykwutj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2pamhxysp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hclplwjr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ptydawcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwhiarrz.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2wpgmphdg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2wkkvmcvx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bzscgdgq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2inwqqigf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qlyldgaj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2emuscqhu.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ltgaiabu.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2hpqtcjec.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2hvwyswtn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2pskyuhaj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pilhccsb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2lxmnvwit.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2lnttimis.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2fonwtkxm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2duepagzz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2lwwffxhe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vsgfbtwn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2nawvbsun.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2nkrlsxvd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2vacoxvsy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2razibaon.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wayeeqdf.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qyinvnsm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2flzvsuit.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mwpejkln.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nntzbhll.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2vdlibexg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2iobuyxpk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kgzysqcd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2rcyayfrc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2fyrszhtx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2njxlojkp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2whetowzl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yzmoqnzg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ryklndjj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zfilkyjm.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dtojktnb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ytkwbmbc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2brknmsvl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2dbympncq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dickycxg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hyiltzyt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mjvfqetr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2efraianv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2oofjkwrp.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2tipzvfyg.html


<!-- 参考信息 -->