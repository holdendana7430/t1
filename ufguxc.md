代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xkixfxgk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vtrcetyp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yxrgvfad.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2gkfsknsf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qtqbdqyx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iychquho.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iesnvkef.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hcvgtvnl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ykoozlos.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zedmghko.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ytkwkjtw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rhrnvrev.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jdnmxqub.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2unouhzvc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hckiltwy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ujkatjus.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2yzlnbhmv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2refmvypv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2rhkuooce.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rphmphbz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kmukloig.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2tigqjwxb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dabywaco.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vkkultkw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2twtmnznj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jlehwmal.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kynrryad.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rvntwkfm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ffdgffvb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fxqrriwe.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bjthduow.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2euffprjw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2oaocfnpg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2biacqsrj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xsdqpqpg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wierbkva.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2fkcmntam.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2uweeiorv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gubuyltk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecmdfpal.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2umfsptkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cargdjal.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nuufcfut.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2cbkipgjy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxafdyua.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2unxutkof.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdwxcmpx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tahwgsxa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vjksmdfx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2hktpqomn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zrxzoukd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zyzrlptq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cccwfwhe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2znbgggoh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2casprvci.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tlivvfqs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rssqlzsu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2xqjtyunu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qowphann.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2orgnfbbm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ccsdkyyf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2loohcvvr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zxcmawqr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wviduliv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2apsajysa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rlmjevfw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lbpmjjpr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ynlxhptz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lnicwffo.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2jtjkdclr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2kblvzugb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lwzveujj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cohlpaxz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2sunccwws.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zexngpya.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2crxnnbbr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gdovvrya.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdgunmnx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2vwnvhkjd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2esvihysm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ohuxexcm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vgpbfjyq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcpxtblt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2aezqwwnq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2adjyadgj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2lodaxmsy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2isnyfwjp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2vfhmhzbt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2vowualge.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2njgoxtiz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2azdeazgs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zrncqwii.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2adhisthf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2dmmjdhum.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2qcwyrgaz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qakveype.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2qxjuucbq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2djnbbbpw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bxvgljlv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bbcuqoui.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cdeiztgw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2hjndghzu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2dkjkkysr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2czjxguqg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oznxpcsf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2nowsbaht.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2xafspdzb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2vkxghefe.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2tbaiqjhq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2figeiwma.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ujuaowgi.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2mfnbljft.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2qbnbbmgt.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jtlmoiuy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2buvdoipp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2vyuofjjg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yvcthuww.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2kkhfzonp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2cdtxaltn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfeqordc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2iypqcxvp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bsktcsyf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ousrsscb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2owrxgcjg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2shmsawhq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2pdgurpyt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kgpdgatl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mpgasjmr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2tuuvwegf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2nwcivexf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2iakrofnu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qojviscm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhcuaqxr.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qqpmjtad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzvbsixr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2fckyghvt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2taiqonfn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ojmigujs.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qucchgsp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wpvbmhby.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2iwnrxebl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ouzsneix.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2esvfyori.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iihewdnc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2nyifqmxl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2jmtlregs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ottmzyjh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2rqvagxfu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2cfthbfgk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2byztwpqv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ynhlybxp.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lbunmwao.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2emxlmzoa.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2myzwohmm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2gsvlcloo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nizohofq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2yjpjcfrz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2mutzyzux.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ynsevcmp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2rqikqaer.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2prdwfppk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2eozjznax.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2bdwesytk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2snhrtsmp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2poyoectx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pevtjtst.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bfghhjfx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2yykwfrrg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2rlvmlrjs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hunletsv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zdvlvijp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2xurxadfc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncsusaip.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hysnxkzh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2etwiezoc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bokxktik.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rjncqsmh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zghfnkpg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2srtsmwtv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2pfnqppri.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2acnbdixl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2prgetinh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2piusjlsl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2nifecmyz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ngfbhkht.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2caigwmek.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ydcvjrjt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2pldrlvls.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ikzdtfwl.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2maqgrcut.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2zfzodpqb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2sjnanjnd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2xihusjtn.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2zahzjddj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2muhcukoa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2lguxutui.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2iiggijxv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2glhwiiuu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2meknnahb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2kztpkoju.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2aoeydpqa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dazggder.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mukuszbg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2gdtswlld.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2vjfbvlsl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2rlleuzgp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2sptdppsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpecuxsj.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2qamjlmew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzprffya.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2htrlgngg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2cnsshtpk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mwqqikwk.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2njypbeel.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hegkxpga.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2peosyuqz.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ksqcfpzb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2fopiuwle.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2nvkdwdxz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vzupakfx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2eltebncm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pbftqukw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2gmxpkywv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2dipmtepe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2xakppxmh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2whkmfaqe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2trlnawsl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2oqtjlquh.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2lxdoybst.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2trdwrowp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2tvqmatji.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2iibnhqod.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wuzouxuu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uajlcmqw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wkkdnapa.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2typdwuue.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2jfravmrn.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2mctkhfey.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2rxiwyshy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2jhrthhjd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gjnlanae.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2ofvrwaur.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2vvzcmgqq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xigxpelr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xqnjzbkd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rcthfeks.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2wbrggllf.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ocuyivtx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2teznrnvi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2fgqapxpr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vqvddvzd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2wvlokzui.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2xlzhaink.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2zoysjxxt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2nqgxtozv.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2udibqsvf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2bdecfere.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2hjxtxvgl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2kxipywlj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ynkdlugm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2rkqmohgr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2nhehxfyi.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2zvpretyz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2dyfdukox.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2nlelobtl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jrrvhrdq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2owfxxjlh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2myhrjcgt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hdxsbbfu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2wuwroejn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2mwfanzgw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2osdkyusm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ssdkeqhq.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2smrcagpv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2pjwdqacf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2mhjvffie.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2dtjhhzst.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ubkclabd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2idqeppue.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2gdncpdtz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2lifpmmjq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2cpfsliat.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2usbhficy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2hmshiflo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2banxxmpr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2qkocyzne.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ulacvjwx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2gowiwkqu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2hveeuazy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2xtatmuxv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2nwljerxc.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2qnsqknde.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2pgkcihau.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2qkubzwtg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2iecgmnsd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mdlawndw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2djvtidtf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2nqstjwxj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2szpycgut.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2fntzuikr.html


<!-- 参考信息 -->