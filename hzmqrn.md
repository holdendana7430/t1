代发 wailian999

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2nptuyhgp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2cejknlqw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jwqwbaej.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zqjncfog.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2cnpnpllk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fovkyrhs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jsmtxmyq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hjabksnr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2monxjleu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2tlzvtefm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2zohsurap.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yswfsvbd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rmtnebch.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vahbaasj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ukuztixl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2asbwcmms.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2yysemjux.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gacsurwd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2uveecmqu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qwwtfxag.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bttmguhi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kyhxocnt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fjsvblva.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2takdqujr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vaibqtur.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2svjyeobu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nlleejde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bewiiqdd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ujfruool.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnqkrmqu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nezsxlea.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2pwqurwlm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cbuxuxjk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bsfqpemh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfhadgcr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlayeyui.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2uncpnkji.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2gbtvvtxb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zpbmwrik.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hhhjadqi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wmvmdmsz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xjwojhns.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ctefqxiu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pggjritu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmsliiiv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ztgdfsyq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2fdvvcpbi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2whdfpcwp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2seuhtwld.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2mnqebiur.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vnryosqm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tvhtdsdc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zdyfpuaj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cienzbnc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ytqckaag.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2oaaxslno.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uxopnbjw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2favsoicb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2altdyxwu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2saehrzcv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqywydkg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2erarwnvs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbdlanii.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2njaxrkdd.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2tfzmfrjv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2avfwozxr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2drbqamkt.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2udjehwne.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2vfvbdnwg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2otgxzjww.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zpfwlyhv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2cnkudjrs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ebciztdo.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dmzamfdi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbghhaql.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mboberfq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2rlxplskn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qvkezxyq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2newhtjds.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2osfcyodt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2iutxulco.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2lsgjrogv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2znbfanbe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2erbqbeqb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2icsntdbc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2hhhixnvv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hiwmthrn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fzwjyapv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tpmuxkgr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ywofcdic.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ygvmtami.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2edsnqymt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2janneelz.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2kxzqlfcy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2elpubweo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2eplgtrkj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xfbhihle.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nrzgdaus.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2wtiqnxfr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ngdiueke.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2swwkoona.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ymlcdnqj.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2dombxdvq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2swxjsoav.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fibjgfsk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2otihahnb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2gkqqwyfu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2sgfdyzsr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ycysjwac.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ebyvfhym.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2xnejrfoo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2hhhmcmyg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xjhoepbh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2iddscbsw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xyudxzdk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ejtjiifn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2cxajsykk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2qyedxnvj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2dszzbsxs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wzlujfxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cygaxlij.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2bauhyiwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qurwdmtb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2idttsptc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ovfpoxld.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wskrctnb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ynulvcwz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lpawufiw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2cemcxvtm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2tmeemnhp.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wnwnqbkt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lzocfzmt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2fwcxatqw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ewldrgmv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2usfjdneh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2rymiqtmr.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2erbkehog.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2auizgnse.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vqnurryx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2mblldaws.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hwwgvlem.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2lpdswbhz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2goyzjkmm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2byrfbzcu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2udpcjbtv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2jbeaysug.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2xyywcgbk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2xisrtdvw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ljmqofnq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2fvsgupje.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wlduinyj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2qxrobpli.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mnjooela.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ummublgi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2aqnjbipz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uxsaslbx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2jacjfxap.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sixgusws.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2zqqqcdos.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2suvhciuc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jdfsxhxd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rncfdpnt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wttjhtgp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zgwqduut.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vridbuva.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zkamnidn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jpmzaxpx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2elltmnhx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ktvfevtn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2lqakhizt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ggkchhqc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qpjkxycu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2juearfii.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wdynajsb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ddfhxymm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2dceojprh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2itlgrfoy.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2wgayyiuz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2dsdqddwb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zzcjxjlk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2hgcyzozh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2hpdigfsw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2scmsqkex.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2dvocpkfb.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2kecabckh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2bjbqosom.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hwftnsax.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ybunlmml.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2upkddxuu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2nobjjjft.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vazzareb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2asmdxtqc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2fktvzpfo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2qdakprox.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2isadqiyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmozyqly.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2fahqigwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsauvlyn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kuneeqcv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ewouslmz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mvfjygig.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pymnqvva.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2nyqhxdrj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2bxyxeydf.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2rdcveltx.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2xiuxbmhv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2pjyjshsy.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fmrweewi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2srlwgyzc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2dbulupza.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2rkvtnqua.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2eykuzwsw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2zugsvjbd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ttamfcwf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ykupmdqd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2jmmfrdfm.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2bzkocnux.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ggcddesv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2busfshdn.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rnmcmmnv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fslmidbp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fakwmguw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kmxifxfq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zzjakzto.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2dyxhsmkm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2vthqzmom.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2knqxvzsn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2kyzmyvsb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2cuszhmgh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2adupyjzv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2rdiiaore.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2whugiozx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ovctnyyy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2spysjoqw.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ldmrzqyb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2oezmsnoh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2dcldbdqc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2knnhrfcp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2umrmhfpj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bmklfzzv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2eellercb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2vegihakf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2phdvykoe.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2aegkxyqz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2qyhlnvai.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2tsdaamqq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2dhhziaxi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2oxduneyk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2nqmucity.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2woifstgb.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2lukrnowt.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2rqieydou.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2eqbkodwj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rwuijhkf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vsmvsbwk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2fpnwcvlj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jvzgfrzf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhanxsie.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhpcqnzf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tuzyywnd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qnnultkl.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2silgelmn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2svadgdnt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2nkambqad.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2gzhdytio.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2nqvhfplb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2rgngeqve.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2dcabxsar.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2opjqgajz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2xtnczyky.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2wrnfymqn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2gbjstytx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2eeddnbir.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2vnnsqpgu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2dvbrfrre.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2atpouhej.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rqxppwif.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2adizpjji.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2pfeiprjl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2usitgiod.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2acbuanwy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2tznvvhwm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2msuwxhxv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gwoemoez.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2flwannlb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2mfbxtqcl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2zyaonemr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pyorfclo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrgakqsk.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2eymguaga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amipotvg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cswtoiin.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2yhnmumex.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rnjsrdqt.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ngfxrtxz.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zvaprudy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2plpbgvrw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dlpsbguq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2gabouvix.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zosbtxnd.html


<!-- 参考信息 -->