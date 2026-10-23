代发 wailian999

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmkuytxl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3sbijzrgj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbdemdps.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gfiqrwki.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3unzbrftt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3pcrhdtki.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tucldabf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3isgwpfpn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xvcdqujd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3esaqxzej.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3myrwwbak.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3epkmlzho.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3slmhmkdz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lvlcqxta.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xdrlgmbx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3atpyzhzi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gmplecbh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cmdyruyi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sremstnh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3mpumblny.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bdplhqii.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kszaisgk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3dlncalng.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3afgfzalf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mtyetzlq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3arzqwdpj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3lkzuoldy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rilhoklo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xcjlwotp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hnnaxweu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3biernauk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hwqwqnyc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3joxehlpr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3iazweydc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rajlaohy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nkulvqhr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiynlhwt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bwvpswzb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dazxyftz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vzvrrotc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cbpdtnig.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rumywsis.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3okcjxhml.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3anliuivl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3pduhluqa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uknkhukv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zdtfftyd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3obiebhen.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wdzfwumg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hxsspxao.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3lrtdsiuz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dqlpmjas.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3owktmbtn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mcgwwjdd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bthyvqou.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3shogqpin.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3dzqbenty.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3opjtkruz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gfgpnzzx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3gshzybnm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3fmykkpnz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3wzefjumx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3jvvftrin.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3arubwduj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3pimslfwi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jjemdvtj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3cdlndnpq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ztdbxkkw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3mcjaoexw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qtumpjye.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zlrjfbbm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wxuhfyml.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vqbkeiri.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bxdzrvxo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sbiwxbeb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jfyjlgck.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3jxkeudhn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rlhlykzl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rsiasowe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cypepwjg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3swhiczhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yroaotnr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3qclytdvj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3vtsmrsdy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3fhwhjdrr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nykttagu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qcnxjmki.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kdzteqrc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3zsblgwqp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3tuykkejq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3eyqwsiif.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3vdbrkhgc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3rcmvcyfa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ikibttqw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vxkhudmp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzplitzo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dohjzomo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xkhqwrnc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3lmngaxfm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksvajimx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fsvonsoa.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rgloiclg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oovleris.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3emrysgkz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qyfhmuse.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qccrulbk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ytjnuhuy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3flqmuqzs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gapxddsj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3lqxwfhya.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3nnfzwiug.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ikqfdxng.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpqnvwma.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pegzxkfk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bmhpksno.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3quwhcasv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3egoeygov.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3fgfcxpyh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3fuzppeux.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3uzoxgnxo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3gpniinjo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3drdovhwj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvtgzehh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ymlzpgsh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3fgoyjeeg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3zletugeu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3gzqguony.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3xnihuqmg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ioxbsomu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3stjmuezg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3owfeowrq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wlegtjdu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3gxbxvlyl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3qejcdaaq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3geprpdsu.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wryoiraw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3pohsvgjk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3avvlamdw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jslcztts.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rtkyugft.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tnsxzjtu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3rtndxjgv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3vwjlozmj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3wzhunpnk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rryciqas.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ecrxnnbc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3baszxxao.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3iiofpaxa.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3zbdgmohw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gjfyqkze.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3nmaanrga.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3actfznqr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3jwsnbgkj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3txqhutqj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ydrkpbbo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3jtgzmuzh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3foqvpusa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3yzpczpaj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ugcskvdw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqixejza.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3mfyawbcv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3igguvlos.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3jshtovxu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3esqynxtp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3odottzas.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3hhlhbpfx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3unphkrdy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cuzkttiz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3rxvotprg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3sntffnqb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3lczeoxfu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vbyugxxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjoeuxtn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fgbpunxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3runbwpky.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3clxaxqqw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhqehvlf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ucjfrepj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yrsdkzxp.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gxtpdqou.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3dcacjnkt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3vjunfgrd.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bvsnzseu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3znvwimqj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3bimvwtvd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gfsljydx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3dvsgujlk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3yeksfdpn.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3obqxkjhf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3idcrxawt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vuhqttfj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ztsrdamd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lmplgoys.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3zbxecamg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcfpznac.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ioylayaf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3nrfgqqmw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bamiauny.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hbfuxdgs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3btvesaqc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ebhyjvth.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3hqatbcxh.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3wthlsnvo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mveemqvn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mxipufdw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3dbshvnkw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hczdxpud.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3dbhjxamr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ezdehmny.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hlxisrag.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iiquerqg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3glqhjpvc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cophfxtb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eitpcdmq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lrtqfhsk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qjxkssbr.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3kxyzrcni.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3lgkccxkx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3iuaytrrb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3hmstdyqq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3jqsgrppt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qjwehnvl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3mgcglpwi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3dnoltgua.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3sdzppgem.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jmpgwlux.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3aaksnmki.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3goqanchp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lwqwnsuh.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3cqfxlotv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3rfubirja.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vueazdtf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3kzbdyksu.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3dxlxwlze.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3cuvdkzcc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3avjpzdoa.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3axvgdalc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3zchssfyt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ntoyxwsg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ghyxypyx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3lfpodzwc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3swevoqop.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hnmdgrrs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3hqscmcqi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3jkmlwria.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ndiqmhie.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3hyrstxhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utubwzoz.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3wfvkdvsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qncozgzc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fprvrdsz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3fcjnxutg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jlfbsvyy.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3btspvfgp.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3huhsnqvm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ixvvirpe.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ixcymzbz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3wwqmkjut.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ggfssukz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3frrnnjra.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zvtmsnwm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3xzvyrmni.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3hiqjutvu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3qbbhegqn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ltjkupbt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3fcinzixq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3cmypxbzz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3kxtrnkwn.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3sajqwqiz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3hdorszxv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ogjisvnb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wgtvklwr.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nmpfbmhk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wteiqmlh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qhdlqtvf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ouyqudmr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3yzyhdjwd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3zqjpserp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3hllihxae.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3agjvjuww.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3uawdzgax.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3katwlhjp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3rjpbcpyy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xpnxexpw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tadklzls.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3aezymkrj.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3khdiqawh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3vlnrupcd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3aamcipab.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ccdptuzn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3videkssf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ejwodkyn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3mvwdcqav.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3efkpqqyo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ljdefpnp.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3nlaawlfr.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3yyjutgwp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3podzwaoa.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3puptjglm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3zuexanhe.html


<!-- 参考信息 -->