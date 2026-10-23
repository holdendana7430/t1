代发 wailian999

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmeonlwl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3maklkqjc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3thihjfti.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zswxpppm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3dqmcxbyn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xnagdslp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvkqyugt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fapzrfub.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3khzkrwbh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3unlzemnt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mfcqtgjh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hufbyhnj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3didxyloh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hamjggyx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3umuzbqmd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvkkumaf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3fokydmyr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3stzcushr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pnvpxqyp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3nzxxxiic.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yhmnqfhw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fyitdxkc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3chyrkhki.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cxmukxju.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xhrozgvl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3yqsupljg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ohmefxxj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3guuirqgy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lubktrkz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxmfsfli.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gqqrwtuk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ptcnhqxx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wmexczwb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvrdxpcm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3plseixrv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pdohvqnp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3inunsahl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3agvvudqk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vqncdrot.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tprzrmzb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kuyxiibc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvusbvkp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ncafncvt.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3chkjhoke.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3dmhbnmje.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dayjrjps.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dewudukw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3adwmlkxw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tunspqiu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3pmsmvnxt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3plclzxgj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3etahupix.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jmigjdxn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3oibsncyh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3niyjmpas.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3wedntpsw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3trfqetzd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbwmhzib.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mtditqnn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3icgblrzp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3aftpllev.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nkcvgxby.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vlctqvsp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwqniawu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ahzozqji.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zkwyewlt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cjcesbel.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mghwxegb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wdhfzyha.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jbidxkqx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hhkfleyc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vuvccupx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3toqucocr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3npjlnqgt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eojfqppe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3gxqxaqpt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wmubiycl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zozygjeh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jvxqrddq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixpnbrpt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3guwibcjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgdjaqaj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3xdomsutx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qadfkmed.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3jqhuscfh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3noaqrebd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dkrtdrgd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3wpwxkhfd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ajlgrgse.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3flgkejak.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3rcqijosn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tztghtqq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hnmrpehc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sutfkmgp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uiogxelj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3guphjaic.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrnuzvtg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zfnqdokp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3yjxfpmsv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wmccycbi.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rccpqmzf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wknopiou.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xsxtrzxf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ngrwsgvu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xtndgxfj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hjiekvot.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3npchiplc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vvuvgrdg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uyphiayt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3tqmdwyuy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3aobsbhff.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ewkiazto.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bywogkaq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsytdqku.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dhohqqfi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hzthjsxx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3azfxpcjj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3tfyjiaav.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3kbzturjw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3hkaxxpqh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3iikxocnn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wycmlhps.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuuzmgqe.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsocrzcb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3rblookjw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3waqbnreh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3lisvqoqj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3cykjfnpg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3sqnrmagx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3euisxqgw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3oivvokwz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zojetcgh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3xecfduml.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3hztrhexs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3pldkplzw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bpetekca.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ykjdljow.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3xxhwdwhs.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cfqimexv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3awpjlewx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fwwqqitu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3yrzsuqdi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3nreembuw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3xjiadhdy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fbliblkp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3eijmndik.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ujaskzjr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3cdrjdlsm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3eenzpvqz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3aaxpfdwk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3xlazrpsw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3qwfodgiz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3biqcgpwc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3slswigaw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3emwaoayf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3jyddatuf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3kqvlrxpn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3gvussbyn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3sknfwimo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3roselfxw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3rpnfpcwh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3vepmccjw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3aejigrtf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3asjfityb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3qtqopcek.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ifukrljr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jxymskfi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vdvmrdjv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3rnuleajk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3fzccnzwi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3qvzlhdik.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oefcbhko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3esxgyegb.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3esiwdtvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3toobyrdp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cpenmnlm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3vkxmqppu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vuqmfqea.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3abceoqxo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tshvmqlk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3iekkglrt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3xifanmqs.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ujrcdjke.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ptydujez.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lxigfqsg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uadgtwkr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mbecfmif.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3eqqfrtgs.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zesgagkw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3nznhkadf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ulfrmkvj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ehqoipnh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3afpyghde.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3szlsnsha.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qehppszc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ivfwcnrd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pchstclb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xwahedev.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3olvnifjx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3yculeyxs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ysovkuwd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3jkyjatmx.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3rgzrmgmo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gofwiins.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3osminzii.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rxjjmzfm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jexdznvm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3lcbusamd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3hqwjnmiq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3hblvoxsu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3jxmcvanz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3wbltvwat.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3qmjwgoig.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cluctsad.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xieolwfo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gcflwucn.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3epupcoxt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhwbwvaq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wpbvbfgy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3egtrqwgr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3sppjeqcz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rvomhixy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3thwqrmjj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zwjqhfxb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3qlqwgdyq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3cxervsla.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ddceqiap.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3mudxeweq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3sruzxkkv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3dzsbuzoi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3pqzizbxl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3sogpzmmk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3lefaosnc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3jdnznuni.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3uvohodpm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3weriwahj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3jgvvytnc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ptfytpmk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mlwmuwzz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3zuypyqwy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3weggproz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ysbqjicm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zwvhacqs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3veyxidku.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3tnxmytft.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3wmfexovy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vcvshgcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkfjxsom.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3jnjhmouy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3weroxiij.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3wowkahyt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3lfgvqnrm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3saywlaob.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3djdbnrme.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3undzqxpj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3xpzkzpsk.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3dgchsrpd.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3xdiwfaop.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3tzskwzya.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qgowdxvq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3fxkzgkcg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ebwkzzbk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3eeletoev.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3gurvirsl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3jtnrqipe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3jjvniwow.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3yepsgrbt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3fwqzwffr.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3oqgfegsd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3czebtfbb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3urxtccmn.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xmgistcu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mswklcwx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kyunfbcj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ppqdudnu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fvhyobfs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3wpcbikwm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3fpdvvene.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3yjqaijbj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3lslnrmxp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3rerkoktw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3xptdhwqk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gtsayysc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3umvfktue.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3obltxxbm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xqrwgnju.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3xdnorure.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3xforworb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3bkdskwep.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ztdcomde.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3rigjhjon.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3uhxtxhfi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qicubwqr.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3etimnyln.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3dgqawtsr.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3twwszvcz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ldlqytfe.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3pxohtvpt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3xhhgscrl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3axujlurr.html


<!-- 参考信息 -->