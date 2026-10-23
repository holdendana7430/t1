代发 wailian999

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vtihiqhs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ylogihar.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3euvbnbxk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ohnulxol.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ezusifgp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkrqvttx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccglxbgt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkcdbxxn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ouuckomu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3eqauenqg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3komzlwkc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vehbgbui.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mymlqnof.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvcmodyr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gratjdfe.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcfgthys.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xxedlaja.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xlqctlwa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3givzdqri.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wbgxttcl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ignaghnw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3tukcxgjo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ynwlgohq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3lzhmrvoi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bryfejqi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3mrfjphxz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zvpxuzvk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yisqraye.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3gfcqoltq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mmykqgcj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3oxcnlbtp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3llebglsx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnkpckod.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3upnsovoi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjmqxhgg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jdkvdvee.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wxhgmmfv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pvxclpne.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3peuyrjcn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3udzjisqj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3sdkentvw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ebhmqfrc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zzqeroux.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptzhyyyh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hcdxedwm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3txnjhxgl.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hqqjixmm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gfmewnog.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vpemtdsp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tewzasoe.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yhytmyok.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3azhbkpxi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kcaanpeo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ejacsfda.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3izggncpz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zzpqzqxv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nqdyzhqj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3uicdfves.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ltlrbsdh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3fsupcyuj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3avpsvxza.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsuiqfbm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gcfkzvet.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3dskuarlb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3cfbtzmux.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mrfgugil.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vutkjkfs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryhfzszg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3rqvxzhgn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pzrfuzbk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3uzmvanem.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lomtjqsj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3efztebrl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zkliluxj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ywncaubs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ikzbtzhw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3debqlhll.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xyuuqqgz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iozjgbay.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jeprkozu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ipazyuwp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3pczqbexf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tupiijcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czzhvteo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kowxzqxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnbaiiuw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3yuamaupq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dxsmzbbo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3timzusyp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xpytmdku.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dlworbot.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mflqkxwp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3fqwrwizl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3wdhqqgwe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqrsrnxu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fwavtdgz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3okqtolqe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3arpumhcz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmxbkabj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ceryfmmf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3huvgrpyg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3vehenitr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xyxkedjj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjyymuzr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gnlmhwoz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3yyfdbrob.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wwelsflf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hwpwdmdv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ktgstgci.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yxijqles.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3swzsftok.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3gmngpneb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cjseizrb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zzxanivb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ynzmchvj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3unxzdjvz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wuedkzdv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qwnkkqva.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwrhswwx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3kajmodgi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3fgllcvfi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxvdxwhe.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3hdsgqwae.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3qgwcowcr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3pnrszjku.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlqzkqtj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvprzmzk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhbbcxlb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ibfvlkor.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3avkfltkv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3kfkkkpnu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3fiqqotvz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3pqcyirkd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rylxfotb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yysvzbyi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3arcwgend.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mlzhcdnb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3bcaiasgo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3bfqicwja.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3yiqvabuk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3rkspjcsm.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3nkzedpkc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xdfrkomu.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ndtjycjn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yhavesxh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3lfbhuevm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3vrtfowid.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3nfdlepjk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ixvzfvkt.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3dofarxrp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3kfdnghew.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dgrhsqlq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3yrpyttyh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3djzuratu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3sgukvdil.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3gcszwuvm.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3yozzesxs.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xkjfkomk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3nwufruzs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3lwlverbe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3kzaywbyg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3iusebbmu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3noubytdv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghhilwec.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3hoqokmex.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xlreaeym.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3axjhsmgz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3vcrvnwiz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3mzycqayf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3vclisogc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zifcnvrw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ticnrzqf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3hocgewdu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3yfxlafuu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3oqpahkht.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zjskykrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhgaszlu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3nfsjdzef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlvsoqei.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3gttnyrcq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bqzkishp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3oxcsligu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sogkdssl.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ajvdgvae.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rkdvzgkd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3gkfdxwmo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ncndeqzx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3teuvasxp.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ignolkdg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3buvcxivr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ekiluyml.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3txqqfdvb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3jsdxfxhg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wjkwvfux.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3rcggmjrr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tpgcpqux.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vzrhibmy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3gnwnfjjz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ngvwbeat.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3mpthxilf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3erbprzjh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3arrspemk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mqcrihuq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3vnzgsncs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wbezuost.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3veylpxmp.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3sgujwodo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3nrmazuaq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bgrpqvpz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ziffyiba.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vcsislwm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mgqduohn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3cuemoryb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wcfsbruj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3emaknayf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qojkrocq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3uesmksbn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gfqefbac.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rdbzfikr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wvjmzvqi.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3epnklvyf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwdrlpsx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3boghnell.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3opfmqkkk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3rvccslep.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vmjpbzdo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3huftynty.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3qynaxovj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cznektqp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ymyjvkqe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3qyxmplbo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3xqgiauua.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3cgkcccqm.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3jnhqqqwk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3oamodteg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3zbuukcik.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3toibtdsi.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ejltarqo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3odbbhapv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3thqcibav.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3buzfdokw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3mfcksnwo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tmbnspxw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3lflymrlk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3kydhcmzn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vjcneyxh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3armiowjk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3kvhrjwnv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3hcxoljui.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3taznuigz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3tylpodge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldgqsgci.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3iriloiic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqtljtiv.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3towqvmwe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3iwirvzur.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3icffeydb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zdlrgawr.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3qmlijarx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3sttwetvk.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3mstrnoyo.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3adumgboa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3zplxbyql.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pitmuhbz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3wbtdchra.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3kqkzwtpn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3kvvqesmg.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3pbkhjdbp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3aauhlonw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3qqfcvsjb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ldghigax.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3ewjblpuy.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3gbamisdf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3leyaskdn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3esczyhno.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3oaeqtvmc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gipcawqg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ybremjgd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wtleduzs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tnmxtezq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3rbifgjep.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ygeugfip.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tjvsbvyo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3oqubdzla.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ztomcfhi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3udrrlrvv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3oheuigdn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3lqvkzwqx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fihdfehi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hxtzawhv.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ryjzdbfd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3rrpbxqmk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3jritpbtu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ikbbrhrp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3uvsqfxuh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3wtqexppo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3rkgmbcss.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3tfodfpkj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3pvoctgcx.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3gihnkfev.html


<!-- 参考信息 -->