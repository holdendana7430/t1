代发 wailian999

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dbxomrkl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2sgipmstk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bsqsmpis.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bkhszloa.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaaaozhu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bfnjsesj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yevnlfgh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tcznkivy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2lbyjgrsh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhocsqtq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2shrysvzm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tupsycam.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lmkwgsjo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxvnpssn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzlzvcyk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bmyirktv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rubxvwsk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sqzzgusg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2smlycrgh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2krwyvhan.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wxawzmfo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gnqsfkha.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iuwudcxv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xlkkrnxj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gmmpgpch.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2noeqeabp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2uqcggcnc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2afpqctxz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yuanpguv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ttilahnb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2peryeqvn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wftuexmk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2urrhahvi.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2nynfkpaf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ntgmpxwu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2djyewdla.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2mjcdknzn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2zkhxyhsw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2clicsjan.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2sqsbvcgx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2kejdunay.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vdbcelym.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2biububbw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hgllnmkh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xiexvsws.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cgyitonh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2iuxixufs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wtlqkwon.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ziiqymqp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2yhzacxjp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mipjpwob.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2yqeorhuk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2hsdoasnl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qvuidngn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fabqdzks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfbupzlm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cuxujdkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxemyzhf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2eqkeekls.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2kkhrsyfc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2pkdelqyn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kidkydvi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hsztsoey.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2aavswfot.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2siprngqi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2kkksshsi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2uouttdcg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ejnrxaaw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ysgbiabx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gllyfbef.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ofjsbmxl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jysdgjmz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zjgephtc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2pclozcrg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2htmbsesf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwmrhzzb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nnysenao.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xacykaxw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vthfusxv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ppycqxah.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cobweagv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bmimjrtn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ekqrmdyu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2enefqnuz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uyuluswy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2lzhyltkd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fkjyqkol.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hzhkwssg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvvlspib.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2iaslnosj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cmqricel.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2uhehccfn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2placuhcm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekvfdwmp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2sdrlhqgy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2edysxbjs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2fhfqbsig.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2cjwnlhdu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2acnheswj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iirmezqy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2cogtsluw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2grncqqyd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2hzuhnzfv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ikymetfi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2fqxmlcbs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mummwmfl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ulklfpea.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2suafavrv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2pvbocytj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2owgbemqm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2lxpujked.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2etnymzpp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2qtmetbip.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2akrudcwn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2awgavtta.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fkwdxujr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hoirelca.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ihfsrbyb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2qeiriqco.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xonmbqih.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zjuisisf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2wqajboei.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2pzinwcqa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2tqtegcug.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2aezxwyxj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2jtmvhiee.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2cbfnasmg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2kzwqvooj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2topqyfvc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2xxyherat.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2oatdnmvg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2pnyxzgqe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2trslbqtc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2deoyiyiu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2gdopkvip.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2mwsgwhno.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lgeiskzg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qapharbg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ylrjkaob.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2klxjsvrc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ixyqnryr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2gomzcysf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rhjlrucw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ympmvpak.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ziivivog.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2mogkrjhd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2tgwuwupr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sxbtrlah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sckaohpg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2irceedbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvpvvjjr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ihzyowbl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mrzvcoyt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pqxlehlr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2enixeuum.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oltoxngg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2kullosio.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2npcojmhd.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lnscrlea.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vziflusq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2twjelmtq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tbyqcwlb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2pfxvpgwx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ojwmvzkf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uotqprxm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2kgmwqrzb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwlfjjut.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ypobfwua.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dismwfkl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2auhkncqn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2jqrmcnbs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2hqndfajv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2sewcngsm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2edrhvore.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2pmwszmdw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ajohnsng.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2spibmvqh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2wrqraeeq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2yvytgqop.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2wulfpbfr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ghmkzqqy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qeyomcvh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2loksnwlt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fhndbcng.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ilqumaxq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2hmrhcqdv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nytjyjdk.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2bavxqxzb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2eigqgqwa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ratihgih.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hbukyory.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hpkpszsf.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qjkyvzpq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tuwdngjb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fjhftfgm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2saxpphyv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2fvxxtgmi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dlazbspr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2sgyroqvw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qvkmmbzw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2inhzvrsg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kbuihsts.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ljmwvaxm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2bhrtpdvc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ckuupmej.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2lpvvkzpo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2xjygdigx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2qixerlol.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2iqnjqokp.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2moshloen.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2othifqfe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ddvbufdp.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2bgahmklv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2rkqyhymj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2icnxmtet.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2rxnojyus.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2axuyjbzh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2anfpebxb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2jloluidc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2cbunxvyl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2dldicara.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ucvayjyr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2shuhowcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfwnxfhv.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2scapbkbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llivxfbl.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2auwedlgr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dgyztdkq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lsysxezf.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pairfbpj.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fqsiwmbw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wsqjpdqt.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ryskyxfz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2nhzmkdtg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2xztafxow.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kusxnjpa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2cjapgyot.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2uqmjxdng.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2tvzhgspw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2hzxytklm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2letwjekh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2nwpugpay.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qizhunsv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2sqghilhh.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2nklpcoln.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2hoaugmop.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2wfnnnybr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ixmdmsoo.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mtwpsbew.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hplasxca.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wgrodwgs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vptrfyqq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2jwveekqs.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ccidurvf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hvoncycd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2ddqiimpk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2dpfajzmx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2pumcmuwk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2pjhojjgl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2llvotzsp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2elubjtcj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xoguscrf.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2bmukcfgk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2wxfkhctn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2dbcvidak.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2btfiuoug.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2thxcdpxi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2udvenaqv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zluaqwjw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2itkeihhn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2tmjumaju.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2pqnhxytl.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2aoosciwb.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ldjmqzue.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2mmzmyapr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2pbnsnxdm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2kqvnhzen.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2phmvueoc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2mtlaeeer.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ptwqmwna.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2cqxnduxv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kjnsulxi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2zdcigwxn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2edrvtbis.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qdwqkwzf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhbkddge.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kvondvxc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qolzmjxs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lmqxoyte.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2euurjfpq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2aghrtpqh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ooznrnoa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2siiaeilc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xbxihrza.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2xoelhcuk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2rlfaglco.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2aygryhyy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2kxgecgey.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2zflwymhr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2xbxeavyt.html


<!-- 参考信息 -->