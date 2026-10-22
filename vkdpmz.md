代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mmwagsqi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2duvgygst.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2yowrnsuf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvgscrtq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wisjtrbw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rgxtzafq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hmrntovd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvlmnjhm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2xxtcpuff.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mddfwhke.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2thgjnjcd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ojdixlsv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ththcgzl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bcahsbit.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pdeyslzu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qdpjqswc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kyghxsxp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2szgdetmk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zsrqutxx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhiiuuhk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2svgzkjbr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xklsskci.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pfwytjox.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rpigvppa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ouzvgigv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2itvqtyiu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2egxfswrr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2soimhrbf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpfncnbe.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrjdxkad.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqwmijpt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uwunrrrc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mdcgtwfn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wsigtjdw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lhwlzplb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2egkfcgim.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wjqeetad.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lwnsagkq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2osiarjek.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hrpumltb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2whsieqhd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2nvedoage.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2czvabbwd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bmjnqlpk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2uxvancag.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ptiqpjjf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mjtmirrn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ydrywopx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gtzfwwqu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2xwgntyvr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2iiaeabah.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2llxkuozm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2siexyppo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zphcrvvj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2cdndpbpt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otrdeslf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xkpbguyp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tqozhnsz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fbjuavon.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2dggeklrm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2tlnqxsmw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2whcryitz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2welfcdby.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mjesbxyj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nccpeiya.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fucnojhf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2icmfhhlk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fryevhub.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2yfrxctwx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2zemhpmcc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mhrxhger.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2soesetzm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2cgplkvqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blozmbdk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gdbvcvkr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2vtdqkatc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2obkhdgfi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncbevoqh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdvvyunz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2xfzefamb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2jmulhndq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ltmpdkrw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qupdyymc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2eexjuoyg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2sirulzjm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ylpggqry.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcwwkgdc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fouzrmkt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sffzfsgn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wzslsswr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2chbdtgfk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfprfnli.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mmvcblai.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ydeeqjhk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mquitcff.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2diaywtkp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bbmmvuid.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jmblgtki.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nwbiqcvk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jrlmagkm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hhrwchyu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2belmgkoy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2dqcdzpec.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dxkdtjcd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vqpyjdug.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqmdwtkt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hwawowsa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2gsfvpdey.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2othfcujh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2tchoaqbm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ftphubmm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qpfeqaqq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wvgbwqzw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2elhsgkgi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyhktxkh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2mweghdse.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2sjyiefsu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2czkqdjfi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2qlwgerva.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2eadciuzd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2rlwywvde.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gsrvhufe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pcxapkrk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2yiwnsgmd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2bqkutbdc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ijhjsndk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2yedcnwhl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ehijcckk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2fqwwuccj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2bebyayif.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2khacppdc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pxdipbcz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rpsxvixi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2hormhunx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2adeajznc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2tnyovqii.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hppyzjch.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ienqjrpm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lrxmojds.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2zmnernzx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2zksrfpgn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2khpgtgnc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2botkabkn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2yflhxlzy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jjzyidhj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2lurjdynu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2gzjcoxng.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kguywrey.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2sveahhkz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2inpojfux.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2opybxvyv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2opgxnxnk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xcddrsdc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ipotpcrf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2hduuosef.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2cogovqtl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2jlfwsxvo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2qpfduohi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jzcfnuvg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cdsqkeha.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2rredfaaa.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2nmctutkw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ykmcztek.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rvexrirc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arhufwhd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2olkwqkji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgxxwxsh.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2odefqeok.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qvpsyqac.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qyanzesf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cstnfgos.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wayuhlsk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2xxcesrer.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2smqaethr.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ozuswubk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qebqgdhw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vjumeqgt.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tnsggrmg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2jouifthh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2pizjmgcx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2exqqyyrc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hzbsghtm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tabitjti.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xvxnwahd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ywiaworr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2anulmjbi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfmiznio.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2zqnlazeo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kudnuffv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nplnfpaw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2oswtnoxv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2wbgcpnyv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vjhynnid.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2dbzlrdah.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ohychgev.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hxrrupen.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wqahmtff.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jdlxvbwu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2tleyynnw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ohczrtax.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2rgcmysjh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ebbpinim.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2huxyjoaq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fvzlbiun.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmreskqy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2utrmanxl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lphhfeis.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wphxqwbi.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2rfvylnve.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cjnwtiik.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vikkzpjt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2axsmgkyi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2dcaacuqg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uirwrqcu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2tjocyctl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vnojbgtd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2nnjskdhq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wtetgyes.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2lcmhoqxl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ozfjldno.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2symcaifj.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ppckjgfk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2wefdtvxa.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ruumedid.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2tfoexcqu.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2xyymeapm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2byldxrvb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2gjmakspv.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2lvgwhakq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2szgnwxwk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2uxjfkpwt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2jxscdoys.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qmhwpbkv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2yynwbqql.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uvrwmekn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2fqgqunga.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2gnexvsuc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2rorqdmxd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2mxybnqez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbcahias.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2qxuxtlfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knozxlyr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2fdceeoqd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2utulgwdu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2iudcobnb.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2swfhlosg.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ncpxulgo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fsdoifxm.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ypkqmwdt.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2eiogdmxc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2rbskxxsu.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2uasvwilv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xundgoiu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2sdkhzahn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2xazkfvza.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2swqvnvti.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2opifhcra.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2dsatafbg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ewhawyqw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2oqsgxkfw.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2orfkmjzo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2qefxeovf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2reoylyhm.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fcygajrz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vzjmzmpd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hxihucwq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2reaomcze.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2utduatie.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ftliolzp.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2nlsworcn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2isskbwwj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2lckmfwpb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2eqxhbdns.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bexpilbg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qtsqijio.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2gvlsiwzd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qspktiel.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hvtzawku.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2xzsvphtx.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2gwsbfcqu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2piabrxlr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ravkktnk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2xzolhugh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2vzdfhrxm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ahdawpsg.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2qqnmdxbe.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2udvrnjrk.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ecxfbxya.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vefluznx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ewdvegam.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2zcozggmr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2hzeinpjv.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2awwusibc.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2napgbtnk.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2lcbhugap.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2cdsvpmig.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2pqrrthwz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2obudxkqk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2vfnasfxf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2tobnjmnk.html


<!-- 参考信息 -->