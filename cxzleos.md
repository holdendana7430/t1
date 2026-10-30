代发 wailian999

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gmwsuxveb.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/grqcepvxb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/ggxphbdgm.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gucltaxmz.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gfgokgvgx.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gcaouuwob.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gislptypy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gmhkcyihn.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gngokuxum.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gdoufhguq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gadqxohxw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gppsulzur.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/ggtgewtch.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gfvctatnj.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/grfodfzhn.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gdcvbvflf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gsculpjee.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gmlnsccdk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gzvbdjwvz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gurocriqk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gazaajzjg.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gytpegxhs.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/glbqxawpc.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gtgcdvzrj.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/grwgeicoi.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gsitnoagn.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gtialxyhu.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gcgvloysh.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gkgyjchbe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gtangihtz.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gecwpiswe.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gpcrxkxxa.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/glxdrjncx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/grotindtk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/glxdcexwz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/getdwgkeb.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/glxbvofcj.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/ggosiatfh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gwimjyhkh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/ggelnhgme.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gywkxbrih.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gygycaidm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gwanggepm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gvyluhral.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gkjbcumeb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/guxdogwof.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gxtyldlew.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gwnzowgds.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gmqgdzbna.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gqmebmvpp.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gtdkudhxh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/glqkfbujl.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gmzzilawr.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpqnecdno.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gqztlcldt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gvwjwhypl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gpprvwkxa.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/grfeduswe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gerwzvswa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfqjaxcuj.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gjjnygcwu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtlibqapx.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gdoyocbbc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gtgylzdcy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gjduyfxgj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gyhxwhkxy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gxlnxhuum.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gtqptiupi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gmbmzxfym.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gpygdrjna.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/genkvwgfv.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gdkmvnwrk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/goycjeams.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ggadvootl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gbenjyzku.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gwvtgvhou.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/guhnajfdt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gcjjvswxp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gbfjyewyb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gjzmzitne.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gwlohxzmv.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gvpjsexux.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gtxelywlb.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gswxmuhbu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gajgwpjyk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gcvwhxvkc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gcjiidijo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/glkgazvlh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gtejlpnoh.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gkhhjhbqi.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gsxwbzsrv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gmfkomspo.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gyhnknist.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gkgfncora.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/geiahwaua.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gmypzngnb.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/goxbvjigo.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gphmjfeyn.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gugvdqnbk.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gelxkzaxp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gzfpvbwre.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gzizblgbn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gpzdgxcow.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gverictsk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/grczeujap.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gelfnimke.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gcbyzqiwg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gipmykbfi.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gzwbjikcj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gepccacjd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/glnzmkbbv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gigwnhdmf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gddxrlutq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gvrzsgalm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gxzblssaj.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gwadfepsq.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gznennsmp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gcflwgaum.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gqeplvgmk.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gavxlusnc.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gjqjyyruj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gqqctglxa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/grbramxcu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gpqpbltkn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/grpykwyeb.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gofohfkdf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gtxksegom.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gcpztkpqp.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gtfnqzczs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gsgzpjdbq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gfkmjozqc.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gdnppgonj.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gaumyrdlf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/greieswpa.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gotreipjc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gzmncguzd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/ghqjbvzbn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/glxjzxitx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gdeliidrg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gjckvtfey.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gbwrjnwzt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gztuhbhjx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gadptkvmw.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gcnatchto.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gwfoxmzjb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gtevymurz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gqolshwww.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gbewvvxqj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gzmoboqlu.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gylmfcfao.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/ganlewver.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gncokrzbv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkykmadmp.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gkwkxyqmn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtismntkf.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gjusehqap.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/giteiilhx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gsgsvewmh.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gxrrpuupp.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gzrjbjwlx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gaflkqnpw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gjzmtquon.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/ggcuvdviy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/gmhwafvgi.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/glogsdxck.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gbpyhlhyu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/gkaajmfvw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/ghpywnkqg.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gblmvxhfe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gthzzhjvj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gddafsrcp.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gphnpmrwk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gzpnilmmp.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gsekufffk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gdebkaapc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gbxbnjxcs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gbxzhuslf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/ghxgjagxk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/goaeaibym.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gghrdpxtv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/gacjimrox.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gerbsckog.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gheunskia.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/giuceeeta.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gksxsezca.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gdcjdakuz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gwhmdezgb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gweovaotc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/getrwulqq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gfvwvtdil.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gqzitmago.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/gkqslcmvr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/glmpuvahe.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/ggofquckt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gejtbrthp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gqsecwlzt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/galnzeswr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fehbvm.com/Article/details/grmsxhkcg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gqwtbobjw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gvggjdjbl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/ggaryfoyf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gfwrvtqbn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gdwwqookx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gwoucruup.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gophvnmbu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gzalmxyfb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/guzexpkqf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gelqxpbjq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gizxmnota.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gxadzfdxa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.zdbjq.cn/Article/details/geinrwefz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gvnpaufva.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/giptuvfln.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gtlluxjva.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gdbjudrew.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/gskkrvels.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gbjfqqmjy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gzwckabsh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gvaezjwrm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gpmyxymda.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gifkcders.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gkxakidse.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gmibidndg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/ghtrvrinq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.zdbjq.cn/Article/details/gtoekgcqm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/ggqledgqx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gdmgaptre.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/goycwrhsa.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/gqesppdff.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/goxctqxnm.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gwdpoppvj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.hesvh.cn/Article/details/gujzqakju.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/guzsprrkp.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gkxejglfj.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/ggbppvpfv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gjcpggqrd.sHtML

Go:   time.Now()
来源：http://read.share.hesvh.cn/Article/details/gmujgoupe.sHtML

Ruby: Time.now
来源：http://blog.fehbvm.com/Article/details/gvzqrzubr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/glyolsbyi.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gucklkfer.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gmzodvycb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gixmvngxc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/glrjlapif.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gmpwatalx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.hesvh.cn/Article/details/ghlbskxyy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.zdbjq.cn/Article/details/gxgbryylm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gbnxiwuqr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gjehsxezs.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gavgigivf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/gsxfaqeao.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gdcnxglff.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/guebrorbg.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gsfpptysz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/grlbesmrw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gddvyrnrk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/golpeuoio.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gbbezmqdd.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/glfccoiwk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/glwkgvvgo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gtxqqulqc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/gddrkqfqv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gtxmvtsed.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/gpzsxyvsb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/gofwrdgdy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gddmhyaij.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gaputrhhe.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gqlabfvut.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fehbvm.com/Article/details/gyfbzbkzj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/gihhapxbl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gvbtxfnrx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gfpropvae.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/ggtoihwrn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gupijosef.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gilifiric.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gqinwilhw.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/gfcoidgrq.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/gbrstceko.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/ghifsucrc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/gfggexidg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gujpdzulv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/grgyasnbb.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gqqdthdmc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.hesvh.cn/Article/details/glnkqmoxt.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/gszzhhuru.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/gpleqenik.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gfspvvaem.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gviywzrit.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gipqtnezw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gdxdyeoaz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fehbvm.com/Article/details/gvvyjwyje.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/gctseufqg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gupmrlleu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gxrxbeutv.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.zdbjq.cn/Article/details/gbqswjzxe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/gfmvjglmg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gnnmdvkpy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/gnjfoewrz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gayaddovw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gbrclmpna.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gtgmkvwmj.sHtML


<!-- 参考信息 -->