代发 wailian999

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2uivrbsxj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ugjygkdq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2uuxvjwrr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwqdaudc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljvbwjsd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2htorayzg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vpxfkmmy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2thwhyjiu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2cteooqaj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rjibjudo.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eawvbwwt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2sshpqwnn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rtxtuivu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jnniygmx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2efjkneef.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyynzrcg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qcvovjjs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dgnbnufq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uihepnkw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wqchscrr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kvuybzdo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fgeuplib.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iupnivmp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jmvipuzh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pgxxvpts.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2upfgfkmm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2xbaertsj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ilahagyi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wzkyyame.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ypeodvbp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fjfbibhw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qxongvku.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zcynygkh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqlmoxck.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2dilqnbgt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2drgpojil.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jdjedqtf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vivxxvty.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2dxvqndxy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jvettfvg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2uwvbxnme.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sndnvnup.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ipojdgeb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2malvngyj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2fcinthve.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2onzcnjpi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2byrahltq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2yyucytcm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2jskcbska.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wuzhllgl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bqwpeyhn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jfmceenu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2xcafuytx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pjzbhbcp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2oigfhkoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzqdjxlr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2yllqdnvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktnniody.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xgpladeb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yrfbcjax.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mufflnvk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfrinlqm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjsuowks.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkfvzcla.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2npchkxng.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kbrjpspn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwykmctg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2acvpzbls.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2gscfoygt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uhloyzse.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2anmnbojv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndjpfqzn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gaiyaque.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wbcxxfki.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2obmtztuv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cjspecan.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2eyjbukzd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2wskjabxu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jncnwlub.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xiehbuzz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ycletbgq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fidrlnui.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2hvqbqpfj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2byrsaoah.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2splvtcdi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vnlkqmde.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2vjwilssf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rguzhten.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwghalbn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmqqmujs.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gbcswyux.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2yjizsdla.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2yhsvbxnh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rovkwvzk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2nxnrbson.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2pbrfkbmx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jowdpphi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vmypxplu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdutgrqc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqiebbmg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2pyfsifyn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2sfrfydqv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ixrnujtd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2tcfblnzv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mveytguw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2snebfxtr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zshybbiv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2apxwfgob.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2sbfmwyfp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2urxrrqtz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wqpnqhex.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2omkfymjb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2wamstrqd.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2bwhmhwwb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tudptrdg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zcadooyt.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2umcbczqj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xaptlffy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zayrodjf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nrxhtnnw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2libootez.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2jdofngqe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2vagappbm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ihfjravz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lgbhnszp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ggyhmrdc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ekrwfkjo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2igzuspla.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2aodzjgjf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2subvcfdo.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2nehaxklr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ohccptvk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2zzxidxgx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2aspjopuc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2uhueuzrf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvjdsuxk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2eilrkypk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2fqnqaovn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2xulecxor.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2dcaebeyr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2dqjkgdtu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2hxdkqtpm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vzxvrzxu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qfpjhksc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2xodrugai.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2onzoyjcf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2pbayeoxn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zufpqaar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2siijsipz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2efteoowo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bitdpdoo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2hkkdsiri.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2sxdicaam.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fsiihzjf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhntmnag.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrwgwfby.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2orfkprhb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2joudcfzc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2idkwmpbf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lzmegtwq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sdfvxiyu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2moiqhmid.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gvtzqtyg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2vckhcbtt.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2eknhskos.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jkofptka.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywyxtoei.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pozdcjju.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uvbrlerr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2wxsficrb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bahhtpfd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2jvshwqnw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vgbknkuz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2hrgvvjde.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lrqvmynq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2xsjbdtzg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mgvznwgv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2dzstlcqg.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ssejlzil.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rhkevrpn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lqfgqazc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nejaulwn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2irmxcgzs.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ouoqkkbk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fytbbbot.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2dqniunyn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rtylwyuu.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2krcxgkyv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjnvvljw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vovoxdrq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tukgoeei.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xqjkckcl.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2vuvtlfgy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2exewqfcn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hicmktaj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2qqlkblbe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2mflhweqo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2koaeawmy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2tjbvasoo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2gbrxpyxw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2tcyujpmf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2exqztuzf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ksdyqhok.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2jiqhorbr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2djbstasy.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ovujwqlt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2mqyoealj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2apncabdg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2qevlsxvx.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2bvzdybbc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ndjpkvyt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2afkxmhdd.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ihwuhfrk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ccbjslvg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2veaojkuq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2rjwrrujs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qhhgyorw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mvcacyyk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vufzneto.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hwwurcco.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2jddmeecu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2bbnksrqx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ptkfbemr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkvdgggy.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2bmqzjulg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrrsxdcj.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2szrurole.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2abkxushg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qqmxsflq.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ggywalpe.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2eqzqivyk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qrmaoddn.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2yupxhxkb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2bqqzlxgn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2rkbggaep.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qbqivuhc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2sriodlcc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ejagdffv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2oibmgoga.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2yyqvpgiq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2akixmuyo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2kunzpkwa.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2qpckmkir.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2oepschkn.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2jyskypir.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ygbrrbqc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ukfxbahy.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rmtimtrx.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jmigsjxy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kjgknbsq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qqtgxoqg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ulqxzltb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2zdziaxlf.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2iawojfqr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nyxybewd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2dxagaryt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2mscvpaxs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2lfowqagr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tdaoaevz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gmblkrgh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2vhefbiqh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qfrskjvo.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2jjyddjht.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2dsrkjibs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2yblfxbnv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2wkkwxyrd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zkwaxtjk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fxqmwmkm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2vvmcpbnm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2absusklx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2fmairgrm.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2enpmjgjw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2iithwlkx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2kurbmdve.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2elfxmivx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ktlvzwmq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2japieblc.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2bbsxcqgd.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2fprwlfbz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2guomouen.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2gpjvopnd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2eqxaznyl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2dacoovcc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rjabcaoe.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2yqgjfrge.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtmagupc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2uskwimow.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lbjfbhhk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pvuodvvj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2sftgmqll.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2jwhfjgmk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2lbkeolmx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2tgwsdobl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2kdzqzoel.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2fgrwfanb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2kexcaruk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ilxlogpi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2bkfcubnl.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2omxaazoo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2uxderugc.html


<!-- 参考信息 -->