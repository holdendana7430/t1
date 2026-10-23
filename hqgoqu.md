代发 wailian999

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vsoqkkhp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3iyhbupwq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zhflfxyi.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yyovhezy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zhmspapm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jdzpejdw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3feoppizq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncrcjkup.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyrpcmvp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khiuzwms.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tsiuwyrl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dlhyjjah.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3dviiuhjk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3gpmuozes.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3uwplofap.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ysxnbeqn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ujxqlwjn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxllsfva.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uoozttob.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3poydavyx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tpupwqql.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vpuzaqmh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kfddxjnb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3igbewazu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mapgqlka.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lziedybw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kpdhpkdq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3byimvkko.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lczlojsa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qjafqcsr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3iimjbohn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3gnrgcnmf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xkozjosw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wbdlgpuo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zgqxryqo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pexvwkjn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3yybfvrwb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3fbjuryzs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vsvcsqrl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3guvvxujy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dizcslqb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vqdajywr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uafvzmmm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3aklbsjjm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3eszqigbf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3egootyvm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zndzwczz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tvrmtdyt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3udiizvkx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tvkrhufo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3sybkrucl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ntftmiqx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3cfbywsat.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qdimpymw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hiiwarbh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3yvremaly.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3exbaljyu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xyaylfdo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3toyfsgvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrddeozc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ivaahcuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmlcebfz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3yxhmbkfa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jkpwrrfd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ksyftrep.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnkgioss.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvrcizbg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gicdlghu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3xtyglcnv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3phlldmdu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ebwywqdo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3yqonakne.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3djvpiaef.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ounnaaym.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwsromcx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbdpmafo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojuxvxgy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ltpsfvmm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3icawrcex.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lwngyxli.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nadrigeh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3pnlzgnew.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xwpjyzrj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3miygxqmj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gdqvzqco.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tdkwhqrt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rtmgegvr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jcfjemdd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fjhqaqxr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mffrdmip.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3zwfzpjmz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yqhjfpch.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qewqabku.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnogycej.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bawmdyhj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3rpcfxbhj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vdlzqhow.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkiswkge.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3pzembqth.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3osnyzktn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3pkkqcjca.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qimwitpo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tmvufeek.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjfqjsmn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pwofzamc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ndkpxkbd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmfqgwnx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3raoxaexp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3iwdrkrkh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ketzjdmy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ekdgnqfz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yyvuwesn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3jalxbwli.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3mzcsaoav.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3cruvbwnj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3burbxpnb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bappmnun.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3hqluxain.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tlkkrvak.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dtziyxck.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pvedfjgj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3qbqshmon.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ghditpuk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3lyounlhm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rrqqcleo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3sxqvtkum.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3megscsyc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3osajiosq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3pupcxway.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xjkjvvll.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3fpvnkwis.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3vjijjaxd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3lsfpcplg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3tcqdkfwj.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3asjbmklu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3qxjqozdw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pnapybru.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3pwlysqcd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3iiuhppue.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kudrdkdx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3zmzpebmb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3rpxxdpnr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3guzhmajw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3fentvgfk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3jkpvnbvm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3nzbeoahf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3loxpekqk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mmuzised.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ebdgltyz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3sntxabfu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ykgomlgu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yalmhmqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3batozuiy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3plclthtk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ryupiffx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3qgawcwkc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ibhgibzn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lftwejdz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vppesmwd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajjawyjw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3fbcxynes.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hizkljll.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pmlpejex.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zitdqvpb.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ohupbvrg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gqqatbgr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3cegjtojm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3dsnsquhi.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hidnffje.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ddokxbny.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbdzvysv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gdwseqbu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aovdlwhm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3edosaxzl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3vwbraczl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ybemykmo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ifcdtvvt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xxqpipby.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3rqkfusju.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ggwuttgd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dzndcwuv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3jdqabaex.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vlwuqcuj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3xtazfhwn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bnaycvdy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3fuywkeae.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ycmyqsib.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3mlbqsqpk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3bnqdbbap.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3fbihnplf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3annlmahv.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3mdeqlwxv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3trddgcnj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gvdgzqrp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3oanfnlgb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rqmldblp.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3zzllyfuq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hjgyhjks.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3cioqeytu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3oycdvknr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3jcswspck.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bcbljyyn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3zofhotxe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tpvnioun.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3qynusxxb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kzvyjgun.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3hgkmhamh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3algeagme.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rogficey.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3isystbbw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3wysconvl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3kihestlz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ymkeirrl.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3qrscajpp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3wiwusume.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3juhhqwzn.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3hsfshgrn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3iqvxjqwh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3bthkswbt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3egitpkqc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3swgawavb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3wcwxhqez.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vtrctqlz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3rpdduulc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3fxdzlbub.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3lsijaevg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3pdgizlvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fejmhygj.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3jfxqutof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntvbgpqg.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3fygugcox.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ikpdedqs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3awgxusym.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ophekdln.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3luiolcsv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ihwmjwjy.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3xnbbtesu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3cjkvgxot.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3dohjjxgc.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ohhxjbox.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ytywnelm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3fpobrxxd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3zusqbdmj.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3yxnyxudr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3rrakjqik.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3ofdqazrx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zrowwwba.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3cwvwfykd.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3nzrruspe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3vxmvhwls.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ryrofvju.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3usrnqdvw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3morqlazn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3asmideia.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lsxianxz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rxqvmyxk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3mtdukrmf.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3kzsgrjii.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3hineajic.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3vrtgtezg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3gxgqkamo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3nlfymyng.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tomwvdli.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3irfjdzpb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qegraukg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ysnpuycq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3vpzfjskn.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3bocnpnja.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3ufcekqan.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3deeqlvzo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3goqbuxud.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3zsgtnpcv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lmseqdtj.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3rttjevyn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3vzviuegq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3urnnxezd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3pwuosfxc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3uvpobkft.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3jcubxcjn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3ynagqpgu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ydigftpo.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3wwcklhhg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3cxajjitx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3kvmspipe.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3pjtybima.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3musxnsoz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3xxgucnda.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3kxhianmb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3volsfryt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmecisu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3bxnhtaab.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zwiddcwa.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3sciqrynb.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3fnodtusq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3kfpddovs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3azfdqoca.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3towyvqds.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3nbtykwzw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3bhapfrdy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3njlpmkjx.html


<!-- 参考信息 -->