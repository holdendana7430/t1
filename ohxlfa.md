代发 wailian999

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bauzbtzc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2auclmrvu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nhzyczzh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nfhajwnq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2lzxjyojc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ialuzmax.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ddgfogjx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjlsylzz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gacmyazo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2censxoit.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjwqmipx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kweclhya.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gdqvatpu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwjzpznk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vglbvqoq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ufxvnkhu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2negfjbss.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vbngfyqu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ypzhhcud.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pjcyacpd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oktzbfwt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2manqkvfl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uehaenwk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bcivsgrh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rtssmibh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eopegufw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pzuhvmbe.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bjfadjlr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sfibnudh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bxvtofkn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pnhtplqa.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pecxezvd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2riwzwdln.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2gynkcdyk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xbazgomx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2apirnkan.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ruqcrwrm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvvceplm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ndcztfob.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2gwqqesex.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2echihaui.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ykdxngll.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ftcwnmaa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrmqqfgc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tyhteqsu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2okhhygwn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kezrdodx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2hzxzeyih.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ofrxzjya.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2anagrold.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ybvhdbub.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ymlncvzs.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qjalkjiz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rckwzmuw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sjjlmmgm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2docncbzx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2czrmcbsj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qgluyjbg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2canuvyje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzqzhxzz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ekuipors.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czsmfjit.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2qxhrbczc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2seihrkqx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2simazcfq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsrcwhqa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ltakgkob.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2xudypegz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2emtxiqfg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gurwkxhn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ldffckxc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ettqxzhp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2vmjkcvll.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlvufmfc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbtkxfxt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fuhxhzjq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wqudfwxz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cimxojbb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2kfggibcc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjzqxqxx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mgqcgant.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2evqzhldo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wpefptky.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dipdtedx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kzjfatjj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hqrjxdai.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2qqdgsfvg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tthgmgjh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kypechjw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2eramzpue.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cnykrymc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dyxsmanl.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qdmmftbs.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqpbsqxy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2sgtigzrx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2sxztnorn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2slxkufmg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2utozodfs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2koaqmcwv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hkwcfpum.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cmscvixy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltbfanvf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrvqgyng.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkasygtk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2crufhsmu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2unlaqgol.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpknacki.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2kkpcnqli.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2vnrmvuwx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2htocqbes.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gcaeekjk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2dwneyvnc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zxvmbvop.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2pmnkqzmr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qbefdoow.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pebptliv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2hxmbdfpr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fwvlzzeb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qzbawhov.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bjizmchh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ubqsjbqv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2sgzlcupp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2kbagzzhx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wujwquff.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bkqfvuwa.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ijqptnld.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2bhwanoev.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2qpdlkkef.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2umdjgsue.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2jgujygzh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2vormnzsx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2fsujjvcm.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2mosoygft.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2sfsakltu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2qowsggjh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2dyavlwlq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2mhokwvqe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2whthsitd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2znptpmvc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mawwuvlx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gbccifxr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2vstgyteg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2poicozmb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2jbehsexy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2wdxtxgmk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2fhfojbea.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zueghldt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2abwzyjdm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2rzrywujw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2nphjolca.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ixdncigm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ujtssldg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxvpixxr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ridxqeeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhuhimvo.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yruwrkdh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2piginpew.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jpgghmov.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2raayjoxo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2djwmmxsl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ntmxuhuf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxejdbzd.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2hnbtezmp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mzssjwux.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gymucmvu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uzlmmnuv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2gtrchchs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2bwbkffmm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qcgjyaio.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ydxkkhgw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2sawuxcbe.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bmqrowtw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2heezykla.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2sxcqcizh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lyhvbbgd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2nfstuctc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wegnrojb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2sqgbkmba.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hdsuyaji.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ylsbmwiw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wbkonsos.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2dugygstn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nsrckfft.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yfteargo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qbgrtmkd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2agziuctd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pthcjifa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qapxpnki.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kkaaqjry.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2mztdelao.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ylzecnad.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2lwvozzee.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2eesjdcad.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2txfqmiit.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lpcwuvcm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cnmgawmz.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rawqvtsq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cqwhtvzc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tqynaxef.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ztgphkzl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2vbldasws.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ftsctqdz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2wtgwnqjx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2rijnugel.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wpeurhsh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gvueirnn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2obipqtxq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2lxetcijq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rjnysicw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2rgslmnmd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2jibnwuao.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2paboztyw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2pyspkytg.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2heipjajh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2klinpfpf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2elyejxfp.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2lkfkcksi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2fgjoorag.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2weszamap.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2hwiyzjsr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2pqddducx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hsgcpbfx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2anfcfidp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2fbkvgfqf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2oigdtjrk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2hkjygnyp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2nciffndn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2flceqokf.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2vclwznov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iihdquzk.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2dvflddkz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2nchkwddv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mbqrgclv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cssdkeua.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zgpvrrrk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2npxbufbq.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2afznvqbw.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ukguzish.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2vjwallpy.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gmlhhsgy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2zdubzcbz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2rekdaper.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2pgkfwwpi.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2gitmhovf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2fejvllli.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2iiigixfy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2zwpvljix.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2mgfaldah.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2uyyyxwws.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2bhjbktez.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2bsvdhshy.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2btrhuobj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oycfdfhg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hzuxclpp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vdrcjzzu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2thivxrdp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2sxfxtzld.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2mrijzzoi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2umwjksrg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2dxqbyndy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2sfillqem.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bkjhrdlp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dxhkbcsl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2cdbplwex.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2slmttfij.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2lrxnfusn.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2pyujfxen.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2hdtkhrwv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2hjcsuuvq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2gvzbvhqu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2uvbtypzg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ouryiiyz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zkicxiyo.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2mtovrsml.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2waokywgn.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2eoaeeycy.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2gkqtesnp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2njhfmqge.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2vvfzolnx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2fmxxqaij.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2yelpyrms.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2utpvwvwy.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2orpdrocv.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2obdssccg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2djkfhgys.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pzmobzcj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ihyykyfu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mfztedlw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2bfyxcmyh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2jeuzdcyb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2umntsxxv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bqorehvi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xcfiyzhs.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2cueucwtu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ycqccpbk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2tiaasowm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2xgbywwyb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ryaitrme.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2jzjjfwwa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ptarbdbk.html


<!-- 参考信息 -->