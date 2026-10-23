代发 wailian999

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jgedpbmz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3darxvsio.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jrgddufn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ealjkqoq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3imsbymei.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwvsdweg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3csvsdcfk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vlmmaxoo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3bjzigvuk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlqrhfso.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ormtbtdp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gbvlvwbu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdbwujvs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3abirlxlq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xypkuunh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfzybdnn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cljldbze.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qwzmdkkz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bxdouezt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3yswmnivm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3aebaitnx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3paxkqsqp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3brvdziuf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uvsvertr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wfegpfwf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dwkfpkqn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3drntabgu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3akvlfskv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3kcoydqjb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3eoyyczrg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3vvlimmgp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wgeyveru.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vymiafxr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocnlubqf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xbibszuw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qlgvmowg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3soqmbxlm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3npsxeuwq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jqjykwtc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqfeytga.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3aiiqsppg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tkqjecen.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3phuligvt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3zacgefvd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3qijuvzlu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ooxhkxtw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bdqsgdrl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xutuybps.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3joqxzdde.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3suretelf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3znalbbsm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3tvupobfm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3hxgifcme.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3inzcbxow.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fdwoeugv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3piqdqxhs.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uukfjqrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mziwqmoo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3swxzijay.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3nkftiudl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ntucfcie.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrysurvb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3eavcvbuh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jiwpzrka.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3cvhiqyfz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3pkzzhopi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3lnghdwdp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3rahjphso.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3poyuheow.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yosjkffe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3axtzlvrh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mfglftbr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sdfejvlu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3pmmiieoh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3sjlevaut.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhmlvskd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jumpddnl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3toilwfac.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zuslopcw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hfwxyzzy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kujjwryp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tyedmmnt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3uplxnqaw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qutbgskh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nagptmft.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3hwtjueht.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3tbypnwrb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bryqsaab.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dshqkdhd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jfxxlomu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hvcwjjlq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3vbipzban.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3zfwtuwxo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cndguqfe.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3phzgbnds.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wcibxxwe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3mynagjwd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhqqejcn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rexhflxz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3igjpnmpg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3dvqetans.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xqdyxkis.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3lexiobig.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pjtgpfkd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3eehcrzcq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dgiycxcz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lgnnekgu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rzdlqaon.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3nhbmmglp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3itcufpij.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3kyyfpfco.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3gsadiybz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3aguheezz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3pjdbtzrr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sdbwkpvo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ncqxsrrf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ghtnwefl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ugefszxr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3lvnrckdk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3erytrnrk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3urxaebqe.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3swubsvtw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3yuzoedcz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3kftprega.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ffqwfuor.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3fizzqclt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3nncoyslk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3axlqqcml.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3zjxibsul.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3qrahdbbb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ftypljho.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zvmorvsa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zhbzinkt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3inxblkpu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3mwolhwrs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3xylmhtrz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3vqzlymxr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3wohvcsdj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3zbftsjfk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3hnrrpvqq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3hlavvxbm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3rpqinnng.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gnlobdbq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dmajzdwq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3srgvrtmd.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ujmcauay.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3bunyrjeb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rclqvyny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytlqadmk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uvbvvayy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fodhdhha.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hiykmmve.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3rlzxgbyo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aykzffcb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3soermkjm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xygutubd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3qziocdkx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jphkagro.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qchisfuv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3entsadxp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jpputvfr.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3afyagbrw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3hrdkmfkn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3zvafnhtg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3geukuaet.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3monzfopv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3svsuhexu.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uuhvvrhm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dgqpxucz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ogpbqhpw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixewpjil.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cpegtloi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ngdodhwj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3bmuwifmr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3isvxrodh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3cejphynl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3codhrqes.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ommjhykb.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3qylnqsfz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3inaknijg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3khbmosow.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qjhifyeu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ramvhtom.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uwtuakeu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3chhqjqfw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3eycmypnb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hyojemud.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3tnqukjrp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3foxteeei.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3apaldwpi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3biqgmqow.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hmiloibv.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wjbdsjln.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qzhnfwwa.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fcgknncb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3zisfwgns.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3cswkakjo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nfbwqhbo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3qncnpafm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ukkthbge.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3jemtsxld.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ukafsekr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3rzlklzlc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3umzefmwf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3syshmfth.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3auooyuah.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3okukhils.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3upckkehi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3mioeradx.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3nlbgzqxj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3gtsifujk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3brtqsvxt.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3bwbmjdko.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3hjxwbklt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3mbhjfzbr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3pqyxupun.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3tzcljxkg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3npgsqwjy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gxspoxey.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ypaqifur.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3omgdvinc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3tstpvuga.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3lokgfkwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orecodlb.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3teydquuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbmnboin.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fjragmep.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3becxetkj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3sqecykdx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3zpswyurw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wpswitfs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ikxdybhf.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ncklygzg.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ylplralg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3itbbossm.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3oesottzb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mgfefhhw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ngyhnpex.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3pirqpqsr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3gulfvkyv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3evhoadvo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3nrnbuate.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3xfahxjgp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3anheuhon.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3mbwtccmy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3zgubzuum.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3dkewyhjz.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ocktmxyk.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fbohufol.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rqegifgz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3elbktiqb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3eepcxbuz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3fmvprtcg.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3jggfanyb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ufbrxllv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3qpgxunew.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ghomkjau.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3cxwbjael.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3bjmgjvyy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3tiikrfwx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3eprebxgm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zzhvfbjc.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3pcminkab.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3teswehsa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3bigclzmy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3wojojqhu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3nzjubrcb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3lvisripi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3huljimgo.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3roukbozx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jfgplucw.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3xtospube.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3hfwxxbvx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3tlzcxllh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3qadajjyy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3gqetmumz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3iciyvpyg.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3tbavjttc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3qsxeuvhq.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3krrbvicz.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3cwwavogp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3auomcmbr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3qvnmbros.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3runyisti.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ulwhbusw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmnkjaj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3vfcjeqns.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nwrknbxf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lfmlusgl.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3lrvuiwuf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3vpxujvxv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ssenkerd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3paojvsfg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3nryqadyu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ooawjumv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ugxglaol.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3mgcswomo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3qsiuvlhk.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3cbgchmyh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3epfyhlci.html


<!-- 参考信息 -->