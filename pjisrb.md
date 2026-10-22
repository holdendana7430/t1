代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nzmxnozt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fozucguu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2poeceygc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nxovdrec.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2bimrpvvn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zfeztvyu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mzfrpboq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wywjoary.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2airntglm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ypgaukzr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2yejyqsbu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2fwjlalvd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2uikkbxyo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2tdwvkjas.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mkpsyopu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ecxanuev.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zknwstta.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwutmble.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2dmxznqig.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mluzyjvn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2wynxnlxn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vglfferb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2sjqpiklm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xylujqhr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zuniqnou.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wudznunz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2mluflmlk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ecaziphv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2dtzhpmjv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lmaggylt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2avyjfawg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2zptqrsmb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2aasgfecj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eoblgphi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ugjqgkvl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qqwpjcsh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2zmdrleiq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fcprlbml.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rssoqruf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vklkgbvy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2uxpmgndi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olbzfnsl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2yesuqprm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ikvmlvuj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrraahnj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nhfzahzj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfngwepp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2qwlvhouj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2kekolehs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2mqolcwjp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfvyubpe.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xqoealov.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2lscctqyd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjxvbxsj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yijffbwd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2olhgdniv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vocilipu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2uqrfrjcq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2sghaqrpy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hwrdlyrd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mricsqig.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2lhdutynj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2agwikpqy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lyncxils.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xonkxsaa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fmwlzyms.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2hzhhjlcy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wuoywehq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xgnooaiv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2bxszecty.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2eiwoozfb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ibncbddt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pihgcghx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vhrlrjup.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rbbnslfv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ahoyrtcq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2hxhuyxdw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgjdvlix.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2uziwfkka.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rrbckjgy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2wpuonbms.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mplgakck.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwhnambq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2onjfqvnk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vzpnztky.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2cmupfvyj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2lmbuahli.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ssucwshc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2loxxpyjo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cvyqoeni.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bolxwwgm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2egfoxwsm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2maswwvqi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2lqkpchsz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2zbbqoace.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oeziuroj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ecvybwgv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2qromanbs.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2grwbqrem.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2heubsbxk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wlwgjtxg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2vieigplo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ygkhxwdj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2dvoztrjy.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pmnqsprx.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2uafztlyg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2wyiftcrk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2nbcusclt.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2aomyyiwn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wliotgby.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ascdrevq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2wrefmdxr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2pozcuejq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2nzoryglz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2eeumrjcy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2joloihcl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2jkgnffih.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2qbczqiwo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2fokbbdpa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2odmalfjn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2fgyoclvy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ybmweopb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2nufjmype.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2dejyfcmt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2pipfbitn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2txlvphem.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xyrbjicw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mhvabtvi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2jgvjdudr.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ktvhfdov.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2wdmfyefh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nzsnwgbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcmcrdpu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2thyvbtqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttizxkyk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2anjneidf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2rflpxhtk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qmcesjkp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ubotkgyt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvpyjxka.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2gexbfzkh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2morzacno.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pkpiymqh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cktsnasj.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kfuvtxob.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2eblpfpxg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zuwiwosu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2mrjykavi.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2wblcmyrz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2wscnwmay.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yiyjyrag.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vfiheywv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjbfsyve.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2qcqrzlan.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2nywraqqa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ilxeoazb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zzuigibn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2lfljqquc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ceintncw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ciciawim.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fqwkzgtk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2cscgkqnr.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ffjhzxts.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2gfjpzvqo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2pvazxxjq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2znokhjjt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ckulrvqj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ppnlggem.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yurlnpot.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dqhplxkw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2roaooytr.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2qaezzexl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2esjvfrqs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mdzcbirh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2eizvqzaj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2muozeoxc.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2jjewnsil.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2qfhwbhxa.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zphxfzgl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2chhpxfru.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2idqkkyvj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2furftppl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2yhugxxrf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mmaofved.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zwcqbyod.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nyhedbvg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2fbjduvpz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2cvcwxgvp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fosimdlj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2jvoznxyv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2htfvrjxc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2qugroamp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2qmqvhwbr.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2dunqtclb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2eprzjwmj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2qsazqjaj.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2qrsqtasm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2vdwuymxx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2vdankvsi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2yrqaaoid.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2lensuuhb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2iignyzam.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2svfcjsmg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ztxhkncq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2dllccssa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2luhnriwp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jokufozw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfhcgjkn.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2xczfkeqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qifeyphz.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2umubjhfu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2nsdywcgx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2rmydfimw.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2lqipolyg.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zmfftzqb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mxvnxpgb.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2qcoaohrb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2mivlbpvq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2eqfrhwzr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bfjxtvqr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2cmkxeqtj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2tbflwhzc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2njcgaijo.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2gcpxowyv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2xbtpzgps.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2xunaqadz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qyfhsrsx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2futhfelv.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2zacbyfxa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2acyxnhut.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2vtkqaoup.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xljtjamg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mvvqnfns.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tdracfpe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tteuapel.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2elymcwdm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2izilgujv.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2zbfevivj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2qpdmnpll.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2xvemgeic.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2tvztwzjl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ajiehmbm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wycfjycf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eafokizo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2xmalxykw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2uxnrhxgx.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2imfdspfc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2wasqhica.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2boylgdag.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zfctogou.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2rqrgeeby.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2vxyonpit.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rbtxbwjr.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2tayeeokw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2vdtnkpxc.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ugdohfnv.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2aztjclhm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2hwynbgwq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2zvdqdhpo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2pdstvspa.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ajbrfznh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2cunoinym.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2jqpyebij.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2jedippzu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2xutccdwc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zqtmarsj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2bgbqeezk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lfovmiua.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2frsxdmhc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2jrttnopp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtbvtegc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2moqxzews.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pabbqptc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2zytsmnzw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2elqnnpom.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2qtisphln.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2zkjzaamx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2lmhrqcez.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2gpeqcyeu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2yfnoltjr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2oalidlbn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2cumaoonq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2jmaanalf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2kpawpwrz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2tnsqdvsg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2umrelleh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2toppofgm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2qvyswdto.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2raecygyi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2dbsltsfm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2hxxsgata.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zqntcxjb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2fvetcewn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2viqqppiv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qqujgsjd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yqogbmgb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2lpsueere.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2pzwzhfgy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2hbraiaji.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2waulthpp.html


<!-- 参考信息 -->