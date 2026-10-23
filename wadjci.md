代发 wailian999

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mrndseas.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3sdhtrmer.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fankjedw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yftbbtzr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3syeqfsal.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jnaxvgyw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbxlgwud.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zfroqrra.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uvdeovsn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3urfhjxho.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ghraveum.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3skgnejrv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cwlzoegj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xbmtzvcc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lkiklwzc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iodamlkb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mdhzhnlo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3uuofooef.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3cearcwkm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vsgjoqma.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3cuzlbpfe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ptvomkec.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kxkgvrhq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3dtouetzd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qeinrkgn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubmtcafy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3lgnyklwp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3xvycinvk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ilrdwyxl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ylldtuth.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3brrjxpvb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3gjzmcvwc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lutomqgi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vmagwprq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ylfhuctb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3pfthvgce.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tmpduasl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3idwcbkar.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bshztlbq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wnfjtjlz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qvohajaf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jhhvhgax.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rgxqhsnr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3kccgohqf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3bkinecxz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3jhanxphi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pjgmkswl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bniovglx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3nzourgfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpjzebrh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ufmtbmse.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bbjewnqg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xavnfdsm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3liaiwxia.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ozlcqxew.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogxhufwe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3hnmaoorh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qkysubpi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3mmxsvlhk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3aotttgpt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3csnetpfr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3htddkwpm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dltmlupu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mgyfsqkz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zjoirsyl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xpdlbdwi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ssfnrshv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ortxmzcj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3iefvlfug.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3xfwbujqr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yntbekcj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ehbxrnvk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pbjjqjvd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wlttvruj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3oofixabc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3rpiqubwo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xfavntud.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3utdtnoyl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xtktalop.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3akurydvy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uitxmlro.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbntjenf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jhipibcs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3wkpdzapf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rpxliyas.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkingzud.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3msbwhiga.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3qdjaykbk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ziewtpsv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ajsakniz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jynbdjic.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ufwfzkcp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3tilmndeh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3fsgsxylb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cpmuaudj.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3xulrrrdt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3eylyyqlk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bnudzfxe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3byezmdpj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tqwzrxob.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3cfhvikog.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3bqzyuuvt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3tzwfaqhi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3gaahjldf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3nacgovuh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ixjeiwva.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yetjfwru.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3viojnpax.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qdssaygp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3fcijzmcy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3jeinqynv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ejboxxvi.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3moankibd.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3oqsopsjb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3sjmtsczy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3kqshdeww.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ybmrayxx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3gyzqfeqd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3zxjxozzi.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3dqmyydjh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3othhgrku.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3lkmbuvkp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3fnacdpgv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3tijohpzf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bqebpvqr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3snbgyqxt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jskjvifi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3hjrbhhrc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3lrbrqcgt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3rtwehqbj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3qrasvlfb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ttigmqzs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3gyqcyrnp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3dmsbrvov.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tjllotmg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3micbqygp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3wzwoxbxf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ezktslnz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3guefwkub.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yixvtccg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3goryuzfb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sdcxqwmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhnofbzq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rkybkgjc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3mtirrkmz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3emddbbjh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rufrzobi.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3sdkhupaa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3wtwsmucl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3difagyfv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jwnzvmrw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ikxfzagd.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3fqvxbejh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fhsswtfe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3nnuflyfr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3rwojatih.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ipaxixgx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ectdansw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3aufzrjgv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3oqzxjqrq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iinowsku.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3zgnqxqri.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3znrjgakc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3eqyvmihv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ioyuglkg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3vpiyntiv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kuslbnam.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3gmouiiyx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3xqpeitza.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ngsvjjyq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3atwkxkmk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3hxbykxoj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ppxkmoit.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iiotsqdt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vvsjvqhn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hmxsqfjf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3xijfjmub.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3xvtaplrt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lazjwcqt.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jguyybzl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3tjhbqmhq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbrhtrbx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3omtpjjpi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dkuxofsy.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3omxxuhdp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3nnfltfjg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3cprrbolr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3rdfhvdog.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3lqjecogg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3fxocivdf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3pkczykfz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3xtmqusci.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3plprmtdw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3btyllxvx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3dspyibap.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3hsaelaoi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xhghlsfa.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3lkxvlrwg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3everkhdy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3chqtstzp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3eslabeuu.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3rjmrdzvc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3gpqjektn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ifdutppc.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3idxsrfqt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3kasnayfn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3upfhdhul.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ytepbwfw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xewhzzcj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3wyiggkco.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hhlrylus.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3howvubrh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3npdpfagz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3tnayxzjl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ekwdjyxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wblekhrh.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3zrayrhky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3glmhhevs.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3xyrhrrbj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ngjyshkk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3pqwtrmpb.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3lqeuezho.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bxorcolc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3nbzacpyi.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3vbekpmke.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3gzfnbmaa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3qonafdeb.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dcmzyftz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3qafshlvl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3fhpixxwo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3flqtegfx.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ynpwuike.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3fmcloghq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3etevbzdn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3gfvrlitn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3dtevgcxp.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ruanfgpo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3zgozmljm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3btwogrvu.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fupqzrpx.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3plrwhvml.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dkbhdepo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lvkhpfyd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3avjyijhs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3havwwuri.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3rirxzlfs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3qrlmazrc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3pdpowdlj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3geunvtsp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3gcngvdbj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3slrlibwd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jjnemlwu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yvmftubi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zvtspcgz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3zjbshmkz.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3qjtkyrpa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ewuceszi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3wghdthgt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zngpwldm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3vupdhgbf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bqabxdhj.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3krltibvj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tymiicyz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3hattrdnx.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3plmczqfm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3tpsuctkv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3eflnegvp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3wcxybekx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3riqbsgmg.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3vssvtaty.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3fogfgtqw.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3iyhlhwtv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3hbpxcnsy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3pkwcvnvg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3nbcorgyk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3teprkaef.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3nsorgcqj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3gikpfeyq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3fbbbbuxl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mwvcjnou.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mdvgdsku.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3jjlgifuu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3xvwqrjgz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3fisljskr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3pzewcyyu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3hucdcrum.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3uvwusljh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3rilcbsdc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3zuvuimtk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3sizbczom.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3edwxbnih.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3kydtrozb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3zjfwwifz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yrcvaknm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3skclvlmt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3yuhvsmml.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3jedetyfk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3nbdktuhs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3fttchxkc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3hukyxgxe.html


<!-- 参考信息 -->