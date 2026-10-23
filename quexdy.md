代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3cayofscq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nkcrpeig.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3alaopokx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bnyexlvz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pkeoletn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3dijdfjgo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3sgyzitwy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rcmluprq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3givcbjli.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3kllqlqpw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wrutklxf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgadaeio.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkfwckln.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbkeuigd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3deyfjehi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qdsdugun.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ceekpofc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ersbrlza.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3raqxgsmm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3iuzvjzdu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jihuiyqb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3chubxmiq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3egwsncww.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzxrtxov.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bjtvfyst.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbbiyyxo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3srqwxmnt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3dcteosdp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3gqloyzfh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ulyqazjy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cliqwplu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fhdjudju.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jfpucmpe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fkindwkv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3yfewtqoh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3sqvisgjd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fcqduhly.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3fykidumb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rqxddqqh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vukefxib.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3aisepkls.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zwyykdnc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3uyrmartq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3aoeqxbpr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3botnnpkk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dokpjiad.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zmbqauet.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3dzaojgnu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fjnuivhm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kswmlody.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bncbnora.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3iflvyxsd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3omeqerkh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3glersfvb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3mouottvj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3rasqnsez.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3oxhzmhuy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cvwacapf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3arhijzud.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dxsgufrx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3fqxatiqn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3noxyfhyu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3udioytyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uiakllhm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ixphscok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjrpwwtr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3hwrwpewu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnjzuxq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vtzgfamt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3udgpybrb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wacbzrdz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3simgagee.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3uhgsqrwl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3azoadnor.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcgzkfll.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3kfyxkhvr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3pwtohfik.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3scjajcbt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oiyfhmtr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bxrofqea.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3spxyxpob.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3yzgdhprz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vybcjbzk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3arzaqcik.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tvvmzkst.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tnotdzhx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xirneetk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jokgvkxq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3scvrovks.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xgrabtsd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3euvgyfsn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qxjwvthm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vmeqcnoz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3sihodhvc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3avqwitip.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lkgtrmuw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffanxzgg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vwkzdnub.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwzljyjm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3viqrkeln.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3gdtjentz.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3vnzkmgjf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3tszoihwd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3scrxyqlt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3skeshrne.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rubnjdqj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3blfckekv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qalwbojs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qdiodonr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3nzrmgwka.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rgqrmclg.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3wwpwujgp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ttmyqkcm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3oxamgrqb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uhyaompb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ssfkgubz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3hbcewunv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3qbfyggec.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3eschpist.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3sduyizdn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3tliwvmvi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3jisvnaix.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nsrvrafl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3caxlrsvw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gizzoxmz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3uyrqbsjp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3dmxasfuu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3hlmpbfeu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cabjzifo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3mhpazgub.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3tuyaufbp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3gzkppeop.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3qqwprfqp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3flrydrpw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3zawmbwjj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3lsjusjxv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3biaanijo.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3mxfkeclh.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3cpnwgrub.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3npuubnkg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3oecpvgxh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3qrblracs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3rfrrbltm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3exacxtql.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3svmblvzk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3bgokedai.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3baufeeai.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3yqiopdap.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3pjvcppbe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3pbcvfkwg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3foelsqjd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vczobscg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ccjaobhh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3unustwci.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3hqqgkbcy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ldlyzlmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edkoeats.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jilsnuuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxqaygci.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nkuzmley.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zgaxoukk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3igeqbnal.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfnbkour.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3lrdscdxk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3gpawkuih.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3xpqraeyh.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3afwcrthm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lmczcpdp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jecucxij.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fabihesm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3bbjwsokp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3zskoaepx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3frohlbgy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xehuekwo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3likhxsyf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3awsbihhk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jsriitlz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ywvlvxwv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3slyiicsm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3tgydgtml.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3cymafwsm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3osbrptum.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lmdmyute.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3xrqwcwal.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3xsikfpao.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3pvbfknqy.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3marfkbjn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cczboqjk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zcsptcpu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cdkfwzwx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3domaiyeq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tnjnbzdt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3weirvhvw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ciprexfk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3soxryeep.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3bvuovtfl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3qqaphrim.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uowdyudq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dmbmglme.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jgaecsiz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3spistmqo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3rmtvxaan.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfengzw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3fqrlglbt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3qpqqzenm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3nvgxrdds.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3owccxzza.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3lwtnogio.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3huozrxxb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3lohfjlkv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3yczivbtr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3bidnxzcs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dlllxfhz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3zznqdndv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3fswceyaj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3pwflnkud.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3hfzhhkif.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3qmlywtnl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3qeihudqn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3tzfyeqaf.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3qxcawwop.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3sfymdexp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pncvchwa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3qhuxgxkj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ddlgxekx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3mmdygyct.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3fbcxnrcu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vqoykcdi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3wwkisiyy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3hdteuxas.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ktruacvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imderswb.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3innplkns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxpbcftl.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3jgblvfms.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3srbxmwvw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3zmfcaxvo.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3yhxfteyv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wgvmkllo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3izzqwitd.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3uadaresi.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3jgwlhpqg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3bvcsmgce.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qdzikekx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3tzvsnrwo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ihvfqgrx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3lsddctwp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3lnhvlvzv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3xjuojtpo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3fqxerhpe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ydevgrwb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3vlsbmhle.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3jnwxgawq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ophnwtwd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3idiskiqt.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qvawfqbp.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3coakvtkl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3sctzdmdj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zohkssfc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xhuhwpxg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3clyhgdwy.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3pmwjrhjf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mmqoaobb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3zusgcfeu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ymlijnhq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3kyjzimxt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gggwoddg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oxiyutnt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3lyofhhah.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ysvufgwi.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3aohgmptc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3rmjmziwn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3rdajcxlc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3sflecipa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3fpfqotnr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3pkqxxmdd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3pacynbos.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3rgekkiaz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3alutopoo.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3dhafpvqz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3sbhxmwcl.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3hxwcfcdf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3khvpxjmx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3psavhfay.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rszezumk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3rhnljvlh.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3muynzuly.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3rmgnlpkp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ohilhfut.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jhflgdao.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3cdmulomd.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ymgnpwke.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3xrqjluou.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqbdjhtg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzkiklbl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3buakpfep.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gzkpvand.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3rwjzdasv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3dppdisok.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3cwnsfxol.html


<!-- 参考信息 -->