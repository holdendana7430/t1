代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bgvwzxcb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hskdqxho.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrskcbzm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yrqyavvn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3eoblwwax.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiutsugd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bjgqfqfk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3solbodje.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggfuqusl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3slbypewa.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwtjabux.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmlodpbb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3onkdseua.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3swzgwrcu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kbfzpzvu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hbzbwfau.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3utkarvbc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nqqpffvm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vetpkjqq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nafgbigs.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3iczbkery.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3rpappdtp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dgfjsixd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dmwaplzj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3eacimuxq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ggbsykkr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3cextfbhk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3synkbgdg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3dlwuomur.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxvzrzqr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3yjdcgina.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xjivromp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ibdyabdz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3eyrajcqh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pcnvzhuf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndevgqxv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wfjnival.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3eanaefxv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ynibnvmv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3inptjvjw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tcpgxcez.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jnkgrcja.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bemuzqid.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3cmwjxafh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3lqxpyyxd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3prwtguwi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3stqcguka.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3gncevwhw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vnovnhfj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3pkwtnpef.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3glqxqwvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxxypgzm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hqpwuezn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmkczpuk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3hpdgukkx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wtyhlmyf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vvhonwow.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3saxiwqni.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3twuqmwcp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgzizexr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ylkjyylu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3uidwctiz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqpdxxwa.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nmurydii.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ofgkwtms.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cvoxiihw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnbaujsy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oczzdknm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqanpkab.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jvfzprqh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3aplpfhiz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uctvisfm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mbebagam.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3sctqhgop.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cswbrixc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fzfwwrjk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mvedbttd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zxbfrrrv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3wxhvzptg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3havgqino.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ardxxfnk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3lwkokckj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fgjsbado.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kipighnk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxddmquq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmlvkscf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bodemipx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ejyyjlqj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ueftfmne.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3lizgvgrp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3padsdrwx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vtupikfl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3atssjcfp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fxizuwon.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fpeykaik.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvkkjltx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3njmgfptk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3onlwrsbu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umbdpmis.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3oyugyhga.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3tvkhuovh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yuepxcgx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uckjqscm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kkdwqqbj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3wezmkbni.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ppcbhond.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3zjtcfilz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qznkkodx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hmexazpp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3bcyghydz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3piqycuwg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rgyjoxwi.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zxzrbdrp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3beuocfjy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3jlyagglp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3mklckpxw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wswnptpq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3mgsonxpx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3rhyaghfi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dudowary.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ayxgvgfy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sbbdojab.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3qirxntvd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3crnlkaoa.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3rnlcswfs.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3qphcrcts.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3vwmqhhxc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vfucqpks.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3hxcjylte.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3dpxfhgjl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3kfnmytah.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtymcucy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3tmwfdzct.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3swprdiia.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3wuxbsxzv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3hglxhqir.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3mtgecgnl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3douproyp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jcxpzzsy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3kvfinvqa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3oltbfbtu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ytjilytd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3faoynfoi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aydjtecv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tocecxfv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3vqfznaqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mydvthpi.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3citicyko.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3iepqmhip.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sjdnpzti.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uqcturyk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ziwfipya.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3exndxddi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cskqjcdr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kdfltziy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wgjluqex.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3fpkkeetu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bdlvvdjc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qitlvdqg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ksmlvtwv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3lswnekfo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3bhnafopr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ogjrhvga.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dhuvjonz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gmvwbywb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ucnulqla.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eacknewg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3hxpjtsgb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hftzzfns.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cjzhvgmy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xkfximfv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3pzkzxwzl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3pgtkavxm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3famnwssu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3lwkqdcbc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3zsmkativ.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mghbfqdw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3aevzaxmu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wvpkzxkm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3eeinpiav.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nhtafpnn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3soixqboo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3erbpxudh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zegmbpif.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xfdloevh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eckppoqo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pfnappge.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3icjimati.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3lscbhzxs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3perbusev.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3iruuabss.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3tsjwbeys.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ozwenwlh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3keuuynak.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3bqqgtehk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3maqwbjih.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3thvccbwd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tvrbalrh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3vqrlfcrp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3jfgkkmnd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3owdzdiip.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3upafhjpv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3tohrhvlo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dxpbkwqa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3clykzdck.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3tlogpwhe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3vtgrmfrd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3lpngrncl.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3wdgtsbpr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3nrzryefr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3vhhzpjpa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3jzsmvfer.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3wovdjrqn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nxyerbrp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zcayhqio.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3drqoalie.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3jdvfdeav.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3uuwerbgr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3dxiopsqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqhapmda.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ldgscdfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jenjjocc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vyzwbrrm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3rucfrtbs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3rgvnoadx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3lsbhhwac.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3aykqlefe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gqhwcndc.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3sapsrblo.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3jritsena.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3empsqixd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jregrcmh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ygnovlix.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3vpyalklg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3nxcwtisr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ekudqpup.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3xejomntb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3cfcnpdky.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3eoxhsatl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3lecrwryc.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3vthmeqjq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3wbldglzk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3mletraqu.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ovrczzmq.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wlyaoqlb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hryjbygj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dneldyfn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zbzglhoo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3cchibwmz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3qgaxmffg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wirutfnn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3egarpvvb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3vhqjcslu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3cywobjua.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3znuficqr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3knjpsbmk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3acfcaaiw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vjjeqlqz.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3opofacwm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3otjsivax.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ucyfeiwh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ybwccnpc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3nqmwakwc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3emleskqm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3voqtgmpw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3fjhaietb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rgkxpahe.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3hnpvefxf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3snryudqt.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3apphwypr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ohzxcdtn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3rbucpqrs.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3xbovfseb.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3gzizquvi.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3sarrifps.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3kbbuuovt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ftrsmafc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rmrrucop.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3mytbyvru.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3givlkdff.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3yfslvqch.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnfvnsex.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3rncwflhq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ixewymrc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jgchzhdf.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3zqmmxwjx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3thubxqjq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3yrvooovf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3qfwlvtdz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3rgewbtbm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3xoxldvxl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ccivqqgu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3qydmrtlp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3fpulbcpx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3vlvugwyr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3poaiquyo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3peahzoxr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ukdqikfm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3oapoclzv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3rhxyzzph.html


<!-- 参考信息 -->