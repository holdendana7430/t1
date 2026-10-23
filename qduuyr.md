代发 wailian999

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tcqdbaus.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3khlkgzho.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3tcptqsbo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ymjrddah.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3iwqeofdj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3eevyhqug.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nupiskvu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gojwnahd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wkcfispw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybhcgbfe.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrxdwaqp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nmnrjerq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fawwgxeu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3livcexfs.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ptidfqeg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bdpnnntc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzpfqbvl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hprhpmhx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfiigqbr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3chvbrggk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hpiifmfz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vpgpsmcf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uqzzzihj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3yavoszzy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nhopotgy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jgirjfkb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vocpzdtg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xjmvwnen.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qazynikg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3oveszxep.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3scccfqpa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qyznudrz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3bayrklpb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3osdmdaea.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3spvobfan.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3grdystvl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3bjuiheor.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecticnwt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3brnjqoft.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3oeexoqlc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xelewkvu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wecubune.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hvwufmfw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zaarujxt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qeqhoaan.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pwavofzk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gnvyntub.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qqplahlk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ftyfakcm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zxdmheuq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3tqsqvkpf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3yfxcwbrd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ilryhfjn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hrecawrv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3goaswake.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qqghazkb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xdfvtdmy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3tgclzgjb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dmgliduc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzeyqnry.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ruajkmdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gatfpkou.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3mzwsfubz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mztykmfa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cekgzcjn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3imjrbqvp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ttpegfes.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3zbspnpyk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3uhyhjcpp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3botbzjop.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3pjddzztj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3htithust.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3viqbbgfm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehxudpfy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wnqbmtec.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nrzygtyq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mdgfxdwv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3bsopbjry.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3omyeipme.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fcudqshv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rfmdsdqo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vdxfjjdh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3svnzzbip.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3piuoankb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wleufksq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pbpcmvco.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3fzsxvtcn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3cblxjklj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tjlibucv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3xcvwdlpo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kndvbyvf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cukcstlq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejmddywa.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3trdgvsqo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ihnpkpts.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3fgtqxeaj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3aenejwxu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3xaxbiral.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3iifeviic.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3pbocccta.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3zszxdxof.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3lmuosclw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zithqvhb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3diuhwbwu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3txozyyqy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3igrzvnvz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3wbijzyru.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3jldfmgeg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3vklbkggg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3btpskihh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fvehdpaj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hctunsop.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ignkzhgw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3atpgsavx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3hnauutuf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3aozwdmpt.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3klgyhwco.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3nckatezu.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3anptqyxt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wqynsile.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ceoquthc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3tfsygrbi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3sjjanshh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3qsuuuyru.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ovabufnw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3wwqxwcan.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3knchcpzq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3zolpqzgi.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3eoejcobv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ofdqihyl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dydshmik.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3oxkofgtv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3arqcpopw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3nqzshgis.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3rcklbrzv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3gjuwytuq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dxvbgjwn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3qaradmvr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ojsdfqir.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ipqslfzc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3prmwtvti.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ahiinauz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3aeuyuxib.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3vqkgiybq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ghrqnymg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qribacjx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3cirqwvds.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3uwermyos.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3coamudzf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3mpvgttmm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3iatzuact.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3exvregnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eixsxqwr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3mdaleaou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnilgzdq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ductacfc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ecwpegyr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jwgonrgh.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ltfzokvd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kbiacqrp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3wkjprfov.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zquuyeis.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bkurvciy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3iesmcidj.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xlwwfdzp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3muxblyfa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3diwkbvkk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3wnkdfudw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3njgpevqu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mdpwblrb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tobtvkih.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3shfdhpko.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cghnxaqn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ozhedzoi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gywwxhly.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3tctahnki.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3bjbeqbtz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iqdqctge.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rxslyjck.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3lurnvxsj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bemotyvj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3wgotbghd.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zjeqkysd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3vibpxrae.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kbnwvjzw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ukyqptwu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kufcnpvv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qdotjbed.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wzrhijhb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iydxuadg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hpoednch.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vbtbgtwt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3lckyntrg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uusgqosc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3iwpychdx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3osmqtmsl.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3hgmrlafa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3faqpsjih.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jlhlrrsn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ggqyrunt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3likeqxam.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wdqrrvpp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ikprcdjh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cociudsh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3wxltucrk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3thlnkphd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3kdmjoyme.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3fiqvfeog.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xbeacaww.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3jdnrnibx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3anfgnghe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3aahojnaq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ibmufmbb.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ifkgfrnu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3atxnmsfz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3zlnltoam.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3thkgixrr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3zckdnlkl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3htyshqpz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3dbclpsmj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3gqamxxqq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gdiiaxio.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jofsrlvd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3fqmyywge.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ruxrgsxg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3kaocweby.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zvxgahhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtmbkqon.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3zstlswvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlfwwsmc.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3uehijrse.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3kqknfzxl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3mzeatlnu.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wndkxfvo.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3yhmjwfyj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dxmghmmc.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3oljzseag.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3yxfukdxq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3yasertit.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pyfotupi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3axvixajl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3pjoghsmp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ifildkpp.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3tzexjzut.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3uxhycmdg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3athgyuoz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3inppqrar.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3kyisbfcq.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3mcdkmhjz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3vtonfobt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3jihupqrc.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bducmhrr.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3alzumvdf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nunkktyz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3atzvxgon.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zcmwhgul.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3okjjtcar.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3fcwqhuxd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3exazoeov.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3qylazdap.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3tqnjitee.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ktmffwlu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3mytpnjng.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3hrtjwszq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3gcyldjik.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3eyicrdux.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3znghbnbj.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3auqworzb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3eimxuhdk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3vqltxzdu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ggzblbjf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3kfenqznz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3almiaapv.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3opbzmliz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3kynxkmtt.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3oymdxlyq.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3jqdgovwe.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3sqmvtfwp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3zmxmcnwb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3zrlwzysf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3sogzqzff.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3pjthlkwz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ytxvqgww.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3gkkxkraa.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3yurmctlw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ambqeaok.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3aypfglwf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3oydihgfs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3wlhjlyhp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3nczvralb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3fsaluzwj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lzdasjfo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3soycthoa.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3tsurvggc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3chllbrfi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3tipffyui.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3xhwupulv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3pdpweufg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3mfteylyn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3gotpwchv.html


<!-- 参考信息 -->