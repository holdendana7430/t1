代发 wailian999

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qkszvgss.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lugzrqzw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mfmqwddu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eounaixo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2oenanqoz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2koutmoeb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwqlpjbp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiqznuan.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iimcegnd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kqutduhn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pimixwdi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cotdmaks.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nfycolpl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ytifejke.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmljzikq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hhdiwxmo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2daliipys.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2dhpljkwl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2sxulsyun.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyghvurg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2avdczllb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2yrnarptb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afuukzjs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wpszsldz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vrobrkqp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gveuuxch.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mmczojyq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mzwxubjk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fzqnihud.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qfivfbhv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vtblhkvm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2yktzapcy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vphhpltg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zpcgewco.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mvekpdip.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2sjhvmura.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2cweozcmv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jkiveiny.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ippgqxyy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lnnldttv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2sstybhzx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2odejmbvf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2urjteogb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zrftnmcu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2pitkbbxr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xtybqzyt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qxypcetc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wnsosrrq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2bcnxqtru.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ujglhlht.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2eacicpsx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2nydznvfq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfycssqj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2yekffdmm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2lcbrkocf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bufpuout.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2coffdcgy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dsdnbvsi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mcnshlcc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2aquztpqa.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ruassukh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2cmjcdxvd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2iurfarfd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ncnetnps.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xeyocdwn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2pmiirysu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lzuedmbt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gxeeomae.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2efbskwzj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2whamscow.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oejkokqt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zkxvtpxf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ijxtlrkl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ewiovtth.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2attiweam.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dezsbvty.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lzunkbxc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxdtztlu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mducgnji.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngazcsdo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xffxhjan.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tpbtmhup.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uiuuqgkk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2efsvivpb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2icwfughq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vuzmpvru.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2toaoklle.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zljgkvco.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vroflljs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fzbtygrj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zpyujtuq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2pixfktmk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fpgokuia.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2shppcjjs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2raqqopph.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2itcnpqnc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2nhnebsfm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2yuloufmq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2oqunpgzr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zcgbhngo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2gdsgwzqb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qldrpbiy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mmpctbuz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hupoczkq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2gbtydmtf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qyxuewet.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zkqxuhrq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2utqxjswk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ljahxyyb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tybmxadi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rzkridji.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2raqzocpf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cgzchygk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xxzsqlkt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nvnfcwsn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ikebqohb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2mqabuocp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qybxxakq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wcydfhhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yafzvoyu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xtidnvur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybfvrrur.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2vkrwdfat.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2rqgvyybw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvjzinzm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2glxiqxnt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2afwercky.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2szcwqupx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2swtovipu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2utwivdpm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2gpnvhowu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2mjpmtkba.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tvlbmxdn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pirsehgb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2leggzibv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kisetuia.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2thbcigvd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2nukuawmn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fywecnot.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldqyxxsx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wxmtbwoq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2fyyjpulh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zvxlnpre.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2craaxnbb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rrsjjbiu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ivnwvfeb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2qbglpwqp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jyrqfofo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rkhkguls.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ersvmabb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2npfrxqar.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcsvmted.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrlqougl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2eiquovmj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lypnkhrb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2xycluyen.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cnegiuxt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2kzsgngoo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2lxjznwhb.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qhhknciv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hfqfzsuj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvcdhgcw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rehnbdum.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2krrpkigt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2dglwozzh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2uizcjbwn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfwhvzpu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2qnrndwlj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hhynaejc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2raqjfdtl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kulkuvyi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2attpikbk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2mikyapgs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2badkingp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2qsocoqci.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2hbkfrfhq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2qrwcobjp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2rxgwblmc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2akgbwlqd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ibydrzyw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hjnbuzwf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2zqprdhmt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2droiboie.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2zvmktpxe.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cjbewyin.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2hjnnxslt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2smyhuskp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2igxdoufx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2cbnjhbtv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hgijapnw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2brtgvjin.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2fziokwjg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2tmzsdjho.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ghxqxumd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2tfnlkbhr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kxxuozws.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vhsxdylo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2gzngmlgx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2uczqwexm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekniohoz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2unhmiaak.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2dxionhan.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ritydbwp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wpvrwggt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2zdkfultm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2pgblgnpo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mvlukngv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tttoyclx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ozagupkd.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2jfrddprt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2dcavsihp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hezazoyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2armivolf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uqyuutdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vttyljvh.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2jqfxzpvu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zwsnumsz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tbtevrfg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2neztgrbn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qluxphzp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2fsyocmay.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvovzajj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bpzmkxdy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hjplsmde.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2cjhynaok.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qeqlpjyv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2egwqxaun.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2vnkvsxxz.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mpmdwtvc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2wdaweoav.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ppbtctfr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fsybvahl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vfbzxwuc.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2mavyhejs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bxynpfyd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rvjcljnw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rqupweig.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2gmkdoygg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2tasqfvzv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2bduzfpjo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lpnewxac.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2rywouncm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2jjlrexyk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2euarezkv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rdzklnbu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ejqraums.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2iobpyaum.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bexefkym.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2grmcyyob.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2oscjgmwu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ydyhkqbg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2dxbfezbi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ctoxvpmq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dzslopwr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qoxtxdzi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2sygegrud.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2dcoqxmax.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lfztjgtg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ophjpirw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2wghltfnr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ashltgnr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ijwljowr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2cqzwzrjg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2arxdcuyg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2juiwfjpf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ruzutfpn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2xeatcmjh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2sqntcwvr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mcrwqkar.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2zdgasxnc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2rlpxvbsn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2uwayqkop.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2fjjuqyad.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2cjzutxoj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2tyazlynj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2habvkwrh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbftapi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ogelyxqu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2jreymbvb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ysxyvyzv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2unlynzhg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2yfnkywih.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2nrqfajij.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2wligiyww.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2syqqkpla.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2rdkwusad.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2esxwnprp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwpzlcvu.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2nrxfhoxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzwghupf.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2wncimkkf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2dpxzactx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jeswswov.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2khzpurvs.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zodsjyfg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qysqujom.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2qfbhddur.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2zwvbodgh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2lzvmffcj.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2sbboulzl.html


<!-- 参考信息 -->