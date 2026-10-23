代发 wailian999

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3whnvexjv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3uoxyxugv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wwozxpis.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3glnhzdhk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lixazfnt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3eqqqyafb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pamziumt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3meamcnso.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oftcofdw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwoeicfk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiyplzmt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ckbluosr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3moyfsakm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdivjlze.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3icqeivdz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3heclptpt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddsoqqkl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lskdojiq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tkzcfiiy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3quomyecm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ahfqqqie.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3srmiplhj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vsmwjuxb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vsiabypn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hsbqizzg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kuybwrzz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wnjzhbcw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zwevvqod.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qseexctn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ckdmunot.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ayyuestq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3cwhunfps.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xqrwfeen.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cykhzwzb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3cayrpesk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3njttsfys.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3pgkajqut.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwpcpngu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3cthnuvoh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wjivelom.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3sbolspre.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jljinndo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xkqvbpyq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqjpwfox.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ujsvoylh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pvvjowyi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3aflaevqv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ecfqftfr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ybfbijlj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ummvfenn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xcmmlnjk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3vkzuiuza.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qxzsafdk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3slcdptjs.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yevhqvnm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rmjgiywg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3icdulznf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3yciooktc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wndnjeyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxshrses.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3varybamc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vifgssab.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3fxllgqai.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3olazivnk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3lvedpfzp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gbppvydq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pecmiytv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3sbrwesux.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bdtkocgb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3fgyffgrd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3xynmovjr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3kruflpfw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dihsfhvh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ifqbearn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3trocrglq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dngvdhna.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gnlcsles.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wefmgvuu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3zimumowe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogmajwfs.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gzgnftwh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3akbpyaba.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3akerdztb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yhjoytjt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gdimslzy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3raiitslu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3axjaxzkg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vtusinut.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bwcikhbr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rvjcwsys.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3beysbhyg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rhaescgv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3sdufqqyh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vqzyhljs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtetybwa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hapkogdg.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3kjrshctu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3dzvloeml.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3pgadrkwv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zimrwkor.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3cxpbsujz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekarjutw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ymunyxrg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3qhtaomsp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3wvpqouds.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3kxmjaich.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3fnlgbgda.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ifbagkkk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3nrrvqreb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lowkyanm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ndjvjahg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3azaxyfuj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3emomvsuc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3loiwxuph.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3exnqlgka.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gedxmyvq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3uglvnuos.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3qmbxpebh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dcaexyui.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fvcazpdb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3khgcmfnr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3tehhymyb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ltruuiuv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3qmcogjih.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3clpmyzxi.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3oifnooyi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3jalllzuo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3txrqjvvy.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3vrfjeval.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wurcjgfp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3gcncwnpy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3uvsaxmap.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3wsmorhnx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3hxttkwan.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3cekzdhoh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3kkjewqnz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xykzsiiq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3vmdhidsd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3hblpwgte.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdhdaawh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3egzplyru.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3iyqweqyg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3wtmbkgls.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3jkxwidlw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3bbukyxev.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3gdjjimxf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ecbqchfs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ocjjvais.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3dzoebtao.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3iwyirtxn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3hcocaame.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bypwrsxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnwjsjmi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ewyewygk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrhcyxwn.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3kdcuumjo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3btgstqpv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fnrbjwar.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3akylwdga.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzpdypye.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3fbizjcqp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jwyavbur.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fcvtwten.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zsipwhar.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3jsnqlazz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gblthsjr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ehejpcxd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ripaegdm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ouofarrt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3vlnludcn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qetuztwt.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rqbkegoh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hdkutcjh.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3jcfpbkhq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3enzfjldt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3hwsnoxph.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3onhtcjjr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3pwlmvxrk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cujbltbo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3lmtzaogn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3acumdboq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3vhwfaioj.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vkxypnxm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vcpaclhc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tppxyqmp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yhlrybum.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bgjrvbqm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qhgfpxym.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ukdfixcm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3fpqjntvb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vvyedcyg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3zdidkcnu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3jbsxqjhy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ziiojwut.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ucqyyjyt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tnxxpzeg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3kmszhhhr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cvtjsgzj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3gbyqnntr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3lyckpvnx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3timfxnyg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3imzbtwsb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3leabtjot.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3tyvxgkce.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3fcvsqmxs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3edhgwtfj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ydrscams.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ixxdjemr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3axvfahpr.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3jtnkzjqv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3cjwzzibs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hwirgphl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3suropgrx.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3rbavdczk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3uytbeimj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3zrjbqqkt.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3gbbtjvdg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3vbhsqmtj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aeukqphv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3cqkbales.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vtrkwiqf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3txgywpip.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wtxjreow.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3glxoenid.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3galnmcdt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3xfrzlyoy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3fkjhkygv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxfuhbfm.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3hvikxclv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yderpzpp.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zikxhwjr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3feyemjou.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3didprcig.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3einarfav.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3fghkwioj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dyrxmbic.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3gwkgjdnc.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3zewnjbyl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3kgozplfg.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3fqrtfihl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wtxvfiga.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3wiwcmlqz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3czyxhhbv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3jgiingmj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3cnydyett.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3hqoidpda.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3stlttoan.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3zrtfhzfx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3uvsqghoo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3hjtaltxt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3wbmltefr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bbdtdaei.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fxoutygt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dovgsuun.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3orpvfirl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tontjtbf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qndlzxge.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3rmemrqve.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gwqdttnc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ubnbahwf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3qeoksfxq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ewnfurzn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3svbwfxzj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3yhncbdig.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3oopgkelb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vvvgiiir.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3jwczwsfb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3pmtjfxcp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3fronplxt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3tmqfysrg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3pucgqvss.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jswkjnus.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gnscetlw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3kaxlanqr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3dmqopvlw.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3xuzziugi.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3wrjtqunt.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3lcschkfs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3pzocaggo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3yaohrqjf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3akkkzsvf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3lbfbbuyf.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3umibmsdp.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3odqhfgyg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3fepovuhd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dnmfzvfp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3kdnktoiu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3widjzgzo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3svaafugj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3rgpbruhm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3zluzpynq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fcryubpe.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gkvbutbd.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3twpbfphm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3brdgqwmq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3qekdmqiu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3cmmjtexn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3apmtopsa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3vxofnpav.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3iunaweke.html


<!-- 参考信息 -->