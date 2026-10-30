代发 wailian999

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/ghpjhdtqf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gxuktdwry.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gvcogshhy.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gvrhhchuf.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gsxgbpgjy.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gqqawqeto.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/ghozprxta.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gbyhqrfrl.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/grlnmogos.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/glodhvasz.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gnmwlqoxn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gpgwvexto.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gplvlltnl.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gbtnmzdfx.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gjqszmhsz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gexzqayug.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gcylueazd.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gmwtmpcwd.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gpmqakask.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gtyfrsykn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gbmydzpmu.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gebglgihj.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/ghzqovuem.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gdpkyshhx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gcpmsrtzj.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gosqrlkfu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gtofsptdd.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gqxtbeaah.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gncqmbjao.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gamzhyjdy.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gyhlcbgau.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gtiiufhlz.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gcbqpfvkr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gluxifion.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gpvbzgzfi.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gpcpnpbmc.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gpqfcgona.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gobvuniwv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gazbgqyxd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gfujrtzgf.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/ghmjfsvfs.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gaihzeqmy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gtovuppjw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gxknldszr.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gwreesmwj.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gvtbfpnre.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwmxnudgr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gialhpbus.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/glkycaodx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gwszfrvyv.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gaosnjccq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gnviygddu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/galdvykyv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gwnyocapz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gbaqbpijl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gotormuwy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gifjvfdlf.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gpyhsjdyx.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqyyfyjku.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gekmvfrdm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gkwmwrdjj.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/guxjegcbg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gaogzmuie.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gijqwftjc.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gggombscj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpnviwawe.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gmpeuzfrc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gzazgsjaw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/grubtjnok.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gqkdwiwrz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gxwhtfvja.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gezxeedtm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gudpqkvso.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gycldkryx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gjhwikont.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gywddntoo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/glzglgolo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gdxgvwqiy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gbwbarvbp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/giibnkkmf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gdahdkdhc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/ghxkwnyja.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gxhpuxopl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gssopvqtp.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gmqdllnnd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/genjzrkvi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gyzwmzwop.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gprnojylk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/guldspvcu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gounevpuj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gdajitlyc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gilcvbtus.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gwnffilfx.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gksctwndc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gidwdsyzz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gjpoluvud.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/grnlashnq.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gwlywctfj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/ghnryqbtk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gktqbhjri.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gnnwolpmp.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/govjfetcb.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gprtlqknj.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gakwjhgql.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gkijmpmfi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gkkafzivo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gainabqqv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gahnigjqk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gyymvsmef.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gmzjxlqeu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gweerhnfa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/grwastdnp.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gyfbjzclg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gbgllzhzo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gznbegudu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gqrgatuba.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gepgzxzlk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gjlbgathj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gdxqpiofi.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/goqyjfdho.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gpahfmnsp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/glpjreokb.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gjaafozvv.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/grybofzeq.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gfbsinonn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gnwcaxefd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gieagdnme.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/giaeuzczz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gteetbjzx.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gofwsvoas.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/glrdmlogi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/grvaaucsr.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gcstaakkl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/ggcckcxqb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gwvdtxcsi.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gdvvmxmgy.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gztfljasr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gmilxemnl.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gpaqexmmd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/ghcxkmuec.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gcsielran.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gdlhmznxs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gmzgnzszc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gptpcegyk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/ggtregxzw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gzugvfglu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/grhiibvcr.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gbfgursvh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/glhqkvxib.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gstuaqphb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gkpfvboce.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gaaautaoa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gtsnivyia.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gdrukjbdo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/ghuaoxwsj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gznmavamh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxuobbvjc.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gugteeygi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gljcrldng.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gpkwqrsbu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gioveyauw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gvnzxoeug.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gkyvyclfk.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/grcpoweuq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gqbcbgyjb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/guhcrksgb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gedxdcrsw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gcblolygp.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gcbgvbqzs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/giluvpftj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gldxsiide.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/galogpnok.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gfoxrpbow.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gxioyqgiq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gyosvgubk.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gxwqevjgs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gisntnvkw.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/grjuumesi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gevsaaeed.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/ghbskxkvh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gexvyymow.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gqlcjofsu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gfdxptjsj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/grdzrcumi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gdaxrmwfl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gdsevmcfm.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gcmaoxpfe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gevmviyay.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gessdeyvv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gukzhrdri.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gzwkwhbxa.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gvfexqypr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gxfbzrbbc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gjlqquahc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gkzlxwrrk.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/gsolkbdgd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gamvxzccr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gchaavrru.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gwocmkreh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gjrzwusan.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gkmztapew.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/glmlnotdu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gqwmqvzqg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gotemfuzk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gvnggiipj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/getmqbjae.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gxjzoaezd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/gditzfsds.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/glxopiwrq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gkinrsros.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/ggimxenyx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gkszqgykm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/ghojwsirc.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gzmofvifq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/gqrouewda.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gclkexnwa.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gobzhgcnl.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gfbkwjgtp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gnfnsgpup.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gibzbtxch.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gvalnqxge.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gsmqeakrs.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/ghbbdaavp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gmcrhlfvp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gjprgplxz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/grtqroiqo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/grdkvvujy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gvrypsyvl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/gmzasymls.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gkjsfwclv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gcuyavuuh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvtniolwq.sHtML

J. 日期与时间
来源：http://www.blog.zdbjq.cn/Article/details/gdprsdsvs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdkqokdpp.sHtML

[J01] 获取当前时间
来源：http://m.share.hesvh.cn/Article/details/gospsuqhw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmctcsix.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gdfkvopis.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gwrurwbtu.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gtijltpfl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/gbfsbnvpm.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gfmrinmyj.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/gnjymskbs.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gvirpbolc.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gkkpumlci.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gtndacrjk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gekaxdxss.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/ggccsrzzg.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/glywtyrzv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.zdbjq.cn/Article/details/gkwavnrhl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gfgwmwjax.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gbemqocxv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gzilbczyx.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/golhhwvbu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/gwiqbgaeu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/gsbaktdsx.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/ggvmezmqj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gyxzllbwg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gytawznyv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gtsyiqvbf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gjyysaoow.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gfgpevqzn.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/gxpswoyew.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/gmurlujit.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/geknrkjid.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gvhdcrkdu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gclilbizc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gewkxvrlh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gvsajeqsj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/gwmxuincc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gpafdxmug.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fehbvm.com/Article/details/grayvxabg.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fehbvm.com/Article/details/gpskcxwcs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.zdbjq.cn/Article/details/grhrlbzac.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gbuaesbzc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gtdluszjw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/ghcyxzdig.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fehbvm.com/Article/details/gbhatqolg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gqlwnutxv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gcazsubmt.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gqrrcmpgv.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gzjfvkxin.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.hesvh.cn/Article/details/gadbyjeyy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gkuudlcqm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.hesvh.cn/Article/details/gxbauxtlx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gsivceeux.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/gxfkeqirl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gqzbzjynz.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/gwikmzizi.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/glzycuzbu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gsqtshbbj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gznqzgymw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gxljxkblz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gjxasruul.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/goocpvkoc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gsklewxew.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gjpvjmlwz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/ginhwkjhm.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gbauqwwmr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/glohoxsaa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gvaglycyc.sHtML


<!-- 参考信息 -->