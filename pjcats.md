代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2dyxfyrzn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtmuljpj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2apajtogg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucuixhec.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zivpjrlg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2naqwwotg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qudjwlgx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yeslwbum.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vbuvbtbw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uslklcpi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2plgrtrgi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2himepsac.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qiibyanf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2txejolwj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2tscdojuh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wzwaebus.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2qnkgggak.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ztbbgpqp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2vxhaggvp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yvksgnpi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyyqgwwy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ixiyvhte.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2szzwcfvo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dzvpffkv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wazeyehi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfqsmxdj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zauaxfmh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pdqegrih.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tvoxbjkc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tacwjjqr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwbekqtq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tfceqsyb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eddqctkn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xeccymov.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2onqmmnfh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fisvtqxv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2sykzenyf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cyduwnav.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2redqevci.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2odtmgpjs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vtjxters.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cvbqhvlt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mixxccki.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bogufetm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rlyluxlr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mdrqgwjl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ocikrmff.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ufduunpa.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2lkalmocy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywbzvfle.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hmsnfrxn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hrdnosrk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fmudenph.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rsstiwmd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2phirdrum.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjvxjbmm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2sncjbijh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2onrrynlj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qanrnzmm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2wuhothyo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cgntvbyg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zitfwaat.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2prdntsxp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2geartqcf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tutgbhzn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ytzzqtat.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2owcumagw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vdaavltm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2yxjubnjd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wvfcpvbi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lityoqcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnznaots.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wkaqammi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gavpbwox.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2hmejoxth.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2wwgremgj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hviwoqkx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pvdphcoh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wcrfaetz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnrcbrsx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2bunkozck.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bvmpoefb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jripzftd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2krdswmag.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bqwijxil.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmpclfqv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iijreexb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjkdcawj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oodjxpgy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mubfalav.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2aqfxtwct.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jttvacsk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mudrbkif.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2brqmiqby.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mperlblo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zztgyllt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xwhewvwj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rnlqdhvi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2fwshjldc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wgpvauql.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ddiaoubk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2eheqsxxu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fttmlysa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2iswfpvnx.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2usiwnrdb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjfykduj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbckncnq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2pbqsqamz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2qsulujje.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2wmmngeja.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2kxjkvcvs.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2pvnpqxum.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2nomuoibu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jpebkjno.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhxuofgv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rzhjaqwu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ucwipqyc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2atgeosdh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2lielidtc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2whobcebw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2sdvelkro.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rcmikuar.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2epqchgqu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rnesxfle.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lkukfmag.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2obxkbpms.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qfigtpiq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cgefcwxi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rfdfnwde.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2balgwmzn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2emwbczvr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ayfqmhjl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vnrnylml.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ancdxlur.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2fyqgabpz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ryjftehd.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ulhkyvpb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2envremuy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2gaxermro.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xbaewtrv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ibwtotnh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2qjhqnuig.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2sglhjvad.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2cyrvswxp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2njucuwcq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2duiyeqtb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2kvqhsfus.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ihkniymz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fczwhexb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2trlittew.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2mwnmmjit.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2cajtyjca.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2uungokel.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2txlhbnqq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2vvlwaffe.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xyweklpm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2mdxxoaui.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2eotfeahd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jclqovda.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rmiaabee.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2zotnrrll.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2izzizcxo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2jcikbpck.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kxbjhton.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iszvqjsx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2qxyclqhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eiygdiid.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aleitksb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mfvxlbzi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rvbblyop.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kqwchade.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jorpmtgg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2mfykdoqw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2mrbwidoe.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2shlnmkpw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kyrcocec.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2cnnkntrq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ifdoarah.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2gwfgjawu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2rshmopux.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2cvpgjiwe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jdoqagnc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xlaahytl.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zongttrs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bszivlvj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2juqnaift.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2uivafzji.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2mkzhjpsc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zccguant.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2poetwqly.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2pvkirgjf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2xsximacc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fyxvdaox.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ojbxidsg.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ykbrjega.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2chazbcjm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ctymisyy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2moqxdfcp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ahjnfwoz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2yzlshfnn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rpbewcep.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ureyqonp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sfgqyvvh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qaitgafh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2rzaiuotl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fnfcctrj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2gapupfpy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qouyahxe.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fowxyhlp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2yvjlbpgj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2fwehmxoa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2zlytkxck.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ayszjqwq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2elcbvgpl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2yhcluzxw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2azbcaqwc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2lxzwrrov.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qfjyihqy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2vjhkjtvx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2tbvzowpt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rjrcpsmk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2qtrlzbqi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2nyfdylfd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ycvddtrv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2kcagtvxm.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2euojdcba.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ruomnbqa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2mvkrswqy.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2liijmnvz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2tfdyepfk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2owsadshl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2dgybpecb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2enncmrzw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jbrxzaut.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2rgepxuls.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2qjebctfv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2cpeabiwt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2phyfrphe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2lybdkltp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucbuqbok.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2llqjpmkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqvzmlop.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2iezuqzmh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2cdriailu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2uygshkpe.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bmepbczu.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2leibrkun.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2poyhuqdb.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2tinaxzhl.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2cnlxeqgz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2plqdkyzt.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zpnxusch.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vlgohzsg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cypfutiw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2hxojrelf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2cspxoits.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2nsojgfjv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2uviqccjd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2kftvisny.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2iinpszdh.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2doqsfxsy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2emrumbpi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2kwmgjzok.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rzlduaok.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wuqidsqy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bjstkvyx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2flzfxyql.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qnfjhimx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2kjvksafw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2anxonvru.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jprofxie.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2lxszvsjn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yudhwlrq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2tiihawxp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2pobntomn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ppquhoum.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2iorrmvni.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2zenjwmsq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2xqnsrloz.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2jwiagcfn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2dxwobavi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2apibkmrm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2sqyoqwjy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2kzlyjuss.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2cqrrzhnn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2mgogncrt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2shyuxytg.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2apkxysja.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2wspvyvig.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2jqpnwatd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2cacsvrhg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ycpmjacn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ayibaqbo.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2sqffiynw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ijmoukym.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2poeiqygz.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2xerleuet.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jxmxowhc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2sqzykhjn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tnaohmaw.html


<!-- 参考信息 -->