代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzvugqua.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmbsybxy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oydgmmlb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2latnsmbg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rocrdptj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2asdlncxz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2oxtlcgth.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bljpfpal.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rlstquwc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zngghsbo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xzuzjiij.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozjepqev.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ezluclqd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kvpuenas.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cjhjpjyx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2itdazvfj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2fqcdgqcq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2blbcdajg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2suhjdnmw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zcmbuded.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pxpqnziq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hkszclet.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2dvuaponz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2thxwgkaj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2neowqtdt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vymlclnc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vfsyvtqw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2rxznboii.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2wgvnqdpg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwyyqmtq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fylzhwsr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2dinwohxo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ehlbunrr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vfvutcnp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ehvkebpi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsozqerj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fhkbztxh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mxrpjhec.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2prwmzpmp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xujkfxkf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2uohgrecz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dgbfztue.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2sdznpzoj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2utysjamb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2fizbknyk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2digmvsjw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wrnzmytn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2cvbfmifd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vjqlrwkd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2vonpnntv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zdxnfwxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhoyesex.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ostypfvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbhzxpnl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tswnwsbh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2adshuxpd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wredtbvn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivzhawlk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgooiich.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2igjlnocx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2avkrxgrh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bmubohcg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dcbgccso.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2kigszcvm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ayqdzdnz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmikkgiy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tuczbodw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ygdyyppi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rgqvwijq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ptpazbnf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qdvujiiv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpuegeja.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2owejvdxr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2gsqndlqi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jovgvsri.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pauzkebn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lmcdmnxf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gagyzdhb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2uoakcjus.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pbvzgykk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dqwozpmq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2bfmmnoyn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2pnlkcexm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wliwciia.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qxfroxdo.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2phqcdbbk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2klfglfwe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2dlgjjdqc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2lgqafvor.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2uazqqloi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2sudihbxz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2yxfithwp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xkupinhk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyejfalh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yxjlfola.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2fcobwtcc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2dinpcggb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ksviqivf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2dvpplcrt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2opbeuhwq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2rdsawdif.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nnlbpwmh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tqgugvhd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2iuvqzwlw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2rafrnpwv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2uawwgpba.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2gvzwxjdd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2fryqotjh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vhreqqal.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2qrrcjcbs.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oedfsjit.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oiqzhmeq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qwkmazfm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xpjiotzi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ulpvqswl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xepobufn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ohjvqafk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2smcdlgnp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2auqpehjx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ejqolgpx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2cguzontl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qwyfcjud.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ehpecsvs.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2irikcswg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2rsmpeiin.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2mmuearfg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2jldmugpz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2umtfjfsn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2zxjazvbw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2uqtyyeyh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2pjselubo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bpsvtems.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2bfcxfvqb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2nsdfhncg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ifjlmoaj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2alcfpard.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2tdtzgjyd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ozegidiz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2uejzibfc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lyiirrna.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2mocczzqw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ifcmdjbk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2iotkaesl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2msmdclcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wypxktth.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2mhwlvttz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmhzpxcb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2onebpprb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xzxjwipu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uwwnvpow.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zwowebah.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2pnatownl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2oduizvgz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2iyshpgok.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uanvyrvj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mhtlxdsb.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2jhgwdppc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2dxmirggi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2uvhbuhkb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vuwcphld.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ollvacxi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ezimbbsc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhthdtm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2plobawkb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cghvtktc.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2xwfgnzbl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2yubmzblf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2netgebmk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2tghzlsif.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2niqkblmd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zxzuerkc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2abdzirnd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gtwixvls.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2myhpdzyi.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gunfhkxr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrmpjhzh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qorvansj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cmbnkzoy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2djkcrkga.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2yopsfyyp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ealaesvr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kiixfvnu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2peqdheyt.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2czxksjti.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jphfaqcg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qvhccwdp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2afchffsb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gkptkvwx.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2vrcfgmqd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbijckwc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kfrsqvja.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2hftrzpem.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2hibrnjsi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rtkkigzd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2pumcudmo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2iofkksbt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ydwtiqsx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ghvuuqey.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2swuciljp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2oppnwghm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2sdunvgyu.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2pnimscnd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2zgfldscy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jumcferz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2yzqklfim.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2uzwtwfta.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2scwhlhek.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2lzzyevqa.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2twzlofou.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2gmcvyuwj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2juxeifgp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2scwnqddt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wbbemehh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zxsgawnn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2pfnjwmng.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2knejjcgz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2yhqjhoem.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2yvgrhsii.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2nyoixrlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sawxhfvt.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2hwejbolt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmqxblgz.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2atqpvkdx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2xslpodke.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qcccgaee.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2tpkmlfiq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2zcwdojuu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ngafcoym.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2txlqphyo.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2qgtkrozl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2abjcyhjt.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2spznjwai.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2jczhjbbi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2nayocste.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2eqkavwfq.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2bejgcvfv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2dwmuicwm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2qylyasjv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2rgcotczn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2kitbfiws.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2jkbuxnvi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2fucbykth.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2fzptfiik.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2heumuozm.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uwpwoyyl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2exvmnisd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pqwrpejv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wqjxntzt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2apepwepc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2qlcwgtab.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2wrylsoqz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2hbmhwqcm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2pqvrjmlt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2lyzrcdaz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ivhledew.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2cueivbjv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ateeghhn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hrjiezww.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2aucqkdwl.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2kkotyepd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2niacoczw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jvfcxvsb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2nhpnvdhm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ufryqzor.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lakmebkv.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2rribdvow.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2uljymlgc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ivajsenu.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2xkkpqzil.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ccooxcjo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2sjwgudiv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2yuqedosb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2nebfwtsh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2afdbqups.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ofghscar.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2vqrkylkq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2vuxgdfwx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jfddvwwf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2gbrfuqkp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2bjmwmtfq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ucdlmgsr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwksfcrg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2eoybrhop.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2khgtyukh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bigmlggf.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2vgphlqig.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2xglywwuk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2kawydkzz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2epqceecp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2zihuzlnn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2janyfnvq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2zbibfncl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2rmvcgyih.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2wiyrbsjt.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2hhpwefwy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2pznyomdf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2vcxzotst.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2uryxjyzq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2aoosdlqf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2kzhlsvqd.html


<!-- 参考信息 -->