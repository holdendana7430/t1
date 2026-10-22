代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2hkqermcz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwckzsmj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fbbfjmmt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2nxwebrat.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tqmnfshi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lruolyhn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ahtvokyb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuhuqhdf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jeotvlhx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2amspzehc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yqjpnrvo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ghiozjdw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bwjomaso.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tiojeuhc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2fuotegce.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kobfctgu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jddpgcln.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bflazaly.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2pxscptmn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdysphdh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zevtcktl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ispqtyyj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nlgjcxyw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2seoradpo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ishhltxt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuihgzjz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ehvalfsk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xyxljvvx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxbdxifz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfgzpcor.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvydwneb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2huqncixb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yskejtak.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ofgazwvu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gjldjejb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lrclhngs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2zbpfjrqz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rwbjwddm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xlaocved.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2etnkfsof.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cskuznjm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hxjtrxca.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2lnlwxvpc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zowzsind.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2smmzdijj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kidfkffd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2grxtghbs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lkosjruk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2tjwcvlzt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2atzvwadk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xllqjomx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2jggegjjf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ugwlohoh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kkarhtvi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2zsrgnmoo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yapkxewz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2lyawezpd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yxjkwrcn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2poghbeac.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2rbzfzipr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2svtreczu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zeiwtgqg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rmfkbfve.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2kzdthcvq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pvhxahfl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oxokkmwt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tzrupcds.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qutrdxfm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2acvrqohl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2mldicnrq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mvuvuwki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ultgnzoi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nkhdnhwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tulrentl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ugkranvw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ycpaqkkt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cfneoxgy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2phfijpyi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjrysrxn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2nmwetlzz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2nyktgkdj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2tbnzivse.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkaxxcja.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wfgwdeta.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2psctikmo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2asqbdvcr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lwaxkfmh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqqjkivv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2otpelwjv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ikskaqzt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wnprabuz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yelkqzcy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ujdwjoig.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xllyuvyj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wwsseuse.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zqazkvkt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eojfompk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hhhagind.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2rmjxfzoi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ybfrovxa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cnqeemqo.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wlvvlpsw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dpojryzn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofcbbzjs.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jsjigjii.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wghattwf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyofnatf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bjmoiyii.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2dqyfymko.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2yaetqgdz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vdkmyrte.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xzcgroys.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2kjaeeioc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gthznllz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ecusrcvd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvxmppat.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2fqvfzcps.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2erjjdrkb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekwiiqan.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zhebynih.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2rrnqzwsj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cfhvrsiq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2njvodorh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lembmagf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ppfmerut.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ttlpisre.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2efonjimk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jyyizfgm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2nejqsgok.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uucukvia.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wspkappj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2paqyujon.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zbnvuwdf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2kbeazubm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2lqypqqvw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2mnwqfvbz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lexrbieb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2mfyzbitm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2zoielfre.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2kvzggcbn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2atentgyp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wjhnpign.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2sfbpuxuz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2tvdjcecn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2yfkainek.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2nlkthche.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2rqibawwo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ozacmpzx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kssurdbo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wqocsxkf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2axhidjap.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2twjuombs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2haedbxhq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2rkzwvert.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2jufxampf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2zizolyju.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2zdbvvcdg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kzdoeied.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2opvovkpc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2masnhyxl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2xbenpcvp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ofwmwdkx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2wemdruli.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ftrtehnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eiwrbjfx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2gsaabpdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpmutcbi.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sruftaig.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wmtohgfr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2srvazwfh.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2syjwdixq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2havpiiob.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ejrxywco.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzsccoub.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zdcjgsfy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2erkyafgc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fbxhlvjl.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uerrwzon.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vupjqsol.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ptihsfpf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2byiuyups.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tiwhpqfp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wuritwro.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zyactmkl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2baqocqql.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2bykepmfm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztbprfer.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2nzwyvkvq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gxudnpui.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ugojonfp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2revhybnv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2cizffoyu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2qlcdzbyk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2jyebtdxm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2xddetbze.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2tbeyjohx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2crevipfm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2knhllrwo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lzeuvmzv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ixceifhf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2fwjltagg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2polrqyhj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mrtpcxpy.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wyodhggg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2gwjncifx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmuugojf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2skziuotc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2pxcphbnc.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2sncrlitd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2oykisfuk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2udfesffy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2lzwvzrjb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2lgmlznhx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2agxdxtjd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2vbkkjiiw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ruiehijm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ipnmemzx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2yyoiflwy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2fabratwj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2bbsjdpby.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nbmvsqrx.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2gtioahma.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2mlbottpq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2rwzoijqt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2bdbhqrpy.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2gghikiih.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2tdortrae.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2kjbswfvj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2htekmqcu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2fgsncxig.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vibdwmcj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2amekrxhr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2pdzrpcel.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2myrnzgeq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ljomgbri.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2phdqnvps.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2xyvjklgd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2gxatkqdc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2anntgomz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyghpyti.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2nmappgot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2timxsmph.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2dkjhurrb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2qeqeilqs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2gtvcnbvy.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rbthfxzn.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2adjzrmxi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2llkgzbdx.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ugnszhnn.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2qpxsabbd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2wfmexcbv.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hnyetbcx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pauiyztc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2iryyrknq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ffhsxjqy.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2yhvawuva.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2nxmmzlyn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2cdcltxfe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2upwwuxzp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2fiuydpfo.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2mxpryira.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2shvvroge.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2njvxqrku.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2snpzvxvi.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bcopshgc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vtxvpbzu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ieshlsfn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qqpkvpyt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2avlquwax.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2nhdlnkqg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vbvrkwgq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2sxkmjqor.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2qhyextte.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2wnrtuuqm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2okkysaro.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2yxofrdvv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2decioota.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wdaywnwd.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ffzapiwo.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2iumumzip.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2zaxveidz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2eheydkgr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rjprtquw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jmggqtkt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ixkdufwe.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2jjwdzdez.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2eqdittxr.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2onluqopc.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2swfvwdjx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2zdvyzvdh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2jbvhgjkc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2zzxffggp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2knkmrfab.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2rojzdrld.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2akrwkjae.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2iqbarxco.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2kvhzklth.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bzowuume.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2uyhzfvuw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2bcpujkka.html


<!-- 参考信息 -->