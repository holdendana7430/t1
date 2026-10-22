代发 wailian999

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2irssawij.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2uoskpgtv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2royojjnv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qvtnmqlv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tcgxgdmo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wjguosgv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ivfmhniy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaoidwvx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfvruhmk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zfklcwdg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wcyugyuf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xjiqiwnc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zrjqbocf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjqqsrzd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wwqceltt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ltlirczv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qbsaowsc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2unahmhth.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qmwwdszd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzznsjju.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xkjkyxeb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2joqjnrud.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2knswkbza.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ldytwrco.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wblgnbkw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qyljijvi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ahyotovi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eqdqjbcr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iglfumkt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wsbtdvkg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2aewsslee.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qarolgof.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lkyygvka.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zuzubsos.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2finknscv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2arfhfhbs.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ydndeepw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcrxkqdl.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2jqtsmyss.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zfgyryqj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bfavuykp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ydokgcrw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2cmbzlibu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtwpajms.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ijzvxmnm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qdkezdtv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kinzubhj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2pgrtuufp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ymztsxmk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2feawvhyp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2oskhjvjr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2bewwizsf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rbasavnj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2atjwoses.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2revvetzs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wwnivusv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2hrshmfky.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ouyhjuvv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ourangxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdlygkqw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kyuqhwir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tblaufuw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qzdduoby.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2evfxzqmg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujvvptvw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2izsmvuwr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmymsctn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2lmczbzul.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2plnxyovq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2oltguzpw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2oviqapch.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2mtyajcps.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2grjrgegc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zdscukke.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bsewhzyj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qeejpyxk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gstfiavt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2egvqcwig.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zpckjden.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2judsnsys.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xxeqmvqp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2pqbnlogb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gifiyclz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mkhywwtl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cyfdxzoh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vrubrwvg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2xvymvzzs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2glbnuaex.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2avbwbloo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2omrpmqjd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2akxtgihf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzlpyuzg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxtqqcjm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jvitvzol.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2svarmcpl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2dgxttoqk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2njgpzixx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dutbedms.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ykmzmfrq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rjdsesgs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2pjkigeez.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yiehyfum.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkuwqvoz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rqawsqvi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ixvhfywi.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2lezbrxsr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzhdakul.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ojoblfnx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2fipfzvgh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ooecutod.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qrfxxuno.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kpoqgrge.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2foifilrm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2xkkfopqq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wbtxqowi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2hzfxdrbf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2shaumvzl.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gbnjaceq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2labtofjq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wmykwpub.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hmkemsxn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gzwzwjlp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2pqjokntl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2hfxiqxft.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xtkynaga.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ujnefsgi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ekybkptk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2igzsskyz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ccwzeeke.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2skojnkwu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2lefpqyua.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2rcfmftgy.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2jivvzxyy.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2eohbqckq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2mvmidfeu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2sssvfjdt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2pjbegdwg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2qwdwwikq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2hgvexfne.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2eizqqwkp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2degtmiyd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2lsvtjxhn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2huloslke.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2bjuozguj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2mgrmdruu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2tjgzaaua.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vkfoekot.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2htmbyvwn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ezfulawk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2qneazcpg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2fqzcethh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yddeefua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxpjrqkw.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pggebdgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2biztmtxd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2agnkydsf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbbynwqb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yxcmzdwu.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jaaktmmq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cqontmkv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2rbhbnlhu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2qhvekwbu.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cjrzutqe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hcrdqkgl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2apiipwtu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wismojwp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ydfrrptg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2hvyuhqmp.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2budgmapm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jntgjgxj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jfiaasbv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dimcpnaq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vyhdztwd.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kyazosza.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zkwvqlxy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ldypbkry.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ducgtdpp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jribzxmv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2odgehirm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2hccssxlr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rgrouwjg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ouhinuvh.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ppkfizui.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrnbdpec.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bwglrblc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2tzjhxcpy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2afxmsnsh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wosnjizv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2gzcrchqx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dkyqzjdx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gphowewl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2rnnyjjsy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jslpvofb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2shzxggno.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ykzlhgia.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rwhvpdyk.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2yqltxmrc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dnmnmvnr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2dtrbdyvs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ypexoluz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2lclfumtm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vmuqrukw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2yiergsbm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2apkkhoet.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wljttwwh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2uozffmvo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2fiicbkrb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ovjyxomq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gymfxogf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ereruvrl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2uqocwufp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2toesyrvk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2mewfrkgo.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2nxdoxdqs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2kmbqnalq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2hqmdteqz.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2okdjyrpd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2obguxyjr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2qkqvparr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2xjqbtnvz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fljizbzx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2kbsyodaj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2imiyewkp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2poohyawd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2rshfvkhq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2rqfjhbdl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2iyzdxpyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcnhjtux.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2isprzmcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkzrwize.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2koxilwsd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dlduchxu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zyhcaevh.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fzukbzbe.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2bpfxwsbz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bqvclbbq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2natzakyz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2iniaqrij.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2aigtosek.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fnujuaab.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wsiwziln.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2putxyfbo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2gqzbaely.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2svvrjemb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2wqzlddbk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2pyteixoo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2crcwywzm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2gdxwngyc.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2vftibrbf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2xcxdhohe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2rpynowcx.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nedisqsh.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tnaqdpyj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fyffdhsb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mdnilnwa.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iayiamss.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2vmbgohxd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2rrwhhdxk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2xngynsng.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2fpnlwnjk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ksxvslyx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zbgrjgba.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ebkdipeu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2eudtdxez.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vsqhnttn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zvovdkxy.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2eggdocom.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2qmhfccmi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2jnjxlbmj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2khheebki.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nejnonio.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2awjkwccx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vaqcjdhu.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ognzedox.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jdkuxxvo.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2hcppnkma.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2qevszrsm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2uuzkphkz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2eulbmwtm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2mftymtoz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2egpiyxrv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2wyyvcfov.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2mmixgbum.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2mxiixnyv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ewuarinp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vgsfrrhk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2pylqnnkq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2hxqnxasm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2nyhaxkti.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2glfdwwhk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vyenvnif.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tkbhddky.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ayqnoitk.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ejfmdamu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2azjqvpxe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2iagqowcv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2svavalpw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2omlyicks.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2vuepxjsu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2fyvcqpwj.html


<!-- 参考信息 -->