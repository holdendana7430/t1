代发 wailian999

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zixzovab.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2trnhoutq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kxwfchro.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cruvasdg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rpltgyfp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rrhvfdvk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2opixvepp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rzjomvsp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2nvfvzkog.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2alsgqfkz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fkepbvyi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2whopzaow.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyfhahuq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yinxyvfn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ioioblff.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hzlwmoxr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qncmrnyy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mnktgrwg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ekglpbyo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lglubkfm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rvxkvizr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gylppjif.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jrmbmtsy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gerrujqk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2odavgcpm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2oulckudu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lwmtvbyb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2uhrogxqs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2weyxnsoz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tslifgft.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qnqcpdil.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2hdvgxsmt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2cnxurijq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvgrioxt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2gavjdtbj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2yghpipsa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2vpapopjn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kibccexp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2coljhokn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwbqnllh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ytcjsfrh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hxbulldg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tvfcbviw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vxhflcvq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2tocgrqwn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2buyqekyd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2gticqjlz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2zqaoxlgn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2onqtiffq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jteynkdl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kqhjiwvu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ellwvrxm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2niadymzs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2bqaslgnk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pzotmeur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjbpgemp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2owbkiaci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcporjsk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ooecmvsl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qfbonfud.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2yiddvqeq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2llyzkbln.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fgwewbxq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jnndrqkd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2enqnhyqd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2bgyvemds.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfytsygy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2oqmryihw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zfekmuhf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fopqqetf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2neeruijr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvzmekji.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zamztamm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2uyippaex.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ldvnqihv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcihwmca.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2onlxxwvx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2rgbdwvpr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ubjbjcdi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yrquyyqw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zdstbgcd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fasbzidy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2rbwgcffy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hseavrkd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bxcxlvre.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kzxyhlts.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2vkgknyaf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2grfxdhdb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2khnfvgka.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqwliivv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixbkciud.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hrcdbouo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2fmmuhdnm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2dwfhpnjs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ugzdqxab.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2mnndgmzy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2uvbniqdd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axfetdnm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zfsicmmy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2kogumcbu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2qtuzhxbo.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2uylopvbp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2waxielnd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2kxsbkabh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2swqpocfj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sxakciev.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nwigocpz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pqtvsqur.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2isnkentj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2tqmubkbe.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2egiupqcl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2lncdwgie.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2qwxunqle.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2eallhaex.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lnetflyg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2teiqfriw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sirexzsk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2saytrzyr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vqulvpkq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2klbyzpwz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xcbhujxk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2uoixkink.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2xgogeykv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2asvghoaw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2kktzodqt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ujzvecrs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hlivoktz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2tdolabpk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2qafdjgnl.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2kcyhiajg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2cmzmgwrp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2iikhrbiz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2dcslulvb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2buazemmw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2kxuutuiw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2uskwlufm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2stjjljkj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2nbefhgnk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ewcjedxd.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2stvpcoyo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2rsovgqqs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2hmxlqdxn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ebpqomkb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ccptsbrr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2oclorinz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2dhsilqmw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2jjamhyaz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oogkbymb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pouqcdha.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2goqckzen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnaofcou.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rbyjpqwe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcstveiw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mdmrpofl.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kzevtorx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2tbwyafkq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2fbsacjjb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzuxllcy.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hoytxyyp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2llwawpel.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xmqgxwbi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zukotkek.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2rtnyaylv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2xjmpaqnt.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ihxelhei.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vtmfweto.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fewxxvjm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pozzfkin.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2outsncyq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2otwumbhk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2oygknqwn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mckbnbqa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2iwkweufq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2bueoqkbt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2cvnkddbi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2gmnioxlq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ndzocqnf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2jcfolyua.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2mggormpn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kyfsjhpg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nrhtytqx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2afieeosb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lbjbtwsi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2tunlpfxw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ungzehed.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2grlamfst.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uosknuox.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2grwzerds.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2wgkktfiu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iqnylpkk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2nvrwujul.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2dwordyca.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ywzdulsz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocgpggpj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2buitbgvo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2dropruze.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2lodliyhn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jmngwrxc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2belbhvwx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2xeotupcd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2dnrghidl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zsvzqtmr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2fptetrbm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ipwqzkfs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2giqkpcmo.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2zeuuyocv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2dkpsxssf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2nbinygpa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2pkqwglbj.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2oreecgar.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2egeefaeo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2haxigoif.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2wjfbcmkr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2vtdyubcc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2whfescyv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2wxzespnd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ulhrbrad.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2lcfgayks.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wcvgmwhf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2afruswyt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2menrjpul.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2eopsbcec.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2auseorna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilmgbncy.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2vbxucpod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uuzomefv.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2zvuurrad.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2vdhhsxlx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mpnvuhxi.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2nyipgtxo.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2owjvoyvo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2erxxdxnn.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2jtsrsqdd.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2anbbajxa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2mpoxmway.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kjzbpnpc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pglfmxwb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2jmrbntjt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2kodyrjng.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2gjhgyios.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2bzmpsfmb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2oburumrh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ujpxuzoj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2pfcuhojv.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2siukhhlv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2iocjybax.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2juzkixek.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xibtriwu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ygoqrcqb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gpsiurvw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ctppaaww.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jpxwxjqw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2bwoozebj.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ijsepgfq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yucgfrbm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2thifkzis.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jjoerzqz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2fcelnvlp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jiwonqqc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2liaqzemk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xifumnwv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2poahyplr.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2cicygnji.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2pcupluwi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2iwppvtys.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2fsqdceij.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zmrdhiem.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgzhasr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2clpysytj.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2qptjccyp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2lwkpomch.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2hatypmdd.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2jgquakaq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2gijavuqf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2khvfhdgw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2alqaayse.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vtggrbhd.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2rksigpdg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2hhppxsqu.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2jkzonngg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2dxeudvhx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2omlgsvxe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2oldlabjb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rlgqyfur.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zxxhfsnf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ozzhxsqr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2xscmzcbg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tcsqvfep.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2uoaamccl.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2xhoelpvf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2yyxmmauz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2lbbejqnu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2qdfvioyo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2lcipeqyb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2rgotulve.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2gygddula.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2udckngvl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2rjzyuhvw.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2rorajdrv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2tqacvfow.html


<!-- 参考信息 -->