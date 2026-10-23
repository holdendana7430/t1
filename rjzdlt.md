代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qimnjbli.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyhjoofq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybocqwjv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cphmpqbf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gpvhtgag.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3brwyvlcc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ekomdizt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kfofmblh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3bthgfztm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xtiexike.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sxtygtuw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wpttkgxx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rthdxdcd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3yckyfhrm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mvqaneja.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zwgtlxxp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3apdbkcgo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3rhgodxqh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hjxloarh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ozirysve.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3yyfvcodo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zrknuaok.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gqyemxax.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3gucxgwgs.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3sxxtgumj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3hdjchhin.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pipchmlw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3bicmughf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yzdnopsx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rvzxyjne.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3faaukqnx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3fyxtsuxm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3pldinftr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ruvuyowb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3mrjzmaqn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3uiojykgm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gjxzrvkf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wabcehrx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ujyvtpyn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ufmqvgpd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3gofrgurb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3utfykjkw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wntvamvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezunidwv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3uczuunra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqysddfg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wnifbzag.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hpdhcnsx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3htvfvuin.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3oqolvnyv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bsjozvko.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3skddpxsr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3dvqjzgve.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hoxzdzfn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3trifiipq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qxfuzpwq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3pzucmfeu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iihcdmgf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkrzzzok.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xwhzegrj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xvlkesgd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fdxccazm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ckwcpvzh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bsdyqbmg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fmjhntjn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3yshdrrpv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iujswttn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lofguyiw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xvxklaxv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nuexafhi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3cglpjtko.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zjeclvzx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nlkylyxq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ziufofol.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uamykarz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjpqftlw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxewbjaw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hfdgefxu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3owwduwsk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vfvubueh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3stnppqod.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ftmnmugo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ilmpqmyk.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ekkoonmu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3umyxpaum.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ufshvyet.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wufkoaom.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sathlkav.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3frsyxqmz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3nufwtelr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcuzwadd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3bkjgijhf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3sivvmegc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sdgospah.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qtxkkkzd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jieiwgye.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ddezwybj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ilndjnph.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xxmeezwe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wsappyqy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tmqxytbk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3mzktxefk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wyiyayzs.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wercfnhm.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lfqmozwh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3pqjzfsce.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3qfstvmfo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3xvncigsv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yzpgcsni.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3tuvpswcb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3qohsbmhw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3aacgynxv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3tdgdjnrx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hxdlsorc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3taiqmvcf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3pxziptad.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3mlqybegk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3drfesabo.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3iaxdrjfo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3xklfjcjw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ryaspidx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ihoqossj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3jomgrdsa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3mnqwydlt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3aqdzxclv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ohisazxb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3lqolczns.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3azflmbpb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3xqyxbcve.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3kzrlvfgk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fpgyeglu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xwszohhz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3urfmowys.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3iqjhuduv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ouunlpji.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ldrmpenl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npsitihn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3rdsrnsyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykeuuvvk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3beervrui.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sliwqbvt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tespachi.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3komcpvqs.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3lehqutno.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3orvujsuz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xemyolve.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vmjenixd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xpcdfgnd.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pgdlqxes.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nfsygmhi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ipyhqsqv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3axpunlrs.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ukycqakm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3oxvzqggx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dawjwlwp.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nyskkyaz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uukgcyha.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3tfkgucdy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cguuzztn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3timgivuf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qtyimrhy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ejucbkbd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3suzfdorr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3cnryzjdm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yausokvr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3wwyhuzge.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3yhgoyjhf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hqichzvg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ipuuqdot.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3whkitkws.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3fxyoxmil.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3riphvina.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ivxayxal.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3tmzzalhc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3kxcvtfdb.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3iefbebdw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sliepdrc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3omzgcnim.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqdxivfz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3szuotyaf.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3aetjwbme.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvvplqak.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zahctvaz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3sdakddha.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3xcuypgta.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3mqgtqouy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3smfppjqz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3bojztjvg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3nwslmawy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3pdmkcxej.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3uxcbumfm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3bsqejsjw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bvkjeaud.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3qyjplpbs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3kjhkxong.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bjdvgxul.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ucdbylfl.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3jxnvotsa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3tykfetcs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3zeyuvxpw.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3wpeqenvv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3uvhihdsk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3patjthty.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3wqhiukxx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3anqesaem.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3icriaswj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dtrtrchn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3xownyvaj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3zxcsbxgc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3umynpmlu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3emhkxxka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdlkhpum.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3nwpkhtsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kynbnbzf.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3opxdbdpk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3aokjwdvt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3shkztxby.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3iuasofga.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3obpehuow.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3hitpatip.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3xgtvzjfz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3luekqcxr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3thcxpsbt.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3amostdus.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cuilgbtw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3lqjbgina.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ufmtxyqc.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3iuenrjfj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3rthkyenz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3upxflvwh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3pagmypyz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3tmnofdyk.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ivikzkue.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3frgkqvwg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3sasszlth.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mjdipait.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3coaxigrl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bdibuwth.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kgnisrut.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fivngojd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ltdbhrif.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3xaccronh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3arafoynp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3zsngwpfy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3shouzfpo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jpwbujbp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3dpuzsqzl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3yxvpptyp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3mgtyyuen.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ngufhijo.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3fqapzdqw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3jfzufjvr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3zvjegeho.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3udoumggm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3wuxdgcpn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mitiiuvo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3kbllxrfx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3cedgqewh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3lfredvtg.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3lzupcyue.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rmeaddkw.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3lrqofdli.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3qfleerdi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3lhtloyiw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3roeftrqf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3meaarygr.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3khmvbspn.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ycrkyory.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3lpwuruxi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pkmidxym.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3hgphrfah.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3gwykivrl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3qsffikhx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3uuabwobm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3vtfebmff.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hkugqeni.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ywdgqrbd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3vogjlpho.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3gjvxgxza.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3cjpuqhrj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ykqyybdt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wwtwlvzv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3cgcncset.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3kolokjdv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3hbdrihoe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3prdowskh.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3bvoexcej.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3cpdfpjej.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3vvuigete.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3kzdxytcb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3njixsnkk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3ppwilwne.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhviaeo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3octuojrd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3jitvidvx.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3fvdjbkuh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3rtzbkdhq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3vqsinuzx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3koafwjhq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ocravovi.html


<!-- 参考信息 -->