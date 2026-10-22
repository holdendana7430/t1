代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vahzkanq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2preeogyr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ejixlmjt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2arifmpvg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xixwnlch.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fgpfsfiq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2daccvudr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nlemwvjt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xhlrmgwt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ztobrysk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ojkiawge.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fpwpiiqf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2yyjkvumw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbbzshib.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mudkdaqb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2llbltxkh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2dhcddnnw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2uucpvfuv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nqucfuib.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cwormpnj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2toyisphy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxiitlep.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eryssnqc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gdkywwwm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cqlhijfj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fqjzmtyo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xkvgspsg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2avnkiwdn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kktanctx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mwoyakay.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rwtvxpcs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tvvpyiqs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2swroicse.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ztodwpcz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mjlhjunv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2myrhmgrh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qtasloit.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zbgmkoqm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2wpmcmrhb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wudxayfg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jyrfapcj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkesdgra.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2npghpoiw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2btpzokpk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2yugqfxqa.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gxargcjg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2npujbjll.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjyyzwcb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2njwqxvrh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cdvhenud.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2emrgjcit.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2njjsxoaw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wrmiuqmq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pzdwxhtb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2epcacfkj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2thrmhyad.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2eltmrynq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qjvstdzk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qleffwft.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ubdhwnho.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2uyhnxztl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2nxkygnap.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2sjcqzwyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obfcgxef.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ykgbjdau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpyihcgg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ficfunbm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fkstyqnt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2pzzmzokv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2shcpdten.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2opzonmli.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2xtoshhxw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2khqjawhq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2tsosvkfq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynsgpklx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qndhxuwq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2lqlklnxz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zfyclxnu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fggpgvhw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bmotocie.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lvcmtoit.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pkbxxejg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2fpweidgx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ukqwegor.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ziuqhppr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2exrxhjft.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ebhjmcdf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yyhffdtq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tikaaxdc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vqfifrjq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xbwnfkiy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xwciibgm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hiagsmpp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fwpybifm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2slbzyxpl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2phzwdbtp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2twibenii.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2umtkpqel.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrdukcfo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2rgirvzqh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2rxppwhoe.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvoobats.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ixsayckj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qtjrlbxv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zxcekrcz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iypehvel.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzatfrmu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgxkbsnf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2whkpsakw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ejrpetwt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdwmssna.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zyrojdxr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2awscefcm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lfgvafpu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ggbxvsdy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vusjbiek.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2fiuutgox.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2muhwuvtw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2kndbmnvb.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fcdkajdd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2kefmavtc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2disseccz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bdllqkad.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zeakkcuk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2slhxtnzb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2cylvmkzz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2oseotwyv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2nxaulbyg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rsxfurob.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2dkzmhusc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hsrkrqor.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2qxikwxog.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kfwleknv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2dyfdnzzt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2eimgwcgv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ehptunsd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2cupsmtqm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2tobvjkxc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qkvvpuoz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2pvijierg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2fuygkqxy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2qpdnsndj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2xmvzoupd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2wgyqqqqo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2flvsdwxr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ypzfbdxr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2njdnnmyr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2migclwje.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2auvpxgbh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2savifxkf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2aoazokgu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vqykelqm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2zattygyo.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2tusvxkjj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2xfnichjh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fkoakffn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpexldkd.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ijtaoczj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auegmqec.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wrhnhgyg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ltmhubde.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uokxnzsb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2owasndtf.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvprhlbk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2vicgeavb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2kgmkziiz.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2mlcgvriy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lvaabhud.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2uxbanidl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ketgwtql.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2kssyltvz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ttdrsxtg.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2jbhrrgjl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cfnwncfb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wblgdroq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2apicgziy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ygwodtzj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2kimxirvx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvjqxcts.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ijxvlwbz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pqqyewhs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2rwgxkfyc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2phetsbvw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2znwexzev.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uzgjimmc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2bjznzkmn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2mxprcyhp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2djuoulsh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pquzafgp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jtmzvyvb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gwamkvho.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kvkqclbv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ecnjhhlg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2mtkrsvvr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2psnrlcij.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2xfrziycu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbfwrdle.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gxphdsfw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2shonzdkk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2asohgunk.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2dtjpvkxy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ffqblypz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2dhxwekfi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2hweyxnou.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2zloxkceh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jarlzbju.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2yervogbu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2jahaytec.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2bscyqkvk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xmaqeloy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2gmzduhoi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2dnfptgty.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2peszqvzv.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2mhkspaqi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2grzporkg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vbhpkrgx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2rqgkulhd.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2qinptjys.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2zdvofhju.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2qrfqmeod.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2wfcwwjfk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2vhydftch.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2blepmjnj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2tgclnfts.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2seagqypw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lxsvnhiu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2nskmewpz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jwxhqpam.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2bhouzxut.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2apbaapcv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2xnwwrwgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gloidttc.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ibvcilri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awhgtkom.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2jeuxiyxi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2jqdgjtnx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pbiiznky.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wagjmcqv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2omamrtde.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2vtiyoarw.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2xwovehvn.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2wizpiivb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2mxehzexn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2edyktijo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ksigfvcs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2evzbqtpr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2wnsrkcdl.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ymbdikln.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2rngmkojt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2owjxvswk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2uawczsgx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2gkvcizgi.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2iathitrs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ohebxylm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2pfztbajd.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wmrsbxnl.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nolnxqqw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jgnljwsm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hboqsged.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nazapelo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2vkljvimv.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2tjasamgy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ubifonkk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2upmrhevg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2qjzwubww.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jsztmbiq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xodcjdaj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ohnzgxrj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ephhncqv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2edwazhqc.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2tmameidw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2kuchvjef.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2xtkaespx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2skpgzdhj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zefamvnm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ukfilsrl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xdlcvqsx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2mvwvmzqt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xanfjplg.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ivnthmdo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2oipxancg.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ugtumdtk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2vbjccaua.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2orxgmazw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2majynlyy.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2zbppliaw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2cqcolesu.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2qhjbborr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2yzvrejzc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rmwhvwqb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2vfjmsodi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bqmkhafg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2lbohoijc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kxkhvjvl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbfrghwy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2egmwszpd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zqabhnya.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2plztlgzs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2jxyikwvn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2dcduszcw.html


<!-- 参考信息 -->