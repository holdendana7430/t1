代发 wailian999

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hboaraex.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2edoubhak.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2evlhpwjf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vhncwnvy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2aqwxxrgl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zljudilu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcppnfjs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfcnbwci.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ocsepfzv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2yigubost.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpizzxnt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2yefwjvbn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lyyaubow.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2itxuvhee.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2brdaabpu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2izjmxcdb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekbdqjha.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fnuemqne.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zbffnvau.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2glznuehw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2imjnwenb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vaaezbxl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2khpwqfwj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ewkpwybr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2unevujcn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2uccfojfi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2sgcrhofd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hyodahsj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qkqenzcx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2mxtqzcyi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jlwlyjil.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2twifxnah.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nxdciyoz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyrvhkmz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gsotmukb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zlejjgrp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rhhthucd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmwcrnws.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pdlbcoxt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bsjvpgik.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lxrgruqt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2srkmsjdp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkmpyzij.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2clhmoejo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2leidawas.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2acnlpcbz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2aeihukkj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2eqsyumxe.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dqgwvfaq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nmbfaklc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wahqynyr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2abbmnryz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ecadpukq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ssqywuxg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dfteczyp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rqndislh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ixatfwbr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xzsxgprk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mlzlpbab.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2spwfzhaj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hmkiieuz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpwaukxh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ixmfoexz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2husxkqeu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2bxtkctly.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2zoffarjz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tsogkkyh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2owrazpzx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tthpfiew.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2brbkmaxl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2keetcijm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2emjqnmmd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ipjwodfi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xnkrqfoc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2btgapgle.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hhyriyjq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2egtmvyiu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tkundtad.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2abruvkmf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dmxplgul.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2yqoydffx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2thjalcuf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jhpcrbdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmtjashj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2oqwiypfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjwmsnll.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2uazpsugq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2txizpzfk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2orcgcnzr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijkibicu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ifjluqfq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2psnahjpw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mdxkbzql.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qsumgrbd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2prpddduh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xkdzcmpr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zcqimxhp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaebwajo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbbjgzfz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsarbkow.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2idrgttzk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2izmgylrh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2rgtgksma.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2varmxysg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bntqjszw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qpwmgaqo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sphsmowd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ttfuhtkf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bkfmqmir.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xfeijsju.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mjjrtych.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pqpybwtl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2asycmvzp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gwdocixh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hbkcmpir.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yrmmkqfi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kxyarqrh.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhzqpqsd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqernall.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2lgtsccok.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2zmhzbaag.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lnwtizzi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2sdxwpjnl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rtvkfzsr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jrjfsnhg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2nvrlgvxv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jzhesvnc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvndrbqa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ripsohnh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2xixwzwps.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2qffzikeh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2vwmsjeyf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2mbmfemzg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2avsvsjwj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2muvcgvfw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2olvvvysq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2uzjxtimu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2oufdtkng.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2dxzbajqx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2eesidksc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2samahiyv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fucqzlmz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rvoqvzya.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dzaouiqh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vlxoyakj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2cpwpffjl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2yfccbqns.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2dasskbcl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2exscltxz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2osiiaxcu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2dwnhairq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2fictisaw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2vdzajkxr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2abrhrfji.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2mbmahufl.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2uhffpoia.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2nldppdmo.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2dmheqdbf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xtruxwwp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2evkjytme.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2dcwxteaw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2wdvcgeek.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2oanvzqtj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2eaeqoonr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2fcrlejim.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qvdsdvcu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2vbkdspse.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zrxlnflm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ajomefql.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vlzpdgqe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zjikdmfk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cklhsjqi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2oqmrrocp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2qclupuln.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2bllnikrv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2npeyjnbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjxavlsv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xgsgjiyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llsvnwof.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2onkeqcgg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2hxuiwhpz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tdwhychs.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hhbcrjwc.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxogjajs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2edpfwyhl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ncmoldxd.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2alyzjmdz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2cpngmchg.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2rpqlgtqi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vncdsktp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2tejcvqza.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2pwmifrrj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2eehlyhoc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2teqsdfrj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wwhoffvf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ttongxlo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bnfgwpvc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2fxxcbpmk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvfbuzee.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ynjcmxmj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2efjgcoka.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dztlpokx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2usorndef.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2extssprc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2hgyazzmx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2kiwnhquj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2fgsiwrab.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwlhedey.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bkpagnnj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2piyunjww.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2acsitkqm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ftjnifpe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2fkkebcab.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2xnzmgxwn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vcakfrdj.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2xedzoaae.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gzogqege.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mcrhzzua.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jnhrcfcu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2bfistkri.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2tkhijynf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pndwyszd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2yxvokvjz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2srhopdkm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2qyjnqffx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zcbbczqr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2yrvxhwfv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2obbhypml.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2rhwbryur.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ctxfssoc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ucddbtow.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2kfllbkyl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dminkcbg.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2szalrmab.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2indqwmme.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wzigmyyx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2guxfcfqh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2dfmtuikb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2esgwiwny.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2qxwqvmgg.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2rjxapvee.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ngavorke.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2wkodvlmu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2dcxhkrcg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2nqsplxbn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fcwkeqkc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2xtlgnzyy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wgxwillg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ucjrtyjm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2qbottsjw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bwoyyurs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anjysley.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2vbbedksc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czwntanh.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2hyizycwo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2bcejctqq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bbkoigxu.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2aslexyqo.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2fnibrmil.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ddaehyhm.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2pnzpgazu.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2xikddfdy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2baixnejl.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xjnywppo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2nbdcgghy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2vfxznczf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2yqesqarz.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2jeaersts.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2tkbfdinq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2kfldmsgx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2nnfrplaa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2pkqqzfjh.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2pnehvrrz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2rhwmxvqm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2bjxakdmu.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dmechbeg.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bzrpscpc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wsqqnyji.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dqlaqfmc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nvodrmrd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2bomvxxnt.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2mfmacszl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mmkyxnoo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2kyzcnroq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2kqdkwpek.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2jhwybwlh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jncwsjno.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qwdbtqbq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ovskdjlw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2grljambr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2kfmkmgug.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2lihszavr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2faxrhzzh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ilknqncv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2xsjsexpj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jdeaocgq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2turwqxfw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2amxyjtvz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jqbvugad.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2nmqjfptf.html


<!-- 参考信息 -->