代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vztkseji.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ndwvsfzv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3njlltatk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jnfcsjpt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3psjtpjaf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3inyakana.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dzzxkqzg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3zhrivlug.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3fkngplom.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3prutgytn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kolouegl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pendhgan.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3orqqxgmm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vxxmeasf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3niuaavwt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3oxoabxtx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3alekozyq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3tposqayv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3dyepdjqh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nzffzojw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fvzhknxr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ebwpclqq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lzmflcqe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwzcnhhn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3szuxmqrz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3adshqnov.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnrxcjkf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fgrlkuim.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fodttfmn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3slomecws.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qiopcdtw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jhktsxbb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pgvpdnfk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qbxjyihz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3exsxccll.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgyqxydc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oymeuhta.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wkpvdynk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ebobjweh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ikxtapnr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3pyzzmydf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zxwlnbun.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dceuullw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wolgdpsl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qqcqwniz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3coodnuja.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3apufwabv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mpfyjqjx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tidjfqym.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qpznptwi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rtxmkiat.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3itfatdcu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3owskxuck.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hflnwvjk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3osxzvkrq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3folrurmw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3iqehwavk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vwbulrut.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tjkztkcv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbnpjlbb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yyhtdequ.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fubgspie.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3imcvoalc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wfabaase.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3lzybarcr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vltyqzpr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vjsnjlvk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zolpbzkn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bgtievtu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zofblcrx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wjfnnobi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xtrnczoj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3onduscnq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wrgvbroa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mgdkutyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wetaijdl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ocwbwmop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uudqllib.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ajgwzjzw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vtisofsp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zsntimff.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrrtuhzk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3entyvmnz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mksvtsub.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zcewpltt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3egwffukt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3jkhqirua.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3njkjivuq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3nzghbyzi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldvrlnbm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujtjeqhg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqheeqwt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3glwyhxrb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ziwuqvzx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dwuegjcb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrzvlfqf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dnypmveo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3kbewplnd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mxuhfuqn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lgtgtiqa.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qxaffwht.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xikdhbkr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hfbgzqas.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ptzuyodv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wyfhhbsw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zdlxaeqr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ffclvpst.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tfsyxzap.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bopbpzla.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zcwebbhr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpftgxpj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jzwuxxvl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bnofdkzv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3oooynruw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3vyavwxup.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zgxsnsjp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3mehciucj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdefjyff.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oaedlpcj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3dxqjqahl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3xkybkgyd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3qiubdbkn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3csycohcz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3abirpunk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3zcfmgdvb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vkjcalgv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xmglmnnd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mjudrktu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3vlxbwnhy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3uizelqsy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3iynfgmes.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3uwviamml.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3lhodoxpo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3awnkupla.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ykqjhygu.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3isultsvv.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3khfkhlow.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3xozkacve.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3mvvlhsqh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3lgscwalq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tddevmjf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3aubprhgg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qcoyfmfi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3uagknioj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3dcaupwrb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pjipzmlw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3wqchrjjp.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3rxuzhjxw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3snwtcvpl.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3hdsgpdzh.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ndhtfhgv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3jjrfkhea.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3icfbvrqy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3hglslyhu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3mtgvxxgw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3kryinhsx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mxxhjluk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3dfgceras.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ugcglcoo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3wmsmwyvz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3qrfmnwrd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3getperfd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3uahfdavj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vwtyzlun.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3cmeruuwn.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3tlnisvio.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3oabpyinn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3meymqxtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zguxyact.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iyrmyspf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqxyakxo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3lnjuvizc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dybhqrll.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qaxbddhl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nwvcpgvx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkomnipf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3cuoxmxtf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3llvybluj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pxcnlvvm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kzfbwjjd.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3vmzpvukb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxkpkjch.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3vrkynurh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3fgzalega.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3kfnqfdap.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vlsmyygf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3xtefbdwu.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dzrdrcbi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qiwmhdea.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3tyiyzwdw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3smhundsu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sfwnhsse.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dqqqtrtd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3uncmupao.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ywvgupwa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3tpviclkf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3lhfupfyo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3xtemtsyi.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ficxrcno.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lnuixnip.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nmgfpqsa.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zvzuscyc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3aioqrawk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lizmbsll.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tweihpmx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3kzdrwxcj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3agamoeia.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3epwnnnrk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3dijsqxqd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tgvfnfdh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uwlopzrf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ygjnlfhz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3wtzvtytd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3dwjzprbg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bfbunvea.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3dwlmrmlm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3cxwwyudq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vlzkxlfl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3aqgaehzb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3rejwfqvz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3raokobgt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3sbtwrvxp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3mnpaugou.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3zmfzilzu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ignznvtj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3aramvdll.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3rgnzqxmj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ejdlycyk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ivqutqvc.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3vtzokavu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3akzaenvn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3vzfuekme.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3llyybydw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3fkloslrl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3hwyquiao.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3klsgabdb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xezhzlnz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3nohjbhyc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hmkzekbq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3nveywgsv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3phvetltg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3vhfdpsyx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3klcusrgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idzhkokk.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3uogwruyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujjfremb.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nsswfzcr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3fjpvurjx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ogighxfu.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mthztyga.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3jxzfgajp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3kwoxiger.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3izdiqygy.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ppbnaekx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3yldgvmpj.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vvaajlcc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3lbsfuekz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3uwbqnddd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3bzxoicma.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3vloiupwy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3mbbhtjog.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ulsdeipw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zruxrdrl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3bqjgernl.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3drjdwnop.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3klrahflb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3kkhjztfx.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tximwlkj.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wsfjyryn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rmxkxfow.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3anwgukts.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jedmjcjm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3grwyetue.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3lyvolbkg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zryebhib.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3alxwcovb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3juhesmbx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ncleelnt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3govaowby.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3aeozxbxw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jjbizqch.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3cxjjexfo.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3dlikmabi.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3oypbcngy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3snowoewb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3luzfwxmb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3kcatyoja.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3stmrwdxt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3sszezcuy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3hilgjemq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qubjiuaf.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3rncxwrje.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mceglsee.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3jrlyvdmh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3qbpagfsc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3qxuowfvi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qgnmrbyg.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3jiefcpdu.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3qroytkjy.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3rttldoyo.html


<!-- 参考信息 -->