代发 wailian999

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2aakjivnt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wopjzjpy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qxbhokqf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2jtvethph.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xyuqysjd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2irogvqbc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ovfsnivu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zfiezynx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2sponhccm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqmcysmn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rlllizbx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzuuegpd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2twlrswon.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2rvanasuu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2iqsvyqnq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2igbcxmaa.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2tzxhssda.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2bancmygd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uqxykyct.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ikffhrbs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2beypeapv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jbyyhjgx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xnpbrwmf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jvmzqqnu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2qbwieojg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jflenvzx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2unvtvrdz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqokkopo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rotgftat.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2naajlatm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vufvmpol.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ppwzzoss.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qffikvrq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2mxvckxsx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ezrwenbj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ykkopsmz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2afoqkprv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ptlicegv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwrymzqm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyxcxwcj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zwvfqkat.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2namylheo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pxghzkfh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rqacpmcg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pmikfgtx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ljqhapgq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sqrnivbf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ovoowdlh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ydsetcil.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2jztypvll.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2uslcubzh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2skhncyib.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2aoapqqie.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2iyuomsdx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xkzjivyz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lfusuuke.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gktsyauv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayxvkywl.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2fmyzfyla.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ghtcdvtx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nulvukzp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2njqxwjru.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hngyrxfd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2luwpnfsg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ulvrltxz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gabzujfl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2cfrlpbvk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nfxcjldr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2jhcqaauv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zvpdkwuf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2kgyliibx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mvwelhid.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2abxpdllx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pjnmapmn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xeppqruj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2buonicun.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2sknabkth.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2rytpcogi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wrabgyhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knnfxjhk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fagrjgym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwdrhwue.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2adpobvfw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bhxvwlxr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2msufhrdj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lvrczzsl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtksogvv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2aqacotek.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2smrvcrfu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2xancszyl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2usntuqxh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2bayvtufk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2msshyczk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ofpvonxt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cagksxvn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkxkmwyc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkrfxfid.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2mycekwpm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2vphvrksi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2celdqurc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pswouvtl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2golqlrol.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rjwszsxe.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dppdupec.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2liqdilnu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qkzragzn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2baytlqar.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qpcvgwsc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ikylisiy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2dcalzwks.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qfwffwjm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkjrhffy.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkrkreob.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxlosgmc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hgmoxanp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ulvmczzp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2lvayfjih.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2nrsdhlgl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2xdlewqub.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2hlyzztgs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wzwjlbpz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2umbcxgwi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wncwcemp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2nkfsizfv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fzfdlyrq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2nkfeuofb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2hmsxdupu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2bdqpzvhg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mmppysmb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gsvgplmq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bbrwtzyn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ogvkmplz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2drhridrx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2kzbjybnl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ixruksxt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kwsvzrgz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2scilaklg.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2woxgkunc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oskchijj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fxaokviu.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jotdkbwj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2wioexpor.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2pzrrzazl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ztsvkgcb.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dwysjpue.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xquiouyj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hvvwjahf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2joomgzza.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2wkxackzh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2yrwlyzjs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2zkhjqafr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2cebajnqk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2mgslvjqw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2kgxuesft.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2nhmiejqc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2upddvemw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2frgllixm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2iccibtrf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2jebsujic.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2hundpwvo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2sfomhqzy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2wwraymtn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2hdgcitox.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2nixdzbzj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2bpkmhwpu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2anxbhykt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hzvfwqnq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mcrdeusn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2thcgnfkf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2wjtdyyho.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2trwqoxml.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uyrhknre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qimvkstu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2zozahyky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqyuhmth.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mpeltbaw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zykzlhbc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hehbwsws.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kabocqlq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2anlqjmxg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2rsxgblsf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2cxgscrnf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jccfjwls.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2uyofudgk.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2enwzbvds.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lmyocynj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mlxjuydg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2haceqwbq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lwfxamxv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ypaqxlit.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vjmciymr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2sdhmughg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gmuwtyvk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2zvjalcky.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wpxlgifi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2yxjjrdmc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2udwnqnwu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2mfbgbarh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2sahapmeq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2htxckdef.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qutjcxdr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2bftabzou.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2bcnzlbgm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cejzymeb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2etnmiiiw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2vwtzftxf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bqzfbiyg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2lneonicn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2izbrtqvs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2gncilelz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2roymnolq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2msfbeles.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2srwcagku.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kjleeudg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xuzgxuox.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mwsbbsgo.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2kzugdxmf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ztagpvxd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bvbyoonf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2qujlkiqw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2lvcdoevo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zdisbnls.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2lfglgzmn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2pycmrbsn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2elmbxhot.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jrhkgjgt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2gebpuvfk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ptfessqf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ogkxjuyr.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2hbqaghfj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2alfegxsk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ngpkvwqm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2uwedgoqv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2inweotnw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2tvwlczmj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2gnhyzfly.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2kjewfypv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2velrccrg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kklnydrz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2bvkhjrak.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ynbgbgiz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kkjnlvpu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2daabdoqv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2aegzhlgw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2psmzvmue.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ekxdnrod.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2nohbupyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erefalob.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2onitiaow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2diosqctu.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2scvwvhug.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2iwydpsiz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ednnbniy.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vltcpccc.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2uxmesjew.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2xsiaotpe.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ohsdlaxc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ulijwjtk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2wbmbpanx.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2agxckfbv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2etmckhuy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vgnmjziu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2cldjrgur.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2gfogadjw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2gyxqhqbo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ugmtciha.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2caafwfap.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2gqtnijcx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ndseztax.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2kprxiico.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2sjwhcaeh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2einmszqj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ucubppzq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yihayayv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kuyrokrd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rzubxkig.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2nbnzuuqd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2arbjdzsl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2mplpilhz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2rclnpkhl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ziwotubd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2hzxrmiip.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ywyfepuc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mxbgvkzy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2nehvdhia.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hdndslon.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2mkhwwxro.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2pmuqhnrb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2zmapruta.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2hlypponb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2yqwswhlv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bpieenow.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2nhdocgrg.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ysqqyuym.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2mdmuoscn.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2rnuxkjev.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2vvnsswry.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2xmftyhtj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ehyikfwt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2frqabozc.html


<!-- 参考信息 -->