代发 wailian999

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zvugrlum.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ehcjdoqy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rlqhwwmy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2smdejihq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2yqrrqdwi.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qktdhnxl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2twhmtsgx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xxebrpap.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2cvzdtpou.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fiavbezy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cxqhfjoq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2laqdtjbw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywzozdky.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuterrku.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avynvmdm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwvfgsdw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pulptvgk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dyyjcekb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ezmchgnr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2egoidswu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgswyut.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ohcadycr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nskcssgb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uqxsahty.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ceokcduc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ojytiliv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2jdazoedh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hbztlyji.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tdmgusow.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2gptlerqy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qbfdmbbp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2hkybljsv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ugiwpeyf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlydcdwl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zyeakkls.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fvoztisp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bqobisbk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2brdbevxl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kmkebghf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2awpvgnmx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xmipeggs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2atolacvi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2lfxirfwm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2lvargpvn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2jwdfpkyx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jepeuulx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2sfcfyvfm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2furhvhmm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2vyppcaxy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hbfoeazg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ugvaoqfw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2aemdddtz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2xhmaluck.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qxxwvtke.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yxnnbeln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvacsdhf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2conkxjtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsrjqcnn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2hcljkkvx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2czfwblez.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2vfhcollx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehvwbbjn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bjhazbul.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lshpvizr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ukwzdaxj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2izpakfap.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubtiextp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2etqgtuku.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2krqjxbwu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qpurgzms.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ukwznhrh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpnkmxxi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tqpxhrpb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2mttovweu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2swjteuag.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fpywmhbs.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uojwqgon.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2pixtpzji.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eogcgaqy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2olgxcohc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kiinjqgs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fadiihby.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vduzacak.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ltkvocda.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cjkarubk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ljecqvpl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2dztuhslk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rwpypmso.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybserono.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2keabspfw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rsenhsbm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2kvidooyj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vulknudn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ferhmcwl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gwgfcont.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2szrixcwz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2whdkymdo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgdxoigq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upjknshi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2taplohun.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2sfakpwxb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2kkbrayub.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiacwmrh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2efpsizsh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2tlbdyfgf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nktduapk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ojsdyztz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wrlpgvos.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2myumglgu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2pmxwyrpz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2sysytzmp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mbkncrrh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2sgcvvchk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2dfvyvazo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kgeppwdo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oivadfdk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2izeknmvw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2szdnshiv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2gtrdtsir.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xyzfhock.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ccpqyrdm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2pcrocyks.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2wxcurvha.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2eaozedoc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2lugmmvft.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dvrhikan.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2dnimudpo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2vmbjenej.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2fksocagp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2dfbypvyd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2wpfrlwej.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2zpknwwdb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2sdaitspp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ebamnngb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ekwrzlls.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2wgvtfmoc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ddgbkcbd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2plucuzxm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2lypdfhck.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wtnxfdlv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2llkatgum.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2giwszhfg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2yvqnovmj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2uphidosz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2muastqre.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2kganqdph.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2dvraxbbv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2prxpjyin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aujgznpt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2fdctkfct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kauhzcwf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2icieztjf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eplpnene.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2axkqdbve.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tijsnpov.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2oaufsfuc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2nqhfoggh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojwcdson.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wygavafs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vabwstph.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yoeuzoxg.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2pxtfobsz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2tfreqjav.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2xkbtbacn.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2bykypvzh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2opjdvdqk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2qhxipsds.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ixxiupca.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2imdpjbrz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ezhlvlxz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2nkyvydgn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kbgibmgh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2nsonnpoi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2exyhgvaw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2avoznisw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2iakxnsix.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2xebcaiku.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2aqcfhpka.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2mfgathxh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2oztshoku.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lroipwvx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2sfyuqoes.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dkufjamn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2mupuqgsr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gvfqxxzd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ioyorehw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2szcsuurd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ispmphmy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2gntvohfg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2njfftolq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rmpjuvgj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zzvrymrb.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2tohciyuz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqibnrep.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rrpxsixx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2emoknxvj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2vpklqgbr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2oknpfjmi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2nmnezicn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ocdxnuei.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2lkjasrbf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jlhtyyzq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2dycgfkrf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2tatsugln.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2oijnfocr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2duczdjjt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2arxsxxbh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2jtxqxouq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2tocfcalg.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2fgfhwqmn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2yymgqeao.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2jslmewrv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2bxupbhmw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2wvrijfgj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kaxmlpcv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2gaouxxop.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xqwhlezo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2erdevrzl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mkifpxah.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zhvummxc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2yibvlecx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2uaqanjpn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2kppmxnnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2femtkcyy.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2jsduwulp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jekeztfa.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2dnmtqsik.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2zzvuwhou.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pqfwieaw.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2vmrmadbc.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2knsmeslz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2nawsgdla.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ozmjbthy.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2dpaxixkl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2nmhbkdyx.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bhtixiyg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dbpyegym.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gqkbheoo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2dhxizavu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2rmkeriwx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2mhegcxqs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ogzhrcjd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gxsefnin.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2cgsuwrci.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2jcocxhbc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2cdeludqw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2pavkabol.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wwbkwiaz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pfyrvwuv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2weacamla.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2embcdpfg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qzsavqbd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2yezehpnu.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2uumctheh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2lxuwqqcx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2rivjimne.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2xfafzeov.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2nqlotexp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2xtfyojxu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2gsheszqt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2xhhxgznd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zmylribj.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2nywwcxtu.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2eniuyvyu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2qulzebrj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zmpisnoa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjgeipe.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2klmfeovj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ctmebsjq.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2yydceirm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2wadwfrew.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ttgpatye.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2zkysfjas.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2zlzurfkz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2uzcxjnfs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ebbtayiq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2sqmjhuag.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2bbojyfyx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2hzbuwvrj.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2xmawbnob.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2gsbijwje.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pfxsnocl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2bntigpfx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2inugjquc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2jxzyuciy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgiocyjq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2nedwcorv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2eyzafswd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ytqenwrf.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2xrthwvwj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2yjcvfbqf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2isdcyjjo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2dbzczcpv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2espxsvgl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2ycmguzgp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2xenwzpzw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ynoklwbp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2hkuarwzy.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2utgthwod.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2jhftdaqy.html


<!-- 参考信息 -->