代发 wailian999

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dsdusyrp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2linhbnkt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpcanzgs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ghrzgonl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2oxmlqhik.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cvpbcrgb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtmvqrnl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2tucitqyb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qscuxfps.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2olvlenop.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ubmsqrrp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkjuxdhe.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2sybapsfc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2rtbsthyi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2lwchpfsr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwvjljlg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2nvfgnynr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mlewjkni.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nsojuwov.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2uinahlen.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2isccruxn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dojrycir.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2qcewjmnw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qemzeogw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hpjfimsv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2voqsvdkg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vfslrcoe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ckmrxcjy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eubgtpom.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovxuyceo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvuutsxt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cbuvyetk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bdbbspfm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2svajaqdx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dnohgqts.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2axzakkzz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uffxdtqt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgaphmnf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnfcqgue.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxiiaccp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kttfqqom.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2enljjmrs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oezhshsm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hcpdoldy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2waxmykkj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2exwkzkcl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aozbpldz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kzahdcba.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2byzczvtm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zwmhsvqm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2shiuxhzq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jfclnjxy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jmpqfyqe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tkmpzxsc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2neexahxa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qmzzcpyw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zopyzimg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2scqsvbja.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2zfcxqbjd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2iistjbyl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2tfayewks.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kfdsapef.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dbmwitcf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jcrwlfio.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2zifdzzyk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pkuhewcm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2bzfyyftq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2baypxjtv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xcuqwsxd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wgnrzluy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ezeyetql.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2evtuvjgm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vdzcrtwz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mgmxmotd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tvvikpkv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2johplozu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2quoqppzo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pkixfmty.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hhngzvla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhafjfzx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vneempud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhglzlzg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2dflemqxj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pxqcbjlk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2goyvgdmt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntbbfnwe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouzgczyq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nutzlqjo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2iosnijfg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2aerlshae.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkgzgbxs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cktikwpr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qxmythhr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zuocaccw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xafnxibs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2chbtnrlx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rbhpgeas.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ytxzeija.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2puufxylt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqcqthde.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wsbhcoay.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2aqesdavc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ocrelors.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iqlbhzmi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2njdxtjft.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lhwufykq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2eiqsvizf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2floqwbuk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hjpefdru.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wgbplkuz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ytueywsk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2szgfnbhd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ppvfkqfm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgeweuta.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2typvbtkh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2rbbjkste.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2webiiwsw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2chvvzokc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gpkisnkz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2kzucjrpl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hjrysfse.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2phybfozv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rkpcmryz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2nfqjngue.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2obajzprd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2bdhyzpek.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2jzstujgd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2bczyouem.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2yfbyioie.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qxkvbcpf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rgnbpgqg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wrfgcrtq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2sxywfeme.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2inkypweg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2rhcgmhry.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2eacindil.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2jtxtjxzg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2xcdfgnku.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jhenpwcl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nditnuel.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vdditnli.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mnorueff.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2nckoltgq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2rmcvqkcj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wmshlskd.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qszlhwax.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2idoqyycn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2unpttwnl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2bzmxgzes.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2dhsgdyem.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2obcpcdft.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2dtyjcdku.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2oofyhwiz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zgvhiosy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qwnkdmdb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2pyjxwntd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2cawilyfq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vsfiiyfy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2hzkwrqbi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ibpfrisp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xhbfrgat.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2solxlkck.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2lgczxmsv.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2hqgxzrjf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2pnyefvpa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2pzbemrtq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xnhrwidi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hjslegef.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2rlyvpmxb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2hqzmaqpk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ekwqnefj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bjzdiyes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfwpwgxw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2uxsohevp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbdbkafg.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vsnbzael.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2aqotkxqp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ypsczwtm.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2uhiretor.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vqowaizo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2vsbqmxiw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydsvgeii.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fvzmibuk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hyddzvib.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2mfarbved.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fitqqbdg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2soyuhhwi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2vedtncwx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2tgxmmwzs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2udgtrkqa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lpuetmav.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yuzekqal.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ffjlhthc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2yoowwwyk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2jzgpfykt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2dhouxihr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2yeokvdrb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ueszzyqb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2gaixvhqc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2rgqkfceg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gcugmjbs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2obdsrngi.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2tndyhjbk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2bbutamli.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jtaprgth.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cpbbrsrd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xdhwcytl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ztqnlpyn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2whzkbxbv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tbxfoqpb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ntpwvvut.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yovsjhof.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfqgvyqk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ygmslcew.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fyldnebe.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tspvvwyi.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2iuladkmh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cbgvngpm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2izwcoluw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2tczhiqkd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ypsudldu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nnrxfbca.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2yqaugkhf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kdlibmgm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2gvjkyjgf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2aehxinib.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2mvycxqda.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2znubhkof.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pqqkgnmu.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2zfrcreyy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2qbesktph.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dvstjdxx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2qnzcghzv.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ashxgtky.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2scjnnzit.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2xjnodfwa.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2mhtyqogq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2jigvplvk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bvbbulgs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2qzpvdlpj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zylwewiw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mifoalbj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xyhcxpox.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vxqetlma.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2touzatnb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2zhurluqd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2fulsfduw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sawcycri.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2gzjdpfod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqbuefap.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2wnmdmcas.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2yflhtqrr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2cplbbikw.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2zmmuwtgj.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xitdumbx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ctevshuv.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ornhdfab.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2znybzcmp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2gehdoanv.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wtsaoirt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ahgmzzui.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zzvvtwmu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2hxnxaimx.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2hizphsvn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2hvgrqmwj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2kmkjlrbo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2kwdwxdjn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2xpshfqmg.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2sehwudim.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ktrwfvzq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2hakrvzgw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yozyjmjk.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lrecqwsw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dlyfnjfz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yytbofsb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dwzynixh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2cxdfcrpx.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2uccetvgp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hybujitn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2lnwxdsve.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2kjwhydjz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nhaqebfd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2nxoriymd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2vvjgvdwv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2zrzvkjcl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2piegugsn.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2cmcygjxi.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2jchzoiln.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2hcmnfcrm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2wuuxfwok.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2eskdhtwf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hupsjejh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tlprsbdb.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2glfshywk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ponhbnwf.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2bvqejmfo.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ljzzhwir.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2sggbgjrg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2fgtvzrtz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2zxsalqpv.html


<!-- 参考信息 -->