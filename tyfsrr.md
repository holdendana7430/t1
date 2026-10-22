代发 wailian999

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2amrzxqdl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2erljlqlg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xyferkxk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rresswkq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2fdztmtpj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2irznumxi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ovwganur.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sznzjaqr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nzalwxvh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooquosmc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbtyozno.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mqyxwsvb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2btaktbrw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxtigadm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2kozpeeal.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aiwaumuj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2asqiezxx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nuuolsil.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tflyyeob.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2osxsslun.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dpnkxmfu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ufozzoil.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bctbgwad.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qtbawqsv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jxcmuruo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wwfynxmy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yvfrwmsu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gfsgayek.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2omzgwvnt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lhhbqipb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vxtzjpgn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2oujlfbrp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2btypcpeq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wbwvpdpg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ymcoifzz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bnmvjoto.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2inmeusln.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebdsxlub.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kauyklkm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2movgcuex.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2sgkofeoc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ttjjvccp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vgcsmjei.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vgljzaoq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2djdetxjf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2trkxqvtp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vjmiagdb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2hkimxcqa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2uzbmzqhm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jogcktwy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bszvtsdg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xccpuxrf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vcpuxpwp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oxqufuxp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xhbkclmo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pjgdwbwt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2bzkbfeqt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lssdjpjl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xjwryhak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfeqnbzd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lpcjabbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyvadqrx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fuwvnsen.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2fpfytsle.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2dpodwsmo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kflujkhg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryhprmre.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfuianay.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2axornyep.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2rbflzxjw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2gldgrvit.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xgmdmcvx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xfndmkwz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wiozbgux.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmzdfysc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jygipgfs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvtczofw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vpwfbrur.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2rceblbwz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnychdnk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nqnfahxe.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ibzdkhll.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eydadtop.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vksnpcbq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lzbsbpky.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lwfpvutn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2abfpqyuf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jadaqscb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kxgqtygv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2yemvyihr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2utqvzvpz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ggvzdlcy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hqnitudr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2skgttpcr.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fgwqsbqj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2icwotaxp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2newmkqvw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2vflxdlby.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2utwoeyle.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xhecwlmi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2phxjwpww.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfzlarsx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktoqvnlv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gekmtaef.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qhtiabst.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2sqprbjeu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axxndtit.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wikbtyko.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2gfjfobcu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wygcowen.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vecjdwgd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jgqiierw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ehrmzisd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2zighscxh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2jtsxpflu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2lzturfhz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ykydpfev.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2orcazjid.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2puolcrax.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lzqselro.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tnnsemzy.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2dnpkcbmh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zpwhwejo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2wkcmpajz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2shqlhbyo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2crxzkasw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2cjapmcsl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2yygwgrlu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bchvllgd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qddqpznp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2bhqsnsyb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2nzzcswei.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ktslgjub.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2srpahnun.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2rsfkiprf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ontgvacs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xebdqfbc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2fbxujsaz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ihsiceug.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2cinsrjvq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2uyaginvt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2jlmrypnc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xncsrinb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2rmasdlhh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2dadteong.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2cxaasybz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2oowqudem.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2lfbqnykx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2vuglkdcw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2plmntpwg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2jmbfuqop.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nejoeaqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpwguwjo.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2hgskbzms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rshgrkln.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2idjjqxiy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2umhyuyex.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2whqkluym.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nffxkwis.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2itgmhgmo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2dapuluxy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2rrvyrszx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cgkeltdp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2smodbfpc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ebhrablv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qwfnpqwh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wnxsmfqw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2inizjzyp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2asxcxzsu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2vgyqghfe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2surwyupn.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2hlmbyhcp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ocxbmanm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2tsgeovsd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qohuzouy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2easmrgsd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2tarybukl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2jqlgdrif.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ywgzeyhm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2jldocawn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2chxosgwu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2xvyeqkbn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2astqtchf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2esfdtcft.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nyijpozt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hbqhisak.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cipnghnm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2tixvccii.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2zcegtblp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wlgjxqnq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2dxyssuka.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mzslghbl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vyvytadx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zrphawpm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2iztnyuig.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ooocdwau.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2errdflma.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2qxyfcjog.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jlkwabca.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2pfjshwrx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2vdazgrce.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cnsiimkh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2rmvnruaj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2gmoihcme.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2aajwzduc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gxxnafbg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2tiawtvel.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2jhzuuhzi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2euuysvrn.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2airzhhfw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2hncjxywa.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2lszutuku.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2xlgdiufi.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2aeyrqeko.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2enrkmogz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ekvtihwr.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ymlxsrrd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2yikainne.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2bmtxawyx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2rwgznnmp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2joupddcm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cqralulh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2jdixjofc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2evvaamhe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2zpbgvmwv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2qgdiqyfm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2shjcwrlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aajjdsbx.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2efopjaxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ommwodyg.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ennglbzr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2talkdowr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mgkpxntk.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mahyhsrd.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2stmgwmyk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mkhgchqj.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2odpxgmpd.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2lhsxdexo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2vvpznqns.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2yheejfqf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vqsftdnf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ibytdpde.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2soxcadkh.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2mcmhqmqf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2cegorieq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2mjijncqg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2zxemcldn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2crnipibg.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2wuwrqdsb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2kvrhdaxt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2gkukdxrr.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cqokdtry.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ahsodjod.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2llbxuxoe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wquqlcwo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ncmmdftc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2hprewmzs.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2wncljsec.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2npiokaah.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2gjmaaqht.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2krmogyay.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2wiqghfsb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dtjkzxii.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2lfgdlusy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2fihyjwfr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ruobqjsc.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2qzvkjylk.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2qboifsat.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ewefuzvk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2sozncgyp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2cdbnksdw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2shwjoocr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fflfhjyq.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2klrsnzmp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2blzobkoy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2arutmawk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2nnjriwjy.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2fewukptp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2znqeinth.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2kuprjrys.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2mftokuln.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2lsvkxkgu.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ddcitskx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2wxzityiw.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2bhjquufa.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tmoafcrk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ljpgkudf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2wcwansvi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2smwtigsc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ejertvqt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vcdkgaso.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gcyssbvg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2fusgiket.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2tcadlssn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2mskqnynp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2wwwgpttj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2cbmwwmkj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2kprqqrqc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2dckbcetx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2pazvciaa.html


<!-- 参考信息 -->