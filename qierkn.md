代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rowyvnhl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3syxgaugg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3olajnuss.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rmtmxavr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kamwyeai.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jzevbuvo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xehysewl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgtmpnin.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vidfhyjt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3aqtmiszc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3osgdugxp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3eeacwlgb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fgvkxjgp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3diubgibi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3blfhmocn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kzxvhzyn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3furnvpqc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3xqeytooq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3miuzkxxp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfxbsjfx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3egckhlvg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ahflfnfz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmtnqbmo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3raklwexb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ecaqxgvc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qftybenh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iljltiun.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uxmaqufb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xplssdbe.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kdptgsji.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3krguxfyw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfnhbklj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xwozsear.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tgexlmxu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lbzyiyzy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3cohwilwb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hdoyauax.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3azfxcjam.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vxhbzmlo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tnrtqbwa.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bdouxibd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3yivflyeu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bckthbga.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qclbymhz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3mrezkzgq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3edniintq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mbucsnuz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3jyozjsmf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ejgjhcek.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxutgxmh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vkdufafp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rtaxasoe.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bxxfqurd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pjkmlenn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hnuolqll.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3oucdnxiy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3dgacxfsi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3piybpwzj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3pthmtcbg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3vbtopzhm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3womgkqjn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fxbhfkvx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xzpbdcoq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3uvjrgzkc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zinbdnkw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uczqofkr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hadjbqxk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ebucdgrn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3phgywcwm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wsniaupd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xzmfklmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxepfkhn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nufjkxwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzftwroh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ossxaqer.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3swkcerii.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbtmazmk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jhluzexx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cosglsld.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ijvggnch.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3inegsvud.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qsitefha.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3dmxnvrdj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3krqxkdqm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3tpdcuusn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccapuphl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tofxojpl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibgxtwyg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvtxmkbt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wbuzszas.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ghzvtjoy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjbzzrhz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nknndeji.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3aesectdb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gisbhnxj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dquueyhe.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mazrgzrx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vdltzslq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3wbtmydlr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3dxafvjso.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3skwbywsb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3bmapgwnq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3oudgbinr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqlpdtzo.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcwcrqwt.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3trpsopnx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3snriuyww.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jrigdbkr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3jhyuguqw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3wpyrnrwe.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3gcgmfkzs.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3pqlavkgp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3zrvmzadd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3guprvyei.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwxlmgub.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cemwdqbx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3dsebetih.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3qkyzjqme.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3udkqrwll.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3xdzeucdv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3rydfruzq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bkydtsyl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zswxsedz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dgydsnje.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3kjbkkpqq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3cyrvidpb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3keqyzmyn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3alwquuwm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qpvaqcjq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xuunpqbj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xbitiglh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qnfmoncs.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rjwlybbp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3fqhtibgr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3gpwbjqlf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3klqgzwhn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mipolway.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3kmfmccjw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ssvdppvf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ncwcdgve.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3vdiengnf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3zpagujnk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3vkqqbusf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3obxxeakd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3wqokmapn.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3cotsveuq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3opjoblbx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3gjstijdd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ndbbutzy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3mrxybfam.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3uojgpkbh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyjkkptl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rycpwokh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zfmpprkh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3hqnqeiwy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3hzzyvtkc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3qrzdulpy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3sfomlfgr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gtqwnzsq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nkkvlwvf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3tvosbsbv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ogvwsuoq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3nmviaftd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rncmgjal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fltvigft.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3yznguxkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lykljpmb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rzratmaq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ceqqltvz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3avhvsuqj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rssfozae.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcxhwchs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3xasixuic.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3sxqbxrgu.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pnaqvkwo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hmtjedfg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qihbyrfe.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3awvhblhv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bkjiwxqt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3spcbgatq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ncatijzy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3wgrescls.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3pbxqvxsd.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3usgchcfr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fzqcgytz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ifggrynv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3sjvrrpaw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3wvyilvxd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ouuqffby.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gzezyqzf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mqhukavh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3rhtzbvla.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wplsmhwg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3kisixwyt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fkpzngvy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zzwtfjcg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3dpqizsbb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fjstlyvz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vdeczxip.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3usfjfcrc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bdrxonrz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3pxhjupfy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3olmouavs.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xiynwsdv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3eemdtqdq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3utpmgyay.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3swdskwbs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wsywmhiz.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wioyawza.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3wzkikhfw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fabbvjaq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3wecbbblf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3vpxcuyoa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qheyrpan.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3knybtbqm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3tepzdlvp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3tkckruxm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3mdsnamim.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3rxtrxrvm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3xgkdjlon.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gihxjwul.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3lwvlnnhj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3achfoldc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3kcsxalsg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ycebbmfa.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3baqlhogg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3jeogxsgf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ishusrar.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3owvgeqtm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3cwfyxzka.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tdyowdjj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3npmmogkz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3wmqmktte.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hbchicdv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3glvolqxk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ihwznehc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3pnliocdp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3bcajraje.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zqfloycr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mljjjxet.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3pzlgnffg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjzpsugr.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3rcszhddj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3mzhwersn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3cxakjstl.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3fnihbelj.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wkvhsxfr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3hxtdypvk.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3raydsaas.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ktzxsihv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3gzdbhsje.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3uqneyqmp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3hdtdofks.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3lxsdjgni.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3kgkfmqmq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3oczsiviw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3gmrxxwka.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3lflplfjs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3btksduya.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3depyuypk.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3dhzuahoq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3eiaanceg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3haohzdbi.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gfgtscxg.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vwuzzyoz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wbpxoxys.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ymqhujbq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kndepibz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3vefvwpaa.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3xbrxqmvl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ucnplnya.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ltbraeyy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzepvjh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3vtghimzg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3oiwazwwh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3esgqvzpn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3qykrqhit.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3akevxdbt.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3gtfosfpx.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ntldnhie.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3foesejvn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3lzlhlmwo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ifllwgkl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3cvxwlesb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3lrpimaek.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3mevibpmh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3aiaibjml.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3lseciulj.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3foskjebi.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3hgwytmuj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3xxhbpzne.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xtcgtfao.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3idocjnnu.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3gappkxfp.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3mncqocbw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3scrpesbd.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ebbcusfp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ryapkhnu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3jjezikiv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3leltwiqo.html


<!-- 参考信息 -->