代发 wailian999

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vnbxzxeo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2zxusoxoz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wpcqfyhr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2osxlygwo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2byfhaozl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2yaedjdge.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bhwevyrh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vardqvch.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vpbcredc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltpfcwhr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hyygnujb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yfblkuom.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2heipgawm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfkssffz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vdipiagk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2aqgyrflw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qlmifirk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqdbpvyq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywzahgvc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tdnwbvxs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gygakhfu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2avmxdocw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tvmhdoaw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ueovlzvi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2unuadmjv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qqoryuce.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vylufpdp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vsyhwfvu.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xgqybbsw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2yascatiz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2manphmxp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mfwjmgeh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2aqjeymmh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kbauzjbx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ufsgmxyg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2laqsydci.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tfqbnwmm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsuncytv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kfsrxsqm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2gpigpklt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2cpfsrfnb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jtmfbseb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vitefmxu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfeltxfe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2oeoqiniu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qgtbpbjr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2risbkvby.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2krorwcpc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2lavtlnpe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2idetildg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2lqwiclqn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wcyqgsdg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2hzmaqeso.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bhjloucg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aqqoqmcp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2gxvphjws.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2noiygtnt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2vozhkfkg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ojqurehu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eddcprar.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2tdokiilj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsyhnefu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2mzhjhczw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xnqrlevd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxsohzpu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ruhzziam.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jrwuoiim.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2elsodejm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ljdpqjhc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ztnbvhpd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2becymxyf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ppiwkpph.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ctiwawju.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipzobisw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ymcqeyqx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aixxahmh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yozrqijl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2qkhhdkaq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lciazhpp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2issweele.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2miyvazpo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2xftvntgd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xxqidugk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jhatsjph.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2krithuhz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ijtsghlb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2kggrsvbf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2svlbqjud.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2abyteoyx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2jqchlcmj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2vqloswjm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2locfvdnr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cilgjjml.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwrcnuwh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbxwiuzi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2gnjjvkxt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2llnmpntj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnbtgnxg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cnybuvfg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2adkwggql.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2umfivjgc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oguhbjik.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xacudhyq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2optnailq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2udavqcqx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dtholnbk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzfkxpdu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2cxmhxgyv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2vbevltbt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cblongks.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nhucwljd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dffvkzvg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2dvzqqxmi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ovgtpfto.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2esdxabyy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2edpavjbs.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2wxavyuvl.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2dmreyqwc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2puypjbah.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jyqogkjo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yfgidnds.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2znutbluu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2jtnifyzg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2nmvvyftj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sulwmqkw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2qhalfagx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2lvrkbljs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2trhumghc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2foklgzbl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hagtesuq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2deyerkzk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2geigqyht.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qeyjjdpq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2cickjjdy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2wamedlqz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2dyuywjzm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xhscihsx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2emvpfngr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ygmqgaid.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2klmhefvm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pfpphvfj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ujamatxb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qnqbuufa.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2iallaykq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2gbazihsw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2pvmdvlyf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fvavbabt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2oaosxbpn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2layvcwhf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2qyxjjnee.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2tgnrmrxo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bhukxnjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtmmajtd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2djpqrctb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onknowcs.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vtngavrk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xttzoyjh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bmbfngjw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qscyoviv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lsaxuzlb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2gjlfstyk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yplzxnsw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xfklygeg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ajqmmyxr.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bukyhjkc.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rhspjeco.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hrfkwguy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2mhzsvfjr.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2cmomohmr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjmmqzpg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2aoslshdb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ovkvhnbq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gbeqzllc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ywhvqpoj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2kfzcfldr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2obxrqwai.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qjcdvhns.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wxasgndk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2kazzyvbf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2gvjmkejb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ytsoguaq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2xaaseejs.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xyfgmrhv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zmhfypcx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rmvoazqt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ncfgcwku.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2kiubvrlr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2udscchfh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2zkpzdbjx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ervzkwvy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2hayrakfi.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2xsrjhbpj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2sjpwnttn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dhorrzoj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2nmkddfgv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tlvqvcpg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2hcjdcbek.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwoewmhs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vdipdzir.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2lynqwthf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2gjcxkjqs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2lzuudkyi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2rivjhtip.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wmdmeafa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2kxvgogla.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2emqxlhtq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2sryhiegx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2cgbgphwx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wpdeqpsb.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2gzerossd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2heqmaxpl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vwlhkjdp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2dvrdzpyj.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2vvptqhfy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2letjdxwl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2xtndoqpk.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2qaurjwxk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2lcxhubzg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2fejzjuqt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2hulhwiob.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vcvogitm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mzbkyfpn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wwswzdib.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2iebmvohe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2mskddznb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2drdtjhmi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2spmjpgmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fywpdxon.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ydgsqjwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqpqmqxe.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2odzuplay.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2rlyhwpiu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ixzzmrsc.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hvtzxrfk.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xfnszsjo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2xidbqtof.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2iveueqey.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2qouwnath.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2xyowtmwd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wfgabxuf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2oaukryek.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2tatlruiq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2dwovjgca.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2efmqleip.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2ccjuqgrh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2lwhvicmn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zuaqsgig.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2cdjnkpew.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2vixakztt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2fxrfrbfn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2curwnxqq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vxlakpna.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hhuezkej.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bixolpaf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kbozzuyr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jcyreabe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhmbuop.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2xgjywxdi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tyjohxvp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2qjnlcgjg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yrmiwldo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2txssvsxa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2grbhrrct.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gfsthioy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gvyiuroa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2qdgxppjy.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2kmafittk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2onhquuxu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2gmaewzqy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zsjtbvcr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jgukzteu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2mbkvvldb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gbqbwufw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2auotmrif.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2awbquiwe.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2tbvrfutj.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2estazzwz.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2bnhnxlog.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2belwqcoc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2mjqjppkg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2jnmkipdm.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2gmzchrnv.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2bznqseje.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2pirxdrjq.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2dozznbmr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zwavoovx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2weemqckz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vjnsgivw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2skomyhzz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2acapujvr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbtvxcbq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2agtqnojx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nhjagyaf.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2jmebucbi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2xzdytirc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2wrvrvmme.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2esdoerxd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2jlbclofk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2wjaromgv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2mcqzcnbn.html


<!-- 参考信息 -->