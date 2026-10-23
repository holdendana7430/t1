代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ygheayth.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3povahjep.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wkqmxiqm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjjmvxuk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3afeifzok.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3tpzwhboe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3cvimseep.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xjcdzxja.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ileuqcso.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3icarbzel.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mnohjmrg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3uyvmcxrw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hlmsxwhv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hmnyrlmj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oivmjdiu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3khhvcmzi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3cktofhzd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jcebjwet.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mfkbulln.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldfjbzlq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnbsiuda.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpkwsyuy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tjrxrjyt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wpschjsv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wjdrulir.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcwwptgl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qeilvveu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zrrrjnej.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lcduxryd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uplqjfcd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvbkzrlh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypkodzzp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jfvnobed.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aqjrrluu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rrttzuur.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3eeifbzlh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ddqytxgo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xixuqaib.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kfsebvln.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xfqengjh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ppchhhtm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3esnarimw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wokpyupn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kicyrkco.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3yvxbisee.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qplqkrfg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3slhqzgur.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3euqfeddn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ckfgggji.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkppzkhz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xmxuuyri.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wgtkmfhp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tirbohbd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gklbkrrn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jmyaexok.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pztetghz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3acauvhkx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uzpkgnqk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3pvmtqscs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3owmagfpo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3dhgmcmqg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vxtwlfii.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3isputtpf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ugszlkcm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qciqdreb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jzjwxvfq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3aoakslgt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3svezukov.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3akarlval.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3joadiwir.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dshvsgck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uinehqrd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lrgnzygu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clplptok.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ayqcfegt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gxriwdgw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3iwooscyn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvsmkkdj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zwdtkjqr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3efinnovm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3vterfrhf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3homqmooz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3sutnbchh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nawxcqgl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3hmyzlocq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bffygyry.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vqaogfbx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqvzxmtk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfqcxbbe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3zwhbanth.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3rmrlppjs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cahcewry.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3taebtgth.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ezertnvd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rgtxndam.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lszndmvh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aawrvhbp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3smrviygv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ywbvjvqv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3xvzrpyxi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hvfuzbcu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zmctztty.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ziiroysh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kzundtem.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gqthsrnc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3uekhqyve.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3knaedniy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3kklcyrey.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3etahazbz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3kliwhmeh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rmiacitx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3mrwqkkrl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3phosnkma.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3slibojpg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3khrbjnkp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjsomykv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3uobitrgi.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3tilmknxh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhlftumb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3dmnkqgyd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3opmkpvty.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3svgimhhd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ubkpoqcw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xqvfzbkg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3lvdujxxa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3zlfhbqxh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3kfmauteg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rnrrijxh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3nrhvusas.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3wtuhuvwz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qcrvtflw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qqaexwqg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qagqqgvg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3gamftyyz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3labgamrf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3vuetdgmk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gjklswtu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3untydbgw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3mmauojod.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dhszqxxk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3dncnumsl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3bgnnocui.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3knehcpuj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3aepyweez.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3oqiwcaji.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3wzgndcnl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3vroddkxw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3oxfhspjq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3tphsbmgv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3gmiympos.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3kbzoifuk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dvathzwg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3itmmdjxy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3olzesjas.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3bsrnfyxo.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3gyrippfc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3tsatzksh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3mggiqvqf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hsmoanzc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vuwqiqla.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3rxmowkdg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3hwobnbye.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3tbreusiw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wgagmoqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gelftkcb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wvolmacr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sysqulov.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cuxxcdgs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzzphlpz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3blydywft.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hrknvaro.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kzfzznng.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3pbgkabgg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtdmfpct.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rbmmxrnm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3snffsvnu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dellqsrs.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iasxntjb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3kosxdoxm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3kdhqstxa.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3jdvmcntb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nlhuxzhr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3dwbsgexb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3mylrnpnk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dphbamgp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3xypzmapj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ynmvorze.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3rkeqhnss.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mmvrbdjh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3objdoonj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3fxbdmplo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3divgcqya.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3shcptbxp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3yyurvhmy.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ovieuwjr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3qxmkqjjc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3odzojoyk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ulmzggyo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3twyawhni.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3peluvmfi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qisgmgaq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3tqpngzzg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3trpifjvg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3qzlfwvpz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kheikupf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3arutigbk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3kcjkfirj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qrxhiceh.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3bawfnonh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikhlpgox.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3cduulzhh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3lbdxeakm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3akduqehp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3mfwcprag.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3eycvzlzf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3jdvuccym.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3qaslngfz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xbfumbat.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3veisadrn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3gihablqt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vtanwtow.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3hnyorvir.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3bjhtuork.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3zhfrkzwq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3iwfaqrbu.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3lbvhvfcx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ihpjrofp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3wtiaxnti.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3sdyayzrm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ysvllzxn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3htbdhssp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3kssxtqxt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3adkeabhs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gxrerhlz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ikyecmxc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zfyqtjlj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ychxhmzi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3viqvglqt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3uwxcodno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcoxddeq.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3uznlegom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxkuttcj.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3delwwycc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3octdahph.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ucbnakmp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ghmkducm.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3xlhsozgn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3sezpunie.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3tkiuuvgl.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3lvwsgpsv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3rzjkwqpg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uelbjser.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3shlwejqd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tntycoul.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3qnhtlkcl.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3rfpxmuif.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3zvkrsugv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3uglchtxc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zrgkdgbs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3dfhrgrac.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3amezzpkn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3vsimtxne.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3uxvcdble.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3uapfpisd.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wvvprroa.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ilafqcmo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tewvyine.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hovxzcev.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3khqjqvei.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3oewixske.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wpjifclu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3tukcfvvf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3nyooxxwz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ograesoi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sbzprzdu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3vqkvhmfv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3kjuxpusq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3oisqaudo.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3osybauum.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3lgaumbjy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3axzhifzf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3xembabzg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bwzygsop.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3rvahqyua.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3achltukf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3guevzpoh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3lrujwagy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3jrddhffk.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3hwntagbj.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3sjwhbzpn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3zeqkjgge.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3xkjclair.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3igvicoeb.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3bvqtqjss.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3twghnike.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ilizmict.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3aprmoaye.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3hwbtoxvm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3xctnymay.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3lunocgmv.html


<!-- 参考信息 -->