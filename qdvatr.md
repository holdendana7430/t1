代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oucyjqwo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfvehqhj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jxjutbzf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuqcrzve.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nvvrqpgt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rqgyskoc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3czgnhrlf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ovdfkhki.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3fzfpsugs.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jkthpqip.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3niepscdl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sjrvjacm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tumwyymq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xwuwghej.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gpuycmqr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zoyogfvx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3chofwbqa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zyjkaitf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kwcvtwqb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3oeewytmh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3aqetqcsh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qpnqtdsg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3izlwfjdh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3remwozzh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3aahucbyc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3cprvazdc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3udzcmeyr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bltzvpeq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3xzeslwyp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fndzxmnb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3evwisdwz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ghvqmpjg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3yshbtwln.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ahqeqgvb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ttjktubf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3svgpvvrn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3mqeewzxd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ajpvorzv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nqolmaww.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3sxxzfasm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tpypmgfp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3jerwtdjk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kbbhdxub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azksonvt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3umgrhfmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfrupvzr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3geyuqbov.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3befjgirw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3rtqjgdnp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jvymeqvf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hwhdirbt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hlrnnprh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3fshpenqe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3vailgjsb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3bmvvidvb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3wwqpfpys.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3luvhuxzp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jqlzhthv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pfjzalil.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbecsgdd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xulfomzi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ralvscii.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ncyttbma.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lprwriwa.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hjjbispi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3fncdywuu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gqsjdicu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tvqqhqbq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wjeycwze.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dsvgocar.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jdkdbnwo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zfkflntw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bsduhhey.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ftwempzx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3msmyftde.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqzcsium.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3moypplxi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfekduxe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhmlkexb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3sbfdvwhm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3gbhcqrzo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ongsbowj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3sryddnrj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3nefyezwc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3oxycarnc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bzbedaam.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3eqglpjti.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3kjwlznii.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ktrnrjhn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3vonbmjll.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3lvwhflbe.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lxjkeoah.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3anluxlwx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3avexsfdv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gtafidoz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rfvmzaxw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3yjftsygu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3tagwqkec.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3kuhzfusi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3dsxfalzj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3gupcyiuk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3lbczrwnn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xaeilrmx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fcxnpwyn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xwlktiyp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3murksfhw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3swnajcta.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3baesdprk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tigigcnb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3sgekdzpp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3gpnpgeqi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rwusubsc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3gxzzhgcr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3zfpqdzrz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3rqvfssfs.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3zyrxaddl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ndiwaeel.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jyicedgq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wxbjgvcq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3lchqupmk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3dlziavdq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3olerhwlx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3qjgjumdv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3suuyvkjv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bezkhktx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3notiasuu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3diritibf.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3dxtwufpy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ozgrpomw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qgzrixic.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fuowmfeo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tqpcjshq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3jrwtebit.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3omajjwaw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3puuztbha.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xxyqeuao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyrjnrrr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3kshcdqyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mofnqpsq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ebkhhbkm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kdedoqmd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zetjauhq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vmezcynp.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lpvejhjx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3cmblgbof.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uiylxkiw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mcjkracz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zqgcitwf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3sqhljxox.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcbcnlro.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3vgxhoxgo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ifdnttou.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3nzvgxcoy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qkpjycfa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3miphnbgf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dvgpyseu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bowubdge.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3vskmvtbf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdhdaaip.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rzeawrhn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3tsorrsza.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3sxizzlys.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cmqjzaat.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3iikjtlwo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ozqoylpr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ikoujxgq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3fvftvsjy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vimktvxu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vuwmkawd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yqciimwg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3yfxmydlu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3acrvwnwg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3pcijmaab.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3krthciie.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tzbuekzq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zvprpbll.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3jrnqpclq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ahtmhhwc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3iyjdqlli.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qdcdygoz.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3afehtsxg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3elgkeyel.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gdvzommv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xpafcmhr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3mdulhule.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yvvpovis.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3tupkpkla.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ykseqpxn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ffbjdneq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vfllpayv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3russaoee.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3sobvtsyl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ppaxcijj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3mmkchmuu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3eubwbdsd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ilbyzaxa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3foyycahx.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ghmzjstg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3vyzyfqgb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ixyqvtns.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3zqwrrunc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3nfaprzkh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ozvompdm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3hykbtagm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3tlgqsddz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wmwpgnyt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3wppaavcx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ruzutzpx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3vgasgwpg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3gjvbuhxo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3oymulyra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbwjjdlf.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3urreunae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwgueftg.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ajcwrikm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3xepjmxsz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3oraouora.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3rhakxeuk.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3suwnehwt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3eiqzidsv.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3grnxgpck.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3bxolkkim.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3nrrwhswz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qkymprhu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3smfxqmmy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3csjucmne.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3xbnbwizh.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3nhfrrkrd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3olzkprve.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3mvmkvjxn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3dejxhtpx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3fdosbela.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3jgkpwkxi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3knhwffgf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3xzfizruv.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gatiymsw.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rmqpoqtu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wxjlytyp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hkjkobdq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dzfhqqgx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3njcbcmsg.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3hsaatvjk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jzrckcrw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3upsspfuo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3calrcnam.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3qvdzumxq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3gyzohzqn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3meszcxoz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ttlemoub.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3aypuwvyt.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3tzizyjgh.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3brlncisb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3wxjhjomp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ztpbbuae.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xuleflif.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qcexukrc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3szbqpvbq.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3tknvhwip.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3kpatvrgl.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3dtxyvirq.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ovicymxk.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3fgzuymmc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3rpjiyapo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3gbwqslkd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mgpnckgr.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3beofvpud.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3jjjbhxiu.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3dngvhmgw.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3yfaitzqm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3icqvmcnj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3kjaskfym.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3egqrmtlm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3rkahdtcm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3riyciujl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3fjwmkpsf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qsfdloze.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hzbtyvot.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3umlzmaro.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3nkmmnmka.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3kqclracz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ydzclzcw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3recqveox.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3nmrdoigz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qjoowyzq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3zpypvsuy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3egpekbzv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3liypkrpl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3gbgbnikg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3qpsvxbvp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3lmlcdoym.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3zpghuhaj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3kpabagac.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3aopctgwk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3gjxxvawu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ihrwjdeb.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3nwbibyxs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3iftehoic.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ukhljtvf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzluozlp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3baqxypgj.html


<!-- 参考信息 -->