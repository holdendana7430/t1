代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3iiyqektl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hqsynswe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ruhjxetn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gcabnvru.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3damhgkok.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3egzxamzt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3nkjmjtgc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiutvqbj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwuglsxt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nmatinbz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3sfquyqli.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3lkcxgdag.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3pgjmuoul.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bbhlobur.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kbhbzbag.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3meytwfxo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nfzzhxms.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ejdtqnxy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3dfdfghrl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uvamdqyo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3rxqevdxd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vkjhclnx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cagnzaav.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvtxulgo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyzwothp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnasoahq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xvjxarhx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yapfbnwz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3khgevtga.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mprswbwv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3dtqtelcd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vgydzcqe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3awpywjsk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggqusghp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wmsxjmdi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3udnqqaie.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3secwuift.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uioiuwkt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3huduhmpj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3wjsexguo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3jiqoicre.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xhfynqip.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3icypkasw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qwrascbv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gfmarfqs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3usihpvvd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hspfdswh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3rdvwtldh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3wcjvpcns.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3kpxeesmj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3keugirkg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3zyvqaxkq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3laiuummm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqvlkafs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hbozhcbs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nlgptcow.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mtxwtoew.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3chvtygvq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hnjxlgeg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3frxexwdx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3udnjczfl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lwdtlogn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ukzzigxq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jhjmbzkf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nfsdybjq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3objluvhv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vkzmjsrb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3eqxmyhjg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3yapiijoz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hytohirm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3foqfqnbt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3plmrrkfs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ejjygxua.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3umxawtpx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vvwmsjso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gycqscir.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3zsiqpxum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irofletg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3omezbyxo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mbwnajuy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfidgiup.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdqcqbfx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rwzpvfxm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3awhhcqtn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3aentpckh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3aludxeph.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3futoneqj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ufobwxzq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3pnevdwvc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3glmjjdrq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ueecbyol.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fgyoalvi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hadjriir.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3aucnwjmw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3qlpkfsep.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tfmyscpq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ziqgwpmc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mxdjygzd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ybisssdz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oaiakjfw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ducanndm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hgxhhrbv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3blgmkbnv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3xpkhpdzr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jpgkqfkk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3kvidytod.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3kahnumle.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfomabat.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwnodqmp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ziisrzgs.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ukbusntp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3tfevyale.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xrzooybo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3goqybakl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3zwworldg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ytpfpdkr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3gkmezmfl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ornjlgtm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omvmyqvg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3igprtyhl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3kxfqcdkt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3uwbjidcj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wudcjndf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3bkgimgjz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3rqndmgvo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mlrwjqpb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3huoxxkhm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3abpfwduk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3spiptfmj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3iyznxnen.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3dkdihqqx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lovayrmu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3icszowhh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3axrlwguk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3obuntrrw.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fdoqidms.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3htmuhehj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3enxjkkzk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3itjnbnii.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3qiaaalvj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ujrrrajw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3qtuxjoqx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3alvchykc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3darjaswm.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3tseowoej.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3plhdfmsi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3cvyuhgfs.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3utzntlbk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ezeosxxp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3usxlpnnm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3uyaxrzxk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3riyuluyx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xbfqiati.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3utzjferh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3bzmlnnbu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3erppscod.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ilcvbtua.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3zrfonpqc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3zskynxqj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3svuigmou.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3notkfiul.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3rhbswazz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3davqazni.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zufvvzcr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3fdhmrkdd.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3wqkyxxak.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3urrsakuw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xgabkrmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxxujsel.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3myblifiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfqlldhq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3cdvsyrxi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3mouoxmea.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zaykmkwo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zlyznbja.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebvkrztj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3avsjtzsa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3tpukkagj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3luqsgutb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mwtapzcc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3txtkahyt.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3voqzdcyu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ljdrcjvj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3avsxjhur.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjuswqi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3reqpojzi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3xbfncugu.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3otxurmia.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vrpmydxl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3kugwgaoj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbddfosb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3qvbncgww.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3bldfdzbv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3kipxfuum.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cgjxqfsk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ogxkxczx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3xxzehnek.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3atkbarbs.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3aeiyehso.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3yeyazeja.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ithikdzx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3antkprbe.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3slhdgvmf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3eqehkbaw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jmpdhhjj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3datkfbnq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3imagzwol.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3aqqyhddg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xmuolirw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kavpkiwm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3onaaqvmg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dwoxungp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3wwdskbqp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vicehzzv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jbxtfxhi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3qztmeffa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3xkskisgt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nptzeirs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ekphlpki.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3mxvumyzj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3jivooicx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dquepbus.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3huzpevnl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3xhjfnpkm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hgncpqfr.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3wgehjoxk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3cbeodcad.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hinmjxcz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3dikcjgoe.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3kkviognp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3eyaepgqo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3yxtealrd.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3zvvlrsoo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ldeqtkni.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3oyqekddk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3oijvbeth.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xkhtsemo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ssberxao.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gqvecjuf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3bcgufuus.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3stvisjqb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3hweoogti.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3lgucgyok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnfnkemc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3sbeqktkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbgqjbjb.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hrpfoore.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3oblzasjy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3mqheqaiq.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3johgtzls.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3zjsdlprw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3bxtyfraz.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3umtitlas.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3oefrrdjl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ahtbcugj.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pbcvukmg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3fxnywzua.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nhpbkjvr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3xkbxunqd.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ylmwzbdu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ytkdhdup.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3xvuydecl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zpffxhnb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3zggmshnx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3tmitbype.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jgofmocr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3qtdbwzns.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zppufweh.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3eojnaexs.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ayvlprti.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jabgtogt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3upuxavax.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3rkwuhfpa.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3qxopfskl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3qjwwiiwu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3doovppjk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3mipkmxam.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3fgnncsco.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sdlsfjxw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3leoaeqaq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3czgrcfsc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3jbzrogse.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3mfatmppa.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3nmgciqes.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3camxclmj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3uzueaazc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3gxywchce.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jrlwoapl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wszcnfdo.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3nbpizkri.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3mujtfjnb.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3muvfxlfk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3dyehnvvf.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3uctnswdg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3yqizwikl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3aekldchu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3oyionhpc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3xoyapblt.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3glugpnuf.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3kzkwfcog.html


<!-- 参考信息 -->