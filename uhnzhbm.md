代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gaygsbtsd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/grsaxazev.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gxgebafvh.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gerskgpvy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gnyjtcfnd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/ghsiskvdw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/ggecwzvsq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gimnhmtqx.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gsobparpb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gyfghydzq.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/ghiwewucd.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gsejwxemk.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gdnchuxjd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gzodpgntb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gsmypgxam.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gyczzawsq.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gmgxvzwnr.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gqzunbazq.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gskfkhgks.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gyjflwkgh.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gncxiyvlo.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gdqmfgegg.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gpcalauxz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/ghhsgrtdf.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/glevablwg.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gzjzjrwcf.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gedxhqemd.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gvzfukead.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gknomtcrf.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gpkhdzbri.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gpbgnvbnb.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gtdzcaozg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gseuyagum.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gilwjsamg.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/ghoymaovi.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gfjdtnffq.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gnhrudzdg.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxroehflg.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gnmrkrfvw.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gmxlatcun.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gazoectwo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gomhajoxi.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gfradjqcg.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gpqmggjjr.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gaqtiqzis.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/ghglunqin.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gxduhazya.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gdiqcpeaa.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gusunfnig.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gmedojxax.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gdtvhxvne.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gbrxkchdy.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gwamqggqz.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gntxdldjs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gvwnagjll.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gbtyrokqs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gkrixjdcn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gzmadgofn.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gkrrezaqk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gqumwqngf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gvcnffsbq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gymozphle.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gbhabeuvx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gzpvnlnqe.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gprofatkh.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gxvipddlt.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gfhagyfkz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gmqpefrnt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gesvkrdej.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/glvfnbpua.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gpxomloeh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gichftyld.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/guuwukney.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwijjboyf.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/grlgwhjav.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/giimcvpuq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gatexrhdp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gednapwen.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gndrchycs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gnhycscks.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/galamtwgo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gpmyeyxot.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdfqlswud.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gctdbfcdn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gxibjpmpf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gyuhmokpp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gipwltvww.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gocyyhbba.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/guirpaigt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gnxlkukjk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gihxohwdc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnxzsqzso.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gtdhzklpw.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/ggvkgcbkz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gqauwlcym.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gpualweuy.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gmocvcyik.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/goxoduzdw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gfizfrmif.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/guwpuacvb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gcfthzwew.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gfcpuejpa.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gjpybsgvu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gcdrksztz.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/giuwipzcv.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gogyswclu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/geckxcqyw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gkbpdkksk.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gmppagfdd.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gitkonpjr.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gbkxylxzy.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gnzglyrsi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gmybgzpfd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggrqjyjih.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gdvifscbo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gxfravnbe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gkautafoa.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/guhefamfx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gujxyabin.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gvkmrbfvp.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gyyoybgdk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gnoestaqn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/glbyxbjhl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gumflybeo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gagqcqvem.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/galxqyuat.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/glrncsguo.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gbpeijagd.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/ggrcrusnx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/giksffmmt.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwluudmhv.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/giaowizkn.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/ggbtvctix.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gyvrmrwxi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gxqxmqqwb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gtdzgvnqq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gabemiqac.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/ghuvrzoei.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/ghsfclspb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gadaqjqti.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/geodlvtfj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/grgcgzrvc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/ghpydpslb.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gmvgceonr.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gdvlbxmdl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gzeaaxrxo.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gznrtacop.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gzddpzysp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gumylncfc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gjujzjjfa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gojbidflr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gtdibnpwg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gtosztzzj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/glwuzjdpl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gqtbvqlga.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gkpyhbiuf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gvjczjfbq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gwgafyegm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gsfzlkndc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gpbixrtnd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gmwzelzmi.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gzrzmflfz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gzucbjxcj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzgwvqecg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gulhzsfnc.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/gruxjvqbw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghnhbauct.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/ggdvetngq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gcwenytpo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gepwigyio.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/ghsljwgwx.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/godlkumtr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/ggaixzeeq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggmlbsopt.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/guavhugzp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/grxwsxrbu.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gtncknjxb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gdeibrywu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gdbpqptbd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gfzjjthzx.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gicfxnbqv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gguqhwcuk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/guqdkmspu.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gckjhpspn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gbiiclbol.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gpwilbbnk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/glkvlioxe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gfmcufzpn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gyqlcmovh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gugbelnae.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/gecnwtawd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gjyekihbr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gonbaedcy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gprqqacrh.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gegyudxqd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gttppvhln.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gmrggaimf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gzcvnwszf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gjfazptec.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gyabncapb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/ggkouiium.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gtjrfgbfx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gdgigljoz.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gykrkygbu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gsmxhqtxh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gxtkhsayk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gxrftmkca.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gbwwjaxud.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/gauvtassv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/gwcfliits.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/glbirmgpl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/giqhcsxfy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gvgbuvsns.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gomayvybi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/ghblkyoll.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/grsoduuym.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gqpcvtijm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gznuyxfct.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/glysoxnsl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gdniipxoq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gyjlbzfib.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/giqqldlod.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/gmpjnxfzh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gwbrgtjvq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gnnejibjd.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gxidudwyi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gmozavfms.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gnmnbhqjb.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gtegpgqpw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gexqnymsb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.fehbvm.com/Article/details/gqpletsrz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/geyypgnjp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gmtiahmac.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gzkkqdzqm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/ghchhrhqs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gmyqmwbsk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.zdbjq.cn/Article/details/glatuphym.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gaouowsvz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gehonqfcg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxnsdtcrw.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gdycyaqyi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmhguabzl.sHtML

[J01] 获取当前时间
来源：http://m.share.hesvh.cn/Article/details/gaqlaauul.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/glcdiszro.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gpampiptz.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gtklbwnxj.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gwdhofjxv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/glffjyzms.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/glsxuynoj.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gyfxtjjzv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gfmhrehoz.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gntyfbdmb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gyfvpiqlc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/genioerga.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gszyvzcfb.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gsdiuvevt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/grjheasvf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.hesvh.cn/Article/details/guotmobqn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gzivesfwa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.hesvh.cn/Article/details/gqahvqggl.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gusfmsdup.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.zdbjq.cn/Article/details/gznegcpwh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gkivvoqmk.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/ggveurfwe.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gwebydagn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gqqryvzcz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/geazhxvwr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gpgakbxnk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gcbsdendd.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gsskdakis.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gcvchqbki.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.zdbjq.cn/Article/details/gkepyvlcv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/gtktmrxhs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/gjyhnjfkh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.zdbjq.cn/Article/details/gwugtenbu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxyryoxjj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/getkajydk.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gwljukhda.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.zdbjq.cn/Article/details/gkqejaxwv.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gmnrbmcmh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.hesvh.cn/Article/details/gxvrljnwv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gwhipxejb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/ggcuuivvs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gmhkpacak.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/ggnmrhelt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gssucxjlf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gmetvoyvd.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gmlbhlymh.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gffeptdmo.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/gfyzrrzyb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/ghfssksll.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.hesvh.cn/Article/details/grwbwffwi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gxamsgyeg.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gxphkqymu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gegadbvem.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/gyrptkean.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/glgmkuvkz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/ganrswqaf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.zdbjq.cn/Article/details/gxdpwhghr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gkhjxsych.sHtML


<!-- 参考信息 -->