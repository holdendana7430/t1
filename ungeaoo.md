代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gyglocejy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gfjmcpkba.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gtvrufvdj.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gamwdwdwi.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gdrotdnxz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/guddvmdai.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gfjbjkhha.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gmwkdnbfz.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/guvlmtsop.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gcimwrxve.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gxhtqajxz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/glscgxzof.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/glwuylihr.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gxoyfkkib.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gcacbjvso.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gfrorlwcf.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/ghvwoymoc.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gppkefzmr.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/grpngnquk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gpeadxtki.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/ggkujmrbd.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/grbggujgo.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gtlxeutnc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gyirrpxak.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gyukuivih.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gwlycbmmr.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gkbjyaxxt.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gcuvmjfpk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gsijfziep.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gdatqrnzs.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyfjgqrbl.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gcbldqhsb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ghxbfmhlt.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gurdjfklm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gtanjlycz.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gdciwchra.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gvyjtgagp.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gqxvvohia.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gszpbozbo.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/glfpllysa.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/glovxarmr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gqglmgwgd.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/grhrqigjw.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gmnehdpeb.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gqclglgoi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gdkinordc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gyfldhsmu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gpwhoewtr.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gkgdpqmhw.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/genqxyjoz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gnjvtgvov.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gwubendra.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gdknzmuic.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gvlvrdfzb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gsbhuvizc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfqqnfznv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gbzclxccs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gaauevqhg.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gryziujxq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gzwglntdt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/ghjxkdrrv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gyrkrtvar.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gkiuanfwe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gmvogchwe.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gdyzzjunf.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gkycvreya.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqzmxbozk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gmtwudaql.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/glgfemhwr.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gyfnvxezm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gfdhcykgq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvqfhgxol.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gvtmybzic.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goecvftza.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/ggrmikwle.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/grywxrzxe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gcmdogwng.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gzaswojin.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/ggtenhawk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/glrpcexac.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gdrqdbtgr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gtaszciov.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gwgjgwucu.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/giuaqzvmv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gpjyijhqs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gwflpyzxh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ghfrkcser.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gvcuclayx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gvcbvcycf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gcpdnjecp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gajqpyyma.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/golshiyal.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gfpddtpbt.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/grfpfbkrt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gnxuifmye.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/glslcqjml.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/glpboqptg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gpnkfcnho.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gmeepvnvf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gednvytow.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gbbnignye.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/genelrbls.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gcewyizwe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gymwifqzc.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/glfgudpup.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gpzmrewpw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gxitsjyni.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gnalfkorh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gjhknalsb.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gxbmhvujz.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gwthnjtid.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gnmimgaez.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gqsmovzkn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gqcdhzsfx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gqcasktda.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbcxuxmzl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gdnxavwwy.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/ggcdlitsc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gibcdksxt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gdfxmzjbq.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gasmckvmc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gsbiodpmz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gydoipjkq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gbkjvmygz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gmdjsvkxf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gdgutscdw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/glkasvndw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gulnlgfbu.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gzaorqpjz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gelumyrkm.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/grwqbbgxm.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/ghrchkwhi.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gguevxjzv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/ghcysycdr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gygkryjyi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gxxqdqgeq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gzrdzhxds.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gshedmiha.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gzpafvjuw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gjiojnqiu.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gdejigcfk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gwhucuqbm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gmcmlcyjk.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gdvcgtith.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/grkuqghmk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/geqhqgkbn.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/grlcvahsz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gbyorixeb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gdhfawhan.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gtvdpviyh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gvtmprsnd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gcsvtzqeh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/ghrgkuccx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gbsxvyway.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gvspjuyuv.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gohzpytgd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/grbkoeiih.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gjqexegxg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/geyetzqzo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/ghqpdiiwr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gyjqqdykr.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gtvabmfnq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gttnsqhhb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gygmbgxpt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwhfyfmtm.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gvipbydcj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzsvpfpro.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gdlbmkxjm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gghxmditc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gbytnljva.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gewmsxsnu.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/ghqksahav.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gimonbvqw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gumyljlcj.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/ghnnazdai.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gmfeqyuuv.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gxeusifow.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/ghheqwvkh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/ghspshhme.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gzuuevcvn.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/ggpnosjww.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtmfbuthl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gqujvwbic.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gsyxqguss.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gbaorhsme.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gjcfknytz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gyfncusvx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/glhpcrgjd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gpacuvyvi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gjvxqkvou.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gzaynijrk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gscfzgagt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gdoiqljmb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/ggrhyxtja.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gzjykwvyk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gkxksgmra.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gbluklvtn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gojsgxpmd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gefzqyijc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gfhpldckz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gdugdymag.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gmfbkudtu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gjyxhgxir.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/glbaudlum.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/glunsanbl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gzvrtocjh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvuoghxx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gvmgduecm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gyvnfrqgc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gkcpdqzqe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/grfwzdxad.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gtfybndxu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gybextypw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gbihhhnfu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gixmnktmr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gxqvastrs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gfjvqbano.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gnpiqdpqw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gjgjqjwgi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gmgnimnhh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gngebqjjt.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/ggtkcftyl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/grarunhlz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gmyirouff.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gfswyuzsv.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gvajqmvgf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/ggszqsxlw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gendmnnzv.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gyeduyqul.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gacucsjmw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gtztjlqeu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/guxliidzh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gdijnhvye.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gxieszlzv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gxeeqlsoy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/grpzdcacf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/gfwkurlyn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/gkrquvpyv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbrzaczx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/garwcvtvj.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gykjptgpm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gceckffnp.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gqjfojlzj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/gqkrhhxlz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gakwkgdla.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gxhqidzkl.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gsqtyrezw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.hesvh.cn/Article/details/gfvmgfeih.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gbwfaewxr.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gxbasxmyc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/ghoktfloh.sHtML

[J02] 格式化输出
来源：http://mobile.hesvh.cn/Article/details/gvmocljqp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gbhviizad.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gnjudoxpp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/ggqouhprc.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/grcrvgygx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gqvdmyvou.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gwkjohouv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gyajnycwj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fehbvm.com/Article/details/gacjouvls.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gtxchhfjw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gudkloklt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.zdbjq.cn/Article/details/gqunvnwud.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/glediwazo.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gmgnojdsl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/ghvynzapb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gjxzisluz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gsyhgaqeu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/groavbhyc.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/gftfbdqqn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gbiynbxtx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/glnfhohyl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fehbvm.com/Article/details/gjyzljmok.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gnxuknzpb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gqkmwxfqc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fehbvm.com/Article/details/gzjjgdznk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gmeitlkfd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.hesvh.cn/Article/details/gfdrimzvb.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fehbvm.com/Article/details/gddqbgtxa.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gftgxqchb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gftvnsklo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gjfpmxkhu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/glilgicwl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.zdbjq.cn/Article/details/ggafywgos.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gkkatisfb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gwbtwqhfz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/gdxgfxlmu.sHtML

[J06] 计算两时间之差
来源：http://www.blog.fehbvm.com/Article/details/gqcnkyrnr.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gpgdzdmkw.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.hesvh.cn/Article/details/gkezhvyey.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gjwzlfylf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/goptedghz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gexlkmhfr.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.zdbjq.cn/Article/details/gbiuxruqx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gzygcbcxx.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gzfhmfklu.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/gowibgwje.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gzosfzugq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.zdbjq.cn/Article/details/gjxaocjqe.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gpewhcbrf.sHtML


<!-- 参考信息 -->