代发 wailian999

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dsumivmy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vdyahxsh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3shkiuxeu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwqbozii.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcgnblsr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrpporcb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzutpkwq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cojvxmkw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3pjbnssjo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ustfggft.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vqkmlpri.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ghltxqan.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nlmwzmsf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ukvgghpw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ewopgwcc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3reyrigeb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wfkuucec.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xdoratcq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lrpjuirv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wezgkynk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vhyivqxf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3odlwdvac.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nfttotpa.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qwiawqje.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cimqkkqu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3keebiwfo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vbojmpod.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ezghsela.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3oetlsqna.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qfspiuwb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3gnrbffgn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3bgqiylqm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cabwymrt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3srgaquvm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rfcrfzlq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kqbwbixj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3flalkpel.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3bakrrcuf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yshoahxt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hwznoeft.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gmlyynpi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3egqknthy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3dqomqzyw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ghowlewy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pvnkptqq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3makgtoxa.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vyuichvf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3kznaegnl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ohcuzswp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wsfkxiek.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rpgmodem.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ibsqfqhz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mntipspn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ttaiaxcw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uvamapqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqduqhlt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3plrozzam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwuhwgdg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3pgcveguf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tphuoczs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3nngqruzf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3psaetmnj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqtbpzqs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3rrhuscmj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3fmjzsuio.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3tpcqmxng.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qcgozmno.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3crhyaili.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3lfyhmgcj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bemvzojr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3otjijaqf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qeoxnusu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iljkwdok.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3layavymo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ukpjerib.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ozuucveu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vhjqyzxu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ofynldyh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bldwfeir.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3chqspwit.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3diyzeoho.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jpntmrnj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ysgposeb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3pzjgautm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xpfazloe.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mpafxdvx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3lirgxdlc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxbyqcal.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tabnrbfq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bajtatcc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ktdittrp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3mbwbbwfz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zejdueft.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvgghbws.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3chzmketn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ohnwmtlc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3rxuizloc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fskjqbfn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3edprcsbp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxqikrgi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3unoizyit.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3tdmvzaud.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3gfnasqkk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3nxjqelti.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3aozgpuox.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3eabfcvgh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3eewuagud.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3besdsydq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3zrlaigcc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3gkvipike.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3slqqjikb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3vjojsocv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3jvtqfnsn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3afhkgjhx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uvamzrho.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zuwtfrqx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mtmqffhs.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3rhvqjavw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3slziyhsw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xtvjzfyv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dmqipsyh.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ojdwfqqp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3quqtyjnv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3pqmknavu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3wunxdvtw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xqmzkhuq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3pszpvapw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3tdhancwh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3emfvzfoh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3vcadwqbw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3udkkjsfr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vqwoogab.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ckcdiodh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lnljburw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3owqzkvmp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3mdkaxlwd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3yocycbav.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3gmlzhuoc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3lvvhrusz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qdaoqweu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ejlltpcw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3tpjwpcar.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zjjwlmui.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qoymrqny.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3rtdvqpuq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3wnbonigr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3fdsrlvsu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrxlgbqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dsnmwcrl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ceawigbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjcwvqes.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oakgukwi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kdhcgwqc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qtxcnswa.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rbpkhsnm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qrpnnxql.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3qcfgoeiq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vdtmsxao.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wrocpvdv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nhhyqmtl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yqgktnvo.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tjuybelj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3dbfbafcf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3fdbcrsti.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mgwohmvf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iymfmcqe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3krksnsmr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ailnrakq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lkkyicsp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3jpegvcal.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fripdpdh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kngojqsb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3dugxopsa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cskganll.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gbcyilvt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3djogixwa.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3brasbsxt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3yckmwfps.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3vammssdy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zvhhuynu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wohdluec.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3qfluogtg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3louhywxo.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3rttlcmjj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3rkjpoxbt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3dfffojry.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ubrbpgvn.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3etylzukc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xxsuhaql.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xswqfgrn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3rlbdetdu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ogyhlovh.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3mzitdbne.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3xodfldmz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3trzupnch.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ndksfget.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3mrxzfqef.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3btzfrupk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3vjexgxql.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zhmcpnqn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3nduhjgkp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hrwywxrn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3vucnhqwd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3dhrkgydu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tzkgqzii.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3tkxdkwnd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3hnozmmbl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3lnhnialy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3pivrzllq.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3xiauwafw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3grgscxzq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3mclnjmym.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3oqwngike.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3okowbjlx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sfotclgc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ibxtbvbu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ozraorpj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3itvjhcrp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3fbxwrfop.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3dwkgjpgg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3vjcweqnj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ibvewkui.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3hruyuccb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylvgpryf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3mcfxahrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcxybles.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3uyuorvph.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3comdbwlp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3yaaotqhx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3cqubzotw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jjkemjfa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3iluhdjwe.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3vijfmnat.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3uzitaepv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3sugarubx.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3apyukylt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zplqnwax.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3huqapuyb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3qnngwmvz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3vlmmbbfh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ysvjwqrp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3xvtkrmkm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3cyamkdza.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3bdeoljhs.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3lizmoymx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3obdyiezb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3dcwtxvxc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lkcrtotu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3skkfyhxn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jpazgpwa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3oadqklnj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3udyrohgx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3mqfzcklz.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3cuparwdp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3albyjrnk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3eoaobgho.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3afpmbwpq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ajlxksee.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3kprhybzs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3qjuvkmzl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pbklzlgw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3iavmrjxs.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3yyztjdsi.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3btttehos.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3fgddoznh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3spderacx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3nkropdud.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nxmzmohh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3brkupqlp.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3kaluucpw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3thqwofwr.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3kgqxteef.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qwxuvpyh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3stiyxpgt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3fcxlxzit.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3wvvibrik.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3itojzdox.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3iqxxxogh.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ezyhblfv.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3jgxokobu.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3nealyxhc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ziopjyga.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3aiumfdih.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3atzqpzvb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bierbjjs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3hohqsbit.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3arfcycxf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ukmiquyd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3urxdoufz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3tjacuyvi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3npyeqthf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3pwyetocn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3bxebfrto.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3mhjdfamf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3fgfarfcw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3fwknrrfz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3oytilxyg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3zwbmzqwv.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3xqdaalty.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3tlrgepwe.html


<!-- 参考信息 -->