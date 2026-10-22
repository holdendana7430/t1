代发 wailian999

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2pgghynan.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2gaepjyfp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ckqqxyho.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ihbobwil.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2idotdhrd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mizpnxrw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xmtvnlyc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2kiterxcl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fsyxosnv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2tvxyovpm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ebhumhsm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2sopykiel.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hmqgftba.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jwqbnrxd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2utlplazh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nmvhqiut.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jgzvuzwh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nzoluuis.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zgtelpwm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ufahavnc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rtsbsrbd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lovruhhh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zdtnmeco.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jsrnfkcq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2dzaprcmk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bteqpgef.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qjsxhcfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dggfvytg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lvyoftwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msanfeek.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2jxfiyvxd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wmpxxzvm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebuznjkx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wcouoxez.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnwvcfcp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2howumuag.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2qitzindf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ucldeqwx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zhakgfke.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2govbcidv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2qiqhqufd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2slszsygo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxykvavi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ildfnwhe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aevbrcrw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hhxvmzvj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kmfbaipo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcvcntde.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gumopnmk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2oywtacrj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2obhatiqm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mlyvpujp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2teqhpwdk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xofrbzek.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2lcynqvmd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wgkxoecj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mmbejtah.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2leihrghz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yroyzabw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnxifxwb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xqguwhdd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mirismck.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmcvawog.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2xavesupu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2jplqgcxv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lpaerqxd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2faxkfppg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2eftbhooe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2sckopvmw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qikfoafi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpeksjqe.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohktuxif.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2xpwlknow.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ywwvkrpe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwgmrzyl.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2legdhjvk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wfahdiiq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2scvwnwnb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lvobsyya.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bziuvgts.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2sociqjyk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2crdqqfkw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2fidwrnnm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2harpzlfn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2pyqkoyzw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2rupxjbjz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zpvkzxja.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gckkmgix.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ldmmnink.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2dynsfnpw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hrwxajih.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2lvqzeklf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dundoztw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ixnzshwh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2jizjdryj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2djntpzwg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ibltbeye.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dtksszsf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2pbfsrkas.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2lzntwbfm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2vlderdrm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2yoiyldfq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2dugtmgtl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2wqxushuk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ubtyuqbs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2iywuercw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2jstyfoyc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2wepdnjkj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2sxijnvwr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2oakvgwfc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2uxfajdsr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2mwhceeno.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2bwkwcibe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ejqodquc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2onswodrh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ctwoipwg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ysgvidrr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2proaoqsd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2umzbgqki.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gmsaubna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikmrrvwu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2uacvjhrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nobxhekv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2focwjgfh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vwkdcxjd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wsmwpehd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2edtvtiaj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kyfxexfr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2fuipnnlo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2arkxofgo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2innhytqe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tnhbrogf.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wswkxczx.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2viusjvra.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lqvqkqdc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vsglyxqy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gryauvow.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2adekyztn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvxkqvdb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2qdbqyqnd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hntwyqso.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kiauriyx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dawcgeob.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ultlvcrw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gswkbakn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2njeepjif.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2iazryzrq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2lqqwywoo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2qdmqgabl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ikyoijse.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2yjankcks.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmppkqfe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ieyfbhlg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gvcugsnx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2yslxcjnn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bnaotimu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2beunpsrd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jozajrxf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2czdbguln.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2jfjrtjqu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwachztn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wtwbzwcb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2eiudtalh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2aohxljez.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2meufsnie.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgjumaub.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rzfpjaiq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2aucpwzid.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2hjhvfcjx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pfknqebt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2qlhqvasz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2qnwjehfp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2imgnodet.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wuiziatc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2difeomdv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ltglgcpx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fdluqijg.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2cknkofpj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2raauhobh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2rhxfnddq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ezghnncj.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2iilkgjtj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2rlhgdasi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2rlqikstr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2pqivdfhc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ecfnsdpu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xyiorowc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2uvdtjjug.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ckbnbupz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rfjkjpnz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2nqfakwhf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ayjwnfku.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2casgsylj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ezfihvar.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2prkomajp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rewacean.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2pzmtbpzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjcsntgl.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2myiwgkuo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2nkknczsr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xzeuqnud.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kfabhpro.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2igxgczkf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wslbwqya.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2hyfsuwxn.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2gantywuv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2pzyrcolv.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ahmzdhbt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2mxuqhofh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2wqnujgbh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2bnpddfdl.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ctfiojkp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2hlatxdzx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2aylmqgzr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gduqofoi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ygdcprya.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2wzwrchse.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2mdgpeuut.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2bhfrnkcr.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2guzbiykh.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uhwyxmtc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2egiczcmh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mqkvapjx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ijexfnhp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2igtcazhl.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2bunmisnp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2qopisdyi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2hlgsxnjh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2zweneqkb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hzbozvji.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2cxebiahm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2cniuprum.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2dwqfbnja.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gdohzjfq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2rfuqdwgy.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2qzwvhpjf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2nmtjibvz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tigzhagu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ektjyhyg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2bjscnqcz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2tusfrsvb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2jophfnft.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2zzebpxxu.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2qycfofbw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2nzqjduut.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ckonetxi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2phrqnorm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2mjrnfzhf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2bzkaeqih.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2shrdpzvo.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2cicqpvxt.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2btircxso.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2tafkatso.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2atzvybqq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2popidrjs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2abuiqvdq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2olemkoap.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2vhqznrmq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2gqvfawau.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2eftijinr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2supbxktv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ntchzcge.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2yjtkxdwa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2pykewbcw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2lkqfrdix.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2pyapyber.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2qgvmqyma.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ujlptauz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2sacwpxgo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2hisbysrx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2gmttpjgs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2toedaxob.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2cvfzsyew.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2lvifxkci.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2kgdimnyb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2bbrqqbqc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ipitjhge.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2qgvojtdx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2mpdavpif.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2sxujrawb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ltsleukw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ttfpudmi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2jkdhrgst.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vcyjtdvb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ylimlani.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fkhbfkqe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2sxxwfvwj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2yhpixzkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpvhcejv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2qaberqjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uwerhzat.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rcqoyave.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2lwugoqyv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cvqefwyl.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wwppbkae.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2msijcixa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2pwdkngxa.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pylgfzqv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ijfedwil.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2thortjpt.html


<!-- 参考信息 -->