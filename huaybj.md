代发 wailian999

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ysxzwnfd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nsbqorhv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hwqeknlz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3velhzojt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3chsumnvu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3cbeifcaz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dbniiaml.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dssfofrq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ozbaencr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3dcmiotph.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3lnckjdww.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3bfqewtan.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3izkobwrs.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3uvlyelpo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ftpmjnxs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ipkcnggs.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3umtlmsor.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3hynouuhg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xozqgzbi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3emtrtric.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3dppuftbx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qxqxgfew.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lyixqqjr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qyxjmquk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ubavwoan.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fklzwnia.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xcgjhohs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3rykhiswx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3djvsgtde.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xdbdpfkn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tgntrsfu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zyyhzxmy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3oucstxfa.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dzxucdxj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ltloxbpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dknzwhbu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3upjbtnst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wzhraqxq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3difoowyq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3igskhesd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwcitruu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wfndlarv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jaixgvlj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kvufmeux.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3afzifyib.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xvpcyliv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ziysissk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qubojoas.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ymaahogx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlzfzjay.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzwhsmjn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjunzzqg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kmnwkymh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jhtlvfhm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3njheehus.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3miktzfeb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pigqooto.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gehiqrtn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3knifhwfv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3levoreje.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lbdqjfzf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tfkxwmve.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3iqiptqlc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3fcqpvwxc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ccshmzmv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3aaldkqib.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ipqqkcux.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tcjqxjkt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bdrddgmr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kwmldgmh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3iouupadz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hnxgaakl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3qdkxrjyv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdiodymd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3sbrwgdws.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rjmwepwp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3oaebatty.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kkzgvqgr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccaljpmt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcauslva.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3sqccfhea.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3mkqgwqkc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3wiftcnup.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3mqnkamuo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3xebirxtx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gazrxjxw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tgvcnvsd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mrysrdnz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3pctxlskv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3xcdkyjrp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ybhtscdk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3inmmhxjt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qpsbbzab.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3jnfrkzkm.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gqqkserf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uhvnljcv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rwhyjamm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3bazdgkui.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wurodqoh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3myeqwbmw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3feheiskv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kfroiozg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3waczaldl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3uklrzqut.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3belhbrmw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3tkgbijrh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3srihsovw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3oqtpbhcd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3tzqgcqjr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3rktzdyon.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3vaqutqmo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mzbflhqa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3kdrcesgl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ggtjuefk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jyshpbid.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgbilcaf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xgupspzi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hsycdirb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3jrykpark.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3hdqjwpbx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3hkcvmluz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3qcftbktp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3btzelcgq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ndlmuzol.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3fsgmbxbu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3arergsid.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tzeqhygb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3smznbivp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htqbrcej.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3epuiifzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyqxduyk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rhhdzgtn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3udhoddbi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vfzbltqh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3azrsdfvk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3aaiqrewa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3znkuzbml.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3keuqhlrk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3tabtxjkr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vseilmhz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3zwxjluby.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lxudafqt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3oqhkgzjd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3dkihrfrh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3rzavnbfj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3lqmemjiu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqrtarsj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xlnoisqd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sigtaelo.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ryzubckm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3lckkoqyb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rfzlimwz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3htqosffc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ntwzpwlw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ohyptrxt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3gwatmyxm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ukwyznkn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3enofztpu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3mzmfqetn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vobleynm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uwmsotdt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nkfyrdjk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3skofwpwx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qfamgoji.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tpzoheck.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3izqphdhc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tnacoqwb.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wdtrujrn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3szbkkren.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wtiwvqan.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3govmmwli.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3lijdelyx.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3wwzkwnwl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmnrqebh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ezjvxgsr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3vjyhzrpq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3dufytfnh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xoprqcpa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ahxgydzq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3uvnkqhcp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3wgrscxcp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3npxbyask.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3scazdifd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3qhmuxauw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qwmmxoen.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3wokulunz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3leqwopqc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3fkxurvzk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3aegpczat.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ffiwltwp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3rglzpzel.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3nnrygsox.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3wgaqfnoi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3rszsgtbu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3daytrhru.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3uvwkrutz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3sawhhxmm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3usxlxtkb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3negcdaqx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3pnsyuxdx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3suqbfssj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3poosuegy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3vbsszdze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzbnwgqf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3haceqrpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmezfsxy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3gwvqepnz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3fpzyqqvc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3agjahcam.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jdhskeoi.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3gbalrxmx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3pzquyymi.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3tgqkovra.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3uzazxoxy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3vyjtmnox.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hpqtqijm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ixlyvfit.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3zhkjcbac.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3jhhuljjc.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3fbvghnww.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3lnghwwpp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3zibrxtfk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3dcvfhflb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3yugphwdv.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3hzjhraiz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3lvazzvmd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3osbiorzv.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bqwofjcv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nifudaky.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wtgqwngh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tonysmyj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mubwvtgx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3gykrssoh.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ujpmjefy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3pcjdcklq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3cpzpewhb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lgugiimi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ylmprrfb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fyivsfxz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mrbrknwe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3awdyzzwk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3onhlnyaa.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3mqoxjwgs.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ovknchci.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3dhxzrcfc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3eagtenlp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3sxhqddvs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3heyyzmms.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3uexszzvw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3juvddiuk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nbtuvgsp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3cohlixhu.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3oogzlgul.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3xpjxtfrh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3jqvivtni.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ufjuhooh.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ocesraoz.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3grcsvfzl.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3kmiodgaz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3ejbggjpe.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3wqzgiavv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qsbvgoqr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3gjmjwqqq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3vvtimfnk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3qrioxodh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3dyhdxazi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3obsajapu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jkhtpwsa.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ctygrxjj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3fphjmhaz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3wmkhckkg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3sttouvxh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3sbtfyryv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3etltedro.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3dlgehmpe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3tmwrcgjp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3dcvwmmrv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3gmftyywx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3yxhaohvv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3wtwkiuxk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3xyyryjfo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3emwugysi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3upnkpcwc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3xsknxghc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qtgvewfs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3jtnxuthv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3suiowqds.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3dvajrvzo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzbbrwda.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3bdiveiup.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3esrzimpg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jlugvmus.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3cucudetm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3wsuccsfp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3qrsfgnqz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3wrsuljxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emqbgnon.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3fbyhgdua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtdimkpv.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3gdncqvhf.html


<!-- 参考信息 -->