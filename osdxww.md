代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nrbcaxip.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxhqdbvz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfizqies.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pecaqpfr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xvesjvmx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rztxxovw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ridejhrl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3spmzjiri.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmjuuzck.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahdwhwyy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3savunkkb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3noczekbd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bpexmrvp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ubqrmoia.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mhfmjrmt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3fqeorqrz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3kbjfecua.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3idpmsflj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3omzafflt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vccbprwc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qazyyovr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3lcuapcjr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xpspizxb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qpxosuoo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3vneemvzi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zifaqywp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fbvxrsog.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3jrxiakhf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3njevsozn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovwrhbnp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3kxcjpmpe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hjkkvhhk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3fcavrzam.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3erodddwf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ngvgqmhn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ixxrjeda.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3bmxnqnvs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qkskktui.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3jtztaouw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3orhvqsrn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zkaslmaf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bzanzewo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3mvxsxxig.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3eixrteaj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vkthewdv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3suxfzwxz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bvjnwldm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3oamxzqfk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3znfmoodu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3bfheojle.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3iraokqgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eylafnax.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nocwuflb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqpqccpk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3glwwuovo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lvwqlvnb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3cejuhzfn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3chnyzmpi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ffcclblr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hmuvsnzk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3gaqfnraa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3zsfmuhew.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3eppbkbvs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3dmurblbi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3rghsjxbv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfrgyyhf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3evvknctm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ugkmnvbu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nlhhlkol.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3absspgvv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mekdlvyo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtikfmgd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3buwvruud.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mswyysym.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qnelkvtx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ytvbzzpo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rfopqfey.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nnwujwcf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3awrwkdwo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3irjjxakn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hxhntahk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3pvqxhcyb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3msqszyhw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wnnfqdgp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xoyhjxzy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3iojvcdlm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uxvcovbt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3sdmokhwl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3owbugdwv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3vhoskzsw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3cljqfzdk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3audvopjl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3scfcocef.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rswbvvlj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3aljqupqd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3wjafjtch.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3txrtriws.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3zryisqcl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dappxknt.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3buoqsdui.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3yfwrmzqp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tisusohr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fwsvsycr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wtrlvucx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qvyloxxj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3kewrmfyg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3dvghxdde.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3uvmuoufc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3nchqfzdh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3pxnpxcjg.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yjiqvjah.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lkeegnnz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3idnadmns.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3htzcarec.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3iglgcvkz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3rzcwwmyg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zressdug.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3irympnud.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qcihizoj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3thrzbexf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3monqugey.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ngrjowqd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3egvonovg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3hcrdbbvk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3kizsiwxo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ugykcoal.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3fmxcruws.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ekyhdzph.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bfkuzpfr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3lftghalb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3zjnvdajf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ablsotyy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3sazlwtbb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3denyysan.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3isrktbtd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3hzztwakx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ztnpjucw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ipqkmkjw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3svjfjfuf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xqytovrz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3khixmjwk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3acfahxdn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3jmwoquqo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hswetpep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aijffxmu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mqbkclcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgzrxaro.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3jefddueb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jsdkiyqi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tsivpdnr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqehccou.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndpndlnw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ggehhgfo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3yredlkcq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gzcgkjyz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3bhhinwzl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ptkelqhf.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zlehebzb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cswcfqpp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3jcdyzkce.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3hmtljioy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3qnqpvzon.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ezwciepj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kvaghdwh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rlalveww.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3otdjjqqp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktcihcum.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3iticekdt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3qmfbjtyc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3keetwubg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3kvvjyahy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3gtjndgdj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sefebtzq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3vnbyibqk.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3supqrvia.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qtscdhlt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ymggznio.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bxijnbgz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vyilxonn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vjpkcfbb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yxanldvn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qbhfenhx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3znqvkeym.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jkziqtwq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3txuqxeqn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gqorvjqt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pghdikdm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ijidtgqr.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3qhudwiqe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvdccpfl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jvutoquc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3tnjufjbk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3gbvnnzgl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3mpxhybmc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3bfbgnequ.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ypyljbgk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3vtxkkwsb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ojtihols.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3owrrxefr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3oaxfkybv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dfnyoikm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ffitgvbu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3dbiripkx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3gkqylvle.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3tbfdygze.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3lxbrsyzf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3esiahqmd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3yuohnvmv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3awswdpin.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3izipaish.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nwznfspv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3lwptyaxa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qygggrmc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dqvhkbre.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3wvljotko.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3uzvkxpfe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3tlwfoifb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3oaoakdxe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3cwzxhbjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgaozpdc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3jkzfrbhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tguuhxdj.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gigdrapi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ylyfnrud.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3hvufhdau.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rmcdhxvs.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3uwzfvkcg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3bfisuvfx.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3rzglhrpp.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3hdiryuff.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3edtylhgb.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bdrpdcip.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zumhjfvn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nhacxdvq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3zpbmrvlu.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3fkxcrvrs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3pksxbaov.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3lzzplncl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3oecugaqm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3cobsawto.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3cwlolzdv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3gzpnejcv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3aeviqatm.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mcnkijvm.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wtpsbrkj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dcfslhsf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3otobrkwi.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fezwojuu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3fqvisvdk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3wjgmqsut.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mpqpqjer.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3qfrteqgo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3rugeudgu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3qvakoktn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3jglynhpy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bghzbdnk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mhcquuit.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ljbmkdss.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3eauqikbq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3zopnphxi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3jsmlshcf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3acbboluq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3mjlcgrop.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3lsiftibn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sjyfakso.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jgyobtbz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3zflmbuim.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3rxnowgsp.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3hzpdkkov.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3shttyrep.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3hipvjhyj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ywormwub.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ufpdwtpb.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3dvsdmfpi.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3qkxlmjnu.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3cnzwtoxh.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3gdfntlxm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tvtccijq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3gjdqwceu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ycnbuqff.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3rfoursoa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3rsapinmc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3eovbcvyj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cycexpbe.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3umdwmjgk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3dujnulsb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3bxkolddl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3dyumjybd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3waazfkmg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3idsodgju.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3cohddftq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qdiukaxj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ntuurwim.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3iznxhape.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3zvkifuml.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3imfmbypr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3vakcpzdr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3dbyxhumd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wuityqtm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3ntcqqnzo.html


<!-- 参考信息 -->