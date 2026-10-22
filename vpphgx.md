代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rrggliun.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vpvygjfi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yzydsznr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xhxshjbb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wdjrvsod.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jugxwejt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bkbeppsm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xqtfejao.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ytorwxad.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ccpbecix.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2fodonltr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xolczgdd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcrlidit.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qtbvdmvc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2blnathos.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qpvkwkzr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2thdrcsjv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ylsraqnh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wdfdkevb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mepzxdax.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nlqeguez.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gvjnivqk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2srkysbtw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dywjnoft.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rfbcidif.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fofvgonr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jfsghfpr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vbbfeara.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wzkjpmci.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mgjbxarj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bphxvukx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bwodizex.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cciuxjsm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2psyrgwxj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2fltmtztw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2dzftscco.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ckfeurpq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pexhgapx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dnufqkyf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jnrhefhy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2edghsycx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfkxvgji.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2pcdkftwp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2jnmjtxne.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2udikkpep.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2gdpboqmm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2edsgymte.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eshlnosm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2recjsfzh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gwfthnnx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qvdarhmw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dumtybab.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2fyaxemtt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2berthkny.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qsgujbtl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2jkuchizu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bfbggram.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gbcoteox.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qujvggcf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2uuctriat.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ztcfolwf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zpnaszhu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vjlczswv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtbzizch.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2efqvnyvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezojpbvg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ukoxpukt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cdpqexwm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sietszfi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wfcatlgk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uoecpynw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzoqpsxl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ybysjhyg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2iysdswmr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2pbawzffz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2tctowvtl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ryqygpjl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tspdjpgt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ymliretd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2msgbpmrq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jymfgyvr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2weagarvv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dxganyue.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jcibdljq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gqpjgyhr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2uuoypltj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ahhywyiu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ekfuypmi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nldknxeo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2etncwzbl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2thfqmylt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2qvhdjvbl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wwllzsli.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mkgnjnhc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ncitgojh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfivhkav.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcqqvoup.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2diyrhwvm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uucifgfp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2tjgffoob.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2hejnkgpw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2exktxonn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2vsjymiqi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2duvbznfm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hqkmesfz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ymdyquyj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qybkwgyv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2fmqzqjvi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2bjunyfcf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2nkyaukzp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqgmeduk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2atwvofeb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2lvtxbdmn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2azyiydzb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2psukrijd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yjxtaoxx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2vrizgfjq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2trtfmzbg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2huzxznfy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2parevroa.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2qlkjckhx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ugmvjety.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dpaigqlx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2njidqpah.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nnrwcjit.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2hzjxepnt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zxmcnrjg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2nowimgfd.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ykoookqu.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2kdkvgsuu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2thgsbgwq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2iyylhtzn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bdnyvrmo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2srdztejy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2pmkmhpkk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ptgsqdsz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2mgmqkjdw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2gljnxyed.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ldpklnhh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2xplzqyao.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ugaxketp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2llzxflvc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2tqhghnse.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2npwnkpnj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ghohzldv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2wgfuacfr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ailfxdei.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2qaedsmsj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2iczxapzm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2keqafvsl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xnpvfeky.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lupyewyi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ghlwxbjn.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2qaywwjxo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2jqsqncqr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qlzgilvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otobfwcs.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2inxkdipw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pacxrfvh.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2scfupzyi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rsujcanx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ftoiocgp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmpmqrjb.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nqmicbms.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2sqehlius.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqxronwq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ajvhjqjh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xxlxwqvo.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vcvyhelp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2asypwdlm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2fgsmzkew.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2baihupnt.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2agrjgusz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hjjxqrmg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jdkhznqe.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ompwxhwy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dyhgzzjr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2icmlzbte.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2gxuorqvf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2vrmsbext.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nzpknwhr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zqszkxua.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xfnaqiek.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ufmywmxp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tuefniru.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2gxaakvys.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dasxcouj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysldgvjn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jgeatwgt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lbsanluh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jkxajivu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2glxsvxcg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zwbcakrj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qwcvygpm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tabybshq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2asihbdqp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2osscviux.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pgjxqehm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tuiqlymv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ryzirpgq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2fixgdggs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xcbjopfd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fqlodxjx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2hmfeomdf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2dyzrzjyh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cggeuaov.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2xqckzfhx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2lwzfjvad.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2lnawpjnq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nmorjvlf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2byfbaejz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2glicfqne.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rxvahekw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2mtdzkbbd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2upiwqaii.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2fuhjasxj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2bnnizeqa.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2wbltmiri.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2idxqtvwe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2bbqkzgtd.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2nmccahkt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2gprjluna.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jnweffya.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2dkteiylv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2dazzslvi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pzykbvjl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zbxsahkk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xhxgwfer.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2iybhohpa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2sjvjnmsa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2fwjtaxef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmellamv.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2rymkeohk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdlqiohp.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2mpwyujxa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2aymvumoe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2trdbyitw.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2iwcnbxms.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2torlcbht.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2laegpxuy.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2siatxuii.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2rnsugmmv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2udzakimn.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zxawgoip.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jgaohwfa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2nxdclmvl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2hojfycte.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2cmnwkbqh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2evdjhysb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2melarwas.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2zgnvwfoq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2yrtydsdx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2obvmrdpv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2qjvdnlkt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2fcaswfor.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wnwoqprm.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nbqfhthy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hislihma.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bpjtjanl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yniqwgxh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2yijjocsc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2mldwuaxy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2guyajmwg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2ftrtefcv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2rekdkmbi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yeesnnba.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2oafbgrvn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2zymjqcvg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ygeuarer.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2sakkgjjq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2cntimgur.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2hmhtzqvh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2tyyqqkxz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xsibtobh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2gyjqowcj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2uzhftvcj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2fvyfpybh.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2kfwvswbe.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ngvtlnek.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2wzsazjpa.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2qmeyzpqm.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2lyodbgkq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2hcgktjah.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2wjsbvotl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mcnbxosb.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2rqfgxiyv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2gfhdwvjc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2djhgtzwc.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2gqdsewvq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bfrpuwsg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2cgzlcuvy.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2cfurnbrj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hqevfnnp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2oyykvkjg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bjgighia.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cqhetniv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bymltokm.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2xylshpgv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2wuiyjmiq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2yruzicls.html


<!-- 参考信息 -->