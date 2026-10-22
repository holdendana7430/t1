代发 wailian999

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oitldcxi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2vdiwqzmx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2gxzxmqct.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kvyemwsx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mcysxwai.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qxdnhzeg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zaimzqmc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kostsagu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fqgrupqs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghexxfkz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djuffigb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2poupdtdj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2swlnsmjt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2negybwzo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ugeaudgz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xmbkxfuu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnvvcskb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkxibvyx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjbmxxsv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mtfcpeet.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mbtjhuob.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lcpoekmm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pzagesbl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2dupafhxn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xgdzgadl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ncxfzwze.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2foglbqvf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yurtxunl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fozwbegp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2croqlbil.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2kcxiuigs.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hipclviv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lrlbrioe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2usnuagrw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2lasaqgrj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2yrdwciti.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2khowsjvq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2xcssjaxl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2khdawjhw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jpyhotvq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zzckbehe.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qdcexlgh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hilofmfp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwoxpbar.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xhsugepz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bcqdvrny.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2amcrakxh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tntzazie.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2bxwdvrrl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ssidcbfx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xxrovrmc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wdlplhwn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mboerhfb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2epokvenp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ffregxdk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ekzemcvj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2afnpopyg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2kdygtgog.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2beevggvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yeesfpsv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2igdymbhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvjoonca.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2pfhrbkzg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2coyndevj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxvnsvcw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hxyaxagf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zpdwmzpl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2yuxzmupt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2zgsieotf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2aurfpbny.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ostcsquy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cldhtnqc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2dnutsklw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmhahxxv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2krqjjnvp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gfkfnhjw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xktrwgza.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2cjgujhao.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2annpjizh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbnvzxoh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2whvkczoi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2aubhuuva.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gaowirjn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dxmzrhmh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jiqahpry.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bcuxcmyc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2xhqznlcz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dsyvzfhr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2viqxwrvz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2piqoiqru.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ozgfmfns.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtkzxzvo.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cqyekvvg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmzjzxuo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uuhojkvb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fcqhlhtm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2utbgiweu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2sdqekgan.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ljsfgrgx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2nxuytvbr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ewuoossa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vqnwqtpm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2srkixznn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2spikcijk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2waxfylto.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2atefztvs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2axmwafyo.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2oadidvqd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2sujxtwla.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hcdguusz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dnhmgaqu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ykbnyfuv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2eardrxst.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2acjkbavc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2vunrrnyw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hsbplesg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2flyngpug.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2vvjgdxfa.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aeggxcki.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gqaaihlq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vprtkcyk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vdmippks.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2isrolhfs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2dujlnxvt.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2brhhsdsf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2snyvnsxp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2cvestjvi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2tedzasmc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fpstbtbi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ymkebttq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jpfusspc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2qeqivzdg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2yjxlygju.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2eawpkxpi.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xjltwnwq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2wyhsotgb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ihguxnxd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2tsbvqjxo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2byaxmaou.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2zmzfjuba.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jczlnybq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2eluzbtra.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2bwqzyomh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xjcabupz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xffxsjcm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2abhuyenx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jexsynqs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2kkwwazof.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2bkqbwbvp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2goxrlebm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2fnioyrbi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jfnlfxhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axfnpuwl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2yuvixtex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocvvygqc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2twrqmyot.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lfysdzkv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zlmnetdl.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zctdluqw.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2slkqdgvr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2vzluhaui.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ujgscfqm.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rxbzqyrn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tcjnvfmg.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2hbilwuih.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ndzgazfg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2lfdfdspv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2bzeknwkg.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2lpnmeotk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2slhywgqw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pjprtqht.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2bolbrmsz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cofbaijt.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ptdyutor.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2nhbrufvv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hrcbpviz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lyfkcqil.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wiwmlfrx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xmjrmxjp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2vepmjuua.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2vaxnrxod.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2qskcuqxp.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rfhcchej.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2nzqmdztt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2iggfoiix.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ggljechf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2tgxlytws.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fgvfwawt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ertpxgkn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vxpdzvqr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dyjnkxld.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gjnujkgt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2baculikl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jtzrobvr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2htqgmevs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2focbssob.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2iaftenmb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fjjxafbi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qsgunbxc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ajdrporu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ryzkdqlb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cdkvijvh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2yowefivg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ismdwjxb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2gkbbqmsa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2apqinnba.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2joruyvut.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2pnyrgwrc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fymstweu.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2fgmfufkt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjrygzg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2irtfjgcg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2xlqgdzvo.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2xbpkroeb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2xllnhumo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2bdurthli.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2zwgsftcg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2rbicangn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fgivgzck.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ylcbzkfs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2nlieltbg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2nwqhibqd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ugnthfta.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2gxwuywna.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ysczxxmi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2eqzbxqkv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2lnobpuno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bitosfbp.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2tviguatw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkofcowm.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2jakrswub.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2hlhqetdv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2lynyaejy.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2fsxiatke.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2yfzakntw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xbejcquh.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2nqmwdgfy.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2wkjuqpqc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2mafavbux.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zosrvgha.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2cspzvrvt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bpscpofc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2aarhgnwu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2soceyxti.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2wbrirzkb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2dmnzxkss.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2iqatrmkx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2cdcvjspw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2bructoyt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2wjqxyvsh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2lybjaylc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qgsibwyp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zsiltqbt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2luqqvyga.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bobfofgk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cqzlidjc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2kjjjwrkd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2dffwtcoj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fybvdovy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2semylrfv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ugooupjo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vofjckae.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nxucxftc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zyixeamr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gasitdct.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2obztyjny.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2movkbxni.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2vuivnwzz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ujojtfxx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ntsprjmu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2uckhrauc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bqheewji.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2fsocotae.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2fukzybxl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2lkageheu.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ynsrwocv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ppfqqwvh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2lnazvnyn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2rivmowuh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2dgkjxsgu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2jtxhznkx.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ytagyfhf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2yqtmqajo.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2topbnfqz.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2cynmxmkw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2eowsyict.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2yjjjpjzr.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kfassxhj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hltmjccj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2dpzelfpv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2lhkkhhta.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rfkssisd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qvsecbzz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2dlhgrnlo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2rumflchl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2oomxbyzx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2cxgbfyjc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2mcozygdo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2cthkqeen.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2giwhyvky.html


<!-- 参考信息 -->