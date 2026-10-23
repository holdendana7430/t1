代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ickdqhzh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hixdaevs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3yuisdnuy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3rbyvmqtq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gipswuss.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjuswiim.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3vllngfya.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlyginyp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lcqbpsrh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wkpfmpnh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vufaxwrc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3exiyxanm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3idjlydxe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cbvjldrd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3afqwjgur.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dkwpmqtz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gdxydxtr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zgmhhsez.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3guejnjjb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dthjghzo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3muuixgyh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3psmhbapg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hzohuiqq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjqdcwta.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uyfslomt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjmmdsgp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fjedqrzm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dbjohbmz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3noenxdzm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xivrvxyw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xmxlqpoo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cjhdnyec.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nigaodxp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgwxbmbe.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktlrfcvu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3woyxfdsn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3havtsocz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kqzlsvod.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gxwyrdcw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3vlqpfnkz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xsuanwmk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xyxkqupv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wfnyrhxh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dfzamoun.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uztjxrxe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zqadewoq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wcbuarfl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jcznfyaz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3esnyypos.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3axwaqtpf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hfrpphkv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xtcsgati.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3aeivzpxm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3twtdvtls.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dphdvckz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3dopogdmu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3kvkbggtx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kengbvaz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3yzzbzpep.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wbnsbvrq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3clistrim.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lrqobjya.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qskueujq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3hozbhrby.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ibtcmwtb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zwhoxszr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3jusjelzi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3auygokao.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ucfuxfps.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3allbvgwg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nhuuhoik.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vpsbfysx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3kyvwyfgt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ydzjxniy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lzyrhzjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prlhongn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3qeshonbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fykuwala.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3crniypgr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hvpfnasu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewfwncac.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dveystkg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzlfkbkw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3eytvrrbo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nwqvbyak.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3wcryxofy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3sdulkkrx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3uvgobjtt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xykgjpxm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3flsxajps.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iockswmt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3knttscfw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jfkrjdqt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zfpgdprl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3heeypprl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3twwunfjl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rmpwhbgg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3auclssdi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ytavnyza.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sjextwrw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fgcrfoqk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hqggfwhy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3pxomdfhd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3srhotwix.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iswucgvz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3puvkeqcj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3qqswvyyc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jytmtlkh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ghrxgujt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3enslwfys.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3txiwhcem.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3tyyrqpqv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vwycenxr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3txewlkba.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jgxpsssg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mpflhrhb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3vuvzkkxe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dthsbvsw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nnmaaauz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rdwkrmfr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3nmfvniuo.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xsdpcewf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxdhwkew.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qjcencgx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3lepfrwpg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wbyuekpe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nfvxvqxn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yqyjjwik.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3dtjopxsv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jnvawgry.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3vkopokox.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vubdmsvv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3lbrqjxuc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3qfwybtsh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yzayxnmt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fvmzbsvh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dqiqrbsn.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ksrpqvkc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3mltxshch.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pkslnowu.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ioicvwzb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3tymffaep.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3newbllib.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3yceatdnt.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3eczklime.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3skttltam.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ccbgrbhj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3eisxbqub.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3hpmagbda.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3uzkosuck.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3hhrdiyqm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ddmjfddo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rjtijcic.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3auochttx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3mrqujmbd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3vlqsjwae.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nphdhkas.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3vgzfeviy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3eaildrse.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3rtrpliyp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3knqzidhd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3nxiltwff.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ojutpbuj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qxvibcpt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3qrsdfvfq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3tuymuybp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3qjicjvbt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hvgyzjqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulmtvxnz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3nbpvtsph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrpboiqv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ribufwht.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3puzbjsnv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dyirdeji.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gxektrrz.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojrienke.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3pvgxwhup.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3qblkoqyq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3piubtkfj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lnnhtdxi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3zlltfhme.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ndudftxl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3btrdjxce.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3rbcohcjg.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3tjzawext.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3epblzhia.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3moedpcfb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ikzvfmph.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3acmqtkni.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3djykaoud.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3kmtqhbwx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3csrxpngl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ykamygze.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mcmueqmm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3aekcyoyv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3lfhhblwm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ekchhnqz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3dkohjjyl.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rbkmspkd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hpwneoym.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dvbzrzqp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3whhmawsz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zptuwgzj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zkenkcwm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3idlcszae.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3jnpcrydv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dnfumkzg.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xffxhoav.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tsdrvlgt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eyzmtzgq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jykanftn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wkemmull.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jdqswmrw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3tckzvdoq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3poymqmyz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3kicehdwk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3rbltloor.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bydtfidu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3xvotxlpo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3nlqlrlgb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3fdiiqgtk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rbxnchxr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3saileeov.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3hpqmtuec.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xuxmwbeg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3rcsriqti.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ijrfdhez.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vcfyrxir.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3iyrhfklq.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3zswmijby.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3gmfvwrxc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3gfflsuac.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3bynldvme.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3fhreplpg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gxqekfhr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3kcpnzumi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3mbsnvcdi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ddkuwdcy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hrzgxylq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3jvnmzqht.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3gqcomakd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ytdjreff.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3lxqtpowg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbujkdqq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3jcdtgsqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhjzpqpr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3kbsysesw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3kathjogb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3iiydtgbr.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hrsqfguu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3obkjjfej.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ixunsdjb.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3gkvxajna.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3mobvyxuj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3sfkhielk.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pmdajebo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zfqybtko.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3xpsryihc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3bkgbnezx.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3bgmgursc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3qytaicph.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3dpjgowps.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3iaexcldi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3wykcahfq.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3pwiflwrz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3grdzhzaw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3nlhysfgq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mzohoisd.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dcmuoycu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zcsfxife.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aoubyblm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mzujqaii.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3aoopawrq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3qlbtkqsi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nslolmjy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3czewjpmc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nmbsmnbi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3dpjrmiuj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3qxcrnfxi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eeqbtmtq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vvofozay.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3isoutdsg.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3ecaymoba.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3qphqfnzi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3zfmlcuno.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3erfyuwss.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ujlnpsac.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3huxucqrd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3yahoqtha.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3lzpkppns.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mitbnpyu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3qhfhmsyq.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3bqrhhieo.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3fzbifiyg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3pegufqgb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3kmcqafld.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3jvzydogp.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3jjuwlbsv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3bkfjktyr.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3kvirrkxa.html


<!-- 参考信息 -->