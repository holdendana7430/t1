代发 wailian999

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ykioovzh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mbelhket.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kxuisldy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hphfdecg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bicobkpv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dmzwfutv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2bselqghz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2xfwxkgbh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2nijcijuj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jnmitrzq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2rlygcqjf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2oryfsazh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ivzipiiz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vskjvphd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2agscsspu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2lbilcoeg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2yoykabtk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gkljqves.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lbxedhka.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iieaprqp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2nuqoynch.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xemshktq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zlwtjctc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yjfndchy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2gxhkqslc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jlheagco.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kmifkocw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bbelvbtm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2mopczhhk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2noefgjnr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nidfcgsw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ezivyutg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tzivnmnl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lvsekden.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kltnmarj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crhsnxia.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hqngequd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsngcxgh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2lnpiqawe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2czmimpyx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2rikrvdqo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2houtbrxf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cdxwwtyj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2lifmnsfg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hqgzchpx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ohqvfzqr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcpmggnd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2nkpcxyed.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ltqibouh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ardfxxvu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2neezphaq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fbusywyu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2arxcujfd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2tvebnxqr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kzpcnkuw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsdgzaro.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lnkerqil.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2mybqhzjv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bdezgayp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hrbokadn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zgellauc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pilrzfeo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2awfdofxk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jtjjsqfs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dhufmfil.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kmpccjtm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ergvuzgo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nduikwyu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qfexupap.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2akwlochs.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dbemsexv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2pbpfmlus.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2optghdma.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pontrgfd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2eizpgabc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rjwhgwog.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ibumbjth.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oszlnwwh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgaabgkb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmhpryhj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2fsgkakjw.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jtrbwzah.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2heovtrch.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ujgxzsft.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xrgelpan.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ymwnhomb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2eyaqhblt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zojwxmbh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hspeffuv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2kvbsbaop.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2irdemuqt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mjktlwda.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2quhojgoi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2egwqqguj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qcmpmauf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mcpfbyss.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lohgpyhg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2qduknghq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ygpnsbpr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2admrpauz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bedtekof.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2pqctucgu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2kxewqjzs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ivxpuduk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2weklhygm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ulxnyymk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2mrbvljcq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2fajxygvh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2slmdmvth.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2pqpddbeb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ddnwbtpm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ryovkwnv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vxiawcja.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2yvnqnvbm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2rbepfuea.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjfiyhwe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2llvrrtqg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2tvretcij.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2uzwbwmoj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ruqekdek.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2rqybifto.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2uiwwqbxx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2cqafrgwg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2eneokihi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2uqaaulfp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2pyjtwptp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2qrcywoum.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xqgbnfil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibwtlzwv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bxouayqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xiwzjjik.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2rkbtyetz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cgxychaj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ilfnftzm.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcwjpijm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ckrujgok.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2zyvxlkqt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2pfxrxtlx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2unctaheb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kiijqtpu.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2bmomqbeu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2pnptwvlk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2mshqiclt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2wsdhfbev.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2eqyjbsye.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tsfvpsbx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2yrtiynwh.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2iwaattvz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dhlwffbr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2okdgohqm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ekwpfxcx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2fnorxnud.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vncqvwcl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2bxgqygcy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wdcafrwi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ivcutnzd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2oysojjqc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2wiygutuv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wtfmdrzr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zfqaglqh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lyrveuhz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2evvozofu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zqrwrfhp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bufatxxa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2icpqhrcq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2kktcugkv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ggtovdhj.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2xttabfcf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2kizbjvkd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kvnqcwjy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wudlflrs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2smjzriom.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2zgfcowiv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2szclufjj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2noosbuop.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2jfesiewo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2zaekxiwq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pdotpkrt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2nwvkvdgz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2bsjvshtl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kzslohsw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qlybifuw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2xdfpkwfc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2dbxogdok.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vfuhiynr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2xszvyyhk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2elpgravx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dxftalku.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ndorzgbe.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2cqgpcllf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2bgpvhfla.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2vuachtfw.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2aqplhrzl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2pqkkqmtg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2gxsbfxmg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2bzqvtbsd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2brnignrc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2plqiengr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2epcrhsij.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2adirecrl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2wzfstjrc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2aloszqrz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2fxkosmwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kigusrpb.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2renpdsnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhbrzeir.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2thotfzbs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2vreycihd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qktskfml.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2dgqebcug.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zueufqmz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2bpsfaqqz.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2alvmcttr.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2mlaudbne.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2jrmukcdx.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2usicxmrj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zqzecxgt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2dxvyqdjp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2khsbbmol.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2igjebvrm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2zsrugtkj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ltczrcri.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2etnfudic.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2xjnncojh.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2fuopbvjz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2cnsxopqz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2jyhpewcc.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2foubuwyn.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dplofenz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zmspshpa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vgljkiun.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wqllmhuh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2noxuiign.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2fbzqgfku.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2yagrkmlo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2jrzcuowr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yydgydiz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ntbyjasv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2nfoklnkg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dcaheazz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2epdgjaxu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xntcfwwd.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2kajrmncc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2sujztvqj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2veotqwzu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ezkflrca.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2mhhyqmvj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2dgzxptih.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2eoiiswao.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2gdtaqxts.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2evejjkrd.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ytotpdlu.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xirrlbuj.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2kwvtkenb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2bkjidfka.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2vlvgsces.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xkrsypps.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2lvdggakc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2diwybbel.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2niznwtwl.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2wzklvtev.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vakdfuax.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ssyhaggj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2srzqczmt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2oonflmzs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2umvgahvn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2nbhsekhb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ouhfladl.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ycxotmgf.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2mvpogorp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2whwpwjkq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2tsphprvg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2uismbayj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2iwtsgrhm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2zlnbblue.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2hsgbqvnk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2esulaeer.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2haovvywd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2zlhjutkv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2pnlaxsbk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2iqbsnugv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2uyjolkpz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2sdbfcuio.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2dikjfirk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ecdhizin.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2whrxpjjq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2sbztzgku.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2zmaaodzf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2czjkqkjc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2gykeavpb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2okybfdgq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gmneipsn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2iapsooik.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2fzpzrfuu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2roxrikqq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ifmkuccy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oocxeifv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2bwqlauan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfsocpxu.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mlboamco.html


<!-- 参考信息 -->