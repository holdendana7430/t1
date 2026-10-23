代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ubywmpdx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ocmerdnt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uauqvjbt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ikrlrhvy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ncuznvpw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3bkevthmq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vuzxdzfj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rgknhzrn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jofpflba.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zotxrakp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vsancwhg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsakjsgm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnjzjfvp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdzvcvxw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pemppfgf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3acmmprfc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lpzflotk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymqdqcdm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cbwhupdf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3boebtaub.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xlrmyrjz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bdznrzna.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sesmrexq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yefoihet.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uomcqdpk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3unewwdak.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jydzxmwu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lqlmedhq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3svnpyefm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qrbrlvyv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vcpemsmj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ffpiuyrt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3okljdswc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fyjidloe.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3gxgvprca.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ixkfewnm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3drjnbijw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gbzhhtzq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3jsofjxwo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3atnehlat.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3fxmhrjnb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xghuvfng.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3cbrwszxm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kmelmwyq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3hnanppkf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3voxdihxx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ussnxdpi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3orgettgd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3nwtvkhra.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sjnwzqqf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ddkgsgkc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3podibfyo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qeoubmgu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xzghzhbf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hyhfvrrm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qnzsphof.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3yfpbcepf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3njomngnm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gmllytsz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qbhsxxpf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3hhndkubj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ozvzllxx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lfovmuxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sstnzrqs.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qajxhzkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqkzogym.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vqmpeven.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jmhvcihp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3bzauhrwl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzzvvctl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zokcktia.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohwzwsrq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3dibkxkvo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rminccsy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3dfnaijmd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rwisuzls.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3klreqmru.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qrcskrmk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gssmthcc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kihknhya.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqwmzvlu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3qqnmawry.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ovdahpeh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkxdarpw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3opvzbruz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3dyetnyxs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3clvuipmp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xzlbvyih.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3okxxtovm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mvighjnr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3zukrwsif.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3mwluaqvu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rakosdgi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3vgfxlgba.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3onoiuthd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uvtumxnr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jccgento.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mnmeykpt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tuhntthy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3gkydbgqi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zorqstlu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3pbwforlz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3fkqwbrxn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rvxlqutp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3voajoemm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3solxqjup.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3orafkvoh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3dvervned.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ujjmwjgv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3djdcyibo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3orozhmaq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3xvmtoeit.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ilgroehi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dljdekcx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3sbpvebeg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ceqwswdz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rtknqhnn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3injajelo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3tndcpjmy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xlvqfhda.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dwmwaave.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3vkztqhjb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3odlygwsd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ospjyuax.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3potoybut.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3oglmgkyd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3probtoqs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xqonxfjt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3edtqhxvh.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ixrehrfz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qtwnycrc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3kehwqksb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3spjgiptq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3beggntnk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3oebkqgot.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3kgpmkosz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3hijavpkc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3rdhmpyop.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3bqjsnnno.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3wqapiglr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zzcwfsvf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ktdslgko.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3qlhjnzbc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dhcosdxa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jdxtebva.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3doxygchr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3qdkwwpvl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3irowxdxi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3irwghjoc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3bkbnjqnn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zrbhvgvm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3chwckdvx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3tdbjwtly.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3acoaaebu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3kuypwvjn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nvyvgpyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbtxrgkk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vplpafvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfljnifg.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3xqymshto.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3dnwbxtyy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3daxxokbd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3urlkkezv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3afxkridz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3mymijkdy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bwpgbgev.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pzkzwoxe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ixvjopio.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3radsdvar.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3frircnjb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3qmmxxrek.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3uswxwfva.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ynkumxlj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jclrdpjm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dgbikyqo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lkoizwta.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yzkqksgu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3skqclezr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tjezvlve.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vkbwfoqd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3rdyoaglh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vodpdjwo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3kllcrjad.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ybhtzfgb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3oirzkqbn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3mxdtgvle.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kxaywxca.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gjnztfpe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3orrlneoc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3euamsity.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3bajndlml.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3nfqkxbex.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3kefztjiq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3amuftmnj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3elzcvgrr.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3zbpmmiuc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xscseevf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qhbyhmld.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wbkunopl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dalotrxz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3qlosolqu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jubhnakd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zpztfdom.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3jclbsvzg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3lerdxayh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kskldywa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3zdwxrptg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3lhaxbpva.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ciyaazme.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3cbtjfhwi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ppekyxec.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3qqlugjnm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yccyrkwn.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ccvqtiso.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3gdhhwslt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3oyejpppz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3yetftwjh.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3jvcpwdlf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3okruooqx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3qgmwbdat.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3eqxtffpw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3nurlquew.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uvcxsaje.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3lqwuaqtz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3bpsomqsc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ptnaqmqm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3apwrvrzu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3bhlxnkjv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3yzfjoprq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3uinldver.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3hbbzuvjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hljlmzcu.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3lqnhazpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3drsrhseq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3habzobfz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ttfxjubl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ahgywgiz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ovfypvam.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3oshtauxt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ppqnswhh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3eaiqxjga.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3gbouqqcn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3oguwddlb.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sibeebmp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3jycvudby.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xntducpz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3crimxccq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3wekgadse.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3lirjbcbl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3ebnqvoij.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3gtlqflbu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3obwccjhi.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3gxtxrxif.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3sxtmqpdz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3sexfaxif.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3frstepig.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qzsvujbh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vjbokzdg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xshhklwp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yheuujbw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3xivcjmec.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3mvyjsdyi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pkkdmdfz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3athnszis.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3xdqgzlwl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3qgkpkmma.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zbefmnne.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3xwsmnmew.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3aahmkncw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3nrpigczm.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ieebmmgj.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3wnyncixz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3byhzxtgq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3fbzaqypl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ltoiqcpr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3umwqdikj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3wtffqmet.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3pzeocwks.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3vmdgbxbq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3itjktiol.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3eiwzaubg.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3djyrrjco.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3fecnimks.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3szdrratc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3yrktewof.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ukoyzqxm.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3clofsngh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3fixzgddh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3hrvzhwms.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3afxqzrxq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3lrstcsoc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3xhjzubba.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3shkflgds.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ygdzpydu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3gieumcwa.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3imzpsytl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3divrqpeo.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3xbayfxep.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3jjtsieam.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3pzltusvs.html


<!-- 参考信息 -->