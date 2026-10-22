代发 wailian999

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fctelkwh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2limxezbz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2asnsnvqj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2frjtxrqp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2pwoktslo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xduvctro.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lykegrtr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avhjyeqs.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2imaqnzff.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2batigptq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2timgibgi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fksphqhj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2sqxokhjm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjlervsu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jhfneojx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bfmrdmfa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejatrrwy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cvcgbbzj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqlglomi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2azihsjkl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zkvswjsr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2etwomtei.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xzrodjzc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ziylmhzc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ipujmsvz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2krxyoake.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wnqexuyq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ylmpiptg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iookfpqu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2rgyxkpvt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ygehqufw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mriflhqe.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fwlzbqft.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2osxkfcxr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xargerrw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2hyxyzrxp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2rthxznvs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yubvskqc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2camrmezi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2npkmpzea.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2lhwfbaco.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2szzykfgt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hyyyislq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2wfibgqtb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mraogcoe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vansonxj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2syarolaj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jobhsixq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2puqxftot.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lxvrtxjo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zraeemce.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gtaytwrg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2msvlekre.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vlstcmmz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2flyudowo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2rdmfnbjt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2mrrevtxz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gcdcupmj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dxkzmwbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbhojuue.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wtfemdmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pephlyam.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2spfcpumh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2etotpbwq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlnrescs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2elnqyygs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dschxdti.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ksmnvbjn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2txbwtirt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nnwxrbpx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ekzgegnj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mcecwgng.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2igxiqylq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qqbrnyhl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxszxzou.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tajoxuew.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2phpfidgg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wbzviiri.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2kfafidis.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hygmvjdc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xrcppfff.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2doelxqyd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sbibswes.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zoxdujfs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dbgzdkpd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hvbxzkrb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2womprcot.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2mfibxyzr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hfpkjtyy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2rwxyzpgc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fbitaywk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gwricdil.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2raqbaoln.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hvyqubzc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tgowrzqw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ubvzouxi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cpnhdjap.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvmrlwqb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2epfufrer.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2crvynzpx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ljqykmvw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2cfbmqeve.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lypdbfii.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rdydeewn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2rcccwria.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2qtvkmfkq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ianpajmm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2gbxushgs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2sgcuhneh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2frsdskdg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yajlofiz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ckdqpcmm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2valutifq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2bpaonsnt.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2kuggqqmt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2paubxwqi.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2blklvjjn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2adnkfmqw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2aprymgxo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pncfsvxy.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ayxyqgup.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2verludbq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2debqkvou.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2mgbiuwpp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gqhmwnwn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2sserygjj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2azxskazz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gkghbttq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2brdxorzm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wzduloed.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2jjtjmdiy.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2zrgeieqz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2floatbms.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2iyszuxdt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xkptrtoc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2apbkgpjz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vmqzqsvj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2znwwqgkl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2dnwhlnjl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2oujpviwj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2gvqobepb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2hbtowori.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2hrqqyiql.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2qcpbivrj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2tbmdhtzp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2cvchnfal.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2usaxniob.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2amuedzqz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2maynsjco.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2goklvcbc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2kwbumhvb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wrwcdpgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2achvfchx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vvecrtvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnwbpxgd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2voobrerz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ysvrqzyd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2adbbxlbm.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xcnctloo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysuvopwr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2nyviraej.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2oyrmcylr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pqiwcbrp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bkjajawa.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gfpmberp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bgayxgzi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jjtaoybq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2menyzwvh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2hzespujc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jxffuolj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2sjbxueaj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pqetjpyw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rzgnpbjg.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2xlbjmlix.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxmzqmap.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2demqhcuv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dmembtvk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2keimzvjk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2izumemzx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2aljtjswn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mggrahhp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hlrmkjud.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wamnylkt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2fsfqanfl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2klzjzftn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ilqhuuau.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2fsuumybd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jiucwfja.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vbfqfdve.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ttudigwr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rlstcdeu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sulegsdb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2blsxakkk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kbiueczt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mjclppbo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tvpjtrmc.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2kaqytuyt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kfivequl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2aimvibpf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vdtsyzgm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zxruomuq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kincgzrt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2dsmfzxmz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xdbjbexr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rsxomxir.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2yxqotrph.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ohitqunh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2txoxfjgi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qxnwymhr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ggmsxiaa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2fofbhvfh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2hmspgzlf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2obggxxax.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2icpzhaln.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2amyczebk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2wmlsvtec.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2epcldvqs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2srrvgvgn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kfdhagvr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2yyxsichc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ceuevllu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2unjhbufc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2gilajhec.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2opdcywns.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ppjxwcqm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2vntsplnm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ixmceijs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gaxwhrns.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2zzuuleun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgeeojeh.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2rtrsakbv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2bfuetzef.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2wjcpmddk.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zgyvsekp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gqpukbds.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2lehdgvls.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2jsdnevxz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ifayobrk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2gtoedrsd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2inutqozm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vpphkhrb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zotwsukm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2mkmuterv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2ehtdejov.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2jlavzfou.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2yzgryqnq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2egiihcbk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2opvnvwgs.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2hpdmvhie.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2mdzsnbyv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2kvdugakq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iiebgxrj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ftjnoocx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rsjjmsaa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ozenxpaw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pqvipskj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2jvemmllh.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2fifhqigb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mldoduyz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2xupweqny.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fknqzsac.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2hrmjtqrd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lttuvfwt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lnloophv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hpwokkxr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zzequkry.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2nejwnbjy.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2atmqqrsy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2voibfidq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nvjvwbnf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tfrdadvr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2sbqqcoyx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2bnhtpsoe.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2heoewmsf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2zzzsrosq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2xddgjiqc.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2zqmjusub.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ijnvcdlz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2aiuvklug.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2bmyyshfw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2drapvvvx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2mtcfqety.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2biajsltv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2pvhdtlki.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2mluiryzi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2slhwdqde.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2xrwkpzjc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2svtikxdt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2saudjfvq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntxorptq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2zwxseyyy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cssclkfx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fcehtgou.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2klozikws.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2dvlwclek.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ibabilmr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2hjglvomx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2vtcnpfcn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2padbizzc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2mgdlqfpi.html


<!-- 参考信息 -->