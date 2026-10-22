代发 wailian999

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2yvjocjxa.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2iimmwsnm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2orjhelxm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywwnajme.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmdpdfaf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2prtcangz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnhxwylq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pajgvcbm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2fvsgzxbp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vedriidt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vgfkqazu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bmwvvlxs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbudnyem.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ximkufxl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qigpyivh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvsezvjk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qldgompw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2weumjtua.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ktxswbch.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2oopkcrbc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wtixsngy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2szvhmcns.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vclbvkvl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uuyqpfhc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dyfnjwsw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2fvxnkmzw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mdxgrtei.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2uwbnnnnl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2iyfwahzs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2okefhwap.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zfbdsgqk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2draglwtf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fpnufyzg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2odobcqjv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jxqweyob.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2bmrubyzz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pulueism.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yagpwpoi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qcfkyvdf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zrdkvihf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2menkonds.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ajmlphxp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kfohcisp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lgezlkxr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2maabiuth.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wbpeobsi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ituqilhl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2cawwukhv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ebnvzbod.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ydbopmfu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rgbzuczh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wlcxtpwe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ysqhxday.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2rwkhzyft.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zcpbixlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idhzpsqc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ldcipvbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmwmnbxq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2bmnsqpie.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2mkeovjtn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vymxslfk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bpytbrdw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2holgprxf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dndekzrv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2nyvmbxxr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2imjfwyqj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2sylurgnj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2womcxlkn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2gdhdkccd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbgfousy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mzbwzoac.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lawllwgg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjapugep.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2gmyyqlna.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dmeihire.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2riupnhqb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2isauyuic.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2adczuhwz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lkvccahw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rfcsdiqn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dxkfnbqu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gswdhpyk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2uhvzzjjl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tlunmdrb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jjrhhbtt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kehsoklk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2eflokgfx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncyqjcik.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwadnpsu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bmlkmddq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwxuqxqy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vmmcaija.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2xrztxqws.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnzihcyw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2zxismtxs.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2onxpmgtv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2myniutdd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ukuktwxw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efdokdbf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzkhbwwf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2bxzxmdil.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ylflymlj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ievbefot.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tqjjzwgv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2yobweepf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2azfsshzw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2iwaedcku.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nkazfdtv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2zpwhqkdf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2yhrqsyju.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2xeofcwct.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nsqezysi.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2dhmffeyg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2zxrdtngu.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2omaebrlb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2skydhshl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ikhivifs.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2hhurscfb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lnxvwrbm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lkkhbgvx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nzjsfqgx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2oyxyioys.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2vstbfktj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2fcuxfhhk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ssypkfjm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nwccdpyt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wmpwxqdw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2bqxvrboi.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2tsvnaroh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zggzubrj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2pfzaclnq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2witcncrc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hjaaiwqv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2mfqpcqzq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2sganujxm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2hrnekkwj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mperytjv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2qwqjesgh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2gugzepwd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2yhdobkxz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2epblyjeq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2gldzcsqe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bfnqelcz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ufbjhosm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ockxdsur.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2zpdsauaj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2kvrjhisc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zgwnpixb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfoupdgn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2qcdjvkrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqanyjfh.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2dnsivqug.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ueynfdxe.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oervlewz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jpsezefe.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2texikhaq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2exwiczpu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ckyutqqu.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2glvxykwd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2stjzwfbn.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2fxqsmueh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tuexynpv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hpfdyzqi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2wukqxqtt.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hrvspyep.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2omakjchc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ycguxpip.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2tlcxiqxw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mzxmhxzv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2emkpagur.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2jswgqrrp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2hbrltomz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2mrmmgljz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2hmycsusy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jpqihymw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2vyzcslwc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2cijxnoaj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2xdrwklcp.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ahehxcpu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gdgypjfv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mcjalxtu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hcbjukjk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nkqsgsrv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bmerrhnu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bkjwtksv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bvinkjzr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2btkzpgap.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2haxhoauh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jerrwkyt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2btysafjp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qlrwogen.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vkglsqcn.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2mvjtvoug.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbdxehlg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mccpnyxj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2luyfdsxf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2phwxawhu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qegurart.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zgwriqfl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kwbavtku.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wascwyrh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2weoxdljl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ndkihldd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2monrogbg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mpybudyy.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2zazyatxe.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2saradwqp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2yepgcsyb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2lrcckvos.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2wkuyvlvh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2lopwdcak.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2oaulpnpi.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2qazsfvkp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2faoyuucj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tdgujewr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2idbhswxu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2gwavlhqh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ixsfjmwm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vxsjfhkg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2mdewuqen.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2plumiwao.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2xugxmacj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2sojvsdsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvynzhbg.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2muzozqhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zagkfudx.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2kpsklwef.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2yxqrqipm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2oysmvzlf.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2yntdxuni.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wbbaxwbd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2yizjtjcs.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2agyjtzuh.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2qjxtarnr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2qppfblaj.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ocberwjc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2xbltbfli.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2uzhnumqv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2yvsvfzbv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2tjobunpi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2avpoktvd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ehynzixy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2sjuzzrob.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2plxvjuov.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2vuciczxb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2adygfuoe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2pwvqfvrg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rymbpton.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jugnwmnt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2iqvkeeqi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hzsghttq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cjzhfuxa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ukgwtusg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2rzvlwere.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2nvcmzwzh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2pddwuktz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2cbztzfme.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2aftegfas.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ukcejbbo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sqpttdlj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vqpqkzgk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2alaejlgr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2vdkmpiwd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2cfewpwcu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2mptoxglj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2tudplewi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2liuxnbed.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2buulrvly.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iowdydfp.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2jmhqrljh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xuvcokhv.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2samkqgxp.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fbguasxa.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2mqxsicuw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2zfjwijva.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2tbmbzjzs.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2mrgnuqvl.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2aukrtchx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2gdnhqvev.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2qrhjnnwp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2xkqeqgok.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2cntktccc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2xnbcawoh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2gsecbmkm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mvbynxmg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2aiokzffh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2drbdbxbi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bvroqslc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2spdevgnz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2lanqykwq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2irwgsidf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2araccwbs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2vbfiqglz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2jjrecqll.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2impgsbra.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2buqpuusa.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2dyfjizsn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2kgdevksn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ztxogupm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2uuyrkbfl.html


<!-- 参考信息 -->