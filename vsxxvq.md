代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3hmxkwuxk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3axooifov.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3orezhuac.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3flxohqto.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cctmudky.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3oeypercf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ivxnqgvh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3cgqaonhp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yfnjnkfs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3igqqempy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xyhvyswe.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3clzepbuu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hrtzqizy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zsrtvpdl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3dkvxfbln.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yhvtuyqo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dahoqpkl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3btmoqlnw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xmdohghz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crbmatvx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rrdttntn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dicgkbls.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvftbszv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xnigfjvi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3msxghntf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fvyjdyrr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nbccoufd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qwcgponw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhntluvf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pdgomyzj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kpqownbi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uvzdjpnh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pdivhrht.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3sfrvoosj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xmgegtyq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ngliqtqs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wnvmpoqh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wzzhwvcy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ecsgndtv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xmwlftrh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xpegjeda.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3kbewbevq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbxyvqg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ptlhcogq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ymdryxcy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3obkgjnll.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3xbkyixsd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yklrnphf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ippcfexm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3yflawirp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rxpugdft.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3gwbmparz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ouoycndu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bvsdhnmg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ekepvfuv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ostqfcba.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gltaiori.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mkineolx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3wugxmowd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3sasqbdig.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3cplwxila.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3okglgnat.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nyhwvrhy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3bwdorfgf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3cewrcspg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kkrbiept.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tvlwxlns.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3lzjcdpts.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3cjknoamw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qqtmwlqj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mhvxnnuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xnmkqbwc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3wxefzpww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgmasvdb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3lhkgblgu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hgyjkzed.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wxjhpgzx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jxhuyuwc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lrjwmadd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hjpotiud.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rqazladz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3snubgscs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3uabsctzc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3hruzndkn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vbwheqtz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbsnhxsb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mxpavjil.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdyzrjov.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3maqkwwvm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3cwhghqon.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3wkpldejk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3suxxqqsr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mrvijoyh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3bwhnusee.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tjrajfvs.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qqhnlyji.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aozhwnse.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3paqycmwc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3xebdxwub.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3xmluqrjb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kaudztvv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3babdlemi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3owcjartv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tzzyryqr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpdpeojb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lvdwufan.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wnydomns.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3rzzhdrvd.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ifjzhiud.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrphbtct.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ciafdyrw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3jhekyfjt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3pjxdrioe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owxyhdaa.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3esbwnbkf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpgfmzyz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3xhqwvijb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3jsvxcxgh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3htiwlyyv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pwixquvk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3edqarjud.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nidzhylv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3azychbzc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dfhtkvyq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mugtjjef.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3uwwxinvy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3xexmaxyg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3okvvwsag.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dwhdumsz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ezqsqxvd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bwkvdfxq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nhwbpywi.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qyoozhcy.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3jpzlsfvx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3tdscndqm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3kvslibgz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vunetczq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3kmpaajwk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3fvbqfmmc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3knxtjjrg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3nclngota.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3tgsgbrxg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ejioarfj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3vyzknikw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3neaayser.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3zznxkmnv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3nuuwerbt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3zegaphlt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jznxcytx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3krdoinny.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3cwdpwywi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3pawhyxuh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3bpkgjesx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3nxceftsb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3iohgnkgn.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3xbtspxwo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3rvblgrqv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3xamsgduy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3kzankmhx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gbeekjxb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3idaglzis.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3twbsxwuo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3acmmuxwk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ybyqzpvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upakpmme.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3icxovehw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdainqix.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3aebsjewy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bpyjgnvo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zjsvslbm.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cbihxvji.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijvdwkzz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3wyuawfjs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tgmrlxic.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3gwcowdko.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ntkthjmx.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3gpdrndal.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lnjwzrqh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hgfoffal.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3dkylbpsb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xtfyazun.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ngbgplps.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3vfhubism.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ifnajbhs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3upuuvxlv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ceuejbue.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddwqtttz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3nfxqbmvv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pyzcsypa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jcnftfad.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3spofrrdx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3szqgcaqy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ulsvqrfv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3lxvogbbt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3guqokluy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3thihqnhn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hhpjlsrl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kmktzqws.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ofwuxdfr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3twkvmohq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3gnhpiism.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3xuqxkany.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pwcpauin.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3mrlkjyye.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3scgrwpwv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3awycargk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3iarjctnx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3skwkhwuh.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3zlntdywa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wyireexb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ytkwqbfb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3cxsnzaqe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3akhvrovi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3uklipafx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ztdoywhu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3hekkdrgp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3puooyeyz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rzibztvh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3uhtysmdj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3jnaeojjv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gyypzztb.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3uoptwwoz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3pqboenqk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3pcrahlsf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3yqmhqzos.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3twofxqsf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3xgpjkncr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3enwjfiyt.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3vaqwvkbm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3tzofqubd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3euahhkpd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3oltcurjo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3tskgjcsx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3jnaitpis.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bknyvbou.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3bllukjxh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3culfxoxs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3vmksjnbt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zwtzctwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ueilmuqx.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3rzdxbpuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qszxljlq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3fjnocjkx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3apkadflz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3mtmxslft.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ujgzzohr.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3unlupkpk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bvyjmkwq.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3lhjbddsc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3rutrpqaz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3oiedrmbp.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3umxdqmnv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3fktxchkh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3sssotzje.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3qvvlvsxv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3izfulbpf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3byvkpttm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3mzfcgiyo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3risqwsql.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3fulxgunl.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3mpvkmzyo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ihiptlbm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3qllkatgl.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3aszpnbld.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fvauqslk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xmclhgqs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vtqvqwqd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ifizjqmy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3srdeiaat.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ylspltfl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3egamyeiq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3hczqflcp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3sacvzslo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3xqqawaeg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zxmimbtz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3mqhtxmrw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ovjisfje.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3hgolfohk.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3mekoyzxs.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3hzycirtu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3xbfapoex.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3tknteytf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3whumredn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3eemdahgl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3qhvdgkeu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3fwhsrkyy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xiatoiby.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3qunlntjs.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mklfmsaw.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3zubeugnb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ddybahxr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3dmkjexrx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3fezughzp.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ymezqrhk.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3waocrvhy.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3nbdsurzd.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3cbfdzxkv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kmbqdvxd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3fuxhxpeh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3iwjwbxfv.html


<!-- 参考信息 -->