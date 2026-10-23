代发 wailian999

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vcnngpui.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ztrwlpum.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ssijiiik.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3aiipzelv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwjixxyu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gncbuvit.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyymulhz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kbkvfmiq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3cgswmryi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xltpqxit.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eeqeanti.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3psgjwqfq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccpntasp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uxdttvsj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3imszuwfi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ojkfywsr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nzwcubmo.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qdtvrarj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gmbcvpfz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ysdlglaj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3jmffofxk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qszoivif.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ymecciou.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xtgsvhiy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3heylwojv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bmxuwugc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yfxrxlcr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3nhshwgfa.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3mnanrxkv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3oykphosb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zzohxfqp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vsafztwc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mrjukhfi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwkhseqp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3pxpnzqox.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kmtipbpl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ovacxqav.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jfziqmnl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qblumwdg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mlnatshq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ggulosky.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qycefiie.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3nqoiafee.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3kerrtqaa.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3jwpjupgc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3idmnqbxg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3izvmgfbt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3mpndpvef.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3grnsaosh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hnpvstil.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pqorwwya.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3lqruuuzg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vonguqge.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3pjgjbmmu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hjlqwbdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npttkkzy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3pcbhgehg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrkkhcea.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ojeublmp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qqkpdojp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmxkaflu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tqnghewv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qqagpiwn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecqwgeul.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ztwnemng.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3eqhpugmh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3eugwfmkv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3vxiywbtt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xlbukzft.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogfkyqtj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3luzfyghg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwyfcbtz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xtfayowo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3zcjkwdxa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3plysoihi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wrjowqlu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3oyecfrex.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3iwrfajda.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ccxijpku.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jcxkrfds.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ifdqjxyp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tsvxnzvo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rfcogjda.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vnqqseqa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gvgsktvo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ndelbexw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3meeqftlw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rokluxsr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3waqdxtqg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zzzosxgn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3splluyho.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jzdpzmnp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3zbqonywm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcfiaaet.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ecttplbw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dvboumfk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3qkutnvvw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzwiwkyv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vigbdxup.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyyboaxt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3oqfixupt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3cpaatfsy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwufsxhy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3plfhzntg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3bzbaodwm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3iwruxdht.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3glzijdbd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iyeeiano.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3fvouyamu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ynbuzgth.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3lbeafqvg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3apchlmsi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3oepgcrhq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ksozgbic.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3plwdsxrj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jsnqyqbz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bnnslrrd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3doozmcsi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3kekevkzf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3oatdozub.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yubhhxvb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3hpubpvyb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3obfvzxsa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3rflzxqwr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3zwcwwxys.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wjoxqegf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3uwsvldxa.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3wbxynswa.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3hzzufgxf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3diyygaxw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3quisfnnd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3wleyqdwl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3otczwnfi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3cmqmirus.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3rqvtnquz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3rhpwnuzb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qtaxcyks.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3rglokcoy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3txhvjnlt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qfkewzob.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3bngvruye.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3oillhwce.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wabwgbtj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3tkpxlnxw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3lbjlqwot.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3pkjwxqcn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ibzmvvij.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dakizxfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvhmulmu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ijqzlnkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nggvtjlf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3fsrmayih.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wnegocfv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3edjjxivo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3lnanrjjc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qetoqaoi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ccuhzsih.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3hmkfrcfh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3myzwevbi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fpkyysmi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3owhtwgfr.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3aygqhhqh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3hoerybeu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3uysajeow.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nfxlfmmi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fdgzliru.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3pyvlosyd.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3vfgznjia.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kudrdzhy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3bsnssicv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3biiuxxoo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3iqyysajp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3nrbfvrly.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zilyuoax.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3zbbfaaay.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3lhdestvt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3eugayhaj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3tyeetvyq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3svibhzzm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3sxcftvat.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lodmmkts.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kanypisd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vvnfuhgv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gowacgzy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fnvdkiaj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hdwvgjmf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3thcftqwy.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rinqxjnx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zilegylx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hikyfzmm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fyubfrtk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nixvmtob.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3ottjobjv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3umbfinhj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rydiukoq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3oyxxkuel.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3btdcgsyo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dsxtedkd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3wjjtencz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3iljysvlr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3tgpkokmg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jpaluhlq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3nuijhljl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3omasfryl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dxmlvojl.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3fdxrdbta.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ncyjzhzb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xmcualsg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3smrrqufd.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3qmjpbqmf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3dgclgjxf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3bhykwdau.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3inehopyi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3evevjsko.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ivhesbau.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3fwwlacdn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3jxmieoep.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3azlufuwv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3acctlcic.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3orsvykgb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3zpbnmttk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3temocmcn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3poqpysio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgaizjay.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3kpyvdvwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydnehyds.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3qqoyjtjg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3xybgsnqs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3qdzldjpl.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ycqfpvfa.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3byscrqkl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3atxrpxqy.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3nxcamzdg.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3etfnfizc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3qcqaqjml.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lsskdegc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3pgerajgx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3pwsbqgxd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3csomycod.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3wsnuaxao.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3igxgmogh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3mecgevrl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3msalxuvq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3xijzibue.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3wlowxzru.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3eoahqpnh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3lleevami.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lljprmlq.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dsdkaxqa.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xzgbbxwz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ipigrdat.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kdwpmeqy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3zdpffxkc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3nogcuyyu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lwuxykhi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3pbdmzszb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ezakiiim.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3qehdyczm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qqzaysnc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3rjxiqkjd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ipvrhdmn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ozlpaegd.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3jybygfix.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ndlfkjkt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3xspwfhqb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jzxffmdv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ezcwdmvs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3llxycjrt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vsukvyfg.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3kqczjzqf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3iwwfvsnh.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3lnrqowcc.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cwiwvkre.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3graaipfa.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ynlpfsdd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3atfsagnn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mczhenoi.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3pufbrhqc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ptcwuawi.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3dlggfult.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ysoxebeo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ukqdboai.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3jaxcwiuw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3kqpoilkd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3oqvnwuch.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3vbztwinm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3nheqkwkn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tshdjvdb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tzlresou.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3bhwzbzsh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ynyomtbp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3xzvuryqg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3vnhfgzfb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3agmcveep.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3kjhktvjv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3pnrcmvne.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3jcxokhpz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3kyajprfp.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3yqxlfybo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3whlrzvkk.html


<!-- 参考信息 -->